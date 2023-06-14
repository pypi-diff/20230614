# Comparing `tmp/mykit-2.0.0rc3.tar.gz` & `tmp/mykit-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-2.0.0rc3.tar", last modified: Tue Jun 13 16:19:00 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-cbqrps87/mykit-2.0.1.tar", last modified: Wed Jun 14 05:33:06 2023, max compression
```

## Comparing `mykit-2.0.0rc3.tar` & `mykit-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-2.0.0rc3/LICENSE
--rw-rw-rw-   0        0        0     3751 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-06-13 16:04:50.000000 mykit-2.0.0rc3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.098278 mykit-2.0.0rc3/mykit/
--rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-2.0.0rc3/mykit/__init__.py
--rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-2.0.0rc3/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.306871 mykit-2.0.0rc3/mykit/app/
--rw-rw-rw-   0        0        0     3766 2023-06-13 16:17:41.000000 mykit-2.0.0rc3/mykit/app/__init__.py
--rw-rw-rw-   0        0        0      320 2023-06-13 16:17:16.000000 mykit-2.0.0rc3/mykit/app/_runtime.py
--rw-rw-rw-   0        0        0     4157 2023-06-13 13:01:03.000000 mykit-2.0.0rc3/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12724 2023-06-13 12:41:28.000000 mykit-2.0.0rc3/mykit/app/button.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.356070 mykit-2.0.0rc3/mykit/app/complex/
--rw-rw-rw-   0        0        0    20467 2023-06-13 14:43:30.000000 mykit-2.0.0rc3/mykit/app/complex/biplot.py
--rw-rw-rw-   0        0        0    16360 2023-06-13 13:49:53.000000 mykit-2.0.0rc3/mykit/app/complex/plot.py
--rw-rw-rw-   0        0        0     9010 2023-06-13 13:12:29.000000 mykit-2.0.0rc3/mykit/app/label.py
--rw-rw-rw-   0        0        0    27866 2023-06-13 13:13:12.000000 mykit-2.0.0rc3/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.418579 mykit-2.0.0rc3/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-2.0.0rc3/mykit/kit/color.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:18:59.990031 mykit-2.0.0rc3/mykit/kit/fast_visualizations/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.418579 mykit-2.0.0rc3/mykit/kit/fast_visualizations/static/
--rw-rw-rw-   0        0        0      500 2023-06-13 14:50:18.000000 mykit-2.0.0rc3/mykit/kit/fast_visualizations/static/plot.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-2.0.0rc3/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.434202 mykit-2.0.0rc3/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-2.0.0rc3/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-2.0.0rc3/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.434202 mykit-2.0.0rc3/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-2.0.0rc3/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-2.0.0rc3/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-2.0.0rc3/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-2.0.0rc3/mykit/kit/path.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-2.0.0rc3/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-2.0.0rc3/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-2.0.0rc3/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.250856 mykit-2.0.0rc3/mykit.egg-info/
--rw-rw-rw-   0        0        0     3751 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1276 2023-06-13 16:17:49.000000 mykit-2.0.0rc3/pyproject.toml
--rw-rw-rw-   0        0        0      161 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-2.0.0rc3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.449829 mykit-2.0.0rc3/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/tests/test_kit/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc3/tests/test_kit/__init__.py
--rw-rw-rw-   0        0        0     4212 2023-06-12 14:37:42.000000 mykit-2.0.0rc3/tests/test_kit/test_color.py
--rw-rw-rw-   0        0        0     3546 2023-06-12 12:14:14.000000 mykit-2.0.0rc3/tests/test_kit/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-14 05:32:48.000000 mykit-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-14 05:33:06.000000 mykit-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 05:32:48.000000 mykit-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    20724 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-14 05:32:48.000000 mykit-2.0.1/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 05:33:06.000000 mykit-2.0.1/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-14 05:32:48.000000 mykit-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 05:33:06.000000 mykit-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 05:32:48.000000 mykit-2.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mykit-2.0.0rc3/LICENSE` & `mykit-2.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Nicholas Valentinus
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Nicholas Valentinus
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mykit-2.0.0rc3/README.md` & `mykit-2.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-# myKit
-
-Python utility toolkit.
-
-![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
-
-[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
-[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
-
-
-## Installation
-
-```sh
-pip install mykit
-```
-
-
-## Usage
-
-```python
-from mykit.kit.text import byteFmt
-from mykit.app.arrow import Arrow
-from mykit.app.slider import Slider
-
-
-x = byteFmt(3141592653589793)
-print(x)  # 2.79 PiB
-```
-
-
-## FAQ
-
-- 
-
-
-## Changelog
-
-- 2.0.0 (June 13, 2023):
-    - Breaking changes:
-        - New mechanism for app: `/app/__init__.py`
-        - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
-        - transform: `/kit/quick_visual/plot2d.py` -> `/kit/fast_visualizations/static/plot.py`
-    - Bugfixed:
-        - folder `mykit/tests/` should also be excluded during build (rc version)
-    - New: `/app/complex/biplot.py`
-- 1.0.0 (June 12, 2023):
-    - changed arg name: `/kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
-- 0.1.3 (June 12, 2023):
-    - removed `get_gray` from `/kit/color.py`
-    - transform `/kit/gui/button/` -> `/app/button.py`
-    - transform `/kit/gui/label/` -> `/app/label.py`
-    - transform `/kit/gui/slider/` -> `/app/slider.py`
-    - transform `/kit/gui/shape/` -> `/app/arrow.py`
-    - transform `/kit/neuralnet/dense/` -> `/kit/neuralnet/dense.py`
-    - transform `/kit/neuralnet/genetic/` -> `/kit/neuralnet/genetic.py`
-- 0.1.0 (June 12, 2023):
-    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `/kit/`
-    - deleted `/kit/math/`
-    - added `/rec/` and `/app/`
-    - transform `/kit/color/` -> `/kit/color.py`
-    - moved `/kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
-    - transform `/kit/ffmpeg/` -> `/kit/ffmpeg.py`
-    - deleted `/kit/graph/graph2d/`
-    - transform `/kit/graph/graph2d/v2.py` -> `/kit/graph/graph2d.py`
-    - transform `/kit/maths/` -> `/kit/math.py`
-    - moved `/kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
-    - transform `/kit/noise/` -> `/kit/noise.py`
-    - transform `/kit/path/` -> `/kit/path.py`
-    - transform `/kit/text/` -> `/kit/text.py`
-    - transform `/kit/time/` -> `/kit/time.py`
-    - transform `/kit/utils/` -> `/kit/utils.py`
-
-
-## Troubleshoot
-
-- To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
-
-
-## License
-
-This project is licensed under the MIT license.
+# myKit
+
+Python utility toolkit.
+
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
+
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
+
+## Installation
+
+```sh
+pip install mykit
+```
+
+
+## Usage
+
+```python
+from mykit.kit.text import byteFmt
+from mykit.app.arrow import Arrow
+from mykit.app.slider import Slider
+
+
+x = byteFmt(3141592653589793)
+print(x)  # 2.79 PiB
+```
+
+
+## FAQ
+
+- 
+
+
+## Changelog
+
+- 2.0.1 (June 14, 2023):
+    - Updated all type hints to make them work on Python 3.8 and 3.9
+    - Added visibility functionality to `/app/complex/biplot.py`
+- 2.0.0 (June 13, 2023):
+    - Breaking changes:
+        - New mechanism for app: `/app/__init__.py`
+        - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
+        - transform: `/kit/quick_visual/plot2d.py` -> `/kit/fast_visualizations/static/plot.py`
+    - Bugfixed:
+        - folder `mykit/tests/` should also be excluded during build (rc version)
+    - New: `/app/complex/biplot.py`
+- 1.0.0 (June 12, 2023):
+    - changed arg name: `/kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
+- 0.1.3 (June 12, 2023):
+    - removed `get_gray` from `/kit/color.py`
+    - transform `/kit/gui/button/` -> `/app/button.py`
+    - transform `/kit/gui/label/` -> `/app/label.py`
+    - transform `/kit/gui/slider/` -> `/app/slider.py`
+    - transform `/kit/gui/shape/` -> `/app/arrow.py`
+    - transform `/kit/neuralnet/dense/` -> `/kit/neuralnet/dense.py`
+    - transform `/kit/neuralnet/genetic/` -> `/kit/neuralnet/genetic.py`
+- 0.1.0 (June 12, 2023):
+    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `/kit/`
+    - deleted `/kit/math/`
+    - added `/rec/` and `/app/`
+    - transform `/kit/color/` -> `/kit/color.py`
+    - moved `/kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
+    - transform `/kit/ffmpeg/` -> `/kit/ffmpeg.py`
+    - deleted `/kit/graph/graph2d/`
+    - transform `/kit/graph/graph2d/v2.py` -> `/kit/graph/graph2d.py`
+    - transform `/kit/maths/` -> `/kit/math.py`
+    - moved `/kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
+    - transform `/kit/noise/` -> `/kit/noise.py`
+    - transform `/kit/path/` -> `/kit/path.py`
+    - transform `/kit/text/` -> `/kit/text.py`
+    - transform `/kit/time/` -> `/kit/time.py`
+    - transform `/kit/utils/` -> `/kit/utils.py`
+
+
+## Troubleshoot
+
+- To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
+
+
+## License
+
+This project is licensed under the MIT license.
```

### Comparing `mykit-2.0.0rc3/mykit/app/__init__.py` & `mykit-2.0.1/mykit/app/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import tkinter as _tk
-import typing as _typing
-
-from mykit.app._runtime import Runtime as _Rt
-from mykit.app.button import Button as _Button
-from mykit.app.label import Label as _Label
-from mykit.app.slider import _Slider
-
-
-class App(_Rt):
-    """
-    Single-page app.
-
-    ---
-
-    ## Limitations
-    - currently available only in fullscreen mode
-    """
-
-    def __init__(self, title: str = 'app', bg: str = '#111111') -> None:
-        
-        self.root = _tk.Tk()
-        self.root.attributes('-fullscreen', True)
-        self.root.title(title)
-
-        page = _tk.Canvas(
-            master=self.root,
-            width=self.root.winfo_screenwidth(),
-            height=self.root.winfo_screenheight(),
-            background=bg,
-            borderwidth=0, highlightthickness=0
-        )
-        page.place(x=0, y=0)
-        App._set_page(page)
-
-
-        ## <constants>
-        self.MON_WIDTH = self.root.winfo_screenwidth()
-        self.MON_HEIGHT = self.root.winfo_screenheight()
-        ## </constants>
-
-
-        ## <runtime>
-        self._left_mouse_press = []
-        self._left_mouse_hold = []
-        self._left_mouse_release = []
-
-        self._setup = None
-        self._teardown = None
-        ## </runtime>
-
-    def listen(self, to: str, do: _typing.Callable[[_tk.Event], None]):
-        """
-        Add event listener.
-
-        ---
-
-        ## Params
-        - `to`: `Literal["left-mouse-press", "left-mouse-hold", "left-mouse-release"]`
-
-        ## Docs
-        - `do` function takes 1 positional parameter, which is a tkinter event object
-        """
-        
-        if to == 'left-mouse-press':
-            self._left_mouse_press.append(do)
-        elif to == 'left-mouse-hold':
-            self._left_mouse_hold.append(do)
-        elif to == 'left-mouse-release':
-            self._left_mouse_release.append(do)
-        else:
-            ValueError(f'Invalid event: {repr(to)}.')
-
-    def setup(self, funcs: list[_typing.Callable[[], None]]):
-        self._setup = funcs
-
-    def teardown(self, funcs: list[_typing.Callable[[], None]]):
-        self._teardown = funcs
-
-    def run(self):
-        
-        ## <listeners>
-
-        def left_mouse_press(e):
-            
-            ## internal
-            _Button.press_listener()
-            _Slider.press_listener()
-            
-            ## external
-            for fn in self._left_mouse_press:
-                fn(e)
-
-        self.root.bind('<ButtonPress-1>', left_mouse_press)
-
-        def left_mouse_hold(e):
-            
-            ## internal
-            _Slider.hold_listener()
-
-            ## external
-            for fn in self._left_mouse_hold:
-                fn(e)
-
-        self.root.bind('<B1-Motion>', left_mouse_hold)
-
-        def left_mouse_release(e):
-
-            ## internal
-            _Button.release_listener()
-            _Slider.release_listener()
-
-            ## external
-            for fn in self._left_mouse_release:
-                fn(e)
-        self.root.bind('<ButtonRelease-1>', left_mouse_release)
-
-        self.root.bind('<Escape>', lambda e: self.root.destroy())
-
-        ## </listeners>
-
-
-        ## <background processes>
-        
-        def repeat50():
-            _Button.hover_listener()
-            _Slider.hover_listener()
-            self.root.after(50, repeat50)
-        repeat50()
-        
-        ## </background processes>
-
-
-        ## setup
-        if self._setup is not None:
-            for fn in self._setup:
-                fn()
-
-
-        ## run
-        self.root.mainloop()
-
-
-        ## teardown
-        if self._teardown is not None:
-            for fn in self._teardown:
+import tkinter as _tk
+import typing as _typing
+
+from mykit.app._runtime import Runtime as _Rt
+from mykit.app.button import Button as _Button
+from mykit.app.label import Label as _Label
+from mykit.app.slider import _Slider
+
+
+class App(_Rt):
+    """
+    Single-page app.
+
+    ---
+
+    ## Limitations
+    - currently available only in fullscreen mode
+    """
+
+    def __init__(self, title: str = 'app', bg: str = '#111111') -> None:
+        
+        self.root = _tk.Tk()
+        self.root.attributes('-fullscreen', True)
+        self.root.title(title)
+
+        page = _tk.Canvas(
+            master=self.root,
+            width=self.root.winfo_screenwidth(),
+            height=self.root.winfo_screenheight(),
+            background=bg,
+            borderwidth=0, highlightthickness=0
+        )
+        page.place(x=0, y=0)
+        App._set_page(page)
+
+
+        ## <constants>
+        self.MON_WIDTH = self.root.winfo_screenwidth()
+        self.MON_HEIGHT = self.root.winfo_screenheight()
+        ## </constants>
+
+
+        ## <runtime>
+        self._left_mouse_press = []
+        self._left_mouse_hold = []
+        self._left_mouse_release = []
+
+        self._setup = None
+        self._teardown = None
+        ## </runtime>
+
+    def listen(self, to: str, do: _typing.Callable[[_tk.Event], None]):
+        """
+        Add event listener.
+
+        ---
+
+        ## Params
+        - `to`: `Literal["left-mouse-press", "left-mouse-hold", "left-mouse-release"]`
+
+        ## Docs
+        - `do` function takes 1 positional parameter, which is a tkinter event object
+        """
+        
+        if to == 'left-mouse-press':
+            self._left_mouse_press.append(do)
+        elif to == 'left-mouse-hold':
+            self._left_mouse_hold.append(do)
+        elif to == 'left-mouse-release':
+            self._left_mouse_release.append(do)
+        else:
+            ValueError(f'Invalid event: {repr(to)}.')
+
+    def setup(self, funcs: list[_typing.Callable[[], None]]):
+        self._setup = funcs
+
+    def teardown(self, funcs: list[_typing.Callable[[], None]]):
+        self._teardown = funcs
+
+    def run(self):
+        
+        ## <listeners>
+
+        def left_mouse_press(e):
+            
+            ## internal
+            _Button.press_listener()
+            _Slider.press_listener()
+            
+            ## external
+            for fn in self._left_mouse_press:
+                fn(e)
+
+        self.root.bind('<ButtonPress-1>', left_mouse_press)
+
+        def left_mouse_hold(e):
+            
+            ## internal
+            _Slider.hold_listener()
+
+            ## external
+            for fn in self._left_mouse_hold:
+                fn(e)
+
+        self.root.bind('<B1-Motion>', left_mouse_hold)
+
+        def left_mouse_release(e):
+
+            ## internal
+            _Button.release_listener()
+            _Slider.release_listener()
+
+            ## external
+            for fn in self._left_mouse_release:
+                fn(e)
+        self.root.bind('<ButtonRelease-1>', left_mouse_release)
+
+        self.root.bind('<Escape>', lambda e: self.root.destroy())
+
+        ## </listeners>
+
+
+        ## <background processes>
+        
+        def repeat50():
+            _Button.hover_listener()
+            _Slider.hover_listener()
+            self.root.after(50, repeat50)
+        repeat50()
+        
+        ## </background processes>
+
+
+        ## setup
+        if self._setup is not None:
+            for fn in self._setup:
+                fn()
+
+
+        ## run
+        self.root.mainloop()
+
+
+        ## teardown
+        if self._teardown is not None:
+            for fn in self._teardown:
                 fn()
```

### Comparing `mykit-2.0.0rc3/mykit/app/arrow.py` & `mykit-2.0.1/mykit/app/arrow.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import math as _math
-import random as _random
-
-from mykit.app._runtime import Runtime as _Rt
-from mykit.kit.math import (
-    get_angle as _get_angle,
-    rotate as _rotate
-)
-
-
-class Arrow(_Rt):
-
-    arrows: dict[str, 'Arrow'] = {}
-    arrow_tags: dict[str, list['Arrow']] = {}
-
-    def __init__(
-        self,
-        from_x: int, from_y: int,
-        to_x: int, to_y: int,
-        /,
-        color: str = '#ddd',
-        width_rod: int = 1,
-        width_tip: int = 2,
-        tip_len: float = 20,
-        tip_angle: float = 35,
-        visible: bool = True,
-        id: str | None = None,
-        tags: str | list[str] | None = None,
-    ) -> None:
-
-        if Arrow.page is None:
-            raise AssertionError('App has not been initialized.')
-        
-        self.from_x = from_x
-        self.from_y = from_y
-        self.to_x = to_x
-        self.to_y = to_y
-
-        self.color = color
-        self.width_rod = width_rod
-        self.width_tip = width_tip
-        self.tip_len = tip_len
-        self.tip_angle = tip_angle
-
-        self.visible = visible
-
-        ## to make sure that we can modify a specific arrow without affecting the others
-        if id is None:
-            self.id = _random.randint(-10000, 10000)
-            while self.id in Arrow.arrows:
-                self.id = _random.randint(-10000, 10000)
-        else:
-            self.id = id
-            if self.id in Arrow.arrows:
-                raise ValueError(f'The Arrow\'s id {repr(id)} is duplicated.')
-        Arrow.arrows[self.id] = self
-
-        ## <tags>
-        if type(tags) is str:
-            self.tags = [tags]
-        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
-            self.tags = tags
-        
-        if tags is not None:
-            for tag in self.tags:
-                if tag in Arrow.arrow_tags:
-                    Arrow.arrow_tags[tag].append(self)
-                else:
-                    Arrow.arrow_tags[tag] = [self]
-        ## </tags>
-
-        ## init
-        self._redraw()
-
-    def _redraw(self):
-
-        Arrow.page.delete(f'Arrow_{self.id}')
-
-        if self.visible:
-            Arrow.page.create_line(
-                self.from_x, self.from_y,
-                self.to_x, self.to_y,
-                fill=self.color, width=self.width_rod, tags=f'Arrow_{self.id}'
-            )
-
-            ## <creating the tip>
-            ## for `angle`: remember to flip the y-sign because tkinter's y-positive direction towards the bottom
-            angle = _get_angle(self.from_x, -self.from_y, self.to_x, -self.to_y)
-            
-            tipx = self.tip_len*_math.sin(self.tip_angle*_math.pi/180)
-            tipy = self.tip_len*_math.cos(self.tip_angle*_math.pi/180)
-            
-            ## Remember `tip_left` and `tip_right` with y-positive towards the top,
-            ## as they transformed under normal Cartesian coordinates.
-            tip_left = _rotate(-tipx, -tipy, 0, 0, angle)
-            tip_right = _rotate(tipx, -tipy, 0, 0, angle)
-
-            ## Revert to the tkinter coordinate scheme, where y-positive is oriented downwards.
-            tip_left = (self.to_x+tip_left[0], self.to_y-tip_left[1])
-            tip_right = (self.to_x+tip_right[0], self.to_y-tip_right[1])
-
-            tip_points = [tip_left, (self.to_x, self.to_y), tip_right]
-            Arrow.page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
-            ## </creating the tip>
-
-
-    def set_visibility(self, visible: bool, /):
-        if visible != self.visible:
-            self.visible = visible
-            self._redraw()
-
-    @staticmethod
-    def set_visibility_by_id(id: str, visible: bool, /):
-        Arrow.arrows[id].set_visibility(visible)
-
-    @staticmethod
-    def set_visibility_by_tag(tag: str, visible: bool, /):
-        for arrow in Arrow.arrow_tags[tag]:
-            arrow.set_visibility(visible)
-
-    @staticmethod
-    def set_visibility_all(visible: bool, /):
-        for arrow in Arrow.arrows.values():
+import math as _math
+import random as _random
+
+from mykit.app._runtime import Runtime as _Rt
+from mykit.kit.math import (
+    get_angle as _get_angle,
+    rotate as _rotate
+)
+
+
+class Arrow(_Rt):
+
+    arrows: dict[str, 'Arrow'] = {}
+    arrow_tags: dict[str, list['Arrow']] = {}
+
+    def __init__(
+        self,
+        from_x: int, from_y: int,
+        to_x: int, to_y: int,
+        /,
+        color: str = '#ddd',
+        width_rod: int = 1,
+        width_tip: int = 2,
+        tip_len: float = 20,
+        tip_angle: float = 35,
+        visible: bool = True,
+        id: str | None = None,
+        tags: str | list[str] | None = None,
+    ) -> None:
+
+        if Arrow.page is None:
+            raise AssertionError('App has not been initialized.')
+        
+        self.from_x = from_x
+        self.from_y = from_y
+        self.to_x = to_x
+        self.to_y = to_y
+
+        self.color = color
+        self.width_rod = width_rod
+        self.width_tip = width_tip
+        self.tip_len = tip_len
+        self.tip_angle = tip_angle
+
+        self.visible = visible
+
+        ## to make sure that we can modify a specific arrow without affecting the others
+        if id is None:
+            self.id = _random.randint(-10000, 10000)
+            while self.id in Arrow.arrows:
+                self.id = _random.randint(-10000, 10000)
+        else:
+            self.id = id
+            if self.id in Arrow.arrows:
+                raise ValueError(f'The Arrow\'s id {repr(id)} is duplicated.')
+        Arrow.arrows[self.id] = self
+
+        ## <tags>
+        if type(tags) is str:
+            self.tags = [tags]
+        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
+            self.tags = tags
+        
+        if tags is not None:
+            for tag in self.tags:
+                if tag in Arrow.arrow_tags:
+                    Arrow.arrow_tags[tag].append(self)
+                else:
+                    Arrow.arrow_tags[tag] = [self]
+        ## </tags>
+
+        ## init
+        self._redraw()
+
+    def _redraw(self):
+
+        Arrow.page.delete(f'Arrow_{self.id}')
+
+        if self.visible:
+            Arrow.page.create_line(
+                self.from_x, self.from_y,
+                self.to_x, self.to_y,
+                fill=self.color, width=self.width_rod, tags=f'Arrow_{self.id}'
+            )
+
+            ## <creating the tip>
+            ## for `angle`: remember to flip the y-sign because tkinter's y-positive direction towards the bottom
+            angle = _get_angle(self.from_x, -self.from_y, self.to_x, -self.to_y)
+            
+            tipx = self.tip_len*_math.sin(self.tip_angle*_math.pi/180)
+            tipy = self.tip_len*_math.cos(self.tip_angle*_math.pi/180)
+            
+            ## Remember `tip_left` and `tip_right` with y-positive towards the top,
+            ## as they transformed under normal Cartesian coordinates.
+            tip_left = _rotate(-tipx, -tipy, 0, 0, angle)
+            tip_right = _rotate(tipx, -tipy, 0, 0, angle)
+
+            ## Revert to the tkinter coordinate scheme, where y-positive is oriented downwards.
+            tip_left = (self.to_x+tip_left[0], self.to_y-tip_left[1])
+            tip_right = (self.to_x+tip_right[0], self.to_y-tip_right[1])
+
+            tip_points = [tip_left, (self.to_x, self.to_y), tip_right]
+            Arrow.page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
+            ## </creating the tip>
+
+
+    def set_visibility(self, visible: bool, /):
+        if visible != self.visible:
+            self.visible = visible
+            self._redraw()
+
+    @staticmethod
+    def set_visibility_by_id(id: str, visible: bool, /):
+        Arrow.arrows[id].set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_by_tag(tag: str, visible: bool, /):
+        for arrow in Arrow.arrow_tags[tag]:
+            arrow.set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_all(visible: bool, /):
+        for arrow in Arrow.arrows.values():
             arrow.set_visibility(visible)
```

### Comparing `mykit-2.0.0rc3/mykit/app/label.py` & `mykit-2.0.1/mykit/app/label.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-import random as _random
-import tkinter as _tk
-import typing as _typing
-
-
-class Label:
-
-    labels: dict[str, 'Label'] = {}
-    label_tags: dict[str, list['Label']] = {}
-
-    def __init__(
-        self,
-        x: int = 0,
-        y: int = 0,
-        text: str = '',
-        font: str | tuple[str, int] = 'Verdana 10',
-        justify: str = 'left',
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
-        fg: str = '#ccc',
-        bg: str = '#111',
-        bd: str = '#555',
-        bd_width: int = 0,
-        wraplength: int = 1000,
-        padx: int = 0,
-        pady: int = 0,
-        visible: bool = True,
-
-        id: str | None = None,
-        tags: str | list[str] | None = None,
-    ):
-        """
-        `x`: the x-position for the `anchor` argument, not the center of the label
-        `y`: the y-position for the `anchor` argument, not the center of the label
-        """
-
-        self.x = x  # reminder: this is the x-position for the `anchor` argument, not the center of the label
-        self.y = y  # reminder: this is the y-position for the `anchor` argument, not the center of the label
-        self.font = font
-        self.text = text
-        self.anchor = anchor
-        self.fg = fg
-        self.visible = visible
-
-        self.default_text = text
-
-        self.label = _tk.Label(
-            text=text, font=font, justify=justify,
-            foreground=fg, background=bg,
-            highlightbackground=bd, highlightthickness=bd_width,
-            wraplength=wraplength,
-            padx=padx, pady=pady
-        )
-
-        if visible:
-            self.label.place(x=x, y=y, anchor=anchor)
-
-        ## self.id ensures that we can modify a specific instance without affecting the others
-        if id is None:
-            self.id = str(_random.randint(0, 100_000))
-            while self.id in Label.labels:
-                self.id = str(_random.randint(0, 100_000))
-        else:
-            self.id = id
-            if self.id in Label.labels:
-                raise ValueError(f'The id {repr(id)} is duplicated.')
-        Label.labels[self.id] = self
-
-        ## <tags>
-        if type(tags) is str:
-            self.tags = [tags]
-        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
-            self.tags = tags
-        
-        if tags is not None:
-            for tag in self.tags:
-                if tag in Label.label_tags:
-                    Label.label_tags[tag].append(self)
-                else:
-                    Label.label_tags[tag] = [self]
-        ## <tags>
-
-
-    def set_text(self, text: str | None, /):
-        """if None -> set default text."""
-
-        if text is None:
-            text = self.default_text
-
-        if text != self.text:
-            self.text = text
-            self.label.configure(text=text)
-
-    @staticmethod
-    def set_text_by_id(id: str, text: str | None, /):
-        Label.labels[id].set_text(text)
-
-
-    def set_font(self, font: str | tuple[str, int], /):
-        if font != self.font:
-            self.font = font
-            self.label.configure(font=font)
-
-    @staticmethod
-    def set_font_by_id(id: str, font: str | tuple[str, int], /):
-        Label.labels[id].set_font(font)
-
-
-    def set_fg(self, fg: str, /):
-        if fg != self.fg:
-            self.fg = fg
-            self.label.configure(fg=fg)
-
-    @staticmethod
-    def set_fg_by_id(id: str, fg: str, /):
-        Label.labels[id].set_fg(fg)
-
-
-    def set_visibility(self, visible: bool, /):
-        if self.visible is not visible:
-            self.visible = visible
-            if visible:
-                self.label.place(x=self.x, y=self.y, anchor=self.anchor)
-            else:
-                self.label.place_forget()
-
-    @staticmethod
-    def set_visibility_by_id(id: str, visible: bool, /):
-        Label.labels[id].set_visibility(visible)
-
-    @staticmethod
-    def set_visibility_by_tag(tag: str, visible: bool, /):
-        for label in Label.label_tags[tag]:
-            label.set_visibility(visible)
-
-    @staticmethod
-    def set_visibility_all(visible: bool, /):
-        for label in Label.labels.values():
-            label.set_visibility(visible)
-
-
-    def get_width(self) -> int:
-        return self.label.winfo_reqwidth()
-
-    @staticmethod
-    def get_width_by_id(id: str, /) -> int:
-        return Label.labels[id].get_width()
-
-    def get_height(self) -> int:
-        return self.label.winfo_reqheight()
-
-    @staticmethod
-    def get_height_by_id(id: str, /) -> int:
-        return Label.labels[id].get_height()
-
-
-    def get_anchor_loc(self, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
-        """To get the center of the label coordinates, use `anchor='center'`"""
-
-        W = self.get_width()
-        H = self.get_height()
-
-        ## get the coordinates for the center (X, Y)
-        if self.anchor == 'center':
-            X = self.x
-            Y = self.y
-        elif self.anchor == 'n':
-            X = self.x
-            Y = self.y + H/2
-        elif self.anchor == 'ne':
-            X = self.x - W/2
-            Y = self.y + H/2
-        elif self.anchor == 'e':
-            X = self.x - W/2
-            Y = self.y
-        elif self.anchor == 'se':
-            X = self.x - W/2
-            Y = self.y - H/2
-        elif self.anchor == 's':
-            X = self.x
-            Y = self.y - H/2
-        elif self.anchor == 'sw':
-            X = self.x + W/2
-            Y = self.y - H/2
-        elif self.anchor == 'w':
-            X = self.x + W/2
-            Y = self.y
-        elif self.anchor == 'nw':
-            X = self.x + W/2
-            Y = self.y + H/2
-
-        ## returning the requested anchor location
-        if anchor == 'center':
-            return (X, Y)
-        elif anchor == 'n':
-            return (X, Y-H/2)
-        elif anchor == 'ne':
-            return (X+W/2, Y-H/2)
-        elif anchor == 'e':
-            return (X+W/2, Y)
-        elif anchor == 'se':
-            return (X+W/2, Y+H/2)
-        elif anchor == 's':
-            return (X, Y+H/2)
-        elif anchor == 'sw':
-            return (X-W/2, Y+H/2)
-        elif anchor == 'w':
-            return (X-W/2, Y)
-        elif anchor == 'nw':
-            return (X-W/2, Y-H/2)
-        else:
-            raise ValueError(f'Invalid anchor value: {repr(anchor)}')
-
-    @staticmethod
-    def get_anchor_loc_by_id(id: str, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
-        return Label.labels[id].get_anchor_loc(anchor)
-
-    
-    def move(self, x: int, y: int, /, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] | None = None) -> None:
-        """If `anchor = None`, the current anchor will be used."""
-        self.x = x
-        self.y = y
-        if anchor is not None:
-            self.anchor = anchor
-        # self.label.place(x=x, y=y, anchor=anchor)  # reminder: don't do this because `anchor` could be `None`
-        self.label.place(x=x, y=y, anchor=self.anchor)
-
-    @staticmethod
-    def move_by_id(
-        id: str,
-        x: int,
-        y: int,
-        /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
-        Label.labels[id].move(x, y, anchor)
-
-
-    def align(
-        self,
-        target: 'Label',
-        anchor: str = 'nw',
-        target_anchor: str = 'ne',
-        xgap: float = 15,
-        ygap: float = 0
-    ) -> 'Label':
-        """
-        Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
-        """
-
-        ## getting the target anchor location
-        x, y = target.get_anchor_loc(target_anchor)
-
-        ## shifting
-        x += xgap
-        y += ygap
-
-        ## moving the label
-        self.move(x, y, anchor)
-
-        ## return the instance so that this method can also be used when
-        ## creating the instance, like `label_2 = Label(text='foo').align(label_1)`.
-        return self
-
-
-    def destroy(self) -> None:
-        Label.labels.pop(self.id)
-
-        if self.tags is not None:
-            for tag in list(self.tags):
-                Label.label_tags[tag].remove(self)
-                if Label.label_tags[tag] == []:
-                    Label.label_tags.pop(tag)
-        
-        self.label.destroy()
-    
-    @staticmethod
-    def destroy_by_id(id: str, /) -> None:
-        Label.labels[id].destroy()
-
-    @staticmethod
-    def destroy_by_tag(tag: str, /) -> None:
-        for label in list(Label.label_tags[tag]):
-            label.destroy()
-
-    @staticmethod
-    def destroy_all() -> None:
-        for label in list(Label.labels.values()):
+import random as _random
+import tkinter as _tk
+import typing as _typing
+
+
+class Label:
+
+    labels: dict[str, 'Label'] = {}
+    label_tags: dict[str, list['Label']] = {}
+
+    def __init__(
+        self,
+        x: int = 0,
+        y: int = 0,
+        text: str = '',
+        font: str | tuple[str, int] = 'Verdana 10',
+        justify: str = 'left',
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        fg: str = '#ccc',
+        bg: str = '#111',
+        bd: str = '#555',
+        bd_width: int = 0,
+        wraplength: int = 1000,
+        padx: int = 0,
+        pady: int = 0,
+        visible: bool = True,
+
+        id: str | None = None,
+        tags: str | list[str] | None = None,
+    ):
+        """
+        `x`: the x-position for the `anchor` argument, not the center of the label
+        `y`: the y-position for the `anchor` argument, not the center of the label
+        """
+
+        self.x = x  # reminder: this is the x-position for the `anchor` argument, not the center of the label
+        self.y = y  # reminder: this is the y-position for the `anchor` argument, not the center of the label
+        self.font = font
+        self.text = text
+        self.anchor = anchor
+        self.fg = fg
+        self.visible = visible
+
+        self.default_text = text
+
+        self.label = _tk.Label(
+            text=text, font=font, justify=justify,
+            foreground=fg, background=bg,
+            highlightbackground=bd, highlightthickness=bd_width,
+            wraplength=wraplength,
+            padx=padx, pady=pady
+        )
+
+        if visible:
+            self.label.place(x=x, y=y, anchor=anchor)
+
+        ## self.id ensures that we can modify a specific instance without affecting the others
+        if id is None:
+            self.id = str(_random.randint(0, 100_000))
+            while self.id in Label.labels:
+                self.id = str(_random.randint(0, 100_000))
+        else:
+            self.id = id
+            if self.id in Label.labels:
+                raise ValueError(f'The id {repr(id)} is duplicated.')
+        Label.labels[self.id] = self
+
+        ## <tags>
+        if type(tags) is str:
+            self.tags = [tags]
+        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
+            self.tags = tags
+        
+        if tags is not None:
+            for tag in self.tags:
+                if tag in Label.label_tags:
+                    Label.label_tags[tag].append(self)
+                else:
+                    Label.label_tags[tag] = [self]
+        ## <tags>
+
+
+    def set_text(self, text: str | None, /):
+        """if None -> set default text."""
+
+        if text is None:
+            text = self.default_text
+
+        if text != self.text:
+            self.text = text
+            self.label.configure(text=text)
+
+    @staticmethod
+    def set_text_by_id(id: str, text: str | None, /):
+        Label.labels[id].set_text(text)
+
+
+    def set_font(self, font: str | tuple[str, int], /):
+        if font != self.font:
+            self.font = font
+            self.label.configure(font=font)
+
+    @staticmethod
+    def set_font_by_id(id: str, font: str | tuple[str, int], /):
+        Label.labels[id].set_font(font)
+
+
+    def set_fg(self, fg: str, /):
+        if fg != self.fg:
+            self.fg = fg
+            self.label.configure(fg=fg)
+
+    @staticmethod
+    def set_fg_by_id(id: str, fg: str, /):
+        Label.labels[id].set_fg(fg)
+
+
+    def set_visibility(self, visible: bool, /):
+        if self.visible is not visible:
+            self.visible = visible
+            if visible:
+                self.label.place(x=self.x, y=self.y, anchor=self.anchor)
+            else:
+                self.label.place_forget()
+
+    @staticmethod
+    def set_visibility_by_id(id: str, visible: bool, /):
+        Label.labels[id].set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_by_tag(tag: str, visible: bool, /):
+        for label in Label.label_tags[tag]:
+            label.set_visibility(visible)
+
+    @staticmethod
+    def set_visibility_all(visible: bool, /):
+        for label in Label.labels.values():
+            label.set_visibility(visible)
+
+
+    def get_width(self) -> int:
+        return self.label.winfo_reqwidth()
+
+    @staticmethod
+    def get_width_by_id(id: str, /) -> int:
+        return Label.labels[id].get_width()
+
+    def get_height(self) -> int:
+        return self.label.winfo_reqheight()
+
+    @staticmethod
+    def get_height_by_id(id: str, /) -> int:
+        return Label.labels[id].get_height()
+
+
+    def get_anchor_loc(self, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
+        """To get the center of the label coordinates, use `anchor='center'`"""
+
+        W = self.get_width()
+        H = self.get_height()
+
+        ## get the coordinates for the center (X, Y)
+        if self.anchor == 'center':
+            X = self.x
+            Y = self.y
+        elif self.anchor == 'n':
+            X = self.x
+            Y = self.y + H/2
+        elif self.anchor == 'ne':
+            X = self.x - W/2
+            Y = self.y + H/2
+        elif self.anchor == 'e':
+            X = self.x - W/2
+            Y = self.y
+        elif self.anchor == 'se':
+            X = self.x - W/2
+            Y = self.y - H/2
+        elif self.anchor == 's':
+            X = self.x
+            Y = self.y - H/2
+        elif self.anchor == 'sw':
+            X = self.x + W/2
+            Y = self.y - H/2
+        elif self.anchor == 'w':
+            X = self.x + W/2
+            Y = self.y
+        elif self.anchor == 'nw':
+            X = self.x + W/2
+            Y = self.y + H/2
+
+        ## returning the requested anchor location
+        if anchor == 'center':
+            return (X, Y)
+        elif anchor == 'n':
+            return (X, Y-H/2)
+        elif anchor == 'ne':
+            return (X+W/2, Y-H/2)
+        elif anchor == 'e':
+            return (X+W/2, Y)
+        elif anchor == 'se':
+            return (X+W/2, Y+H/2)
+        elif anchor == 's':
+            return (X, Y+H/2)
+        elif anchor == 'sw':
+            return (X-W/2, Y+H/2)
+        elif anchor == 'w':
+            return (X-W/2, Y)
+        elif anchor == 'nw':
+            return (X-W/2, Y-H/2)
+        else:
+            raise ValueError(f'Invalid anchor value: {repr(anchor)}')
+
+    @staticmethod
+    def get_anchor_loc_by_id(id: str, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'], /) -> tuple[int, int]:
+        return Label.labels[id].get_anchor_loc(anchor)
+
+    
+    def move(self, x: int, y: int, /, anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] | None = None) -> None:
+        """If `anchor = None`, the current anchor will be used."""
+        self.x = x
+        self.y = y
+        if anchor is not None:
+            self.anchor = anchor
+        # self.label.place(x=x, y=y, anchor=anchor)  # reminder: don't do this because `anchor` could be `None`
+        self.label.place(x=x, y=y, anchor=self.anchor)
+
+    @staticmethod
+    def move_by_id(
+        id: str,
+        x: int,
+        y: int,
+        /,
+        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
+        Label.labels[id].move(x, y, anchor)
+
+
+    def align(
+        self,
+        target: 'Label',
+        anchor: str = 'nw',
+        target_anchor: str = 'ne',
+        xgap: float = 15,
+        ygap: float = 0
+    ) -> 'Label':
+        """
+        Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
+        """
+
+        ## getting the target anchor location
+        x, y = target.get_anchor_loc(target_anchor)
+
+        ## shifting
+        x += xgap
+        y += ygap
+
+        ## moving the label
+        self.move(x, y, anchor)
+
+        ## return the instance so that this method can also be used when
+        ## creating the instance, like `label_2 = Label(text='foo').align(label_1)`.
+        return self
+
+
+    def destroy(self) -> None:
+        Label.labels.pop(self.id)
+
+        if self.tags is not None:
+            for tag in list(self.tags):
+                Label.label_tags[tag].remove(self)
+                if Label.label_tags[tag] == []:
+                    Label.label_tags.pop(tag)
+        
+        self.label.destroy()
+    
+    @staticmethod
+    def destroy_by_id(id: str, /) -> None:
+        Label.labels[id].destroy()
+
+    @staticmethod
+    def destroy_by_tag(tag: str, /) -> None:
+        for label in list(Label.label_tags[tag]):
+            label.destroy()
+
+    @staticmethod
+    def destroy_all() -> None:
+        for label in list(Label.labels.values()):
             label.destroy()
```

### Comparing `mykit-2.0.0rc3/mykit/app/slider.py` & `mykit-2.0.1/mykit/app/slider.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,817 +1,817 @@
-import random as _random
-import tkinter as _tk
-import typing as _typing
-
-from mykit.app._runtime import Runtime as _Rt
-from mykit.kit.utils import minmax_normalization as _norm
-
-
-class _Slider(_Rt):
-
-    sliders: dict[str, '_Slider'] = {}
-    slider_tags: dict[str, list['_Slider']] = {}  # note that the horizontal and vertical sliders store the tags together
-
-    def __init__(
-        self,
-        min: float = 0,
-        max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
-
-        x: int = 0,
-        y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
-        tolerance: float = 0.25,
-        
-        label: _typing.Optional[str] = None,
-        label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
-        show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
-        label_y_shift: int = -15,
-
-        show_value: bool = True,
-        value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
-        value_prefix: str = '',
-        value_suffix: str = '',
-        show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
-
-        rod_len: int = 200,
-        rod_thick: int = 3,
-        btn_r: int = 5,
-        color_rod_normal: str = '#4b4b4b',
-        color_rod_locked: str = '#2d2d2d',
-        color_btn_normal: str = '#555555',
-        color_btn_locked: str = '#373737',
-        color_btn_press: str = '#7d7d7d',
-        color_btn_hover: str = '#696969',
-        color_btn_bd_normal: str = '#f5f5f5',
-        color_btn_bd_locked: str = '#373737',
-
-        locked: bool = False,
-        visible: bool = True,
-
-        id: str | None = None,
-        tags: str | list[str] | None = None,
-    ) -> None:
-        """
-        ## Params
-        - `x` and `y` is the position of the `anchor` (not the center of the button)
-        - `tolerance`: to determine how closely the cursor needs to be to the slider's step values for it to move to a new value
-
-        ## Docs
-        - box color, width, and height should be provided if the box shown
-        """
-
-        if _Slider.page is None:
-            raise AssertionError('App has not been initialized.')
-
-        self.min = min
-        self.max = max
-        self.step = step if step is not None else (max-min)/10
-        self.init = init if init is not None else (max-min)/2
-        self.fn = fn
-
-        self.x = x
-        self.y = y
-        self.anchor = anchor
-        self.tolerance = tolerance
-
-        self.label = label
-        self.label_fg = label_fg
-        self.label_font = label_font
-        self.show_label_box = show_label_box
-        self.label_box_color = label_box_color
-        self.label_box_width = label_box_width
-        self.label_box_height = label_box_height
-        self.label_y_shift = label_y_shift
-
-        self.show_value = show_value
-        self.value_fg = value_fg
-        self.value_font = value_font
-        self.value_prefix = value_prefix
-        self.value_suffix = value_suffix
-        self.show_value_box = show_value_box
-        self.value_box_color = value_box_color
-        self.value_box_width = value_box_width
-        self.value_box_height = value_box_height
-
-        self.rod_len = rod_len
-        self.rod_thick = rod_thick
-        self.btn_r = btn_r
-        self.color_rod_normal = color_rod_normal
-        self.color_rod_locked = color_rod_locked
-        self.color_btn_normal = color_btn_normal
-        self.color_btn_locked = color_btn_locked
-        self.color_btn_press = color_btn_press
-        self.color_btn_hover = color_btn_hover
-        self.color_btn_bd_normal = color_btn_bd_normal
-        self.color_btn_bd_locked = color_btn_bd_locked
-
-        self.locked = locked
-        self.visible = visible
-
-        ## self.id ensures that we can modify a specific instance without affecting the others
-        if id is None:
-            self.id = str(_random.randint(0, 100_000))
-            while self.id in _Slider.sliders:
-                self.id = str(_random.randint(0, 100_000))
-        else:
-            self.id = id
-            if self.id in _Slider.sliders:
-                raise ValueError(f'The id {repr(id)} is duplicated.')
-        _Slider.sliders[self.id] = self
-
-        ## <tags>
-        if type(tags) is str:
-            self.tags = [tags]
-        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
-            self.tags = tags
-        
-        if tags is not None:
-            for tag in self.tags:
-                if tag in _Slider.slider_tags:
-                    _Slider.slider_tags[tag].append(self)
-                else:
-                    _Slider.slider_tags[tag] = [self]
-        ## </tags>
-
-
-        ## runtime
-
-        self.value = self.init
-        self.prec = len(str(abs(self.step)).split('.')[1]) if '.' in str(self.step) else 0
-        self.pressed = False
-        self.hovered = False
-
-
-    @staticmethod
-    def hover_listener():
-        for slider in _Slider.sliders.values():
-            slider._hover()
-
-    @staticmethod
-    def press_listener():
-        for slider in _Slider.sliders.values():
-            slider._press()
-
-    @staticmethod
-    def hold_listener():
-        for slider in list(_Slider.sliders.values()):
-            slider._hold()
-    
-
-    def _release(self):
-        if self.pressed:
-            self.pressed = False
-            self._redraw()
-
-    @staticmethod
-    def release_listener():
-        for slider in list(_Slider.sliders.values()):
-            slider._release()
-
-
-    def set_lock(self, locked: bool, /) -> None:
-        if self.locked is not locked:
-            self.locked = locked
-            self._redraw()
-    
-    @staticmethod
-    def set_lock_by_id(id: str, locked: bool, /) -> None:
-        _Slider.sliders[id].set_lock(locked)
-
-    @staticmethod
-    def set_lock_by_tag(tag: str, locked: bool, /) -> None:
-        for slider in _Slider.slider_tags[tag]:
-            slider.set_lock(locked)
-    
-    @staticmethod
-    def set_lock_all(locked: bool, /) -> None:
-        for slider in _Slider.sliders.values():
-            slider.set_lock(locked)
-
-
-    def set_visibility(self, visible: bool, /) -> None:
-        if self.visible is not visible:
-            self.visible = visible
-            self._redraw()
-    
-    @staticmethod
-    def set_visibility_by_id(id: str, visible: bool, /) -> None:
-        _Slider.sliders[id].set_visibility(visible)
-    
-    @staticmethod
-    def set_visibility_by_tag(tag: str, visible: bool, /) -> None:
-        for slider in _Slider.slider_tags[tag]:
-            slider.set_visibility(visible)
-    
-    @staticmethod
-    def set_visibility_all(visible: bool, /) -> None:
-        for slider in _Slider.sliders.values():
-            slider.set_visibility(visible)
-
-
-    def set_value(self, value: int | None, /) -> None:
-        """if `None` -> default value."""
-
-        if value is None:
-            value = self.init
-
-        if value < self.min:
-            value = self.min
-        if value > self.max:
-            value = self.max
-
-        if value != self.value:
-            self.value = value
-            self._redraw()
-    
-    @staticmethod
-    def set_value_by_id(id: str, value: int | None, /) -> None:
-        _Slider.sliders[id].set_value(value)
-
-    @staticmethod
-    def set_value_by_tag(tag: str, value: int | None, /) -> None:
-        for slider in _Slider.slider_tags[tag]:
-            slider.set_value(value)
-
-    @staticmethod
-    def set_value_all(value: int | None, /) -> None:
-        """To reset the value of all sliders, use `value = None`."""
-        for slider in _Slider.sliders.values():
-            slider.set_value(value)
-
-
-    @staticmethod
-    def get_value_by_id(id: str, /) -> None:
-        return _Slider.sliders[id].value
-    
-
-    def get_anchor_loc(
-        self,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
-        /
-    ) -> tuple[int, int]:
-        """To get the slider-rod's center coordinate, use `anchor='center'`"""
-
-        W = self.width
-        H = self.height
-
-        ## get the coordinates for the center (X, Y)
-        if self.anchor == 'center':
-            X = self.x
-            Y = self.y
-        elif self.anchor == 'n':
-            X = self.x
-            Y = self.y + H/2
-        elif self.anchor == 'ne':
-            X = self.x - W/2
-            Y = self.y + H/2
-        elif self.anchor == 'e':
-            X = self.x - W/2
-            Y = self.y
-        elif self.anchor == 'se':
-            X = self.x - W/2
-            Y = self.y - H/2
-        elif self.anchor == 's':
-            X = self.x
-            Y = self.y - H/2
-        elif self.anchor == 'sw':
-            X = self.x + W/2
-            Y = self.y - H/2
-        elif self.anchor == 'w':
-            X = self.x + W/2
-            Y = self.y
-        elif self.anchor == 'nw':
-            X = self.x + W/2
-            Y = self.y + H/2
-
-        ## returning the requested anchor location
-        if anchor == 'center':
-            return (X, Y)
-        elif anchor == 'n':
-            return (X, Y-H/2)
-        elif anchor == 'ne':
-            return (X+W/2, Y-H/2)
-        elif anchor == 'e':
-            return (X+W/2, Y)
-        elif anchor == 'se':
-            return (X+W/2, Y+H/2)
-        elif anchor == 's':
-            return (X, Y+H/2)
-        elif anchor == 'sw':
-            return (X-W/2, Y+H/2)
-        elif anchor == 'w':
-            return (X-W/2, Y)
-        elif anchor == 'nw':
-            return (X-W/2, Y-H/2)
-        else:
-            raise ValueError(f'Invalid anchor value: {repr(anchor)}')
-
-    @staticmethod
-    def get_anchor_loc_by_id(
-        id: str,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
-        /
-    ) -> tuple[int, int]:
-        return _Slider.sliders[id].get_anchor_loc(anchor)
-
-
-    def move(
-        self,
-        x: int,
-        y: int,
-        /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
-        """If `anchor = None`, the current anchor will be used."""
-        self.x = x
-        self.y = y
-        if anchor is not None:
-            self.anchor = anchor
-        self._redraw()
-
-    @staticmethod
-    def move_by_id(
-        id: str,
-        x: int,
-        y: int,
-        /,
-        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
-    ) -> None:
-        _Slider.sliders[id].move(x, y, anchor)
-
-
-    def align(
-        self,
-        target: '_Slider',
-        anchor: str = 'nw',
-        target_anchor: str = 'ne',
-        xgap: float = 15,
-        ygap: float = 0
-    ) -> '_Slider':
-        """
-        Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
-        """
-
-        ## getting the target anchor location
-        x, y = target.get_anchor_loc(target_anchor)
-
-        ## shifting
-        x += xgap
-        y += ygap
-
-        ## moving the label
-        self.move(x, y, anchor)
-
-        ## return the instance so that this method can also be used when
-        ## creating the instance, like `sld_2 = Slider().align(sld_1)`.
-        return self
-
-
-    def destroy(self) -> None:
-        _Slider.sliders.pop(self.id)
-
-        if self.tags is not None:
-            for tag in self.tags:
-                _Slider.slider_tags[tag].remove(self)
-                if _Slider.slider_tags[tag] == []:
-                    _Slider.slider_tags.pop(tag)
-
-        _Slider.page.delete(f'Slider_{self.id}')
-
-    @staticmethod
-    def destroy_by_id(id: str, /) -> None:
-        _Slider.sliders[id].destroy()
-
-    @staticmethod
-    def destroy_by_tag(tag: str, /) -> None:
-        for slider in list(_Slider.slider_tags[tag]):
-            slider.destroy()
-
-    @staticmethod
-    def destroy_all() -> None:
-        for slider in list(_Slider.sliders.values()):
-            slider.destroy()
-
-
-class Slider(_Slider):
-
-    def __init__(
-        self,
-        min: float = 0,
-        max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
-
-        x: int = 0,
-        y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
-        tolerance: float = 0.25,
-        
-        label: _typing.Optional[str] = None,
-        label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
-        show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
-        label_y_shift: int = -15,
-
-        show_value: bool = True,
-        value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
-        value_prefix: str = '',
-        value_suffix: str = '',
-        show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
-        value_box_x_shift: int = 25,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
-
-        rod_len: int = 200,
-        rod_thick: int = 3,
-        btn_r: int = 5,
-        color_rod_normal: str = '#4b4b4b',
-        color_rod_locked: str = '#2d2d2d',
-        color_btn_normal: str = '#555555',
-        color_btn_locked: str = '#373737',
-        color_btn_press: str = '#7d7d7d',
-        color_btn_hover: str = '#696969',
-        color_btn_bd_normal: str = '#f5f5f5',
-        color_btn_bd_locked: str = '#373737',
-
-        locked: bool = False,
-        visible: bool = True,
-
-        id: str | None = None,
-        tags: str | list[str] | None = None,
-    ) -> None:
-
-        super().__init__(
-            min, max, step, init, fn,
-            x, y, anchor, tolerance,
-            label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
-            show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
-            rod_len, rod_thick, btn_r, color_rod_normal, color_rod_locked, color_btn_normal, color_btn_locked, color_btn_press, color_btn_hover, color_btn_bd_normal, color_btn_bd_locked,
-            locked, visible,
-            id, tags
-        )
-
-        self.value_box_x_shift = value_box_x_shift
-
-        ## runtime (custom)
-
-        self.width = self.rod_len
-        self.height = self.rod_thick
-
-        ## init        
-        
-        self._redraw()
-
-    def _redraw(self):
-
-        if self.locked:
-            color_rod = self.color_rod_locked
-            color_btn = self.color_btn_locked
-            color_btn_bd = self.color_btn_bd_locked
-        elif self.pressed:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_press
-            color_btn_bd = self.color_btn_bd_normal
-        elif self.hovered:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_hover
-            color_btn_bd = self.color_btn_bd_normal
-        else:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_normal
-            color_btn_bd = self.color_btn_bd_normal
-
-        self.page.delete(f'Slider_{self.id}')
-
-        if self.visible:
-
-            X, Y = self.get_anchor_loc('center')
-            w2 = self.width/2
-            h2 = self.height/2
-
-            self.page.create_rectangle(
-                X-w2, Y-h2,
-                X+w2, Y+h2,
-                fill=color_rod, width=0, tags=f'Slider_{self.id}'
-            )
-            self.page.create_oval(
-                X-w2+_norm(self.value, self.min, self.max)*self.width-self.btn_r, Y-self.btn_r,
-                X-w2+_norm(self.value, self.min, self.max)*self.width+self.btn_r, Y+self.btn_r,
-                fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
-            )
-
-            if self.show_label_box:
-                self.page.create_rectangle(
-                    X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
-                    X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
-                    fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
-                )
-            if self.label is not None:
-                self.page.create_text(
-                    X, Y-h2+self.label_y_shift,
-                    text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
-                )
-
-            if self.show_value_box:
-                self.page.create_rectangle(
-                    X+w2+self.value_box_x_shift-self.value_box_width/2, Y-self.value_box_height/2,
-                    X+w2+self.value_box_x_shift+self.value_box_width/2, Y+self.value_box_height/2,
-                    fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
-                )
-            if self.show_value:
-                self.page.create_text(
-                    X+w2+self.value_box_x_shift, Y,
-                    text=self.value_prefix + str(self.value) + self.value_suffix,
-                    font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
-                )
-
-    def _hover(self):
-
-        X, Y = self.get_anchor_loc('center')
-
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
-
-        ## button coordinate
-        bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
-        by = Y
-        br = self.btn_r  # button radius
-
-        ## `True` if the mouse cursor is inside the slider button
-        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
-
-        if inside and (not self.locked) and self.visible and (not self.hovered):
-            self.hovered = True
-            self._redraw()
-        
-        elif self.hovered and (not inside):
-            self.hovered = False
-            self._redraw()
-
-    def _press(self):
-
-        X, Y = self.get_anchor_loc('center')
-
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
-
-        bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
-        by = Y
-        br = self.btn_r
-
-        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
-
-        if inside and (not self.locked) and self.visible:
-            self.pressed = True
-            self._redraw()
-
-    def _hold(self):
-
-        if self.pressed:
-
-            X, _ = self.get_anchor_loc('center')
-
-            mousex = self.page.winfo_pointerx()
-            value = self.min + ((mousex - (X - self.width/2))/self.width)*(self.max - self.min)
-
-            if self.prec == 0:
-                value = int(value)
-            else:
-                value = round(value, self.prec)
-
-            if abs(value - round(value/self.step)*self.step) < self.tolerance*self.step:
-
-                if value < self.min:
-                    value = self.min
-                if value > self.max:
-                    value = self.max
-                
-                if value == self.value:
-                    return
-                self.value = value
-
-                self._redraw()
-                if self.fn is not None:
-                    self.fn()
-
-
-class VSlider(_Slider):
-
-    def __init__(
-        self,
-        min: float = 0,
-        max: float = 1,
-        step: _typing.Optional[float] = None,
-        init: _typing.Optional[float] = None,
-        fn: _typing.Optional[_typing.Callable[[], None]] = None,
-
-        x: int = 0,
-        y: int = 0,
-        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
-        tolerance: float = 0.25,
-        
-        label: _typing.Optional[str] = None,
-        label_fg: str = '#ccc',
-        label_font: str | tuple[str, int] = 'Verdana 9',
-        show_label_box: bool = False,
-        label_box_color: _typing.Optional[str] = None,
-        label_box_width: _typing.Optional[int] = None,
-        label_box_height: _typing.Optional[int] = None,
-        label_y_shift: int = -15,
-
-        show_value: bool = True,
-        value_fg: str = '#ccc',
-        value_font: str | tuple[str, int] = 'Consolas 9',
-        value_prefix: str = '',
-        value_suffix: str = '',
-        show_value_box: bool = False,
-        value_box_color: _typing.Optional[str] = None,
-        value_box_width: _typing.Optional[int] = None,
-        value_box_height: _typing.Optional[int] = None,
-        value_box_y_shift: int = 15,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
-
-        rod_len: int = 200,
-        rod_thick: int = 3,
-        btn_r: int = 5,
-        color_rod_normal: str = '#4b4b4b',
-        color_rod_locked: str = '#2d2d2d',
-        color_btn_normal: str = '#555555',
-        color_btn_locked: str = '#373737',
-        color_btn_press: str = '#7d7d7d',
-        color_btn_hover: str = '#696969',
-        color_btn_bd_normal: str = '#f5f5f5',
-        color_btn_bd_locked: str = '#373737',
-
-        locked: bool = False,
-        visible: bool = True,
-
-        id: str | None = None,
-        tags: str | list[str] | None = None,
-    ) -> None:
-
-        super().__init__(
-            min, max, step, init, fn,
-            x, y, anchor, tolerance,
-            label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
-            show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
-            rod_len, rod_thick, btn_r, color_rod_normal, color_rod_locked, color_btn_normal, color_btn_locked, color_btn_press, color_btn_hover, color_btn_bd_normal, color_btn_bd_locked,
-            locked, visible,
-            id, tags
-        )
-
-        self.value_box_y_shift = value_box_y_shift
-
-        ## runtime (custom)
-
-        self.width = self.rod_thick
-        self.height = self.rod_len
-
-        ## init        
-        
-        self._redraw()
-
-    def _redraw(self):
-
-        if self.locked:
-            color_rod = self.color_rod_locked
-            color_btn = self.color_btn_locked
-            color_btn_bd = self.color_btn_bd_locked
-        elif self.pressed:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_press
-            color_btn_bd = self.color_btn_bd_normal
-        elif self.hovered:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_hover
-            color_btn_bd = self.color_btn_bd_normal
-        else:
-            color_rod = self.color_rod_normal
-            color_btn = self.color_btn_normal
-            color_btn_bd = self.color_btn_bd_normal
-
-        self.page.delete(f'Slider_{self.id}')
-
-        if self.visible:
-
-            X, Y = self.get_anchor_loc('center')
-            w2 = self.width/2
-            h2 = self.height/2
-
-            self.page.create_rectangle(
-                X-w2, Y-h2,
-                X+w2, Y+h2,
-                fill=color_rod, width=0, tags=f'Slider_{self.id}'
-            )
-            self.page.create_oval(
-                X-self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height-self.btn_r,
-                X+self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height+self.btn_r,
-                fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
-            )
-
-            if self.show_label_box:
-                self.page.create_rectangle(
-                    X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
-                    X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
-                    fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
-                )
-            if self.label is not None:
-                self.page.create_text(
-                    X, Y-h2+self.label_y_shift,
-                    text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
-                )
-
-            if self.show_value_box:
-                self.page.create_rectangle(
-                    X-self.value_box_width/2, Y+h2+self.value_box_y_shift-self.value_box_height/2,
-                    X+self.value_box_width/2, Y+h2+self.value_box_y_shift+self.value_box_height/2,
-                    fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
-                )
-            if self.show_value:
-                self.page.create_text(
-                    X, Y+h2+self.value_box_y_shift,
-                    text=self.value_prefix + str(self.value) + self.value_suffix,
-                    font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
-                )
-
-    def _hover(self):
-
-        X, Y = self.get_anchor_loc('center')
-
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
-
-        bx = X
-        by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
-        br = self.btn_r
-
-        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
-
-        if inside and (not self.locked) and self.visible and (not self.hovered):
-            self.hovered = True
-            self._redraw()
-        
-        elif self.hovered and (not inside):
-            self.hovered = False
-            self._redraw()
-
-    def _press(self):
-
-        X, Y = self.get_anchor_loc('center')
-
-        x = self.page.winfo_pointerx()
-        y = self.page.winfo_pointery()
-
-        bx = X
-        by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
-        br = self.btn_r
-
-        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
-
-        if inside and (not self.locked) and self.visible:
-            self.pressed = True
-            self._redraw()
-
-    def _hold(self):
-
-        if self.pressed:
-
-            _, Y = self.get_anchor_loc('center')
-
-            mousey = self.page.winfo_pointery()
-            value = self.max - ((mousey - (Y - self.height/2))/self.height)*(self.max - self.min)
-    
-            if self.prec == 0:
-                value = int(value)
-            else:
-                value = round(value, self.prec)
-
-            if abs(value - round(value/self.step)*self.step) < self.tolerance*self.step:
-
-                if value < self.min:
-                    value = self.min
-                if value > self.max:
-                    value = self.max
-                
-                if value == self.value:
-                    return
-                self.value = value
-                
-                self._redraw()
-                if self.fn is not None:
+import random as _random
+import tkinter as _tk
+import typing as _typing
+
+from mykit.app._runtime import Runtime as _Rt
+from mykit.kit.utils import minmax_normalization as _norm
+
+
+class _Slider(_Rt):
+
+    sliders: dict[str, '_Slider'] = {}
+    slider_tags: dict[str, list['_Slider']] = {}  # note that the horizontal and vertical sliders store the tags together
+
+    def __init__(
+        self,
+        min: float = 0,
+        max: float = 1,
+        step: _typing.Optional[float] = None,
+        init: _typing.Optional[float] = None,
+        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+
+        x: int = 0,
+        y: int = 0,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        tolerance: float = 0.25,
+        
+        label: _typing.Optional[str] = None,
+        label_fg: str = '#ccc',
+        label_font: str | tuple[str, int] = 'Verdana 9',
+        show_label_box: bool = False,
+        label_box_color: _typing.Optional[str] = None,
+        label_box_width: _typing.Optional[int] = None,
+        label_box_height: _typing.Optional[int] = None,
+        label_y_shift: int = -15,
+
+        show_value: bool = True,
+        value_fg: str = '#ccc',
+        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_prefix: str = '',
+        value_suffix: str = '',
+        show_value_box: bool = False,
+        value_box_color: _typing.Optional[str] = None,
+        value_box_width: _typing.Optional[int] = None,
+        value_box_height: _typing.Optional[int] = None,
+
+        rod_len: int = 200,
+        rod_thick: int = 3,
+        btn_r: int = 5,
+        color_rod_normal: str = '#4b4b4b',
+        color_rod_locked: str = '#2d2d2d',
+        color_btn_normal: str = '#555555',
+        color_btn_locked: str = '#373737',
+        color_btn_press: str = '#7d7d7d',
+        color_btn_hover: str = '#696969',
+        color_btn_bd_normal: str = '#f5f5f5',
+        color_btn_bd_locked: str = '#373737',
+
+        locked: bool = False,
+        visible: bool = True,
+
+        id: str | None = None,
+        tags: str | list[str] | None = None,
+    ) -> None:
+        """
+        ## Params
+        - `x` and `y` is the position of the `anchor` (not the center of the button)
+        - `tolerance`: to determine how closely the cursor needs to be to the slider's step values for it to move to a new value
+
+        ## Docs
+        - box color, width, and height should be provided if the box shown
+        """
+
+        if _Slider.page is None:
+            raise AssertionError('App has not been initialized.')
+
+        self.min = min
+        self.max = max
+        self.step = step if step is not None else (max-min)/10
+        self.init = init if init is not None else (max-min)/2
+        self.fn = fn
+
+        self.x = x
+        self.y = y
+        self.anchor = anchor
+        self.tolerance = tolerance
+
+        self.label = label
+        self.label_fg = label_fg
+        self.label_font = label_font
+        self.show_label_box = show_label_box
+        self.label_box_color = label_box_color
+        self.label_box_width = label_box_width
+        self.label_box_height = label_box_height
+        self.label_y_shift = label_y_shift
+
+        self.show_value = show_value
+        self.value_fg = value_fg
+        self.value_font = value_font
+        self.value_prefix = value_prefix
+        self.value_suffix = value_suffix
+        self.show_value_box = show_value_box
+        self.value_box_color = value_box_color
+        self.value_box_width = value_box_width
+        self.value_box_height = value_box_height
+
+        self.rod_len = rod_len
+        self.rod_thick = rod_thick
+        self.btn_r = btn_r
+        self.color_rod_normal = color_rod_normal
+        self.color_rod_locked = color_rod_locked
+        self.color_btn_normal = color_btn_normal
+        self.color_btn_locked = color_btn_locked
+        self.color_btn_press = color_btn_press
+        self.color_btn_hover = color_btn_hover
+        self.color_btn_bd_normal = color_btn_bd_normal
+        self.color_btn_bd_locked = color_btn_bd_locked
+
+        self.locked = locked
+        self.visible = visible
+
+        ## self.id ensures that we can modify a specific instance without affecting the others
+        if id is None:
+            self.id = str(_random.randint(0, 100_000))
+            while self.id in _Slider.sliders:
+                self.id = str(_random.randint(0, 100_000))
+        else:
+            self.id = id
+            if self.id in _Slider.sliders:
+                raise ValueError(f'The id {repr(id)} is duplicated.')
+        _Slider.sliders[self.id] = self
+
+        ## <tags>
+        if type(tags) is str:
+            self.tags = [tags]
+        elif (type(tags) is list) or (type(tags) is tuple) or (tags is None):
+            self.tags = tags
+        
+        if tags is not None:
+            for tag in self.tags:
+                if tag in _Slider.slider_tags:
+                    _Slider.slider_tags[tag].append(self)
+                else:
+                    _Slider.slider_tags[tag] = [self]
+        ## </tags>
+
+
+        ## runtime
+
+        self.value = self.init
+        self.prec = len(str(abs(self.step)).split('.')[1]) if '.' in str(self.step) else 0
+        self.pressed = False
+        self.hovered = False
+
+
+    @staticmethod
+    def hover_listener():
+        for slider in _Slider.sliders.values():
+            slider._hover()
+
+    @staticmethod
+    def press_listener():
+        for slider in _Slider.sliders.values():
+            slider._press()
+
+    @staticmethod
+    def hold_listener():
+        for slider in list(_Slider.sliders.values()):
+            slider._hold()
+    
+
+    def _release(self):
+        if self.pressed:
+            self.pressed = False
+            self._redraw()
+
+    @staticmethod
+    def release_listener():
+        for slider in list(_Slider.sliders.values()):
+            slider._release()
+
+
+    def set_lock(self, locked: bool, /) -> None:
+        if self.locked is not locked:
+            self.locked = locked
+            self._redraw()
+    
+    @staticmethod
+    def set_lock_by_id(id: str, locked: bool, /) -> None:
+        _Slider.sliders[id].set_lock(locked)
+
+    @staticmethod
+    def set_lock_by_tag(tag: str, locked: bool, /) -> None:
+        for slider in _Slider.slider_tags[tag]:
+            slider.set_lock(locked)
+    
+    @staticmethod
+    def set_lock_all(locked: bool, /) -> None:
+        for slider in _Slider.sliders.values():
+            slider.set_lock(locked)
+
+
+    def set_visibility(self, visible: bool, /) -> None:
+        if self.visible is not visible:
+            self.visible = visible
+            self._redraw()
+    
+    @staticmethod
+    def set_visibility_by_id(id: str, visible: bool, /) -> None:
+        _Slider.sliders[id].set_visibility(visible)
+    
+    @staticmethod
+    def set_visibility_by_tag(tag: str, visible: bool, /) -> None:
+        for slider in _Slider.slider_tags[tag]:
+            slider.set_visibility(visible)
+    
+    @staticmethod
+    def set_visibility_all(visible: bool, /) -> None:
+        for slider in _Slider.sliders.values():
+            slider.set_visibility(visible)
+
+
+    def set_value(self, value: int | None, /) -> None:
+        """if `None` -> default value."""
+
+        if value is None:
+            value = self.init
+
+        if value < self.min:
+            value = self.min
+        if value > self.max:
+            value = self.max
+
+        if value != self.value:
+            self.value = value
+            self._redraw()
+    
+    @staticmethod
+    def set_value_by_id(id: str, value: int | None, /) -> None:
+        _Slider.sliders[id].set_value(value)
+
+    @staticmethod
+    def set_value_by_tag(tag: str, value: int | None, /) -> None:
+        for slider in _Slider.slider_tags[tag]:
+            slider.set_value(value)
+
+    @staticmethod
+    def set_value_all(value: int | None, /) -> None:
+        """To reset the value of all sliders, use `value = None`."""
+        for slider in _Slider.sliders.values():
+            slider.set_value(value)
+
+
+    @staticmethod
+    def get_value_by_id(id: str, /) -> None:
+        return _Slider.sliders[id].value
+    
+
+    def get_anchor_loc(
+        self,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        /
+    ) -> tuple[int, int]:
+        """To get the slider-rod's center coordinate, use `anchor='center'`"""
+
+        W = self.width
+        H = self.height
+
+        ## get the coordinates for the center (X, Y)
+        if self.anchor == 'center':
+            X = self.x
+            Y = self.y
+        elif self.anchor == 'n':
+            X = self.x
+            Y = self.y + H/2
+        elif self.anchor == 'ne':
+            X = self.x - W/2
+            Y = self.y + H/2
+        elif self.anchor == 'e':
+            X = self.x - W/2
+            Y = self.y
+        elif self.anchor == 'se':
+            X = self.x - W/2
+            Y = self.y - H/2
+        elif self.anchor == 's':
+            X = self.x
+            Y = self.y - H/2
+        elif self.anchor == 'sw':
+            X = self.x + W/2
+            Y = self.y - H/2
+        elif self.anchor == 'w':
+            X = self.x + W/2
+            Y = self.y
+        elif self.anchor == 'nw':
+            X = self.x + W/2
+            Y = self.y + H/2
+
+        ## returning the requested anchor location
+        if anchor == 'center':
+            return (X, Y)
+        elif anchor == 'n':
+            return (X, Y-H/2)
+        elif anchor == 'ne':
+            return (X+W/2, Y-H/2)
+        elif anchor == 'e':
+            return (X+W/2, Y)
+        elif anchor == 'se':
+            return (X+W/2, Y+H/2)
+        elif anchor == 's':
+            return (X, Y+H/2)
+        elif anchor == 'sw':
+            return (X-W/2, Y+H/2)
+        elif anchor == 'w':
+            return (X-W/2, Y)
+        elif anchor == 'nw':
+            return (X-W/2, Y-H/2)
+        else:
+            raise ValueError(f'Invalid anchor value: {repr(anchor)}')
+
+    @staticmethod
+    def get_anchor_loc_by_id(
+        id: str,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        /
+    ) -> tuple[int, int]:
+        return _Slider.sliders[id].get_anchor_loc(anchor)
+
+
+    def move(
+        self,
+        x: int,
+        y: int,
+        /,
+        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
+        """If `anchor = None`, the current anchor will be used."""
+        self.x = x
+        self.y = y
+        if anchor is not None:
+            self.anchor = anchor
+        self._redraw()
+
+    @staticmethod
+    def move_by_id(
+        id: str,
+        x: int,
+        y: int,
+        /,
+        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
+        _Slider.sliders[id].move(x, y, anchor)
+
+
+    def align(
+        self,
+        target: '_Slider',
+        anchor: str = 'nw',
+        target_anchor: str = 'ne',
+        xgap: float = 15,
+        ygap: float = 0
+    ) -> '_Slider':
+        """
+        Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
+        """
+
+        ## getting the target anchor location
+        x, y = target.get_anchor_loc(target_anchor)
+
+        ## shifting
+        x += xgap
+        y += ygap
+
+        ## moving the label
+        self.move(x, y, anchor)
+
+        ## return the instance so that this method can also be used when
+        ## creating the instance, like `sld_2 = Slider().align(sld_1)`.
+        return self
+
+
+    def destroy(self) -> None:
+        _Slider.sliders.pop(self.id)
+
+        if self.tags is not None:
+            for tag in self.tags:
+                _Slider.slider_tags[tag].remove(self)
+                if _Slider.slider_tags[tag] == []:
+                    _Slider.slider_tags.pop(tag)
+
+        _Slider.page.delete(f'Slider_{self.id}')
+
+    @staticmethod
+    def destroy_by_id(id: str, /) -> None:
+        _Slider.sliders[id].destroy()
+
+    @staticmethod
+    def destroy_by_tag(tag: str, /) -> None:
+        for slider in list(_Slider.slider_tags[tag]):
+            slider.destroy()
+
+    @staticmethod
+    def destroy_all() -> None:
+        for slider in list(_Slider.sliders.values()):
+            slider.destroy()
+
+
+class Slider(_Slider):
+
+    def __init__(
+        self,
+        min: float = 0,
+        max: float = 1,
+        step: _typing.Optional[float] = None,
+        init: _typing.Optional[float] = None,
+        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+
+        x: int = 0,
+        y: int = 0,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        tolerance: float = 0.25,
+        
+        label: _typing.Optional[str] = None,
+        label_fg: str = '#ccc',
+        label_font: str | tuple[str, int] = 'Verdana 9',
+        show_label_box: bool = False,
+        label_box_color: _typing.Optional[str] = None,
+        label_box_width: _typing.Optional[int] = None,
+        label_box_height: _typing.Optional[int] = None,
+        label_y_shift: int = -15,
+
+        show_value: bool = True,
+        value_fg: str = '#ccc',
+        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_prefix: str = '',
+        value_suffix: str = '',
+        show_value_box: bool = False,
+        value_box_color: _typing.Optional[str] = None,
+        value_box_width: _typing.Optional[int] = None,
+        value_box_height: _typing.Optional[int] = None,
+        value_box_x_shift: int = 25,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
+
+        rod_len: int = 200,
+        rod_thick: int = 3,
+        btn_r: int = 5,
+        color_rod_normal: str = '#4b4b4b',
+        color_rod_locked: str = '#2d2d2d',
+        color_btn_normal: str = '#555555',
+        color_btn_locked: str = '#373737',
+        color_btn_press: str = '#7d7d7d',
+        color_btn_hover: str = '#696969',
+        color_btn_bd_normal: str = '#f5f5f5',
+        color_btn_bd_locked: str = '#373737',
+
+        locked: bool = False,
+        visible: bool = True,
+
+        id: str | None = None,
+        tags: str | list[str] | None = None,
+    ) -> None:
+
+        super().__init__(
+            min, max, step, init, fn,
+            x, y, anchor, tolerance,
+            label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
+            show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
+            rod_len, rod_thick, btn_r, color_rod_normal, color_rod_locked, color_btn_normal, color_btn_locked, color_btn_press, color_btn_hover, color_btn_bd_normal, color_btn_bd_locked,
+            locked, visible,
+            id, tags
+        )
+
+        self.value_box_x_shift = value_box_x_shift
+
+        ## runtime (custom)
+
+        self.width = self.rod_len
+        self.height = self.rod_thick
+
+        ## init        
+        
+        self._redraw()
+
+    def _redraw(self):
+
+        if self.locked:
+            color_rod = self.color_rod_locked
+            color_btn = self.color_btn_locked
+            color_btn_bd = self.color_btn_bd_locked
+        elif self.pressed:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_press
+            color_btn_bd = self.color_btn_bd_normal
+        elif self.hovered:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_hover
+            color_btn_bd = self.color_btn_bd_normal
+        else:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_normal
+            color_btn_bd = self.color_btn_bd_normal
+
+        self.page.delete(f'Slider_{self.id}')
+
+        if self.visible:
+
+            X, Y = self.get_anchor_loc('center')
+            w2 = self.width/2
+            h2 = self.height/2
+
+            self.page.create_rectangle(
+                X-w2, Y-h2,
+                X+w2, Y+h2,
+                fill=color_rod, width=0, tags=f'Slider_{self.id}'
+            )
+            self.page.create_oval(
+                X-w2+_norm(self.value, self.min, self.max)*self.width-self.btn_r, Y-self.btn_r,
+                X-w2+_norm(self.value, self.min, self.max)*self.width+self.btn_r, Y+self.btn_r,
+                fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
+            )
+
+            if self.show_label_box:
+                self.page.create_rectangle(
+                    X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
+                    X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
+                    fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
+                )
+            if self.label is not None:
+                self.page.create_text(
+                    X, Y-h2+self.label_y_shift,
+                    text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
+                )
+
+            if self.show_value_box:
+                self.page.create_rectangle(
+                    X+w2+self.value_box_x_shift-self.value_box_width/2, Y-self.value_box_height/2,
+                    X+w2+self.value_box_x_shift+self.value_box_width/2, Y+self.value_box_height/2,
+                    fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
+                )
+            if self.show_value:
+                self.page.create_text(
+                    X+w2+self.value_box_x_shift, Y,
+                    text=self.value_prefix + str(self.value) + self.value_suffix,
+                    font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
+                )
+
+    def _hover(self):
+
+        X, Y = self.get_anchor_loc('center')
+
+        x = self.page.winfo_pointerx()
+        y = self.page.winfo_pointery()
+
+        ## button coordinate
+        bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
+        by = Y
+        br = self.btn_r  # button radius
+
+        ## `True` if the mouse cursor is inside the slider button
+        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
+
+        if inside and (not self.locked) and self.visible and (not self.hovered):
+            self.hovered = True
+            self._redraw()
+        
+        elif self.hovered and (not inside):
+            self.hovered = False
+            self._redraw()
+
+    def _press(self):
+
+        X, Y = self.get_anchor_loc('center')
+
+        x = self.page.winfo_pointerx()
+        y = self.page.winfo_pointery()
+
+        bx = X - self.width/2 + _norm(self.value, self.min, self.max)*self.width
+        by = Y
+        br = self.btn_r
+
+        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
+
+        if inside and (not self.locked) and self.visible:
+            self.pressed = True
+            self._redraw()
+
+    def _hold(self):
+
+        if self.pressed:
+
+            X, _ = self.get_anchor_loc('center')
+
+            mousex = self.page.winfo_pointerx()
+            value = self.min + ((mousex - (X - self.width/2))/self.width)*(self.max - self.min)
+
+            if self.prec == 0:
+                value = int(value)
+            else:
+                value = round(value, self.prec)
+
+            if abs(value - round(value/self.step)*self.step) < self.tolerance*self.step:
+
+                if value < self.min:
+                    value = self.min
+                if value > self.max:
+                    value = self.max
+                
+                if value == self.value:
+                    return
+                self.value = value
+
+                self._redraw()
+                if self.fn is not None:
+                    self.fn()
+
+
+class VSlider(_Slider):
+
+    def __init__(
+        self,
+        min: float = 0,
+        max: float = 1,
+        step: _typing.Optional[float] = None,
+        init: _typing.Optional[float] = None,
+        fn: _typing.Optional[_typing.Callable[[], None]] = None,
+
+        x: int = 0,
+        y: int = 0,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
+        tolerance: float = 0.25,
+        
+        label: _typing.Optional[str] = None,
+        label_fg: str = '#ccc',
+        label_font: str | tuple[str, int] = 'Verdana 9',
+        show_label_box: bool = False,
+        label_box_color: _typing.Optional[str] = None,
+        label_box_width: _typing.Optional[int] = None,
+        label_box_height: _typing.Optional[int] = None,
+        label_y_shift: int = -15,
+
+        show_value: bool = True,
+        value_fg: str = '#ccc',
+        value_font: str | tuple[str, int] = 'Consolas 9',
+        value_prefix: str = '',
+        value_suffix: str = '',
+        show_value_box: bool = False,
+        value_box_color: _typing.Optional[str] = None,
+        value_box_width: _typing.Optional[int] = None,
+        value_box_height: _typing.Optional[int] = None,
+        value_box_y_shift: int = 15,  # extra arg. reminder: this parameter has a different argument name for horizontal and vertical sliders
+
+        rod_len: int = 200,
+        rod_thick: int = 3,
+        btn_r: int = 5,
+        color_rod_normal: str = '#4b4b4b',
+        color_rod_locked: str = '#2d2d2d',
+        color_btn_normal: str = '#555555',
+        color_btn_locked: str = '#373737',
+        color_btn_press: str = '#7d7d7d',
+        color_btn_hover: str = '#696969',
+        color_btn_bd_normal: str = '#f5f5f5',
+        color_btn_bd_locked: str = '#373737',
+
+        locked: bool = False,
+        visible: bool = True,
+
+        id: str | None = None,
+        tags: str | list[str] | None = None,
+    ) -> None:
+
+        super().__init__(
+            min, max, step, init, fn,
+            x, y, anchor, tolerance,
+            label, label_fg, label_font, show_label_box, label_box_color, label_box_width, label_box_height, label_y_shift,
+            show_value, value_fg, value_font, value_prefix, value_suffix, show_value_box, value_box_color, value_box_width, value_box_height,
+            rod_len, rod_thick, btn_r, color_rod_normal, color_rod_locked, color_btn_normal, color_btn_locked, color_btn_press, color_btn_hover, color_btn_bd_normal, color_btn_bd_locked,
+            locked, visible,
+            id, tags
+        )
+
+        self.value_box_y_shift = value_box_y_shift
+
+        ## runtime (custom)
+
+        self.width = self.rod_thick
+        self.height = self.rod_len
+
+        ## init        
+        
+        self._redraw()
+
+    def _redraw(self):
+
+        if self.locked:
+            color_rod = self.color_rod_locked
+            color_btn = self.color_btn_locked
+            color_btn_bd = self.color_btn_bd_locked
+        elif self.pressed:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_press
+            color_btn_bd = self.color_btn_bd_normal
+        elif self.hovered:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_hover
+            color_btn_bd = self.color_btn_bd_normal
+        else:
+            color_rod = self.color_rod_normal
+            color_btn = self.color_btn_normal
+            color_btn_bd = self.color_btn_bd_normal
+
+        self.page.delete(f'Slider_{self.id}')
+
+        if self.visible:
+
+            X, Y = self.get_anchor_loc('center')
+            w2 = self.width/2
+            h2 = self.height/2
+
+            self.page.create_rectangle(
+                X-w2, Y-h2,
+                X+w2, Y+h2,
+                fill=color_rod, width=0, tags=f'Slider_{self.id}'
+            )
+            self.page.create_oval(
+                X-self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height-self.btn_r,
+                X+self.btn_r, Y+h2-_norm(self.value, self.min, self.max)*self.height+self.btn_r,
+                fill=color_btn, width=1, outline=color_btn_bd, tags=f'Slider_{self.id}'
+            )
+
+            if self.show_label_box:
+                self.page.create_rectangle(
+                    X-self.label_box_width/2, Y-h2+self.label_y_shift-self.label_box_height/2,
+                    X+self.label_box_width/2, Y-h2+self.label_y_shift+self.label_box_height/2,
+                    fill=self.label_box_color, width=0, tags=f'Slider_{self.id}'
+                )
+            if self.label is not None:
+                self.page.create_text(
+                    X, Y-h2+self.label_y_shift,
+                    text=self.label, font=self.label_font, fill=self.label_fg, tags=f'Slider_{self.id}'
+                )
+
+            if self.show_value_box:
+                self.page.create_rectangle(
+                    X-self.value_box_width/2, Y+h2+self.value_box_y_shift-self.value_box_height/2,
+                    X+self.value_box_width/2, Y+h2+self.value_box_y_shift+self.value_box_height/2,
+                    fill=self.value_box_color, width=0, tags=f'Slider_{self.id}'
+                )
+            if self.show_value:
+                self.page.create_text(
+                    X, Y+h2+self.value_box_y_shift,
+                    text=self.value_prefix + str(self.value) + self.value_suffix,
+                    font=self.value_font, fill=self.value_fg, tags=f'Slider_{self.id}'
+                )
+
+    def _hover(self):
+
+        X, Y = self.get_anchor_loc('center')
+
+        x = self.page.winfo_pointerx()
+        y = self.page.winfo_pointery()
+
+        bx = X
+        by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
+        br = self.btn_r
+
+        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
+
+        if inside and (not self.locked) and self.visible and (not self.hovered):
+            self.hovered = True
+            self._redraw()
+        
+        elif self.hovered and (not inside):
+            self.hovered = False
+            self._redraw()
+
+    def _press(self):
+
+        X, Y = self.get_anchor_loc('center')
+
+        x = self.page.winfo_pointerx()
+        y = self.page.winfo_pointery()
+
+        bx = X
+        by = Y + self.height/2 - _norm(self.value, self.min, self.max)*self.height
+        br = self.btn_r
+
+        inside = (bx-br <= x <= bx+br) and (by-br <= y <= by+br)
+
+        if inside and (not self.locked) and self.visible:
+            self.pressed = True
+            self._redraw()
+
+    def _hold(self):
+
+        if self.pressed:
+
+            _, Y = self.get_anchor_loc('center')
+
+            mousey = self.page.winfo_pointery()
+            value = self.max - ((mousey - (Y - self.height/2))/self.height)*(self.max - self.min)
+    
+            if self.prec == 0:
+                value = int(value)
+            else:
+                value = round(value, self.prec)
+
+            if abs(value - round(value/self.step)*self.step) < self.tolerance*self.step:
+
+                if value < self.min:
+                    value = self.min
+                if value > self.max:
+                    value = self.max
+                
+                if value == self.value:
+                    return
+                self.value = value
+                
+                self._redraw()
+                if self.fn is not None:
                     self.fn()
```

### Comparing `mykit-2.0.0rc3/mykit/kit/color.py` & `mykit-2.0.1/mykit/kit/color.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-
-
-def interpolate_color(color1: str, color2: str, x: float) -> str:
-    """
-    Interpolates between two colors based on the given ratio `x`.
-
-    ---
-
-    ## Params
-        - `color1`: The first color in hexadecimal format (e.g., '#RRGGBB').
-        - `color2`: The second color in hexadecimal format (e.g., '#RRGGBB').
-        - `x`: The ratio determining the interpolation between the two colors. Should be between 0 and 1.
-
-    ## Returns
-        - The interpolated color as a hexadecimal string.
-
-    ## Demo
-        >>> interpolate_color('#ff0000', '#0000ff', 0.0)
-        '#ff0000'
-        >>> interpolate_color('#ff0000', '#0000ff', 0.5)
-        '#7f007f'
-        >>> interpolate_color('#ff0000', '#0000ff', 1.0)
-        '#0000ff'
-    """
-    ## convert color strings to RGB values
-    r1, g1, b1 = int(color1[1:3], 16), int(color1[3:5], 16), int(color1[5:7], 16)
-    r2, g2, b2 = int(color2[1:3], 16), int(color2[3:5], 16), int(color2[5:7], 16)
-
-    ## interpolate RGB values based on x
-    r = int(r1 + (r2 - r1)*x)
-    g = int(g1 + (g2 - g1)*x)
-    b = int(b1 + (b2 - b1)*x)
-
-    ## convert interpolated RGB values to hexadecimal color string
-    interpolated_color = f'#{r:02x}{g:02x}{b:02x}'
-    return interpolated_color
-
-
-def getgray(alpha: float, /, max_lum: int = 255) -> str:
-    """
-    Returns a hexadecimal color value representing a grayscale shade based on the given alpha and maximum luminance.
-
-    ---
-
-    ## Params
-    - `alpha`: A grayscale shade intensity value in the range [0, 1].
-    - `max_lum`: Maximum luminance value for grayscale in the range [0, 255].
-
-    ## Demo
-    >>> getgray(0.5)
-    '#808080'
-    """
-    a = f'{round(max_lum*alpha):02x}'
-    return f'#{a}{a}{a}'
-
-
-def rgb_to_hex(r: int, g: int, b: int, /) -> str:
-    return f'#{r:02x}{g:02x}{b:02x}'
-
-
-def hexa_to_hex(foreground: str, opacity: float, background: str) -> str:
-    """
-    Calculates the hexadecimal color code of `foreground` with the given `opacity` on `background`.
-    The `foreground` and `background` must be valid hexadecimal color codes,
-    and the `opacity` value must be in the interval [0, 1].
-    """
-
-    fg = [int(foreground[i:i+2], 16) for i in (1, 3, 5)]
-    bg = [int(background[i:i+2], 16) for i in (1, 3, 5)]
-
-    r = round(fg[0]*opacity + bg[0]*(1 - opacity))
-    g = round(fg[1]*opacity + bg[1]*(1 - opacity))
-    b = round(fg[2]*opacity + bg[2]*(1 - opacity))
-
-    return f'#{r:02x}{g:02x}{b:02x}'
-
-
-def interpolate_with_black(foreground: str, opacity: float) -> str:
-    """
-    This is the optimized version of `hexa_to_hex(foreground, opacity, '#000000')`.
-    Please refer to the documentation of the `hexa_to_hex` function for more details.
-    """
-
-    c = [int(foreground[i:i+2], 16) for i in (1, 3, 5)]
-
-    r = round( c[0]*opacity )
-    g = round( c[1]*opacity )
-    b = round( c[2]*opacity )
-
+
+
+def interpolate_color(color1: str, color2: str, x: float) -> str:
+    """
+    Interpolates between two colors based on the given ratio `x`.
+
+    ---
+
+    ## Params
+        - `color1`: The first color in hexadecimal format (e.g., '#RRGGBB').
+        - `color2`: The second color in hexadecimal format (e.g., '#RRGGBB').
+        - `x`: The ratio determining the interpolation between the two colors. Should be between 0 and 1.
+
+    ## Returns
+        - The interpolated color as a hexadecimal string.
+
+    ## Demo
+        >>> interpolate_color('#ff0000', '#0000ff', 0.0)
+        '#ff0000'
+        >>> interpolate_color('#ff0000', '#0000ff', 0.5)
+        '#7f007f'
+        >>> interpolate_color('#ff0000', '#0000ff', 1.0)
+        '#0000ff'
+    """
+    ## convert color strings to RGB values
+    r1, g1, b1 = int(color1[1:3], 16), int(color1[3:5], 16), int(color1[5:7], 16)
+    r2, g2, b2 = int(color2[1:3], 16), int(color2[3:5], 16), int(color2[5:7], 16)
+
+    ## interpolate RGB values based on x
+    r = int(r1 + (r2 - r1)*x)
+    g = int(g1 + (g2 - g1)*x)
+    b = int(b1 + (b2 - b1)*x)
+
+    ## convert interpolated RGB values to hexadecimal color string
+    interpolated_color = f'#{r:02x}{g:02x}{b:02x}'
+    return interpolated_color
+
+
+def getgray(alpha: float, /, max_lum: int = 255) -> str:
+    """
+    Returns a hexadecimal color value representing a grayscale shade based on the given alpha and maximum luminance.
+
+    ---
+
+    ## Params
+    - `alpha`: A grayscale shade intensity value in the range [0, 1].
+    - `max_lum`: Maximum luminance value for grayscale in the range [0, 255].
+
+    ## Demo
+    >>> getgray(0.5)
+    '#808080'
+    """
+    a = f'{round(max_lum*alpha):02x}'
+    return f'#{a}{a}{a}'
+
+
+def rgb_to_hex(r: int, g: int, b: int, /) -> str:
+    return f'#{r:02x}{g:02x}{b:02x}'
+
+
+def hexa_to_hex(foreground: str, opacity: float, background: str) -> str:
+    """
+    Calculates the hexadecimal color code of `foreground` with the given `opacity` on `background`.
+    The `foreground` and `background` must be valid hexadecimal color codes,
+    and the `opacity` value must be in the interval [0, 1].
+    """
+
+    fg = [int(foreground[i:i+2], 16) for i in (1, 3, 5)]
+    bg = [int(background[i:i+2], 16) for i in (1, 3, 5)]
+
+    r = round(fg[0]*opacity + bg[0]*(1 - opacity))
+    g = round(fg[1]*opacity + bg[1]*(1 - opacity))
+    b = round(fg[2]*opacity + bg[2]*(1 - opacity))
+
+    return f'#{r:02x}{g:02x}{b:02x}'
+
+
+def interpolate_with_black(foreground: str, opacity: float) -> str:
+    """
+    This is the optimized version of `hexa_to_hex(foreground, opacity, '#000000')`.
+    Please refer to the documentation of the `hexa_to_hex` function for more details.
+    """
+
+    c = [int(foreground[i:i+2], 16) for i in (1, 3, 5)]
+
+    r = round( c[0]*opacity )
+    g = round( c[1]*opacity )
+    b = round( c[2]*opacity )
+
     return f'#{r:02x}{g:02x}{b:02x}'
```

### Comparing `mykit-2.0.0rc3/mykit/kit/keycrate/__init__.py` & `mykit-2.0.1/mykit/kit/keycrate/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-import re as _re
-import typing as _typing
-
-from mykit.kit.path import open_file as _open_file
-from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
-
-
-class KeyCrate:
-    """
-    Using a .txt file (which is easy to open, read, and modify)
-    to store key-value pairs, aiming to keep it simple and fast.
-    """
-
-    def __init__(
-        self,
-        file_pth: str,
-        /,
-        key_is_var: bool = False,
-        eval_value: bool = False,
-        only_keys: _typing.Optional[list[str]] = None,
-        need_keys: _typing.Optional[list[str]] = None
-    ) -> None:
-        """
-        Storing key-value pairs (key: value) in the .txt file `file_pth`.
-        Access the value using either the class-like way (`kc.key`)
-        or the dictionary-like way (`kc['key']`).
-
-        ---
-
-        ## Params
-        - `file_pth`: full path to the .txt file that holds the key-value pairs
-        - `key_is_var`: if `True`, all keys must be valid as variable name
-        - `eval_value`: if `True`, all values must be evaluatable by `eval()`
-        - `only_keys`: only keys specified by `only_keys` are allowed in `file_pth`
-        - `need_keys`: keys that specified by `need_keys` must exist in `file_pth`
-
-        ## Exceptions
-        - `AttributeError`: if trying to access a nonexistent key
-        - see `self.parse` exceptions
-
-        ## Demo 1
-        >>> kc = KeyCrate('config.txt', eval_value=True)
-        >>> fps = kc.fps  # or kc['fps']
-        >>> output_dir = kc['output folder']
-
-        ## Demo 2
-        >>> settings = KeyCrate('settings.txt', key_is_var=True, only_keys=['fps', 'dur'])
-        >>> fps = settings.fps
-        >>> dur = settings.dur
-        """
-
-        ## added the prefix "_kc__" to prevent conflicts with the keys
-        self._kc__file_pth = file_pth
-        self._kc__key_is_var = key_is_var
-        self._kc__eval_value = eval_value
-        self._kc__only_keys = only_keys
-        self._kc__need_keys = need_keys
-
-        ## init
-        self.parse()
-
-    def __getattr__(self, __name: str, __default: _typing.Any = None, /) -> _typing.NoReturn:
-        """This method is called when attribute `__name` is not found"""
-        raise AttributeError(f'KeyCrate file {repr(self._kc__file_pth)} does not have key {repr(__name)}.')
-
-    def __getitem__(self, __key: str, /) -> _typing.Any:
-        """
-        To access the keys in a dictionary-like way (e.g., `kc['key1']`),
-        it is commonly used for keys that are not variable names (e.g., `kc['full name']`).
-        """
-        return getattr(self, __key)
-
-    def _read(self) -> str:
-        """Return the current content of the file."""
-        with open(self._kc__file_pth, 'r') as fp:
-            out = fp.read()
-        return out
-
-    def parse(self) -> None:
-        """
-        If necessary, rerun this function to reparse.
-
-        ---
-
-        ## Exceptions
-        - `SyntaxError`: if invalid syntax is found
-        - `ValueError`: if any duplicate keys are found
-        - `AssertionError`: if key is invalid for variable name (when `key_is_var=True`)
-        - `AssertionError`: if value can't be evaluated (when `eval_value=True`)
-        - `AssertionError`: if unexpected key is found (only when `only_keys` is specified)
-        - `AssertionError`: if missing key is found (only when `need_keys` is specified)
-        """
-
-        raw = self._read()
-
-        if self._kc__need_keys is not None:
-            _need_keys = self._kc__need_keys.copy()
-
-        for line_no, line in enumerate(raw.split('\n'), 1):
-
-            if (line == '') or _re.match(r'\s*#--.*', line):
-                ## blank-line or comment-header
-                continue
-
-            res = _re.match(
-                r'\s*(?P<key>.+?)\s*:\s*(?P<val>.+?)\s*(?:#--.*)?;',
-                ## added ";" to capture "everything" in `val` (but not
-                ## the *last-spaces and comment* after it). The pattern doesn't
-                ## work without it
-                line + ';'
-            )
-            if res is None:
-                raise SyntaxError(
-                    f'KeyCrate file {repr(self._kc__file_pth)} '
-                    f'has invalid syntax at line {line_no}: {repr(line)}'
-                )
-
-            key = res.group('key')
-            val = res.group('val')
-
-            if key in self.__dict__:
-                raise ValueError(
-                    f'KeyCrate file {repr(self._kc__file_pth)} '
-                    f'has a duplicated key {repr(key)} found at line {line_no}.'
-                )
-
-            if self._kc__key_is_var:
-                if not _is_valid_var_name(key):
-                    raise AssertionError(
-                        f'KeyCrate file {repr(self._kc__file_pth)} '
-                        f'has a key {repr(key)} that is invalid for a variable name, found at line {line_no}.'
-                    )
-
-            if self._kc__eval_value:
-                try:
-                    val = eval(val, {})
-                except (NameError, SyntaxError):
-                    raise AssertionError(
-                        f'KeyCrate file {repr(self._kc__file_pth)} '
-                        f'has a value {repr(val)} that cannot be evaluated, found at line {line_no}.'
-                    )
-
-            if self._kc__only_keys is not None:
-                if key not in self._kc__only_keys:
-                    raise AssertionError(
-                        f'KeyCrate file {repr(self._kc__file_pth)} '
-                        f'has an unexpected key {repr(key)} found at line {line_no}.'
-                    )
-
-            if self._kc__need_keys:
-                try:
-                    _need_keys.remove(key)
-                except ValueError:
-                    ## note that if `need_keys` is specified, other keys
-                    ## (not in `need_keys`) are also allowed.
-                    ## so, this exception must be handled
-                    pass
-
-            setattr(self, key, val)
-
-        if self._kc__need_keys:
-            if _need_keys != []:
-                raise AssertionError(
-                    f'KeyCrate file {repr(self._kc__file_pth)} is missing keys: '
-                    + ', '.join(map(repr, _need_keys))
-                )
-
-    def open(self) -> None:
-        """open the .txt file"""
+import re as _re
+import typing as _typing
+
+from mykit.kit.path import open_file as _open_file
+from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
+
+
+class KeyCrate:
+    """
+    Using a .txt file (which is easy to open, read, and modify)
+    to store key-value pairs, aiming to keep it simple and fast.
+    """
+
+    def __init__(
+        self,
+        file_pth: str,
+        /,
+        key_is_var: bool = False,
+        eval_value: bool = False,
+        only_keys: _typing.Optional[list[str]] = None,
+        need_keys: _typing.Optional[list[str]] = None
+    ) -> None:
+        """
+        Storing key-value pairs (key: value) in the .txt file `file_pth`.
+        Access the value using either the class-like way (`kc.key`)
+        or the dictionary-like way (`kc['key']`).
+
+        ---
+
+        ## Params
+        - `file_pth`: full path to the .txt file that holds the key-value pairs
+        - `key_is_var`: if `True`, all keys must be valid as variable name
+        - `eval_value`: if `True`, all values must be evaluatable by `eval()`
+        - `only_keys`: only keys specified by `only_keys` are allowed in `file_pth`
+        - `need_keys`: keys that specified by `need_keys` must exist in `file_pth`
+
+        ## Exceptions
+        - `AttributeError`: if trying to access a nonexistent key
+        - see `self.parse` exceptions
+
+        ## Demo 1
+        >>> kc = KeyCrate('config.txt', eval_value=True)
+        >>> fps = kc.fps  # or kc['fps']
+        >>> output_dir = kc['output folder']
+
+        ## Demo 2
+        >>> settings = KeyCrate('settings.txt', key_is_var=True, only_keys=['fps', 'dur'])
+        >>> fps = settings.fps
+        >>> dur = settings.dur
+        """
+
+        ## added the prefix "_kc__" to prevent conflicts with the keys
+        self._kc__file_pth = file_pth
+        self._kc__key_is_var = key_is_var
+        self._kc__eval_value = eval_value
+        self._kc__only_keys = only_keys
+        self._kc__need_keys = need_keys
+
+        ## init
+        self.parse()
+
+    def __getattr__(self, __name: str, __default: _typing.Any = None, /) -> _typing.NoReturn:
+        """This method is called when attribute `__name` is not found"""
+        raise AttributeError(f'KeyCrate file {repr(self._kc__file_pth)} does not have key {repr(__name)}.')
+
+    def __getitem__(self, __key: str, /) -> _typing.Any:
+        """
+        To access the keys in a dictionary-like way (e.g., `kc['key1']`),
+        it is commonly used for keys that are not variable names (e.g., `kc['full name']`).
+        """
+        return getattr(self, __key)
+
+    def _read(self) -> str:
+        """Return the current content of the file."""
+        with open(self._kc__file_pth, 'r') as fp:
+            out = fp.read()
+        return out
+
+    def parse(self) -> None:
+        """
+        If necessary, rerun this function to reparse.
+
+        ---
+
+        ## Exceptions
+        - `SyntaxError`: if invalid syntax is found
+        - `ValueError`: if any duplicate keys are found
+        - `AssertionError`: if key is invalid for variable name (when `key_is_var=True`)
+        - `AssertionError`: if value can't be evaluated (when `eval_value=True`)
+        - `AssertionError`: if unexpected key is found (only when `only_keys` is specified)
+        - `AssertionError`: if missing key is found (only when `need_keys` is specified)
+        """
+
+        raw = self._read()
+
+        if self._kc__need_keys is not None:
+            _need_keys = self._kc__need_keys.copy()
+
+        for line_no, line in enumerate(raw.split('\n'), 1):
+
+            if (line == '') or _re.match(r'\s*#--.*', line):
+                ## blank-line or comment-header
+                continue
+
+            res = _re.match(
+                r'\s*(?P<key>.+?)\s*:\s*(?P<val>.+?)\s*(?:#--.*)?;',
+                ## added ";" to capture "everything" in `val` (but not
+                ## the *last-spaces and comment* after it). The pattern doesn't
+                ## work without it
+                line + ';'
+            )
+            if res is None:
+                raise SyntaxError(
+                    f'KeyCrate file {repr(self._kc__file_pth)} '
+                    f'has invalid syntax at line {line_no}: {repr(line)}'
+                )
+
+            key = res.group('key')
+            val = res.group('val')
+
+            if key in self.__dict__:
+                raise ValueError(
+                    f'KeyCrate file {repr(self._kc__file_pth)} '
+                    f'has a duplicated key {repr(key)} found at line {line_no}.'
+                )
+
+            if self._kc__key_is_var:
+                if not _is_valid_var_name(key):
+                    raise AssertionError(
+                        f'KeyCrate file {repr(self._kc__file_pth)} '
+                        f'has a key {repr(key)} that is invalid for a variable name, found at line {line_no}.'
+                    )
+
+            if self._kc__eval_value:
+                try:
+                    val = eval(val, {})
+                except (NameError, SyntaxError):
+                    raise AssertionError(
+                        f'KeyCrate file {repr(self._kc__file_pth)} '
+                        f'has a value {repr(val)} that cannot be evaluated, found at line {line_no}.'
+                    )
+
+            if self._kc__only_keys is not None:
+                if key not in self._kc__only_keys:
+                    raise AssertionError(
+                        f'KeyCrate file {repr(self._kc__file_pth)} '
+                        f'has an unexpected key {repr(key)} found at line {line_no}.'
+                    )
+
+            if self._kc__need_keys:
+                try:
+                    _need_keys.remove(key)
+                except ValueError:
+                    ## note that if `need_keys` is specified, other keys
+                    ## (not in `need_keys`) are also allowed.
+                    ## so, this exception must be handled
+                    pass
+
+            setattr(self, key, val)
+
+        if self._kc__need_keys:
+            if _need_keys != []:
+                raise AssertionError(
+                    f'KeyCrate file {repr(self._kc__file_pth)} is missing keys: '
+                    + ', '.join(map(repr, _need_keys))
+                )
+
+    def open(self) -> None:
+        """open the .txt file"""
         _open_file(self._kc__file_pth)
```

### Comparing `mykit-2.0.0rc3/mykit/kit/neuralnet/dense.py` & `mykit-2.0.1/mykit/kit/neuralnet/dense.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-import numpy as _np
-import random as _random
-import typing as _typing
-
-from mykit.kit.math import relu as _ReLU
-
-
-class DenseNN:
-    """Also known as fully connected neural networks"""
-
-    def __init__(
-        self,
-        sizes: list[int],
-        hidden_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
-        output_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
-        load_weights_and_biases: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
-    ) -> None:
-        """
-        The network uses normalized Xavier weight initialization and cross-entropy loss function.
-
-        ---
-
-        `load_weights_and_biases`: Pre-loaded weights and biases decoded by `decode` method. `None` for a new network.
-        """
-
-        self.sizes = sizes
-        self.hidden_act_fn = hidden_act_fn
-        self.output_act_fn = output_act_fn
-
-        if load_weights_and_biases is None:
-            self.weights = [
-                -_np.sqrt(6/(x+y)) + _np.random.rand(y, x)*2*_np.sqrt(6/(x+y))  # normalized Xavier
-                for x, y in zip(self.sizes[:-1], self.sizes[1:])
-            ]
-            self.biases = [
-                _np.random.randn(y, 1)
-                for y in self.sizes[1:]
-            ]
-        else:
-            self.weights, self.biases = load_weights_and_biases
-
-        self.n_layer = len(sizes)
-        self.n_input = sizes[0]
-        self.hidden_layers = sizes[1:-1]
-        self.n_hidden_layer = len(self.hidden_layers)
-        self.n_output = sizes[-1]
-
-        ## values of these list are from the last feedforwarding
-        self.z_values = []
-        self.a_values = []
-        self.decision = None  # the index of the output neuron with highest value
-
-    def feedforward(self, a: _np.ndarray) -> int:
-        """
-        feedforward for given input `a`.
-
-        ---
-
-        ## Params
-        `a`: Input array with shape `(n, 1)`.
-            Example: `np.array([[i1], [i2], [i3], ...])`
-        
-        ## Returns
-        The index of the maximum value in the output array.
-        """
-
-        ## reset
-        self.z_values = []
-        self.a_values = [a]
-
-        ## if `self.n_layer` is 4 -> the variable `idx` below will be: 0, 1, 2
-        for idx, (w, b) in enumerate(zip(self.weights, self.biases)):
-
-            z = _np.dot(w, a) + b
-
-            if idx == (self.n_layer - 2):  # output layer
-                a = self.output_act_fn(z)
-            else:
-                a = self.hidden_act_fn(z)
-
-            ## used for backpropagation
-            self.z_values.append(z)
-            self.a_values.append(a)
-
-        self.decision = a.argmax()  # the index of the maximum value in `a`
-        return self.decision
-
-    def _backprop(self, inputs: _np.ndarray, outputs: _np.ndarray):
-        """
-        backpropagation algorithm.
-
-        ---
-
-        ## Params
-        `inputs`: Input array with shape `(n, 1)`.
-            Example: `np.array([[i1], [i2], [i3], ...])`
-        `outputs`: Desired output array with shape `(m, 1)`.
-            Example: `np.array([[o1], [o2], [o3], ...])`
-
-        ## Returns
-        `tuple[dgw, dgb]`: Gradients of weights and biases as lists.
-        """
-
-        self.feedforward(inputs)
-
-        ## gradient delta
-        dgw = [_np.zeros(w.shape) for w in self.weights]
-        dgb = [_np.zeros(b.shape) for b in self.biases]
-
-        ## output layer
-        delta = self.a_values[-1] - outputs  # using cross-entropy loss function
-        dgw[-1] = _np.dot(delta, self.a_values[-2].transpose())
-        dgb[-1] = delta
-
-        ## hidden layers
-        for l in range(2, self.n_layer):
-            delta = _np.dot(self.weights[-l + 1].transpose(), delta)*self.hidden_act_fn(self.z_values[-l], derivative=True)
-            dgw[-l] = _np.dot(delta, self.a_values[-l - 1].transpose())
-            dgb[-l] = delta
-
-        return (dgw, dgb)
-
-    def _tuning(self, samples: list[tuple[_np.ndarray, _np.ndarray]], k1: float, k2: float) -> None:
-        """
-        Update weights and biases.
-
-        ---
-        
-        ## Params
-            - `samples`: A list of input-output pairs used for updating the model
-            - For optimization purposes, these values are precalculated:
-                - `k1`: `learning_rate*(regularization/n_training_data)`
-                - `k2`: `learning_rate/len(samples)`
-        """
-
-        ## Initialize gradients
-        gw = [_np.zeros(w.shape) for w in self.weights]
-        gb = [_np.zeros(b.shape) for b in self.biases]
-
-        ## Compute gradients
-        for inputs, outputs in samples:
-            dgw, dgb = self._backprop(inputs, outputs)
-
-            gw = [_gw + _dgw for _gw, _dgw in zip(gw, dgw)]
-            gb = [_gb + _dgb for _gb, _dgb in zip(gb, dgb)]
-
-        ## Update weights and biases
-        self.weights = [
-            (1 - k1)*w - k2*_gw
-            for w, _gw in zip(self.weights, gw)
-        ]
-        self.biases = [
-            b - k2*_gb
-            for b, _gb in zip(self.biases, gb)
-        ]
-
-    def train(
-        self,
-        training_data: list[tuple[_np.ndarray, _np.ndarray]],
-        sample_size: int,
-        n_epoch: int,
-        learning_rate: float = 0.005,
-        regularization: float = 0.001
-    ) -> None:
-        """
-        Trains the model using gradient descent with regularization.
-
-        ---
-
-        ## Params
-            - `training_data`: A list of tuples containing input-output pairs
-            - `sample_size`: The number of samples to use for each iteration of gradient descent
-                - `sample_size = 1` for stochastic gradient descent
-                - `1 < sample_size < n_training_data` for mini-batch gradient descent
-                - `sample_size = n_training_data` for batch gradient descent
-            - `n_epoch`: The number of times to iterate over the entire training dataset
-            - `learning_rate`: The learning rate used for gradient descent
-            - `regularization`: The regularization factor to prevent overfitting
-        """
-
-        n_training_data = len(training_data)
-
-        k1 = learning_rate*(regularization/n_training_data)
-
-        for _ in range(n_epoch):
-
-            _random.shuffle(training_data)
-            list_of_samples = [
-                training_data[i : i + sample_size]
-                for i in range(0, n_training_data, sample_size)
-            ]
-
-            for samples in list_of_samples:
-                self._tuning(samples, k1, learning_rate/len(samples))
-
-
-    def encode(self) -> dict:
-        """Encode the weights and biases as a JSON-serializable dictionary."""
-        encoded_data = {
-            'weights': [w.tolist() for w in self.weights],
-            'biases': [b.tolist() for b in self.biases]
-        }
-        return encoded_data
-
-    @staticmethod
-    def decode(encoded_data: dict) -> tuple[list[_np.ndarray], list[_np.ndarray]]:
-        """Decode the weights and biases from what is encoded by the `encode` method."""
-        weights = [_np.array(w) for w in encoded_data['weights']]
-        biases = [_np.array(b) for b in encoded_data['biases']]
+import numpy as _np
+import random as _random
+import typing as _typing
+
+from mykit.kit.math import relu as _ReLU
+
+
+class DenseNN:
+    """Also known as fully connected neural networks"""
+
+    def __init__(
+        self,
+        sizes: list[int],
+        hidden_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
+        output_act_fn: _typing.Callable[[_np.ndarray, bool], _np.ndarray] = _ReLU,
+        load_weights_and_biases: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
+    ) -> None:
+        """
+        The network uses normalized Xavier weight initialization and cross-entropy loss function.
+
+        ---
+
+        `load_weights_and_biases`: Pre-loaded weights and biases decoded by `decode` method. `None` for a new network.
+        """
+
+        self.sizes = sizes
+        self.hidden_act_fn = hidden_act_fn
+        self.output_act_fn = output_act_fn
+
+        if load_weights_and_biases is None:
+            self.weights = [
+                -_np.sqrt(6/(x+y)) + _np.random.rand(y, x)*2*_np.sqrt(6/(x+y))  # normalized Xavier
+                for x, y in zip(self.sizes[:-1], self.sizes[1:])
+            ]
+            self.biases = [
+                _np.random.randn(y, 1)
+                for y in self.sizes[1:]
+            ]
+        else:
+            self.weights, self.biases = load_weights_and_biases
+
+        self.n_layer = len(sizes)
+        self.n_input = sizes[0]
+        self.hidden_layers = sizes[1:-1]
+        self.n_hidden_layer = len(self.hidden_layers)
+        self.n_output = sizes[-1]
+
+        ## values of these list are from the last feedforwarding
+        self.z_values = []
+        self.a_values = []
+        self.decision = None  # the index of the output neuron with highest value
+
+    def feedforward(self, a: _np.ndarray) -> int:
+        """
+        feedforward for given input `a`.
+
+        ---
+
+        ## Params
+        `a`: Input array with shape `(n, 1)`.
+            Example: `np.array([[i1], [i2], [i3], ...])`
+        
+        ## Returns
+        The index of the maximum value in the output array.
+        """
+
+        ## reset
+        self.z_values = []
+        self.a_values = [a]
+
+        ## if `self.n_layer` is 4 -> the variable `idx` below will be: 0, 1, 2
+        for idx, (w, b) in enumerate(zip(self.weights, self.biases)):
+
+            z = _np.dot(w, a) + b
+
+            if idx == (self.n_layer - 2):  # output layer
+                a = self.output_act_fn(z)
+            else:
+                a = self.hidden_act_fn(z)
+
+            ## used for backpropagation
+            self.z_values.append(z)
+            self.a_values.append(a)
+
+        self.decision = a.argmax()  # the index of the maximum value in `a`
+        return self.decision
+
+    def _backprop(self, inputs: _np.ndarray, outputs: _np.ndarray):
+        """
+        backpropagation algorithm.
+
+        ---
+
+        ## Params
+        `inputs`: Input array with shape `(n, 1)`.
+            Example: `np.array([[i1], [i2], [i3], ...])`
+        `outputs`: Desired output array with shape `(m, 1)`.
+            Example: `np.array([[o1], [o2], [o3], ...])`
+
+        ## Returns
+        `tuple[dgw, dgb]`: Gradients of weights and biases as lists.
+        """
+
+        self.feedforward(inputs)
+
+        ## gradient delta
+        dgw = [_np.zeros(w.shape) for w in self.weights]
+        dgb = [_np.zeros(b.shape) for b in self.biases]
+
+        ## output layer
+        delta = self.a_values[-1] - outputs  # using cross-entropy loss function
+        dgw[-1] = _np.dot(delta, self.a_values[-2].transpose())
+        dgb[-1] = delta
+
+        ## hidden layers
+        for l in range(2, self.n_layer):
+            delta = _np.dot(self.weights[-l + 1].transpose(), delta)*self.hidden_act_fn(self.z_values[-l], derivative=True)
+            dgw[-l] = _np.dot(delta, self.a_values[-l - 1].transpose())
+            dgb[-l] = delta
+
+        return (dgw, dgb)
+
+    def _tuning(self, samples: list[tuple[_np.ndarray, _np.ndarray]], k1: float, k2: float) -> None:
+        """
+        Update weights and biases.
+
+        ---
+        
+        ## Params
+            - `samples`: A list of input-output pairs used for updating the model
+            - For optimization purposes, these values are precalculated:
+                - `k1`: `learning_rate*(regularization/n_training_data)`
+                - `k2`: `learning_rate/len(samples)`
+        """
+
+        ## Initialize gradients
+        gw = [_np.zeros(w.shape) for w in self.weights]
+        gb = [_np.zeros(b.shape) for b in self.biases]
+
+        ## Compute gradients
+        for inputs, outputs in samples:
+            dgw, dgb = self._backprop(inputs, outputs)
+
+            gw = [_gw + _dgw for _gw, _dgw in zip(gw, dgw)]
+            gb = [_gb + _dgb for _gb, _dgb in zip(gb, dgb)]
+
+        ## Update weights and biases
+        self.weights = [
+            (1 - k1)*w - k2*_gw
+            for w, _gw in zip(self.weights, gw)
+        ]
+        self.biases = [
+            b - k2*_gb
+            for b, _gb in zip(self.biases, gb)
+        ]
+
+    def train(
+        self,
+        training_data: list[tuple[_np.ndarray, _np.ndarray]],
+        sample_size: int,
+        n_epoch: int,
+        learning_rate: float = 0.005,
+        regularization: float = 0.001
+    ) -> None:
+        """
+        Trains the model using gradient descent with regularization.
+
+        ---
+
+        ## Params
+            - `training_data`: A list of tuples containing input-output pairs
+            - `sample_size`: The number of samples to use for each iteration of gradient descent
+                - `sample_size = 1` for stochastic gradient descent
+                - `1 < sample_size < n_training_data` for mini-batch gradient descent
+                - `sample_size = n_training_data` for batch gradient descent
+            - `n_epoch`: The number of times to iterate over the entire training dataset
+            - `learning_rate`: The learning rate used for gradient descent
+            - `regularization`: The regularization factor to prevent overfitting
+        """
+
+        n_training_data = len(training_data)
+
+        k1 = learning_rate*(regularization/n_training_data)
+
+        for _ in range(n_epoch):
+
+            _random.shuffle(training_data)
+            list_of_samples = [
+                training_data[i : i + sample_size]
+                for i in range(0, n_training_data, sample_size)
+            ]
+
+            for samples in list_of_samples:
+                self._tuning(samples, k1, learning_rate/len(samples))
+
+
+    def encode(self) -> dict:
+        """Encode the weights and biases as a JSON-serializable dictionary."""
+        encoded_data = {
+            'weights': [w.tolist() for w in self.weights],
+            'biases': [b.tolist() for b in self.biases]
+        }
+        return encoded_data
+
+    @staticmethod
+    def decode(encoded_data: dict) -> tuple[list[_np.ndarray], list[_np.ndarray]]:
+        """Decode the weights and biases from what is encoded by the `encode` method."""
+        weights = [_np.array(w) for w in encoded_data['weights']]
+        biases = [_np.array(b) for b in encoded_data['biases']]
         return weights, biases
```

### Comparing `mykit-2.0.0rc3/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.1/mykit/kit/neuralnet/genetic.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,377 +1,377 @@
-import random as _random
-import numpy as _np
-import typing as _typing
-
-from mykit.kit.neuralnet.dense import DenseNN as _DenseNN
-
-
-class GeneticNN:
-
-    def __init__(
-        self,
-        layer_sizes: list[int],
-        hidden_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
-        output_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
-
-        population_size: int,
-        crossover_threshold: float = 0.001,
-        mutation1_rate: float = 0.85,
-        mutation2_rate: float = 0.99,
-        mutation2_range: tuple[float, float] = (0.1, 2.5),
-        n_new: int = 0,
-        init_score: float = 0,
-        
-        load_wnb: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
-    ) -> None:
-        """
-        Genetic neural network using dense neural network.
-
-        ---
-
-        ## Params
-        - `layer_sizes`: The size of the dense neural network for each individual.
-        - `population_size`: Number of individuals per generation.
-        - `crossover_threshold`: Determines how weights/biases from parent1 and parent2 are
-                                 combined during crossover. If the difference between parent1
-                                 and parent2 is less than this threshold, the child's value
-                                 is the average; otherwise, it's randomly selected from
-                                 either parent1 or parent2.
-        - `mutation1_rate`: The probability of mutating a weight or bias (parent1/parent2 are close). Range: 0-1.
-        - `mutation2_rate`: The probability of mutating a weight or bias (parent1/parent2 are different). Range: 0-1.
-        - `mutation2_range`: The range of mutation change. For example, if set to (0.001, 0.1),
-                             the weight or bias can be offset by a random value between 0.001
-                             and 0.1, or between -0.001 and -0.1.
-        - `n_new`: Number of new individuals (neither parent nor child) for each subsequent generation,
-                   with the constraint `n_new < population_size-3`.
-        - `init_score`: Initial score
-        - `load_wnb`: Populate the first generation with pretrained weights and biases (use this
-                      if you don't want to start the training from the beginning again).
-        """
-
-        self.layer_sizes = layer_sizes
-        self.hidden_act = hidden_act
-        self.output_act = output_act
-
-        self.population_size = population_size
-        self.crossover_threshold = crossover_threshold
-        self.mutation1_rate = mutation1_rate
-        self.mutation2_rate = mutation2_rate
-        self.mutation2_range = mutation2_range
-        self.n_new = n_new
-        self.init_score = init_score
-
-        self.population: dict[_DenseNN, float] = {}
-        for _ in range(population_size):
-
-            if load_wnb is None:
-                wnb = None
-            else:
-                w = [w.copy() for w in load_wnb[0]]
-                b = [b.copy() for b in load_wnb[1]]
-                wnb = (w, b)
-
-            nn = _DenseNN(layer_sizes, hidden_act, output_act, wnb)
-            self.population[nn] = init_score
-
-
-        ## runtime
-
-        self.the_parent: tuple[_DenseNN, _DenseNN] = None  # to store the parent that produced the current generation (after executing `keep_elites()`)
-        self.prev: dict[_DenseNN, float] = {}  # to store the previous generation
-
-
-    def set_score(self, individual: _DenseNN, score: float, /) -> None:
-        self.population[individual] = score
-
-    def get_score(self, individual: _DenseNN, /) -> float:
-        return self.population[individual]
-
-    def get_score_min(self) -> float:
-        """Return the lowest score of all individuals."""
-        return min(self.population.values())
-
-    def get_score_max(self) -> float:
-        """Return the highest score of all individuals."""
-        return max(self.population.values())
-
-    def get_score_avg(self) -> float:
-        """Return the average score of all individuals."""
-        return sum(self.population.values()) / self.population_size
-
-    def get_individual_by_rank(self, rank: int) -> _DenseNN:
-        """Returns the individual with the given rank: 0 for the best, 1 for the second best, and so on."""
-        return sorted(self.population, key=self.population.get, reverse=True)[rank]
-
-    def get_best_individual(self) -> _DenseNN:
-        """Returns the best individual (with the highest score) from the current generation."""
-        return self.get_individual_by_rank(0)
-
-    def keep_elites(self) -> None:
-        """
-        The idea is to continually bring out the most fit individuals from one generation to the next.
-        Note: Remember to use this function after updating the scores and before executing `next_generation()`.
-
-        ---
-
-        What's the idea behind this function?
-        =====================================
-
-        Let's say there are only three individuals in each generation.
-
-        - first generation -
-
-            1. self.population = {A:0, B:0, C:0} <- each score is set to 0
-
-            2. a new environment is set
-
-            3. A B C undergo the scoring system and let's say the scores:
-               self.population = {A:2, B:3, C:1}
-
-            4. `keep_elites()`:
-
-               sorted:
-               {B:3, A:2, C:1}
-
-               store the parent:
-               self.the_parent = (B, A)
-
-               store the prev:
-               self.prev = self.population = {A:2, B:3, C:1}
-
-        - 2nd generation -
-            
-            1. `next_generation()`:
-               
-               A and B are the top two, producing one child D.
-               now, the current population:
-               self.population = {A:0, B:0, D:0}
-
-            2. a new environment is set
-
-            3. A B D undergo the scoring system
-
-            == Case I (Overall Upgrade) ==
-
-                3. let's say the scores:
-                   self.population = {A:4, B:5, D:7}
-
-                4. `keep_elites()`:
-
-                    picking the fitter parent:
-                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:4, B:5, D:7}`
-                    result: self.prev = {C:1} and self.population = {A:4, B:5, D:7}
-
-                    combine:
-                    {A:4, B:5, D:7, C:1}
-
-                    sort:
-                    {D:7, B:5, A:4, C:1}
-
-                    pick the fittest:
-                    {D:7, B:5, A:4}
-
-                    set to current population:
-                    self.population = {D:7, B:5, A:4}
-
-                    store the parent:
-                    self.the_parent = (D, B)
-
-                    stored in self.prev:
-                    self.prev = self.population = {D:7, B:5, A:4}
-
-                In other words, A and B work better in this environment.
-                This is the ideal case where overall improvement occurs.
-
-            == Case II (Overall Downgrade) ==
-                
-                3. let's say the scores:
-                   self.population = {A:0, B:0, D:0}
-
-                4. `keep_elites()`:
-
-                    picking the fitter parent:
-                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:0, B:0, D:0}`
-                    result: self.prev = {A:2, B:3, C:1} and self.population = {D:0}
-
-                    combine:
-                    {D:0, A:2, B:3, C:1}
-
-                    sort:
-                    {B:3, A:2, C:1, D:0}
-
-                    pick the fittest:
-                    {B:3, A:2, C:1}
-
-                    set to current population:
-                    self.population = {B:3, A:2, C:1}
-
-                    ########################################################
-                    let's contrast keeping the fittest from the previous generation versus not keeping them
-
-                    if not:
-                        current population:
-                        self.population = {A:0, B:0, D:0}
-
-                        potential parents: A/B or A/D or B/D
-                        A/B is the same as before
-                        but A/D or B/D is something different (see below for the considerations)
-
-                    if yes:
-                        current population:
-                        self.population = {B:3, A:2, C:1}
-
-                        parent: A and B
-                    ########################################################
-                
-                    store the parent:
-                    self.the_parent = (B, A)
-
-                    stored in self.prev:
-                    self.prev = self.population = {B:3, A:2, C:1}
-
-                Note that while A B C has already experimented with 2 different environments, D has only done so once.
-                In other words, the "veterans" are prioritized, meaning we stick with
-                the previous generation and move to the next environment, even if A and B
-                perform poorly in the current environment.
-
-            Case III (Mix):
-
-                3. let's say the scores:
-                   self.population = {A:5, B:0, D:0}
-                
-                4. `keep_elites()`:
-
-                    picking the fitter parent:
-                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:5, B:0, D:0}`
-                    result: self.prev = {B:3, C:1} and self.population = {A:5, D:0}
-
-                    combine:
-                    {A:5, D:0, B:3, C:1}
-
-                    sort:
-                    {A:5, B:3, C:1, D:0}
-
-                    pick the fittest:
-                    {A:5, B:3, C:1}
-
-                    set to current population:
-                    self.population = {A:5, B:3, C:1}
-                
-                    store the parent:
-                    self.the_parent = (A, B)
-
-                    stored in self.prev:
-                    self.prev = self.population = {A:5, B:3, C:1}
-
-                In other words, stick with the previous generation and move to the next environment.
-        """
-
-        ## handle the first generation case
-        if self.the_parent is None:
-            parent1, parent2 = sorted(self.population, key=self.population.get, reverse=True)[:2]
-            self.the_parent = (parent1, parent2)
-            self.prev = self.population
-        else:
-
-            ## picking the fitter parent
-            for parent in self.the_parent:
-                old = self.prev[parent]
-                new = self.population[parent]
-                if new >= old:
-                    self.prev.pop(parent)
-                else:
-                    self.population.pop(parent)
-
-            ## combine
-            combined = self.population
-            combined.update(self.prev)
-
-            ## sort
-            sorted_ = dict(sorted(combined.items(), key=lambda item: item[1], reverse=True))
-
-            ## pick the fittest (pick the top `self.population_size`)
-            fittest = {k: sorted_[k] for k in list(sorted_)[:self.population_size]}
-
-            ## set to current population
-            self.population = fittest
-
-            parent1, parent2 = sorted(self.population, key=self.population.get, reverse=True)[:2]
-            self.the_parent = (parent1, parent2)
-            self.prev = self.population
-
-    def next_generation(self) -> None:
-        """
-        When executed, this function updates `self.population` by selecting the top 2 individuals
-        with the highest scores from the current `self.population` and applying crossover
-        and mutation to produce the new generation (the new `self.population`).
-
-        Note: Remember to execute this after executing `keep_elites()`.
-
-        Reminder:
-        - weight and bias may have different mutation methods
-        """
-
-        ## getting the best two parents with the highest scores
-        parent1, parent2 = self.the_parent
-
-        self.population = {parent1: self.init_score, parent2: self.init_score}
-
-        ## reproduce
-        for _ in range(self.population_size-2-self.n_new):
-
-            child = _DenseNN(self.layer_sizes, self.hidden_act, self.output_act)
-
-            ## weights
-            for l in range(len(self.layer_sizes)):  # iterate through each layer
-                for c in range(self.layer_sizes[l]):  # iterate through each neuron in the current layer
-
-                    if l != (len(self.layer_sizes)-1):
-                        for s in range(self.layer_sizes[l+1]):  # iterate through each neuron in the subsequent layer
-                            
-                            w1 = parent1.weights[l][s, c]
-                            w2 = parent2.weights[l][s, c]
-
-                            ## crossover
-                            if abs(w2-w1) < self.crossover_threshold:
-                                w = (w1+w2)/2
-                                ## mutation-1
-                                if _random.random() < self.mutation1_rate:
-                                    w = _np.random.randn()
-                            else:
-                                w = _random.choice([w1, w2])
-                                ## mutation-2
-                                if _random.random() < self.mutation2_rate:
-                                    w += _random.uniform(*self.mutation2_range)*_random.choice([-1, 1])
-                                    if abs(w) > 5:  # prevent explosion
-                                        w = _np.random.randn()
-
-                            child.weights[l][s, c] = w
-                    
-            ## biases
-            for i in range(len(self.layer_sizes)-1):  # note that the input layer does not have biases
-                for j in range(self.layer_sizes[i+1]):
-                    
-                    b1 = parent1.biases[i][j, 0]
-                    b2 = parent2.biases[i][j, 0]
-
-                    ## crossover
-                    if abs(b2-b1) < self.crossover_threshold:
-                        b = (b1+b2)/2
-                        ## mutation-1
-                        if _random.random() < self.mutation1_rate:
-                            b = _np.random.randn()
-                    else:
-                        b = _random.choice([b1, b2])
-                        ## mutation-2
-                        if _random.random() < self.mutation2_rate:
-                            b += _random.uniform(*self.mutation2_range)*_random.choice([-1, 1])
-                            if abs(b) > 5:
-                                b = _np.random.randn()
-
-                    child.biases[i][j, 0] = b
-
-            ## add it to the population
-            self.population[child] = self.init_score
-
-        for _ in range(self.n_new):
-            self.population[_DenseNN(self.layer_sizes, self.hidden_act, self.output_act)] = self.init_score
+import random as _random
+import numpy as _np
+import typing as _typing
+
+from mykit.kit.neuralnet.dense import DenseNN as _DenseNN
+
+
+class GeneticNN:
+
+    def __init__(
+        self,
+        layer_sizes: list[int],
+        hidden_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
+        output_act: _typing.Callable[[_np.ndarray, bool], _np.ndarray],
+
+        population_size: int,
+        crossover_threshold: float = 0.001,
+        mutation1_rate: float = 0.85,
+        mutation2_rate: float = 0.99,
+        mutation2_range: tuple[float, float] = (0.1, 2.5),
+        n_new: int = 0,
+        init_score: float = 0,
+        
+        load_wnb: tuple[list[_np.ndarray], list[_np.ndarray]] | None = None,
+    ) -> None:
+        """
+        Genetic neural network using dense neural network.
+
+        ---
+
+        ## Params
+        - `layer_sizes`: The size of the dense neural network for each individual.
+        - `population_size`: Number of individuals per generation.
+        - `crossover_threshold`: Determines how weights/biases from parent1 and parent2 are
+                                 combined during crossover. If the difference between parent1
+                                 and parent2 is less than this threshold, the child's value
+                                 is the average; otherwise, it's randomly selected from
+                                 either parent1 or parent2.
+        - `mutation1_rate`: The probability of mutating a weight or bias (parent1/parent2 are close). Range: 0-1.
+        - `mutation2_rate`: The probability of mutating a weight or bias (parent1/parent2 are different). Range: 0-1.
+        - `mutation2_range`: The range of mutation change. For example, if set to (0.001, 0.1),
+                             the weight or bias can be offset by a random value between 0.001
+                             and 0.1, or between -0.001 and -0.1.
+        - `n_new`: Number of new individuals (neither parent nor child) for each subsequent generation,
+                   with the constraint `n_new < population_size-3`.
+        - `init_score`: Initial score
+        - `load_wnb`: Populate the first generation with pretrained weights and biases (use this
+                      if you don't want to start the training from the beginning again).
+        """
+
+        self.layer_sizes = layer_sizes
+        self.hidden_act = hidden_act
+        self.output_act = output_act
+
+        self.population_size = population_size
+        self.crossover_threshold = crossover_threshold
+        self.mutation1_rate = mutation1_rate
+        self.mutation2_rate = mutation2_rate
+        self.mutation2_range = mutation2_range
+        self.n_new = n_new
+        self.init_score = init_score
+
+        self.population: dict[_DenseNN, float] = {}
+        for _ in range(population_size):
+
+            if load_wnb is None:
+                wnb = None
+            else:
+                w = [w.copy() for w in load_wnb[0]]
+                b = [b.copy() for b in load_wnb[1]]
+                wnb = (w, b)
+
+            nn = _DenseNN(layer_sizes, hidden_act, output_act, wnb)
+            self.population[nn] = init_score
+
+
+        ## runtime
+
+        self.the_parent: tuple[_DenseNN, _DenseNN] = None  # to store the parent that produced the current generation (after executing `keep_elites()`)
+        self.prev: dict[_DenseNN, float] = {}  # to store the previous generation
+
+
+    def set_score(self, individual: _DenseNN, score: float, /) -> None:
+        self.population[individual] = score
+
+    def get_score(self, individual: _DenseNN, /) -> float:
+        return self.population[individual]
+
+    def get_score_min(self) -> float:
+        """Return the lowest score of all individuals."""
+        return min(self.population.values())
+
+    def get_score_max(self) -> float:
+        """Return the highest score of all individuals."""
+        return max(self.population.values())
+
+    def get_score_avg(self) -> float:
+        """Return the average score of all individuals."""
+        return sum(self.population.values()) / self.population_size
+
+    def get_individual_by_rank(self, rank: int) -> _DenseNN:
+        """Returns the individual with the given rank: 0 for the best, 1 for the second best, and so on."""
+        return sorted(self.population, key=self.population.get, reverse=True)[rank]
+
+    def get_best_individual(self) -> _DenseNN:
+        """Returns the best individual (with the highest score) from the current generation."""
+        return self.get_individual_by_rank(0)
+
+    def keep_elites(self) -> None:
+        """
+        The idea is to continually bring out the most fit individuals from one generation to the next.
+        Note: Remember to use this function after updating the scores and before executing `next_generation()`.
+
+        ---
+
+        What's the idea behind this function?
+        =====================================
+
+        Let's say there are only three individuals in each generation.
+
+        - first generation -
+
+            1. self.population = {A:0, B:0, C:0} <- each score is set to 0
+
+            2. a new environment is set
+
+            3. A B C undergo the scoring system and let's say the scores:
+               self.population = {A:2, B:3, C:1}
+
+            4. `keep_elites()`:
+
+               sorted:
+               {B:3, A:2, C:1}
+
+               store the parent:
+               self.the_parent = (B, A)
+
+               store the prev:
+               self.prev = self.population = {A:2, B:3, C:1}
+
+        - 2nd generation -
+            
+            1. `next_generation()`:
+               
+               A and B are the top two, producing one child D.
+               now, the current population:
+               self.population = {A:0, B:0, D:0}
+
+            2. a new environment is set
+
+            3. A B D undergo the scoring system
+
+            == Case I (Overall Upgrade) ==
+
+                3. let's say the scores:
+                   self.population = {A:4, B:5, D:7}
+
+                4. `keep_elites()`:
+
+                    picking the fitter parent:
+                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:4, B:5, D:7}`
+                    result: self.prev = {C:1} and self.population = {A:4, B:5, D:7}
+
+                    combine:
+                    {A:4, B:5, D:7, C:1}
+
+                    sort:
+                    {D:7, B:5, A:4, C:1}
+
+                    pick the fittest:
+                    {D:7, B:5, A:4}
+
+                    set to current population:
+                    self.population = {D:7, B:5, A:4}
+
+                    store the parent:
+                    self.the_parent = (D, B)
+
+                    stored in self.prev:
+                    self.prev = self.population = {D:7, B:5, A:4}
+
+                In other words, A and B work better in this environment.
+                This is the ideal case where overall improvement occurs.
+
+            == Case II (Overall Downgrade) ==
+                
+                3. let's say the scores:
+                   self.population = {A:0, B:0, D:0}
+
+                4. `keep_elites()`:
+
+                    picking the fitter parent:
+                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:0, B:0, D:0}`
+                    result: self.prev = {A:2, B:3, C:1} and self.population = {D:0}
+
+                    combine:
+                    {D:0, A:2, B:3, C:1}
+
+                    sort:
+                    {B:3, A:2, C:1, D:0}
+
+                    pick the fittest:
+                    {B:3, A:2, C:1}
+
+                    set to current population:
+                    self.population = {B:3, A:2, C:1}
+
+                    ########################################################
+                    let's contrast keeping the fittest from the previous generation versus not keeping them
+
+                    if not:
+                        current population:
+                        self.population = {A:0, B:0, D:0}
+
+                        potential parents: A/B or A/D or B/D
+                        A/B is the same as before
+                        but A/D or B/D is something different (see below for the considerations)
+
+                    if yes:
+                        current population:
+                        self.population = {B:3, A:2, C:1}
+
+                        parent: A and B
+                    ########################################################
+                
+                    store the parent:
+                    self.the_parent = (B, A)
+
+                    stored in self.prev:
+                    self.prev = self.population = {B:3, A:2, C:1}
+
+                Note that while A B C has already experimented with 2 different environments, D has only done so once.
+                In other words, the "veterans" are prioritized, meaning we stick with
+                the previous generation and move to the next environment, even if A and B
+                perform poorly in the current environment.
+
+            Case III (Mix):
+
+                3. let's say the scores:
+                   self.population = {A:5, B:0, D:0}
+                
+                4. `keep_elites()`:
+
+                    picking the fitter parent:
+                    comparing `self.prev = {A:2, B:3, C:1}` with `self.population = {A:5, B:0, D:0}`
+                    result: self.prev = {B:3, C:1} and self.population = {A:5, D:0}
+
+                    combine:
+                    {A:5, D:0, B:3, C:1}
+
+                    sort:
+                    {A:5, B:3, C:1, D:0}
+
+                    pick the fittest:
+                    {A:5, B:3, C:1}
+
+                    set to current population:
+                    self.population = {A:5, B:3, C:1}
+                
+                    store the parent:
+                    self.the_parent = (A, B)
+
+                    stored in self.prev:
+                    self.prev = self.population = {A:5, B:3, C:1}
+
+                In other words, stick with the previous generation and move to the next environment.
+        """
+
+        ## handle the first generation case
+        if self.the_parent is None:
+            parent1, parent2 = sorted(self.population, key=self.population.get, reverse=True)[:2]
+            self.the_parent = (parent1, parent2)
+            self.prev = self.population
+        else:
+
+            ## picking the fitter parent
+            for parent in self.the_parent:
+                old = self.prev[parent]
+                new = self.population[parent]
+                if new >= old:
+                    self.prev.pop(parent)
+                else:
+                    self.population.pop(parent)
+
+            ## combine
+            combined = self.population
+            combined.update(self.prev)
+
+            ## sort
+            sorted_ = dict(sorted(combined.items(), key=lambda item: item[1], reverse=True))
+
+            ## pick the fittest (pick the top `self.population_size`)
+            fittest = {k: sorted_[k] for k in list(sorted_)[:self.population_size]}
+
+            ## set to current population
+            self.population = fittest
+
+            parent1, parent2 = sorted(self.population, key=self.population.get, reverse=True)[:2]
+            self.the_parent = (parent1, parent2)
+            self.prev = self.population
+
+    def next_generation(self) -> None:
+        """
+        When executed, this function updates `self.population` by selecting the top 2 individuals
+        with the highest scores from the current `self.population` and applying crossover
+        and mutation to produce the new generation (the new `self.population`).
+
+        Note: Remember to execute this after executing `keep_elites()`.
+
+        Reminder:
+        - weight and bias may have different mutation methods
+        """
+
+        ## getting the best two parents with the highest scores
+        parent1, parent2 = self.the_parent
+
+        self.population = {parent1: self.init_score, parent2: self.init_score}
+
+        ## reproduce
+        for _ in range(self.population_size-2-self.n_new):
+
+            child = _DenseNN(self.layer_sizes, self.hidden_act, self.output_act)
+
+            ## weights
+            for l in range(len(self.layer_sizes)):  # iterate through each layer
+                for c in range(self.layer_sizes[l]):  # iterate through each neuron in the current layer
+
+                    if l != (len(self.layer_sizes)-1):
+                        for s in range(self.layer_sizes[l+1]):  # iterate through each neuron in the subsequent layer
+                            
+                            w1 = parent1.weights[l][s, c]
+                            w2 = parent2.weights[l][s, c]
+
+                            ## crossover
+                            if abs(w2-w1) < self.crossover_threshold:
+                                w = (w1+w2)/2
+                                ## mutation-1
+                                if _random.random() < self.mutation1_rate:
+                                    w = _np.random.randn()
+                            else:
+                                w = _random.choice([w1, w2])
+                                ## mutation-2
+                                if _random.random() < self.mutation2_rate:
+                                    w += _random.uniform(*self.mutation2_range)*_random.choice([-1, 1])
+                                    if abs(w) > 5:  # prevent explosion
+                                        w = _np.random.randn()
+
+                            child.weights[l][s, c] = w
+                    
+            ## biases
+            for i in range(len(self.layer_sizes)-1):  # note that the input layer does not have biases
+                for j in range(self.layer_sizes[i+1]):
+                    
+                    b1 = parent1.biases[i][j, 0]
+                    b2 = parent2.biases[i][j, 0]
+
+                    ## crossover
+                    if abs(b2-b1) < self.crossover_threshold:
+                        b = (b1+b2)/2
+                        ## mutation-1
+                        if _random.random() < self.mutation1_rate:
+                            b = _np.random.randn()
+                    else:
+                        b = _random.choice([b1, b2])
+                        ## mutation-2
+                        if _random.random() < self.mutation2_rate:
+                            b += _random.uniform(*self.mutation2_range)*_random.choice([-1, 1])
+                            if abs(b) > 5:
+                                b = _np.random.randn()
+
+                    child.biases[i][j, 0] = b
+
+            ## add it to the population
+            self.population[child] = self.init_score
+
+        for _ in range(self.n_new):
+            self.population[_DenseNN(self.layer_sizes, self.hidden_act, self.output_act)] = self.init_score
```

### Comparing `mykit-2.0.0rc3/mykit/kit/noise.py` & `mykit-2.0.1/mykit/kit/noise.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import math as _math
-import random as _random
-import time as _time
-
-
-def _non_periodic_fn(__x: float, /, a: float = 1, b: float = 1, c: float = 1, d: float = 1, e: float = 1, f: float = 1, g: float = 1):
-    """
-    proven non-periodic.
-    ref: https://stackoverflow.com/questions/8798771/perlin-noise-for-1d
-
-    ---
-
-    `__x` is in radian
-    """
-    return a*(b*_math.sin(c*__x) + d*_math.sin(e*_math.pi*__x) + f*_math.sin(g*_math.e*__x))
-
-def random_sine_noise(
-    seed: float,
-    nsample: int,
-    ymin: int,
-    ymax: int,
-    params: tuple = (1, 1, 1, 1, 1, 1, 1)
-) -> list[tuple[float, float]]:
-
-    _random.seed(seed)
-    shift = _random.randint(-1000000000, 1000000000)
-
-    points = []
-    for x in range(nsample):
-        x += shift
-        points.append((x, _non_periodic_fn(x*_math.pi/180, *params)))
-
-    ## adjusting the y interval
-    y_values = [point[1] for point in points]
-    ymin_current = min(y_values)
-    ymax_current = max(y_values)
-    scale_factor = (ymax - ymin) / (ymax_current - ymin_current)
-    points = [(x, ymin + (y - ymin_current)*scale_factor) for (x, y) in points]
-
-    return points
-
-
-def _pn1d_noise(x: int, seed: int) -> float:
-    """Generate deterministic noise based on the given seed."""
-    x = (x << 13) ^ x ^ seed
-    return 1.0 - ((x * (x * x * 15731 + 789221) + 1376312589) & 0x7fffffff) / 1073741824.0
-
-def _pn1d_noise_smoothed(x: int, seed: int) -> float:
-    """combines multiple noise samples to compute the final value"""
-    return _pn1d_noise(x, seed)/2 + _pn1d_noise(x - 1, seed)/4 + _pn1d_noise(x + 1, seed)/4
-
-def _pn1d_noise_interpolated(x: int, seed: int) -> float:
-    """using cubic interpolation"""
-    int_x = int(x)
-    frac_x = x - int_x
-
-    v0 = _pn1d_noise_smoothed(int_x - 1, seed)
-    v1 = _pn1d_noise_smoothed(int_x, seed)
-    v2 = _pn1d_noise_smoothed(int_x + 1, seed)
-    v3 = _pn1d_noise_smoothed(int_x + 2, seed)
-
-    ## cubic interpolation
-    p = (v3 - v2) - (v0 - v1)
-    q = (v0 - v1) - p
-    r = v2 - v0
-    s = v1
-    return p*frac_x*frac_x*frac_x + q*frac_x*frac_x + r*frac_x + s
-
-def perlin_noise_1d(x: float, /, persistence: float = 0.5, octaves: int = 1, frequency: int = 2, seed: int = _time.time()) -> float:
-    """
-    Generate 1D Perlin noise for the given input parameters.
-    ref: https://web.archive.org/web/20160530124230/http://freespace.virgin.net/hugo.elias/models/m_perlin.htm
-
-    ---
-
-    ## params
-        `x`: input value.
-        `persistence`: persistence value determining the amplitude decrease per octave.
-        `octaves`: number of octaves or levels of detail in the Perlin noise.
-        `frequency`: lower frequency results in higher detail.
-        `seed`: seed value for randomness.
-
-    ## returns
-        float: Perlin noise value
-    """
-    total = 0
-    for i in range(octaves):
-        f = frequency**i
-        amplitude = persistence**i
-        total += amplitude*_pn1d_noise_interpolated(x*f, seed)
-    return total
+import math as _math
+import random as _random
+import time as _time
+
+
+def _non_periodic_fn(__x: float, /, a: float = 1, b: float = 1, c: float = 1, d: float = 1, e: float = 1, f: float = 1, g: float = 1):
+    """
+    proven non-periodic.
+    ref: https://stackoverflow.com/questions/8798771/perlin-noise-for-1d
+
+    ---
+
+    `__x` is in radian
+    """
+    return a*(b*_math.sin(c*__x) + d*_math.sin(e*_math.pi*__x) + f*_math.sin(g*_math.e*__x))
+
+def random_sine_noise(
+    seed: float,
+    nsample: int,
+    ymin: int,
+    ymax: int,
+    params: tuple = (1, 1, 1, 1, 1, 1, 1)
+) -> list[tuple[float, float]]:
+
+    _random.seed(seed)
+    shift = _random.randint(-1000000000, 1000000000)
+
+    points = []
+    for x in range(nsample):
+        x += shift
+        points.append((x, _non_periodic_fn(x*_math.pi/180, *params)))
+
+    ## adjusting the y interval
+    y_values = [point[1] for point in points]
+    ymin_current = min(y_values)
+    ymax_current = max(y_values)
+    scale_factor = (ymax - ymin) / (ymax_current - ymin_current)
+    points = [(x, ymin + (y - ymin_current)*scale_factor) for (x, y) in points]
+
+    return points
+
+
+def _pn1d_noise(x: int, seed: int) -> float:
+    """Generate deterministic noise based on the given seed."""
+    x = (x << 13) ^ x ^ seed
+    return 1.0 - ((x * (x * x * 15731 + 789221) + 1376312589) & 0x7fffffff) / 1073741824.0
+
+def _pn1d_noise_smoothed(x: int, seed: int) -> float:
+    """combines multiple noise samples to compute the final value"""
+    return _pn1d_noise(x, seed)/2 + _pn1d_noise(x - 1, seed)/4 + _pn1d_noise(x + 1, seed)/4
+
+def _pn1d_noise_interpolated(x: int, seed: int) -> float:
+    """using cubic interpolation"""
+    int_x = int(x)
+    frac_x = x - int_x
+
+    v0 = _pn1d_noise_smoothed(int_x - 1, seed)
+    v1 = _pn1d_noise_smoothed(int_x, seed)
+    v2 = _pn1d_noise_smoothed(int_x + 1, seed)
+    v3 = _pn1d_noise_smoothed(int_x + 2, seed)
+
+    ## cubic interpolation
+    p = (v3 - v2) - (v0 - v1)
+    q = (v0 - v1) - p
+    r = v2 - v0
+    s = v1
+    return p*frac_x*frac_x*frac_x + q*frac_x*frac_x + r*frac_x + s
+
+def perlin_noise_1d(x: float, /, persistence: float = 0.5, octaves: int = 1, frequency: int = 2, seed: int = _time.time()) -> float:
+    """
+    Generate 1D Perlin noise for the given input parameters.
+    ref: https://web.archive.org/web/20160530124230/http://freespace.virgin.net/hugo.elias/models/m_perlin.htm
+
+    ---
+
+    ## params
+        `x`: input value.
+        `persistence`: persistence value determining the amplitude decrease per octave.
+        `octaves`: number of octaves or levels of detail in the Perlin noise.
+        `frequency`: lower frequency results in higher detail.
+        `seed`: seed value for randomness.
+
+    ## returns
+        float: Perlin noise value
+    """
+    total = 0
+    for i in range(octaves):
+        f = frequency**i
+        amplitude = persistence**i
+        total += amplitude*_pn1d_noise_interpolated(x*f, seed)
+    return total
```

### Comparing `mykit-2.0.0rc3/mykit/kit/path.py` & `mykit-2.0.1/mykit/kit/path.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import json as _json
-import os as _os
-import subprocess as _sp
-import sys as _sys
-import typing as _typing
-
-
-class SafeJSON:
-    """Secure JSON read/write operations, ensuring data integrity during writing and rewriting."""
-
-    @staticmethod
-    def write(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
-
-        ## normalize the path and perform some validations
-        pth_norm = _os.path.normpath(__pth)
-        if not pth_norm.lower().endswith('.json'):
-            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
-        if not _os.path.isdir(_os.path.dirname(pth_norm)):
-            raise NotADirectoryError(f'The directory does not exist: {repr(__pth)}.')
-        if _os.path.exists(pth_norm):
-            raise FileExistsError(f'File already exists: {repr(__pth)}.')
-
-        with open(pth_norm, 'w') as fp:
-            _json.dump(__obj, fp)
-        
-        if do_log:
-            print(f'INFO: Json written: {repr(__pth)}.')
-
-    @staticmethod
-    def read(__pth: str, /) -> _typing.Any:
-
-        ## normalize the path and perform some validations
-        pth_norm = _os.path.normpath(__pth)
-        if not pth_norm.lower().endswith('.json'):
-            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
-        if not _os.path.isfile(pth_norm):
-            raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
-
-        with open(pth_norm, 'r') as fp:
-            out = _json.load(fp)
-        return out
-
-    @staticmethod
-    def rewrite(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
-
-        ## normalize the path and perform some validations
-        pth_norm = _os.path.normpath(__pth)
-        if not pth_norm.lower().endswith('.json'):
-            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
-        if not _os.path.isfile(pth_norm):
-            raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
-
-        tmp_file = pth_norm + '.tmp'
-        bak_file = pth_norm + '.bak'
-        if _os.path.exists(tmp_file):
-            raise FileExistsError(f'Temporary file exists: {repr(tmp_file)}.')
-        if _os.path.exists(bak_file):
-            raise FileExistsError(f'Backup file exists: {repr(bak_file)}.')
-
-        ## writing the new as temp
-        with open(tmp_file, 'w') as fp:
-            _json.dump(__obj, fp)
-
-        _os.rename(pth_norm, bak_file)  # backup the previous
-        _os.rename(tmp_file, pth_norm)  # rename temp to new
-        _os.remove(bak_file)  # delete the previous
-
-        if do_log:
-            print(f'INFO: Json rewritten: {repr(__pth)}.')
-    
-    @staticmethod
-    def recover(__pth: str, /) -> None:
-
-        ## normalize and ensure that it's a JSON file
-        pth_norm = _os.path.normpath(__pth)
-        if not pth_norm.endswith('.json'):
-            raise ValueError(f'Not a JSON file: {repr(__pth)}.')
-
-        tmp_file = pth_norm + '.tmp'
-        bak_file = pth_norm + '.bak'
-
-        ## case I
-        if _os.path.exists(pth_norm) and _os.path.exists(tmp_file) and (not _os.path.exists(bak_file)):
-            _os.remove(tmp_file)
-            return
-
-        ## case II
-        if (not _os.path.exists(pth_norm)) and _os.path.exists(tmp_file) and _os.path.exists(bak_file):
-            _os.rename(tmp_file, pth_norm)
-            _os.remove(bak_file)
-            return
-
-        ## case III
-        if _os.path.exists(pth_norm) and (not _os.path.exists(tmp_file)) and _os.path.exists(bak_file):
-            _os.remove(bak_file)
-            return
-
-
-def open_file(file_pth: str, /) -> None:
-    """
-    Opens a file using the default system application.
-
-    ---
-
-    ## Exceptions
-    - `NotImplementedError`: if the OS is unrecognizable
-    """
-
-    system = _sys.platform
-
-    ## Windows
-    if system == 'win32':
-        _os.startfile(file_pth)
-
-    ## macOS
-    elif system == 'darwin':
-        _sp.call(['open', file_pth])
-
-    ## Linux
-    elif system.startswith('linux'):
-        _sp.call(['xdg-open', file_pth])
-
-    ## Windows/Cygwin
-    elif system.startswith('cygwin'):
-        _sp.call(['cygstart', file_pth])
-
-    else:
+import json as _json
+import os as _os
+import subprocess as _sp
+import sys as _sys
+import typing as _typing
+
+
+class SafeJSON:
+    """Secure JSON read/write operations, ensuring data integrity during writing and rewriting."""
+
+    @staticmethod
+    def write(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
+
+        ## normalize the path and perform some validations
+        pth_norm = _os.path.normpath(__pth)
+        if not pth_norm.lower().endswith('.json'):
+            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
+        if not _os.path.isdir(_os.path.dirname(pth_norm)):
+            raise NotADirectoryError(f'The directory does not exist: {repr(__pth)}.')
+        if _os.path.exists(pth_norm):
+            raise FileExistsError(f'File already exists: {repr(__pth)}.')
+
+        with open(pth_norm, 'w') as fp:
+            _json.dump(__obj, fp)
+        
+        if do_log:
+            print(f'INFO: Json written: {repr(__pth)}.')
+
+    @staticmethod
+    def read(__pth: str, /) -> _typing.Any:
+
+        ## normalize the path and perform some validations
+        pth_norm = _os.path.normpath(__pth)
+        if not pth_norm.lower().endswith('.json'):
+            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
+        if not _os.path.isfile(pth_norm):
+            raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
+
+        with open(pth_norm, 'r') as fp:
+            out = _json.load(fp)
+        return out
+
+    @staticmethod
+    def rewrite(__pth: str, __obj: _typing.Any, /, do_log: bool = True) -> None:
+
+        ## normalize the path and perform some validations
+        pth_norm = _os.path.normpath(__pth)
+        if not pth_norm.lower().endswith('.json'):
+            raise AssertionError(f'Not a JSON file: {repr(__pth)}.')
+        if not _os.path.isfile(pth_norm):
+            raise FileNotFoundError(f'Not a file: {repr(__pth)}.')
+
+        tmp_file = pth_norm + '.tmp'
+        bak_file = pth_norm + '.bak'
+        if _os.path.exists(tmp_file):
+            raise FileExistsError(f'Temporary file exists: {repr(tmp_file)}.')
+        if _os.path.exists(bak_file):
+            raise FileExistsError(f'Backup file exists: {repr(bak_file)}.')
+
+        ## writing the new as temp
+        with open(tmp_file, 'w') as fp:
+            _json.dump(__obj, fp)
+
+        _os.rename(pth_norm, bak_file)  # backup the previous
+        _os.rename(tmp_file, pth_norm)  # rename temp to new
+        _os.remove(bak_file)  # delete the previous
+
+        if do_log:
+            print(f'INFO: Json rewritten: {repr(__pth)}.')
+    
+    @staticmethod
+    def recover(__pth: str, /) -> None:
+
+        ## normalize and ensure that it's a JSON file
+        pth_norm = _os.path.normpath(__pth)
+        if not pth_norm.endswith('.json'):
+            raise ValueError(f'Not a JSON file: {repr(__pth)}.')
+
+        tmp_file = pth_norm + '.tmp'
+        bak_file = pth_norm + '.bak'
+
+        ## case I
+        if _os.path.exists(pth_norm) and _os.path.exists(tmp_file) and (not _os.path.exists(bak_file)):
+            _os.remove(tmp_file)
+            return
+
+        ## case II
+        if (not _os.path.exists(pth_norm)) and _os.path.exists(tmp_file) and _os.path.exists(bak_file):
+            _os.rename(tmp_file, pth_norm)
+            _os.remove(bak_file)
+            return
+
+        ## case III
+        if _os.path.exists(pth_norm) and (not _os.path.exists(tmp_file)) and _os.path.exists(bak_file):
+            _os.remove(bak_file)
+            return
+
+
+def open_file(file_pth: str, /) -> None:
+    """
+    Opens a file using the default system application.
+
+    ---
+
+    ## Exceptions
+    - `NotImplementedError`: if the OS is unrecognizable
+    """
+
+    system = _sys.platform
+
+    ## Windows
+    if system == 'win32':
+        _os.startfile(file_pth)
+
+    ## macOS
+    elif system == 'darwin':
+        _sp.call(['open', file_pth])
+
+    ## Linux
+    elif system.startswith('linux'):
+        _sp.call(['xdg-open', file_pth])
+
+    ## Windows/Cygwin
+    elif system.startswith('cygwin'):
+        _sp.call(['cygstart', file_pth])
+
+    else:
         raise NotImplementedError(f'Unsupported platform: {system}')
```

### Comparing `mykit-2.0.0rc3/mykit/kit/time.py` & `mykit-2.0.1/mykit/kit/time.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import re as _re
-
-
-def get_sexagecimal(secs: float, /, include_ms: bool = False) -> str:
-    """
-    Converts seconds to sexagesimal format.
-
-    ## Demo
-    >>> get_sexagecimal(3661.345)
-    '01:01:01'
-
-    """
-    sign = '-' if secs < 0 else ''
-    secs_abs = abs(secs)
-    hours, remainder = divmod(secs_abs, 3600)
-    minutes, seconds = divmod(remainder, 60)
-
-    h = str(int(hours)).zfill(2)
-    m = str(int(minutes)).zfill(2)
-
-    if include_ms:
-        s = f'{seconds:.3f}'.zfill(6)
-    else:
-        s = str(round(seconds)).zfill(2)
-
-    return sign + ':'.join([h, m, s])
-
-
-def sexagecimal_to_secs(sexagecimal: str, /) -> float:
-    """
-    ## Exceptions
-    - `ValueError` if `sexagecimal` is invalid
-
-    ## Demo
-    - `sexagecimal_to_secs('1.25')` -> `1.25`
-    - `sexagecimal_to_secs('01:01.25')` -> `61.25`
-    - `sexagecimal_to_secs('1:1:5.25')` -> `3665.25`
-    """
-    _s = sexagecimal.strip(' ')
-
-    res = _re.match(r'^(?P<sign>\+|-)?(?:(?:(?P<h>\d+):)?(?:(?P<m>[0-5]?\d):))?(?P<s>[0-5]?\d(?:\.\d*)?)$', _s)
-    if res is None:
-        raise ValueError(f'Invalid sexagecimal: {repr(sexagecimal)}')
-
-    sign = res.group('sign')
-    if sign in (None, '+'):
-        sign = 1
-    else:
-        sign = -1
-
-    h = res.group('h')
-    if h is None:
-        h = 0
-
-    m = res.group('m')
-    if m is None:
-        m = 0
-
-    s = res.group('s')
-
-    return sign * (int(h)*3600 + int(m)*60 + float(s))
-
-
-def get_dur(__secs: float, /) -> str:
-    """
-    Converts a duration in seconds to a string in hours, minutes, and seconds format.
-
-    ## Demo
-    >>> get_dur(3600)
-    '1 hr'
-    >>> get_dur(5400)
-    '1 hr 30 mins'
-    >>> get_dur(7261)
-    '2 hrs 1 min 1 sec'
-    """
-    
-    hours, _r = divmod(__secs, 3600)
-    minutes, seconds = divmod(_r, 60)
-
-    hours = int(hours)
-    minutes = int(minutes)
-    seconds = round(seconds)
-
-    parts = []
-    
-    if hours > 0:
-        if hours == 1:
-            parts.append('1 hr')
-        else:
-            parts.append(f'{hours} hrs')
-    
-    if minutes > 0:
-        if minutes == 1:
-            parts.append('1 min')
-        else:
-            parts.append(f'{minutes} mins')
-
-    if seconds == 0:
-        if parts == []:
-            parts.append('0 sec')
-    elif seconds == 1:
-        parts.append('1 sec')
-    else:
-        parts.append(f'{seconds} secs')
-
+import re as _re
+
+
+def get_sexagecimal(secs: float, /, include_ms: bool = False) -> str:
+    """
+    Converts seconds to sexagesimal format.
+
+    ## Demo
+    >>> get_sexagecimal(3661.345)
+    '01:01:01'
+
+    """
+    sign = '-' if secs < 0 else ''
+    secs_abs = abs(secs)
+    hours, remainder = divmod(secs_abs, 3600)
+    minutes, seconds = divmod(remainder, 60)
+
+    h = str(int(hours)).zfill(2)
+    m = str(int(minutes)).zfill(2)
+
+    if include_ms:
+        s = f'{seconds:.3f}'.zfill(6)
+    else:
+        s = str(round(seconds)).zfill(2)
+
+    return sign + ':'.join([h, m, s])
+
+
+def sexagecimal_to_secs(sexagecimal: str, /) -> float:
+    """
+    ## Exceptions
+    - `ValueError` if `sexagecimal` is invalid
+
+    ## Demo
+    - `sexagecimal_to_secs('1.25')` -> `1.25`
+    - `sexagecimal_to_secs('01:01.25')` -> `61.25`
+    - `sexagecimal_to_secs('1:1:5.25')` -> `3665.25`
+    """
+    _s = sexagecimal.strip(' ')
+
+    res = _re.match(r'^(?P<sign>\+|-)?(?:(?:(?P<h>\d+):)?(?:(?P<m>[0-5]?\d):))?(?P<s>[0-5]?\d(?:\.\d*)?)$', _s)
+    if res is None:
+        raise ValueError(f'Invalid sexagecimal: {repr(sexagecimal)}')
+
+    sign = res.group('sign')
+    if sign in (None, '+'):
+        sign = 1
+    else:
+        sign = -1
+
+    h = res.group('h')
+    if h is None:
+        h = 0
+
+    m = res.group('m')
+    if m is None:
+        m = 0
+
+    s = res.group('s')
+
+    return sign * (int(h)*3600 + int(m)*60 + float(s))
+
+
+def get_dur(__secs: float, /) -> str:
+    """
+    Converts a duration in seconds to a string in hours, minutes, and seconds format.
+
+    ## Demo
+    >>> get_dur(3600)
+    '1 hr'
+    >>> get_dur(5400)
+    '1 hr 30 mins'
+    >>> get_dur(7261)
+    '2 hrs 1 min 1 sec'
+    """
+    
+    hours, _r = divmod(__secs, 3600)
+    minutes, seconds = divmod(_r, 60)
+
+    hours = int(hours)
+    minutes = int(minutes)
+    seconds = round(seconds)
+
+    parts = []
+    
+    if hours > 0:
+        if hours == 1:
+            parts.append('1 hr')
+        else:
+            parts.append(f'{hours} hrs')
+    
+    if minutes > 0:
+        if minutes == 1:
+            parts.append('1 min')
+        else:
+            parts.append(f'{minutes} mins')
+
+    if seconds == 0:
+        if parts == []:
+            parts.append('0 sec')
+    elif seconds == 1:
+        parts.append('1 sec')
+    else:
+        parts.append(f'{seconds} secs')
+
     return ' '.join(parts)
```

### Comparing `mykit-2.0.0rc3/mykit/kit/utils.py` & `mykit-2.0.1/mykit/kit/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import datetime as _datetime
-import keyword as _keyword
-import random as _random
-
-
-def randfloat(__low: float, __high: float, __prec: int = 2, /) -> float:
-    """
-    This function follows `random.uniform` behaviors.
-    `__prec`: float precision (>= 0); if `__low` at 2 decimal point (`0.25`), `__prec` should at least `2`.
-    `__prec` normally max at 15-18 (depends on system).
-    """
-
-    ## can't use below because each end only half probability-dense
-    # return round(_random.uniform(__low, __high), __prec)
-
-    k = pow(10, __prec)
-    return _random.randint(round(__low*k), round(__high*k)) / k
-
-
-def randrange(low: float, high: float, len: float, /, pad: float = 0.1, prec: int = 3) -> tuple[float, float]:
-    """
-    if `low = 0, high = 1` -> include both `0` and `1`.
-    if `low = 0, high = 1, pad = 0.1` -> include both `0.1` and `0.9`.
-
-    `pad`: should `0 <= pad < 0.5`
-    """
-
-    range_len = high - low
-    the_pad = range_len * pad
-
-    start = randfloat(low + the_pad, high - the_pad - len, prec)
-    end = start + len
-
-    return (start, end)
-
-
-def minmax_normalization(x: float, min: float, max: float, /) -> float:
-    """min-max feature scaling"""
-    return (x - min) / (max - min)
-
-
-def slice_list(__in: list, __n: int, /) -> list:
-    """if `__n = 2` -> `[1, 2, 3, 4, 5]` -> `[[1, 2], [3, 4], [5]]`"""
-    out = [
-        __in[i : i + __n]
-        for i in range(0, len(__in), __n)
-    ]
-    return out
-
-
-def map_range(__value, /, from_min, from_max, to_min, to_max) -> float:
-    """
-    Maps a value from one range to another.
-
-    ---
-
-    ## Params
-        - `__value`: The value to be mapped
-        - `from_min`: The minimum value of the original range
-        - `from_max`: The maximum value of the original range
-        - `to_min`: The minimum value of the target range
-        - `to_max`: The maximum value of the target range
-
-    ## Returns
-        - The mapped value in the target range.
-
-    ## Demo
-        >>> original_value = 5
-        >>> mapped_value = map_range(original_value, 1, 9, 0, 1)
-        >>> print(mapped_value)
-        0.5
-    """
-    
-    ## normalize the value from the original range
-    normalized_value = (__value - from_min) / (from_max - from_min)
-
-    ## scale the normalized value to the target range
-    mapped_value = normalized_value * (to_max - to_min) + to_min
-
-    return mapped_value
-
-
-def is_valid_var_name(__in: str, /) -> bool:
-    """
-    Check if a string `__in` is valid for variable name.
-
-    ---
-
-    ## Demo
-    - `is_valid_var_name('2x')` -> `False`
-    - `is_valid_var_name('x2')` -> `True`
-    - `is_valid_var_name('cold-ice')` -> `False`
-    - `is_valid_var_name('cold_ice')` -> `True`
-    """
-    return (__in.isidentifier() and (not _keyword.iskeyword(__in)))
-
-
-def printer(__msg: str, /) -> None:
-    """
-    For simple logging needs.
-    
-    ---
-
-    ## Demo
-    >>> printer('INFO: foo')  # [06:15:09] INFO: foo
-    >>> printer('WARNING: bar')  # [06:15:09] WARNING: bar
-    """
+import datetime as _datetime
+import keyword as _keyword
+import random as _random
+
+
+def randfloat(__low: float, __high: float, __prec: int = 2, /) -> float:
+    """
+    This function follows `random.uniform` behaviors.
+    `__prec`: float precision (>= 0); if `__low` at 2 decimal point (`0.25`), `__prec` should at least `2`.
+    `__prec` normally max at 15-18 (depends on system).
+    """
+
+    ## can't use below because each end only half probability-dense
+    # return round(_random.uniform(__low, __high), __prec)
+
+    k = pow(10, __prec)
+    return _random.randint(round(__low*k), round(__high*k)) / k
+
+
+def randrange(low: float, high: float, len: float, /, pad: float = 0.1, prec: int = 3) -> tuple[float, float]:
+    """
+    if `low = 0, high = 1` -> include both `0` and `1`.
+    if `low = 0, high = 1, pad = 0.1` -> include both `0.1` and `0.9`.
+
+    `pad`: should `0 <= pad < 0.5`
+    """
+
+    range_len = high - low
+    the_pad = range_len * pad
+
+    start = randfloat(low + the_pad, high - the_pad - len, prec)
+    end = start + len
+
+    return (start, end)
+
+
+def minmax_normalization(x: float, min: float, max: float, /) -> float:
+    """min-max feature scaling"""
+    return (x - min) / (max - min)
+
+
+def slice_list(__in: list, __n: int, /) -> list:
+    """if `__n = 2` -> `[1, 2, 3, 4, 5]` -> `[[1, 2], [3, 4], [5]]`"""
+    out = [
+        __in[i : i + __n]
+        for i in range(0, len(__in), __n)
+    ]
+    return out
+
+
+def map_range(__value, /, from_min, from_max, to_min, to_max) -> float:
+    """
+    Maps a value from one range to another.
+
+    ---
+
+    ## Params
+        - `__value`: The value to be mapped
+        - `from_min`: The minimum value of the original range
+        - `from_max`: The maximum value of the original range
+        - `to_min`: The minimum value of the target range
+        - `to_max`: The maximum value of the target range
+
+    ## Returns
+        - The mapped value in the target range.
+
+    ## Demo
+        >>> original_value = 5
+        >>> mapped_value = map_range(original_value, 1, 9, 0, 1)
+        >>> print(mapped_value)
+        0.5
+    """
+    
+    ## normalize the value from the original range
+    normalized_value = (__value - from_min) / (from_max - from_min)
+
+    ## scale the normalized value to the target range
+    mapped_value = normalized_value * (to_max - to_min) + to_min
+
+    return mapped_value
+
+
+def is_valid_var_name(__in: str, /) -> bool:
+    """
+    Check if a string `__in` is valid for variable name.
+
+    ---
+
+    ## Demo
+    - `is_valid_var_name('2x')` -> `False`
+    - `is_valid_var_name('x2')` -> `True`
+    - `is_valid_var_name('cold-ice')` -> `False`
+    - `is_valid_var_name('cold_ice')` -> `True`
+    """
+    return (__in.isidentifier() and (not _keyword.iskeyword(__in)))
+
+
+def printer(__msg: str, /) -> None:
+    """
+    For simple logging needs.
+    
+    ---
+
+    ## Demo
+    >>> printer('INFO: foo')  # [06:15:09] INFO: foo
+    >>> printer('WARNING: bar')  # [06:15:09] WARNING: bar
+    """
     print(f'[{_datetime.datetime.now().strftime("%H:%M:%S")}] {__msg}')
```

### Comparing `mykit-2.0.0rc3/mykit.egg-info/SOURCES.txt` & `mykit-2.0.1/mykit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,12 +26,8 @@
 mykit/kit/path.py
 mykit/kit/text.py
 mykit/kit/time.py
 mykit/kit/utils.py
 mykit/kit/fast_visualizations/static/plot.py
 mykit/kit/keycrate/__init__.py
 mykit/kit/neuralnet/dense.py
-mykit/kit/neuralnet/genetic.py
-tests/__init__.py
-tests/test_kit/__init__.py
-tests/test_kit/test_color.py
-tests/test_kit/test_math.py
+mykit/kit/neuralnet/genetic.py
```

### Comparing `mykit-2.0.0rc3/pyproject.toml` & `mykit-2.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-
-[project]
-name = "mykit"
-version = "2.0.0-rc-3"
-description = "Python utility library"
-readme = "README.md"
-requires-python = ">=3.7"
-license = {text = "MIT"}
-authors = [
-  	{email = "nvfastplease@gmail.com"},
-]
-keywords = ["python", "toolkit", "mykit"]
-classifiers = [
-	"Topic :: Scientific/Engineering",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Natural Language :: English"
-]
-dependencies = [
-	"numba>=0.55.2",
-	"numpy>=1.22.4"
-]
-
-
-[tool.setuptools.packages.find]
-exclude = [
-    "assets*",
-    "tests*"
-]
-
-
-[project.urls]
-documentation = "https://nvfp.github.io/mykit/docs"
-"report bugs" = "https://github.com/nvfp/mykit/issues"
-repo = "https://github.com/nvfp/mykit"
-changelog = "https://nvfp.github.io/mykit/changelog"
-
-
-[project.scripts]
-mykit = "mykit.__main__:main"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "mykit"
+version = "2.0.1"
+description = "Python utility library"
+readme = "README.md"
+requires-python = ">=3.8"
+license = {text = "MIT"}
+authors = [
+  	{email = "nvfastplease@gmail.com"},
+]
+keywords = ["python", "toolkit", "mykit"]
+classifiers = [
+	"Topic :: Scientific/Engineering",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3 :: Only",
+    "Natural Language :: English"
+]
+dependencies = [
+	"numba>=0.55.2",
+	"numpy>=1.22.4"
+]
+
+
+[tool.setuptools.packages.find]
+exclude = [
+    "assets*",
+    "tests*",
+    "demo*",
+]
+
+
+[project.urls]
+documentation = "https://nvfp.github.io/mykit/docs"
+"report bugs" = "https://github.com/nvfp/mykit/issues"
+repo = "https://github.com/nvfp/mykit"
+changelog = "https://nvfp.github.io/mykit/changelog"
+
+
+[project.scripts]
+mykit = "mykit.__main__:main"
```

