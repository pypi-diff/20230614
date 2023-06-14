# Comparing `tmp/mscales-1.2.1.tar.gz` & `tmp/mscales-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mscales-1.2.1.tar", last modified: Tue May 24 13:14:26 2022, max compression
+gzip compressed data, was "mscales-1.3.1.tar", last modified: Wed Jun 14 15:22:08 2023, max compression
```

## Comparing `mscales-1.2.1.tar` & `mscales-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2022-03-29 15:41:07.000000 mscales-1.2.1/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2022-03-29 15:41:07.000000 mscales-1.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2022-03-29 15:41:07.000000 mscales-1.2.1/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2022-03-29 15:41:07.000000 mscales-1.2.1/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1264 2022-05-24 13:14:26.000000 mscales-1.2.1/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      790 2022-05-23 14:33:08.000000 mscales-1.2.1/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2022-03-29 15:41:07.000000 mscales-1.2.1/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2022-03-29 15:41:07.000000 mscales-1.2.1/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2022-05-24 13:07:53.000000 mscales-1.2.1/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2022-05-24 13:07:53.000000 mscales-1.2.1/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2022-05-24 13:07:53.000000 mscales-1.2.1/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2022-05-24 13:07:53.000000 mscales-1.2.1/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      804 2022-05-24 13:12:48.000000 mscales-1.2.1/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2022-05-23 12:38:15.000000 mscales-1.2.1/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2022-05-24 13:07:53.000000 mscales-1.2.1/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2022-05-17 19:38:58.000000 mscales-1.2.1/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     6444 2022-05-23 15:41:08.000000 mscales-1.2.1/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2022-05-23 12:38:15.000000 mscales-1.2.1/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2022-05-23 14:33:08.000000 mscales-1.2.1/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2022-05-24 13:07:53.000000 mscales-1.2.1/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2022-04-10 10:31:08.000000 mscales-1.2.1/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2022-04-10 10:31:08.000000 mscales-1.2.1/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2022-05-16 09:48:28.000000 mscales-1.2.1/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2022-05-17 19:38:58.000000 mscales-1.2.1/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1264 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      717 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       20 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/entry_points.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       18 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2022-05-24 13:14:26.000000 mscales-1.2.1/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2022-03-29 15:41:07.000000 mscales-1.2.1/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       70 2022-05-24 13:07:53.000000 mscales-1.2.1/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2022-05-24 13:14:26.000000 mscales-1.2.1/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2022-05-23 12:53:33.000000 mscales-1.2.1/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2022-03-29 15:41:07.000000 mscales-1.2.1/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.1/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.1/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.1/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.1/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1244 2023-06-14 15:22:08.787914 mscales-1.3.1/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      790 2023-05-31 17:16:11.000000 mscales-1.3.1/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.783914 mscales-1.3.1/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/pcsets.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1012 2023-06-14 13:57:39.000000 mscales-1.3.1/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     6596 2023-05-31 17:25:07.000000 mscales-1.3.1/mscales/pcsets.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1244 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.1/pyproject.toml
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.1/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-06-14 15:22:08.787914 mscales-1.3.1/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-05-31 17:16:11.000000 mscales-1.3.1/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mscales-1.2.1/CONTRIBUTING.rst` & `mscales-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/LICENSE` & `mscales-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/PKG-INFO` & `mscales-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.2.1
+Version: 1.3.1
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -31,9 +30,7 @@
         :alt: Documentation Status
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
-
-
```

### Comparing `mscales-1.2.1/README.rst` & `mscales-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/Makefile` & `mscales-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/make.bat` & `mscales-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/source/conf.py` & `mscales-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/source/pcsets.rst` & `mscales-1.3.1/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/source/quickstart.rst` & `mscales-1.3.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/docs/source/release-history.rst` & `mscales-1.3.1/docs/source/release-history.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Release History
 ===============
 
+v1.3.1 (2023-06-14)
+-------------------
+
+- update flake8 settings
+
+v1.3.0 (2023-05-31)
+-------------------
+
+- type fixes require minor update
+
+v1.2.2 (2023-05-31)
+-------------------
+
+- fix some type errors
+
 v1.2.1 (2022-05-24)
 -------------------
 
 - replace tones with pretty-midi
 
 v1.1.1 (2022-05-23)
 -------------------
```

### Comparing `mscales-1.2.1/mscales/concepts.py` & `mscales-1.3.1/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/mscales/pcsets.py` & `mscales-1.3.1/mscales/pcsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,41 +17,43 @@
         return str(self.p)
 
     def __neg__(self):
         return -self.p % self.c
 
     def __add__(self, other):
         if isinstance(other, PitchClassInterval):
-            return (self.p + other.i) % self.c
+            return PitchClass((self.p + other.i) % self.c)
         else:
             raise TypeError(f"Can't add type {type(other)} to pitch class {self.p}.")
 
     def __sub__(self, other):
         if isinstance(other, PitchClassInterval):
-            return (self.p - other.i) % self.c
+            return PitchClass((self.p - other.i) % self.c)
         else:
             raise TypeError(f"Can't subtract type {type(other)} from pitch class {self.p}.")
 
 
 class PitchClassInterval:
     """Interval between two pitch classes (mod c)."""
 
-    def __init__(self, i, c: int = 12):
+    def __init__(self, i: int, c: int = 12):
         self.c = c
         self.i = i
 
     def __repr__(self):
         return f"Interval({self.i})"
 
     def __str__(self):
         return str(self.i)
 
     def __add__(self, other):
         if isinstance(other, PitchClassInterval):
-            return (self.i + other.i) % self.c
+            return PitchClassInterval((self.i + other.i) % self.c)
+        elif isinstance(other, PitchClass):
+            return PitchClass((self.i + other.p) % self.c)
         else:
             raise TypeError(f"Can't add type {type(other)} to interval {self.i}.")
 
     def __sub__(self, other):
         if isinstance(other, PitchClassInterval):
             return self.i - other.i % self.c
         else:
```

### Comparing `mscales-1.2.1/mscales/plots.py` & `mscales-1.3.1/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/mscales/scales.py` & `mscales-1.3.1/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/mscales/sound.py` & `mscales-1.3.1/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/mscales/utils.py` & `mscales-1.3.1/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/mscales.egg-info/PKG-INFO` & `mscales-1.3.1/mscales.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.2.1
+Version: 1.3.1
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -31,9 +30,7 @@
         :alt: Documentation Status
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
-
-
```

### Comparing `mscales-1.2.1/setup.py` & `mscales-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.2.1/versioneer.py` & `mscales-1.3.1/versioneer.py`

 * *Files identical despite different names*

