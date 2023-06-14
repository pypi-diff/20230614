# Comparing `tmp/servicelayer-1.9.7.tar.gz` & `tmp/servicelayer-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/servicelayer-1.9.7.tar", last modified: Sun Jan 26 12:55:43 2020, max compression
+gzip compressed data, was "dist/servicelayer-1.9.9.tar", last modified: Wed Jan 29 13:22:12 2020, max compression
```

## Comparing `servicelayer-1.9.7.tar` & `servicelayer-1.9.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.976825 servicelayer-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (115)      690 2020-01-26 12:55:43.976825 servicelayer-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      733 2020-01-26 12:54:08.000000 servicelayer-1.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.972825 servicelayer-1.9.7/servicelayer/
--rw-r--r--   0 runner    (1001) docker     (115)      149 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.976825 servicelayer-1.9.7/servicelayer/archive/
--rw-r--r--   0 runner    (1001) docker     (115)      650 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      878 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (115)     1707 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/file.py
--rw-r--r--   0 runner    (1001) docker     (115)     4558 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/gs.py
--rw-r--r--   0 runner    (1001) docker     (115)     4387 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/s3.py
--rw-r--r--   0 runner    (1001) docker     (115)      795 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/util.py
--rw-r--r--   0 runner    (1001) docker     (115)     1395 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/archive/virtual.py
--rw-r--r--   0 runner    (1001) docker     (115)     1599 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/cache.py
--rw-r--r--   0 runner    (1001) docker     (115)      902 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/env.py
--rw-r--r--   0 runner    (1001) docker     (115)      817 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/extensions.py
--rw-r--r--   0 runner    (1001) docker     (115)    11315 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/jobs.py
--rw-r--r--   0 runner    (1001) docker     (115)     1822 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (115)      771 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     1817 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/util.py
--rw-r--r--   0 runner    (1001) docker     (115)     3279 2020-01-26 12:54:08.000000 servicelayer-1.9.7/servicelayer/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.972825 servicelayer-1.9.7/servicelayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)      690 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      987 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       67 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (115)      200 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       19 2020-01-26 12:55:43.000000 servicelayer-1.9.7/servicelayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-26 12:55:11.000000 servicelayer-1.9.7/servicelayer.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (115)       67 2020-01-26 12:55:43.976825 servicelayer-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1493 2020-01-26 12:54:08.000000 servicelayer-1.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.976825 servicelayer-1.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-26 12:55:43.976825 servicelayer-1.9.7/tests/archive/
--rw-r--r--   0 runner    (1001) docker     (115)       81 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1630 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/archive/test_file.py
--rw-r--r--   0 runner    (1001) docker     (115)     1604 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/archive/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (115)      177 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (115)      384 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (115)      273 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (115)     3472 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (115)      433 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (115)     1399 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (115)     1105 2020-01-26 12:54:08.000000 servicelayer-1.9.7/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.868769 servicelayer-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (115)      690 2020-01-29 13:22:12.868769 servicelayer-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      733 2020-01-29 13:21:22.000000 servicelayer-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.860769 servicelayer-1.9.9/servicelayer/
+-rw-r--r--   0 runner    (1001) docker     (115)      149 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.864769 servicelayer-1.9.9/servicelayer/archive/
+-rw-r--r--   0 runner    (1001) docker     (115)      650 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      878 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1707 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/file.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4558 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/gs.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4387 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/s3.py
+-rw-r--r--   0 runner    (1001) docker     (115)      795 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1395 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/archive/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1599 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/cache.py
+-rw-r--r--   0 runner    (1001) docker     (115)      902 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/env.py
+-rw-r--r--   0 runner    (1001) docker     (115)      817 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11315 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (115)      386 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/logs.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1822 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (115)      903 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/settings.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1817 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3279 2020-01-29 13:21:22.000000 servicelayer-1.9.9/servicelayer/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.864769 servicelayer-1.9.9/servicelayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)      690 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1008 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       67 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      200 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       19 2020-01-29 13:22:12.000000 servicelayer-1.9.9/servicelayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-29 13:21:45.000000 servicelayer-1.9.9/servicelayer.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (115)       67 2020-01-29 13:22:12.868769 servicelayer-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1493 2020-01-29 13:21:22.000000 servicelayer-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.864769 servicelayer-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-29 13:22:12.868769 servicelayer-1.9.9/tests/archive/
+-rw-r--r--   0 runner    (1001) docker     (115)       81 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1630 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/archive/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1604 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/archive/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (115)      177 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (115)      384 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (115)      273 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3472 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (115)      433 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1399 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1105 2020-01-29 13:21:22.000000 servicelayer-1.9.9/tests/test_worker.py
```

### Comparing `servicelayer-1.9.7/PKG-INFO` & `servicelayer-1.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: servicelayer
-Version: 1.9.7
+Version: 1.9.9
 Summary: Basic remote service functions for alephdata components
 Home-page: http://github.com/alephdata/servicelayer
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Description: UNKNOWN
 Keywords: storage files s3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: amazon
-Provides-Extra: dev
 Provides-Extra: google
