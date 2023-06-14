# Comparing `tmp/mykit-2.0.0rc2.tar.gz` & `tmp/mykit-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-2.0.0rc2.tar", last modified: Tue Jun 13 16:07:55 2023, max compression
+gzip compressed data, was "mykit-2.0.0rc3.tar", last modified: Tue Jun 13 16:19:00 2023, max compression
```

## Comparing `mykit-2.0.0rc2.tar` & `mykit-2.0.0rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.376056 mykit-2.0.0rc2/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-2.0.0rc2/LICENSE
--rw-rw-rw-   0        0        0     3751 2023-06-13 16:07:55.391682 mykit-2.0.0rc2/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-06-13 16:04:50.000000 mykit-2.0.0rc2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.085529 mykit-2.0.0rc2/mykit/
--rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-2.0.0rc2/mykit/__init__.py
--rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-2.0.0rc2/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.282299 mykit-2.0.0rc2/mykit/app/
--rw-rw-rw-   0        0        0     3762 2023-06-13 15:59:31.000000 mykit-2.0.0rc2/mykit/app/__init__.py
--rw-rw-rw-   0        0        0      128 2023-06-13 12:39:40.000000 mykit-2.0.0rc2/mykit/app/_runtime.py
--rw-rw-rw-   0        0        0     4157 2023-06-13 13:01:03.000000 mykit-2.0.0rc2/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12724 2023-06-13 12:41:28.000000 mykit-2.0.0rc2/mykit/app/button.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.297927 mykit-2.0.0rc2/mykit/app/complex/
--rw-rw-rw-   0        0        0    20467 2023-06-13 14:43:30.000000 mykit-2.0.0rc2/mykit/app/complex/biplot.py
--rw-rw-rw-   0        0        0    16360 2023-06-13 13:49:53.000000 mykit-2.0.0rc2/mykit/app/complex/plot.py
--rw-rw-rw-   0        0        0     9010 2023-06-13 13:12:29.000000 mykit-2.0.0rc2/mykit/app/label.py
--rw-rw-rw-   0        0        0    27866 2023-06-13 13:13:12.000000 mykit-2.0.0rc2/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.329197 mykit-2.0.0rc2/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-2.0.0rc2/mykit/kit/color.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:54.978651 mykit-2.0.0rc2/mykit/kit/fast_visualizations/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.344803 mykit-2.0.0rc2/mykit/kit/fast_visualizations/static/
--rw-rw-rw-   0        0        0      500 2023-06-13 14:50:18.000000 mykit-2.0.0rc2/mykit/kit/fast_visualizations/static/plot.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-2.0.0rc2/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.344803 mykit-2.0.0rc2/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-2.0.0rc2/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-2.0.0rc2/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.360434 mykit-2.0.0rc2/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-2.0.0rc2/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-2.0.0rc2/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-2.0.0rc2/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-2.0.0rc2/mykit/kit/path.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-2.0.0rc2/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-2.0.0rc2/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-2.0.0rc2/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.251051 mykit-2.0.0rc2/mykit.egg-info/
--rw-rw-rw-   0        0        0     3751 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1276 2023-06-13 15:43:48.000000 mykit-2.0.0rc2/pyproject.toml
--rw-rw-rw-   0        0        0      161 2023-06-13 16:07:55.391682 mykit-2.0.0rc2/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-2.0.0rc2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.360434 mykit-2.0.0rc2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.376056 mykit-2.0.0rc2/tests/test_kit/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc2/tests/test_kit/__init__.py
--rw-rw-rw-   0        0        0     4212 2023-06-12 14:37:42.000000 mykit-2.0.0rc2/tests/test_kit/test_color.py
--rw-rw-rw-   0        0        0     3546 2023-06-12 12:14:14.000000 mykit-2.0.0rc2/tests/test_kit/test_math.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-2.0.0rc3/LICENSE
+-rw-rw-rw-   0        0        0     3751 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     2637 2023-06-13 16:04:50.000000 mykit-2.0.0rc3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.098278 mykit-2.0.0rc3/mykit/
+-rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-2.0.0rc3/mykit/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-2.0.0rc3/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.306871 mykit-2.0.0rc3/mykit/app/
+-rw-rw-rw-   0        0        0     3766 2023-06-13 16:17:41.000000 mykit-2.0.0rc3/mykit/app/__init__.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 16:17:16.000000 mykit-2.0.0rc3/mykit/app/_runtime.py
+-rw-rw-rw-   0        0        0     4157 2023-06-13 13:01:03.000000 mykit-2.0.0rc3/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12724 2023-06-13 12:41:28.000000 mykit-2.0.0rc3/mykit/app/button.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.356070 mykit-2.0.0rc3/mykit/app/complex/
+-rw-rw-rw-   0        0        0    20467 2023-06-13 14:43:30.000000 mykit-2.0.0rc3/mykit/app/complex/biplot.py
+-rw-rw-rw-   0        0        0    16360 2023-06-13 13:49:53.000000 mykit-2.0.0rc3/mykit/app/complex/plot.py
+-rw-rw-rw-   0        0        0     9010 2023-06-13 13:12:29.000000 mykit-2.0.0rc3/mykit/app/label.py
+-rw-rw-rw-   0        0        0    27866 2023-06-13 13:13:12.000000 mykit-2.0.0rc3/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.418579 mykit-2.0.0rc3/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-2.0.0rc3/mykit/kit/color.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:18:59.990031 mykit-2.0.0rc3/mykit/kit/fast_visualizations/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.418579 mykit-2.0.0rc3/mykit/kit/fast_visualizations/static/
+-rw-rw-rw-   0        0        0      500 2023-06-13 14:50:18.000000 mykit-2.0.0rc3/mykit/kit/fast_visualizations/static/plot.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-2.0.0rc3/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.434202 mykit-2.0.0rc3/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-2.0.0rc3/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-2.0.0rc3/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.434202 mykit-2.0.0rc3/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-2.0.0rc3/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-2.0.0rc3/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-2.0.0rc3/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-2.0.0rc3/mykit/kit/path.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-2.0.0rc3/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-2.0.0rc3/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-2.0.0rc3/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.250856 mykit-2.0.0rc3/mykit.egg-info/
+-rw-rw-rw-   0        0        0     3751 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 16:18:59.000000 mykit-2.0.0rc3/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1276 2023-06-13 16:17:49.000000 mykit-2.0.0rc3/pyproject.toml
+-rw-rw-rw-   0        0        0      161 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-2.0.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.449829 mykit-2.0.0rc3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:19:00.465454 mykit-2.0.0rc3/tests/test_kit/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc3/tests/test_kit/__init__.py
+-rw-rw-rw-   0        0        0     4212 2023-06-12 14:37:42.000000 mykit-2.0.0rc3/tests/test_kit/test_color.py
+-rw-rw-rw-   0        0        0     3546 2023-06-12 12:14:14.000000 mykit-2.0.0rc3/tests/test_kit/test_math.py
```

### Comparing `mykit-2.0.0rc2/LICENSE` & `mykit-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/PKG-INFO` & `mykit-2.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-2.0.0rc2/README.md` & `mykit-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/__init__.py` & `mykit-2.0.0rc3/mykit/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             master=self.root,
             width=self.root.winfo_screenwidth(),
             height=self.root.winfo_screenheight(),
             background=bg,
             borderwidth=0, highlightthickness=0
         )
         page.place(x=0, y=0)
