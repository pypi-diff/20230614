# Comparing `tmp/emlib-1.9.1.tar.gz` & `tmp/emlib-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlib-1.9.1.tar", last modified: Sun Apr 23 18:18:23 2023, max compression
+gzip compressed data, was "emlib-1.9.2.tar", last modified: Wed May  3 09:18:01 2023, max compression
```

## Comparing `emlib-1.9.1.tar` & `emlib-1.9.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 18:18:23.711665 emlib-1.9.1/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-23 18:18:23.711665 emlib-1.9.1/PKG-INFO
--rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.9.1/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 18:18:23.707666 emlib-1.9.1/emlib/
--rwxrwxr-x   0 em        (1000) em        (1000)      554 2023-04-23 18:18:01.000000 emlib-1.9.1/emlib/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.9.1/emlib/_dialogsqt.py
--rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/calculus.py
--rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.9.1/emlib/combinatorics.py
--rw-rw-r--   0 em        (1000) em        (1000)      783 2023-04-23 09:50:49.000000 emlib-1.9.1/emlib/common.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.9.1/emlib/containers.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.9.1/emlib/csvtools.py
--rw-rw-r--   0 em        (1000) em        (1000)    14721 2023-04-23 18:17:15.000000 emlib-1.9.1/emlib/dialogs.py
--rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.9.1/emlib/doctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.9.1/emlib/electronics.py
--rw-rw-r--   0 em        (1000) em        (1000)     4473 2023-04-23 09:55:27.000000 emlib-1.9.1/emlib/envir.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.9.1/emlib/filetools.py
--rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/graphlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/img.py
--rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.9.1/emlib/iterlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/jsontools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.9.1/emlib/logutils.py
--rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.9.1/emlib/mathlib.py
--rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/matplotting.py
--rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/minizinctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    52820 2023-04-23 18:16:22.000000 emlib-1.9.1/emlib/misc.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/net.py
--rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/numberseries.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.9.1/emlib/numpytools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/numtheory.py
--rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.9.1/emlib/parabolicinterpol.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/readbytes.py
--rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.9.1/emlib/shelling.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.9.1/emlib/smooth.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.9.1/emlib/stochastic.py
--rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.9.1/emlib/textlib.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.9.1/emlib/video.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.9.1/emlib/xmlprinter.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-23 18:18:23.711665 emlib-1.9.1/emlib.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-23 18:18:23.000000 emlib-1.9.1/emlib.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      810 2023-04-23 18:18:23.000000 emlib-1.9.1/emlib.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-23 18:18:23.000000 emlib-1.9.1/emlib.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.9.1/emlib.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      117 2023-04-23 18:18:23.000000 emlib-1.9.1/emlib.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        6 2023-04-23 18:18:23.000000 emlib-1.9.1/emlib.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-04-23 18:18:23.712665 emlib-1.9.1/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)     1053 2023-04-23 18:18:12.000000 emlib-1.9.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 09:18:01.481775 emlib-1.9.2/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-05-03 09:18:01.481775 emlib-1.9.2/PKG-INFO
+-rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.9.2/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 09:18:01.478775 emlib-1.9.2/emlib/
+-rwxrwxr-x   0 em        (1000) em        (1000)      554 2023-04-23 18:18:01.000000 emlib-1.9.2/emlib/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.9.2/emlib/_dialogsqt.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/calculus.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.9.2/emlib/combinatorics.py
+-rw-rw-r--   0 em        (1000) em        (1000)      783 2023-04-23 09:50:49.000000 emlib-1.9.2/emlib/common.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.9.2/emlib/containers.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.9.2/emlib/csvtools.py
+-rw-rw-r--   0 em        (1000) em        (1000)    14721 2023-04-23 18:17:15.000000 emlib-1.9.2/emlib/dialogs.py
+-rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.9.2/emlib/doctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.9.2/emlib/electronics.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4473 2023-04-23 09:55:27.000000 emlib-1.9.2/emlib/envir.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.9.2/emlib/filetools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/graphlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/img.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.9.2/emlib/iterlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/jsontools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.9.2/emlib/logutils.py
+-rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.9.2/emlib/mathlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/matplotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/minizinctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    52820 2023-04-23 18:16:22.000000 emlib-1.9.2/emlib/misc.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/net.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/numberseries.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.9.2/emlib/numpytools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/numtheory.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.9.2/emlib/parabolicinterpol.py
+-rw-rw-r--   0 em        (1000) em        (1000)        6 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/py.typed
+-rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/readbytes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.9.2/emlib/shelling.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.9.2/emlib/smooth.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.9.2/emlib/stochastic.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.9.2/emlib/textlib.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.9.2/emlib/video.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.9.2/emlib/xmlprinter.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 09:18:01.480775 emlib-1.9.2/emlib.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-05-03 09:18:01.000000 emlib-1.9.2/emlib.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      825 2023-05-03 09:18:01.000000 emlib-1.9.2/emlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-03 09:18:01.000000 emlib-1.9.2/emlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.9.2/emlib.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      117 2023-05-03 09:18:01.000000 emlib-1.9.2/emlib.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        6 2023-05-03 09:18:01.000000 emlib-1.9.2/emlib.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-05-03 09:18:01.481775 emlib-1.9.2/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)     1095 2023-05-03 09:17:39.000000 emlib-1.9.2/setup.py
```

### Comparing `emlib-1.9.1/PKG-INFO` & `emlib-1.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.9.1
+Version: 1.9.2
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.9.1/README.rst` & `emlib-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/__init__.py` & `emlib-1.9.2/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/_dialogsqt.py` & `emlib-1.9.2/emlib/_dialogsqt.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/calculus.py` & `emlib-1.9.2/emlib/calculus.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/combinatorics.py` & `emlib-1.9.2/emlib/combinatorics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/common.py` & `emlib-1.9.2/emlib/common.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/containers.py` & `emlib-1.9.2/emlib/containers.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/csvtools.py` & `emlib-1.9.2/emlib/csvtools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/dialogs.py` & `emlib-1.9.2/emlib/dialogs.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/doctools.py` & `emlib-1.9.2/emlib/doctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/electronics.py` & `emlib-1.9.2/emlib/electronics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/envir.py` & `emlib-1.9.2/emlib/envir.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/filetools.py` & `emlib-1.9.2/emlib/filetools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/graphlib.py` & `emlib-1.9.2/emlib/graphlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/img.py` & `emlib-1.9.2/emlib/img.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/iterlib.py` & `emlib-1.9.2/emlib/iterlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/jsontools.py` & `emlib-1.9.2/emlib/jsontools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/logutils.py` & `emlib-1.9.2/emlib/logutils.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/mathlib.py` & `emlib-1.9.2/emlib/mathlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/matplotting.py` & `emlib-1.9.2/emlib/matplotting.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/minizinctools.py` & `emlib-1.9.2/emlib/minizinctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/misc.py` & `emlib-1.9.2/emlib/misc.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/net.py` & `emlib-1.9.2/emlib/net.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/numberseries.py` & `emlib-1.9.2/emlib/numberseries.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/numpytools.py` & `emlib-1.9.2/emlib/numpytools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/numtheory.py` & `emlib-1.9.2/emlib/numtheory.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/parabolicinterpol.py` & `emlib-1.9.2/emlib/parabolicinterpol.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/readbytes.py` & `emlib-1.9.2/emlib/readbytes.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/shelling.py` & `emlib-1.9.2/emlib/shelling.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/smooth.py` & `emlib-1.9.2/emlib/smooth.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/stochastic.py` & `emlib-1.9.2/emlib/stochastic.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/textlib.py` & `emlib-1.9.2/emlib/textlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/video.py` & `emlib-1.9.2/emlib/video.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib/xmlprinter.py` & `emlib-1.9.2/emlib/xmlprinter.py`

 * *Files identical despite different names*

### Comparing `emlib-1.9.1/emlib.egg-info/PKG-INFO` & `emlib-1.9.2/emlib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.9.1
+Version: 1.9.2
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.9.1/emlib.egg-info/SOURCES.txt` & `emlib-1.9.2/emlib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 emlib/minizinctools.py
 emlib/misc.py
 emlib/net.py
 emlib/numberseries.py
 emlib/numpytools.py
 emlib/numtheory.py
 emlib/parabolicinterpol.py
+emlib/py.typed
 emlib/readbytes.py
 emlib/shelling.py
 emlib/smooth.py
 emlib/stochastic.py
 emlib/textlib.py
 emlib/video.py
 emlib/xmlprinter.py
```

### Comparing `emlib-1.9.1/setup.py` & `emlib-1.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 from setuptools import setup
 
 readme = open('README.rst').read()
-version = (1, 9, 1)
+version = (1, 9, 2)
 
 setup(
     name='emlib',
     python_requires=">=3.9",
     version=".".join(map(str, version)),
     description='Miscellaneous utilities',
     long_description=readme,
@@ -39,8 +39,9 @@
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9'
                 
     ],
+    package_data={'emlib': ['py.typed']},
 )
```

