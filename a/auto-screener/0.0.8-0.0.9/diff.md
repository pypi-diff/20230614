# Comparing `tmp/auto-screener-0.0.8.tar.gz` & `tmp/auto-screener-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.0.8.tar", last modified: Sun Apr 23 18:01:01 2023, max compression
+gzip compressed data, was "auto-screener-0.0.9.tar", last modified: Thu Apr 27 07:32:22 2023, max compression
```

## Comparing `auto-screener-0.0.8.tar` & `auto-screener-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.582907 auto-screener-0.0.8/
--rw-rw-rw-   0        0        0      115 2023-04-23 18:01:01.000000 auto-screener-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-04-23 18:01:01.582907 auto-screener-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.576783 auto-screener-0.0.8/auto_screener/
--rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.8/auto_screener/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.8/auto_screener/base.py
--rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.8/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      526 2023-04-21 17:13:30.000000 auto-screener-0.0.8/auto_screener/document.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.8/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.8/auto_screener/interval.py
--rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.8/auto_screener/progress.py
--rw-rw-rw-   0        0        0    53152 2023-04-23 17:57:09.000000 auto-screener-0.0.8/auto_screener/screening.py
--rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.8/auto_screener/tickers.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:01:01.581907 auto-screener-0.0.8/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 18:01:01.000000 auto-screener-0.0.8/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.8/build.py
--rw-rw-rw-   0        0        0      645 2023-04-23 18:01:01.000000 auto-screener-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 18:01:01.583907 auto-screener-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-04-23 18:00:58.000000 auto-screener-0.0.8/setup.py
--rw-rw-rw-   0        0        0      850 2023-04-23 18:00:43.000000 auto-screener-0.0.8/test.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.865464 auto-screener-0.0.9/
+-rw-rw-rw-   0        0        0      115 2023-04-27 07:32:22.000000 auto-screener-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-04-27 07:32:22.865464 auto-screener-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.860326 auto-screener-0.0.9/auto_screener/
+-rw-rw-rw-   0        0        0      498 2023-04-21 09:31:59.000000 auto-screener-0.0.9/auto_screener/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.0.9/auto_screener/base.py
+-rw-rw-rw-   0        0        0    20994 2023-04-27 07:13:14.000000 auto-screener-0.0.9/auto_screener/collect.py
+-rw-rw-rw-   0        0        0     5944 2023-04-22 07:38:43.000000 auto-screener-0.0.9/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      602 2023-04-27 07:14:09.000000 auto-screener-0.0.9/auto_screener/document.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.0.9/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.0.9/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    10013 2023-04-21 17:11:58.000000 auto-screener-0.0.9/auto_screener/progress.py
+-rw-rw-rw-   0        0        0    35077 2023-04-27 07:31:55.000000 auto-screener-0.0.9/auto_screener/screening.py
+-rw-rw-rw-   0        0        0     9865 2023-04-21 17:03:15.000000 auto-screener-0.0.9/auto_screener/tickers.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:32:22.864456 auto-screener-0.0.9/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-27 07:32:22.000000 auto-screener-0.0.9/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.0.9/build.py
+-rw-rw-rw-   0        0        0      645 2023-04-27 07:32:22.000000 auto-screener-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-04-21 17:54:19.000000 auto-screener-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:32:22.866464 auto-screener-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1655 2023-04-27 07:32:18.000000 auto-screener-0.0.9/setup.py
+-rw-rw-rw-   0        0        0      850 2023-04-23 18:00:43.000000 auto-screener-0.0.9/test.py
```

### Comparing `auto-screener-0.0.8/PKG-INFO` & `auto-screener-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.8
+Version: 0.0.9
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.8/README.md` & `auto-screener-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener/base.py` & `auto-screener-0.0.9/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener/dataset.py` & `auto-screener-0.0.9/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener/document.py` & `auto-screener-0.0.9/auto_screener/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from auto_screener.screening import *
 # noinspection PyUnresolvedReferences
 from auto_screener.tickers import *
 # noinspection PyUnresolvedReferences
 from auto_screener.progress import *
 # noinspection PyUnresolvedReferences
 from auto_screener.dataset import *
+# noinspection PyUnresolvedReferences
+from auto_screener.collect import *
 
 from auto_screener.base import document
 
 class Documentation:
     """"""
 # end Documentation
```

### Comparing `auto-screener-0.0.8/auto_screener/interval.py` & `auto-screener-0.0.9/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener/progress.py` & `auto-screener-0.0.9/auto_screener/progress.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener/tickers.py` & `auto-screener-0.0.9/auto_screener/tickers.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.0.9/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.0.8
+Version: 0.0.9
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.0.8/build.py` & `auto-screener-0.0.9/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.0.8/pyproject.toml` & `auto-screener-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.0.8'
+version = '0.0.9'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.0.8/setup.py` & `auto-screener-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         include=[
             "test.py",
             "auto_screener/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.0.8',
+        version='0.0.9',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `auto-screener-0.0.8/test.py` & `auto-screener-0.0.9/test.py`

 * *Files identical despite different names*

