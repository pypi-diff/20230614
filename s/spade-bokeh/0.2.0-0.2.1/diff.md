# Comparing `tmp/spade_bokeh-0.2.0.tar.gz` & `tmp/spade_bokeh-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_bokeh-0.2.0.tar", last modified: Wed Jun 14 11:01:04 2023, max compression
+gzip compressed data, was "spade_bokeh-0.2.1.tar", last modified: Wed Jun 14 11:11:28 2023, max compression
```

## Comparing `spade_bokeh-0.2.0.tar` & `spade_bokeh-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.919117 spade_bokeh-0.2.0/
--rw-r--r--   0 jpalanca   (501) staff       (20)      156 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3580 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      382 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)      317 2018-09-17 17:57:58.000000 spade_bokeh-0.2.0/MANIFEST.in
--rw-r--r--   0 jpalanca   (501) staff       (20)     2036 2023-06-14 11:01:04.919373 spade_bokeh-0.2.0/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)      983 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/README.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.899223 spade_bokeh-0.2.0/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)      612 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/Makefile
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.883084 spade_bokeh-0.2.0/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.883250 spade_bokeh-0.2.0/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.910650 spade_bokeh-0.2.0/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)      673 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 jpalanca   (501) staff       (20)      756 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      829 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      641 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      222 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      202 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/down.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      214 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      203 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/up.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/authors.rst
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     4917 2018-09-17 16:24:45.000000 spade_bokeh-0.2.0/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/history.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      315 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      773 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/make.bat
--rw-r--r--   0 jpalanca   (501) staff       (20)       70 2018-09-17 16:25:22.000000 spade_bokeh-0.2.0/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      350 2018-09-17 16:25:22.000000 spade_bokeh-0.2.0/docs/spade_bokeh.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     5275 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/requirements.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      191 2023-06-14 10:55:51.000000 spade_bokeh-0.2.0/requirements_dev.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      454 2023-06-14 11:01:04.920696 spade_bokeh-0.2.0/setup.cfg
--rw-r--r--   0 jpalanca   (501) staff       (20)     1585 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/setup.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.912507 spade_bokeh-0.2.0/spade_bokeh/
--rw-r--r--   0 jpalanca   (501) staff       (20)      218 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/spade_bokeh/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     3055 2018-09-17 17:00:04.000000 spade_bokeh-0.2.0/spade_bokeh/spade_bokeh.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.917137 spade_bokeh-0.2.0/spade_bokeh.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     2036 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     1050 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       12 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/top_level.txt
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.918475 spade_bokeh-0.2.0/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/tests/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     1047 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/tests/test_spade_bokeh.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.560414 spade_bokeh-0.2.1/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      156 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3580 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      445 2023-06-14 11:10:18.000000 spade_bokeh-0.2.1/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      317 2018-09-17 17:57:58.000000 spade_bokeh-0.2.1/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2099 2023-06-14 11:11:28.560697 spade_bokeh-0.2.1/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)      983 2023-06-14 10:59:15.000000 spade_bokeh-0.2.1/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.541911 spade_bokeh-0.2.1/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      612 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.527020 spade_bokeh-0.2.1/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.527177 spade_bokeh-0.2.1/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.552467 spade_bokeh-0.2.1/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      673 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 jpalanca   (501) staff       (20)      756 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      829 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      641 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/comment.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      222 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      202 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/down.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      214 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      203 2018-09-17 16:23:34.000000 spade_bokeh-0.2.1/docs/_build/html/_static/up.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/authors.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     4917 2018-09-17 16:24:45.000000 spade_bokeh-0.2.1/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/contributing.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/history.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      315 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      773 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)       70 2018-09-17 16:25:22.000000 spade_bokeh-0.2.1/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2018-09-17 15:34:04.000000 spade_bokeh-0.2.1/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      350 2018-09-17 16:25:22.000000 spade_bokeh-0.2.1/docs/spade_bokeh.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5275 2023-06-14 10:59:15.000000 spade_bokeh-0.2.1/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:11:16.000000 spade_bokeh-0.2.1/requirements.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      191 2023-06-14 10:55:51.000000 spade_bokeh-0.2.1/requirements_dev.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      454 2023-06-14 11:11:28.562025 spade_bokeh-0.2.1/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1585 2023-06-14 11:10:18.000000 spade_bokeh-0.2.1/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.554165 spade_bokeh-0.2.1/spade_bokeh/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      218 2023-06-14 11:10:18.000000 spade_bokeh-0.2.1/spade_bokeh/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3055 2018-09-17 17:00:04.000000 spade_bokeh-0.2.1/spade_bokeh/spade_bokeh.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.558447 spade_bokeh-0.2.1/spade_bokeh.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2099 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1050 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       12 2023-06-14 11:11:28.000000 spade_bokeh-0.2.1/spade_bokeh.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:28.559688 spade_bokeh-0.2.1/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:11:16.000000 spade_bokeh-0.2.1/tests/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1047 2023-06-14 11:11:16.000000 spade_bokeh-0.2.1/tests/test_spade_bokeh.py
```

### Comparing `spade_bokeh-0.2.0/CONTRIBUTING.rst` & `spade_bokeh-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/LICENSE` & `spade_bokeh-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/PKG-INFO` & `spade_bokeh-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spade_bokeh
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bokeh server for SPADE agents that integrates with agents web service.
 Home-page: https://github.com/javipalanca/spade_bokeh
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
 Keywords: spade_bokeh
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,14 +54,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.2.1 (2023-06-14)
+------------------
+
+* Fixed documentation.
+
 0.2.0 (2023-06-14)
 ------------------
 
 * Upgraded to SPADE>=3.3 (older versions are deprecated).
 * Upgraded to Python>=3.8 (older versions are deprecated).
 
 0.1.2 (2018-09-17)