-        App.page = page
+        App._set_page(page)
 
 
         ## <constants>
         self.MON_WIDTH = self.root.winfo_screenwidth()
         self.MON_HEIGHT = self.root.winfo_screenheight()
         ## </constants>
```

### Comparing `mykit-2.0.0rc2/mykit/app/arrow.py` & `mykit-2.0.0rc3/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/button.py` & `mykit-2.0.0rc3/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/complex/biplot.py` & `mykit-2.0.0rc3/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/complex/plot.py` & `mykit-2.0.0rc3/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/label.py` & `mykit-2.0.0rc3/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/app/slider.py` & `mykit-2.0.0rc3/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/color.py` & `mykit-2.0.0rc3/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/ffmpeg.py` & `mykit-2.0.0rc3/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/keycrate/__init__.py` & `mykit-2.0.0rc3/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/math.py` & `mykit-2.0.0rc3/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/neuralnet/dense.py` & `mykit-2.0.0rc3/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.0rc3/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/noise.py` & `mykit-2.0.0rc3/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/path.py` & `mykit-2.0.0rc3/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/time.py` & `mykit-2.0.0rc3/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit/kit/utils.py` & `mykit-2.0.0rc3/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/mykit.egg-info/PKG-INFO` & `mykit-2.0.0rc3/mykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-2.0.0rc2/mykit.egg-info/SOURCES.txt` & `mykit-2.0.0rc3/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/pyproject.toml` & `mykit-2.0.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.0-rc-2"
+version = "2.0.0-rc-3"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

### Comparing `mykit-2.0.0rc2/tests/test_kit/test_color.py` & `mykit-2.0.0rc3/tests/test_kit/test_color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc2/tests/test_kit/test_math.py` & `mykit-2.0.0rc3/tests/test_kit/test_math.py`

 * *Files identical despite different names*