+Provides-Extra: dev
+Provides-Extra: amazon
```

### Comparing `servicelayer-1.9.7/README.md` & `servicelayer-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/__init__.py` & `servicelayer-1.9.9/servicelayer/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/archive.py` & `servicelayer-1.9.9/servicelayer/archive/archive.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/file.py` & `servicelayer-1.9.9/servicelayer/archive/file.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/gs.py` & `servicelayer-1.9.9/servicelayer/archive/gs.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/s3.py` & `servicelayer-1.9.9/servicelayer/archive/s3.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/util.py` & `servicelayer-1.9.9/servicelayer/archive/util.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/archive/virtual.py` & `servicelayer-1.9.9/servicelayer/archive/virtual.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/cache.py` & `servicelayer-1.9.9/servicelayer/cache.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/env.py` & `servicelayer-1.9.9/servicelayer/env.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/extensions.py` & `servicelayer-1.9.9/servicelayer/extensions.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/jobs.py` & `servicelayer-1.9.9/servicelayer/jobs.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/rate_limit.py` & `servicelayer-1.9.9/servicelayer/rate_limit.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/settings.py` & `servicelayer-1.9.9/servicelayer/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 REDIS_SHORT = 84700
 REDIS_LONG = REDIS_SHORT * 200
 REDIS_EXPIRE = env.to_int('REDIS_EXPIRE', REDIS_SHORT * 7)
 REDIS_PREFIX = 'sla'
 
 # Worker
 WORKER_RETRY = env.to_int('WORKER_RETRY', 3)
-WORKER_THREADS = min(8, multiprocessing.cpu_count())
-WORKER_THREADS = env.to_int('WORKER_THREADS', WORKER_THREADS)
+WORKER_THREADS = env.to_int('WORKER_THREADS', min(8, multiprocessing.cpu_count()))
 
 # Amazon client credentials
 AWS_KEY_ID = env.get('AWS_ACCESS_KEY_ID')
 AWS_SECRET_KEY = env.get('AWS_SECRET_ACCESS_KEY')
 AWS_REGION = env.get('AWS_REGION', 'eu-west-1')
 
 # Storage type (either 's3', 'gs', or 'file', i.e. local file system):
 ARCHIVE_TYPE = env.get('ARCHIVE_TYPE', 'file')
 ARCHIVE_BUCKET = env.get('ARCHIVE_BUCKET')
 ARCHIVE_PATH = env.get('ARCHIVE_PATH')
+
+# Logging
+LOGGING_LEVEL = env.get('LOGGING_LEVEL', 'DEBUG').upper()
+LOGGING_FORMAT = env.get('LOGGING_FORMAT', '[%(asctime)s] %(levelname)s:%(name)s:%(message)s')
```

### Comparing `servicelayer-1.9.7/servicelayer/util.py` & `servicelayer-1.9.9/servicelayer/util.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer/worker.py` & `servicelayer-1.9.9/servicelayer/worker.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/servicelayer.egg-info/PKG-INFO` & `servicelayer-1.9.9/servicelayer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: servicelayer
-Version: 1.9.7
+Version: 1.9.9
 Summary: Basic remote service functions for alephdata components
 Home-page: http://github.com/alephdata/servicelayer
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Description: UNKNOWN
 Keywords: storage files s3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: amazon
-Provides-Extra: dev
 Provides-Extra: google
+Provides-Extra: dev
+Provides-Extra: amazon
```

### Comparing `servicelayer-1.9.7/servicelayer.egg-info/SOURCES.txt` & `servicelayer-1.9.9/servicelayer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.cfg
 setup.py
 servicelayer/__init__.py
 servicelayer/cache.py
 servicelayer/env.py
 servicelayer/extensions.py
 servicelayer/jobs.py
+servicelayer/logs.py
 servicelayer/rate_limit.py
 servicelayer/settings.py
 servicelayer/util.py
 servicelayer/worker.py
 servicelayer.egg-info/PKG-INFO
 servicelayer.egg-info/SOURCES.txt
 servicelayer.egg-info/dependency_links.txt
```

### Comparing `servicelayer-1.9.7/setup.py` & `servicelayer-1.9.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='servicelayer',
-    version='1.9.7',
+    version='1.9.9',
     description="Basic remote service functions for alephdata components",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.6',
@@ -27,23 +27,23 @@
         'six >= 1.12.0',
         'normality >= 1.0.0',
         'redis == 3.3.11',
         'fakeredis == 1.1.0',
     ],
     extras_require={
         'amazon': [
-            'boto3 >= 1.9.71',
+            'boto3 >= 1.11.9',
         ],
         'google': [
             'google-cloud-storage >= 1.10.0',
         ],
         'dev': [
             'twine',
             'moto',
-            'boto3 >= 1.9.71',
+            'boto3 >= 1.11.9',
             'pytest >= 3.6',
             'coverage',
             'pytest-cov',
         ]
     },
     test_suite='tests',
     entry_points={
```

### Comparing `servicelayer-1.9.7/tests/archive/test_file.py` & `servicelayer-1.9.9/tests/archive/test_file.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/tests/archive/test_s3.py` & `servicelayer-1.9.9/tests/archive/test_s3.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/tests/test_jobs.py` & `servicelayer-1.9.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/tests/test_util.py` & `servicelayer-1.9.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `servicelayer-1.9.7/tests/test_worker.py` & `servicelayer-1.9.9/tests/test_worker.py`

 * *Files identical despite different names*