```

### Comparing `spade_bokeh-0.2.0/README.rst` & `spade_bokeh-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/Makefile` & `spade_bokeh-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/_build/html/_static/ajax-loader.gif` & `spade_bokeh-0.2.1/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/_build/html/_static/comment-bright.png` & `spade_bokeh-0.2.1/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/_build/html/_static/comment-close.png` & `spade_bokeh-0.2.1/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/_build/html/_static/comment.png` & `spade_bokeh-0.2.1/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/conf.py` & `spade_bokeh-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/installation.rst` & `spade_bokeh-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/make.bat` & `spade_bokeh-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/docs/usage.rst` & `spade_bokeh-0.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/setup.py` & `spade_bokeh-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='spade_bokeh',
     name='spade_bokeh',
     packages=find_packages(include=['spade_bokeh']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/javipalanca/spade_bokeh',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

### Comparing `spade_bokeh-0.2.0/spade_bokeh/spade_bokeh.py` & `spade_bokeh-0.2.1/spade_bokeh/spade_bokeh.py`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/spade_bokeh.egg-info/PKG-INFO` & `spade_bokeh-0.2.1/spade_bokeh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spade-bokeh
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bokeh server for SPADE agents that integrates with agents web service.
 Home-page: https://github.com/javipalanca/spade_bokeh
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
 Keywords: spade_bokeh
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,14 +54,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.2.1 (2023-06-14)
+------------------
+
+* Fixed documentation.
+
 0.2.0 (2023-06-14)
 ------------------
 
 * Upgraded to SPADE>=3.3 (older versions are deprecated).
 * Upgraded to Python>=3.8 (older versions are deprecated).
 
 0.1.2 (2018-09-17)
```

### Comparing `spade_bokeh-0.2.0/spade_bokeh.egg-info/SOURCES.txt` & `spade_bokeh-0.2.1/spade_bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.2.0/tests/test_spade_bokeh.py` & `spade_bokeh-0.2.1/tests/test_spade_bokeh.py`

 * *Files identical despite different names*

