# Comparing `tmp/request-time-tracker-0.0.6.tar.gz` & `tmp/request-time-tracker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "request-time-tracker-0.0.6.tar", last modified: Tue Nov 30 13:35:14 2021, max compression
+gzip compressed data, was "request-time-tracker-0.0.7.tar", last modified: Wed Dec  1 10:01:56 2021, max compression
```

## Comparing `request-time-tracker-0.0.6.tar` & `request-time-tracker-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)       80 2021-11-30 13:19:00.000000 request-time-tracker-0.0.6/MANIFEST.in
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2904 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/PKG-INFO
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      101 2021-07-20 09:39:27.000000 request-time-tracker-0.0.6/pyproject.toml
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2205 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/readme.md
--rw-rw-r--   0 th13f     (1000) th13f     (1000)       38 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/setup.cfg
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1025 2021-11-30 13:16:44.000000 request-time-tracker-0.0.6/setup.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/request_time_tracker/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-06-10 10:09:09.000000 request-time-tracker-0.0.6/src/request_time_tracker/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2707 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/django_wsgi.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/request_time_tracker/notifiers/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/notifiers/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      464 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/notifiers/base.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2301 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/notifiers/cloudwatch.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/request_time_tracker/trackers/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1738 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/base.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1684 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/base.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1755 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/django.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2156 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/redis.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      967 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/trackers/memory.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      571 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/request_time_tracker/wsgi.py
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/request_time_tracker.egg-info/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     2904 2021-11-30 13:35:14.000000 request-time-tracker-0.0.6/src/request_time_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1032 2021-11-30 13:35:14.000000 request-time-tracker-0.0.6/src/request_time_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        1 2021-11-30 13:35:14.000000 request-time-tracker-0.0.6/src/request_time_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 th13f     (1000) th13f     (1000)       27 2021-11-30 13:35:14.000000 request-time-tracker-0.0.6/src/request_time_tracker.egg-info/top_level.txt
-drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-11-30 13:35:14.227867 request-time-tracker-0.0.6/src/tests/
--rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/__init__.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      766 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/base.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1814 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/settings.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1708 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/test_django_cache_tracker.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     5271 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/test_legacy.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      966 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/test_memory_tracker.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)     1827 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/test_redis_cache_tracker.py
--rw-rw-r--   0 th13f     (1000) th13f     (1000)      118 2021-11-30 12:41:53.000000 request-time-tracker-0.0.6/src/tests/urls.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)       80 2021-11-30 13:19:00.000000 request-time-tracker-0.0.7/MANIFEST.in
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2907 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/PKG-INFO
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      101 2021-07-20 09:39:27.000000 request-time-tracker-0.0.7/pyproject.toml
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2208 2021-11-30 14:51:22.000000 request-time-tracker-0.0.7/readme.md
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)       38 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/setup.cfg
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1025 2021-12-01 10:01:42.000000 request-time-tracker-0.0.7/setup.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.697039 request-time-tracker-0.0.7/src/
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.697039 request-time-tracker-0.0.7/src/request_time_tracker/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-06-10 10:09:09.000000 request-time-tracker-0.0.7/src/request_time_tracker/__init__.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2707 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/django_wsgi.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.697039 request-time-tracker-0.0.7/src/request_time_tracker/notifiers/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/notifiers/__init__.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      464 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/notifiers/base.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2300 2021-12-01 10:00:35.000000 request-time-tracker-0.0.7/src/request_time_tracker/notifiers/cloudwatch.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/src/request_time_tracker/trackers/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/__init__.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1735 2021-12-01 09:49:27.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/base.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/__init__.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1684 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/base.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1755 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/django.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2158 2021-12-01 10:00:37.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/redis.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      967 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/trackers/memory.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      571 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/request_time_tracker/wsgi.py
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.697039 request-time-tracker-0.0.7/src/request_time_tracker.egg-info/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2907 2021-12-01 10:01:56.000000 request-time-tracker-0.0.7/src/request_time_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1032 2021-12-01 10:01:56.000000 request-time-tracker-0.0.7/src/request_time_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        1 2021-12-01 10:01:56.000000 request-time-tracker-0.0.7/src/request_time_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)       27 2021-12-01 10:01:56.000000 request-time-tracker-0.0.7/src/request_time_tracker.egg-info/top_level.txt
+drwxrwxr-x   0 th13f     (1000) th13f     (1000)        0 2021-12-01 10:01:56.701039 request-time-tracker-0.0.7/src/tests/
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)        0 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/tests/__init__.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      763 2021-12-01 09:50:55.000000 request-time-tracker-0.0.7/src/tests/base.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     1814 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/tests/settings.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2110 2021-12-01 09:51:28.000000 request-time-tracker-0.0.7/src/tests/test_django_cache_tracker.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     5573 2021-12-01 09:59:52.000000 request-time-tracker-0.0.7/src/tests/test_legacy.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      966 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/tests/test_memory_tracker.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)     2219 2021-12-01 10:00:38.000000 request-time-tracker-0.0.7/src/tests/test_redis_cache_tracker.py
+-rw-rw-r--   0 th13f     (1000) th13f     (1000)      118 2021-11-30 12:41:53.000000 request-time-tracker-0.0.7/src/tests/urls.py
```

### Comparing `request-time-tracker-0.0.6/PKG-INFO` & `request-time-tracker-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: request-time-tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: Requests time tracker from being captured by proxy (e.g. nginx) till being executed by wsgi handler
 Home-page: https://github.com/razortheory/request-time-tracker
 Author: Roman Karpovich
 Author-email: roman@razortheory.com
 License: UNKNOWN
 Project-URL: Home, https://github.com/razortheory/request-time-tracker
 Project-URL: Bug Tracker, https://github.com/razortheory/request-time-tracker/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-#Queue time tracker
+# Queue time tracker
 Reads time when request was processed by nginx & send time spent in queue before it was handled by wsgi.  
 Designed mostly for autoscaling. Instance cpu is not trustworthy enough, sometimes there can be external bottlenecks, 
 so even if instance cpu is fine, application can hang in queue between nginx(for example) and gunicorn or another wsgi processor.  
 
-##Configuration
+## Configuration
 1. Add header with request timestamp.
 
    nginx:
     ```
    proxy_set_header X-RequestTime $msec;
    ```
 
@@ -68,15 +68,15 @@
     ),
 )
 
 wsgi_application = tracker(wsgi_application)
 ```
 
 
-##Cloudwatch role policy:
+## Cloudwatch role policy:
 ```
 {
     “Version”: “2012-10-17",
     “Statement”: [
         {
             “Sid”: “VisualEditor0”,
             “Effect”: “Allow”,
```

### Comparing `request-time-tracker-0.0.6/readme.md` & `request-time-tracker-0.0.7/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#Queue time tracker
+# Queue time tracker
 Reads time when request was processed by nginx & send time spent in queue before it was handled by wsgi.  
 Designed mostly for autoscaling. Instance cpu is not trustworthy enough, sometimes there can be external bottlenecks, 
 so even if instance cpu is fine, application can hang in queue between nginx(for example) and gunicorn or another wsgi processor.  
 
-##Configuration
+## Configuration
 1. Add header with request timestamp.
 
    nginx:
     ```
    proxy_set_header X-RequestTime $msec;
    ```
 
@@ -51,15 +51,15 @@
     ),
 )
 
 wsgi_application = tracker(wsgi_application)
 ```
 
 
-##Cloudwatch role policy:
+## Cloudwatch role policy:
 ```
 {
     “Version”: “2012-10-17",
     “Statement”: [
         {
             “Sid”: “VisualEditor0”,
             “Effect”: “Allow”,
```

### Comparing `request-time-tracker-0.0.6/setup.py` & `request-time-tracker-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setuptools.setup(
     name="request-time-tracker",
-    version="0.0.6",
+    version="0.0.7",
     author="Roman Karpovich",
     author_email="roman@razortheory.com",
     description="Requests time tracker from being captured by proxy (e.g. nginx) till being executed by wsgi handler",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/razortheory/request-time-tracker",
     project_urls={
```

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/django_wsgi.py` & `request-time-tracker-0.0.7/src/request_time_tracker/django_wsgi.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/notifiers/cloudwatch.py` & `request-time-tracker-0.0.7/src/request_time_tracker/notifiers/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import threading
 from datetime import datetime, timedelta
 
 import boto3
-
 from request_time_tracker.notifiers.base import BaseNotifier
 
 logger = logging.getLogger('django.time_in_queue')
 
 
 def notify_cloudwatch_time_queue(
     access_key: str,
```

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/trackers/base.py` & `request-time-tracker-0.0.7/src/request_time_tracker/trackers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if self.queue_time_header_name not in environ:
             return None
 
         request_timestamp, millis = environ[self.queue_time_header_name].split('.')
         request_started_at = datetime.fromtimestamp(int(request_timestamp))
         request_started_at = request_started_at.replace(microsecond=int(millis) * 1000)
 
-        request_in_queue = datetime.utcnow() - request_started_at
+        request_in_queue = datetime.now() - request_started_at
 
         return request_in_queue
 
     def __call__(self, environ: dict, start_response: callable):
         time_spent_in_queue = self.get_time_spent_in_queue(environ)
         if time_spent_in_queue and self.check_cooldown():
             self.refresh_cooldown()
```

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/base.py` & `request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/base.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/django.py` & `request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/django.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/trackers/cache/redis.py` & `request-time-tracker-0.0.7/src/request_time_tracker/trackers/cache/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from datetime import datetime, timedelta
 from typing import Any
 
 from redis import Redis
 from redis.exceptions import ConnectionError
-
 from request_time_tracker.notifiers.base import BaseNotifier
 from request_time_tracker.trackers.cache.base import BaseCacheQueueTimeTracker
 
 logger = logging.getLogger('django.time_in_queue')
 
 
 class RedisCacheQueueTimeTracker(BaseCacheQueueTimeTracker):
@@ -38,15 +37,15 @@
         return Redis.from_url(self.redis_url)
 
     def get_time_last_notified(self) -> [datetime]:
         cache = self.get_cache()
 
         try:
             try:
-                last_notified = datetime.fromtimestamp(float(cache.get(self.get_cache_key())))
+                last_notified = datetime.utcfromtimestamp(float(cache.get(self.get_cache_key())))
             except TypeError:
                 last_notified = None
 
             if last_notified is None:
                 last_notified = datetime.utcnow() - timedelta(seconds=self.send_stats_every_seconds + 1)
                 cache.set(self.get_cache_key(), last_notified.timestamp())
         except ConnectionError:
```

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/trackers/memory.py` & `request-time-tracker-0.0.7/src/request_time_tracker/trackers/memory.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker/wsgi.py` & `request-time-tracker-0.0.7/src/request_time_tracker/wsgi.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker.egg-info/PKG-INFO` & `request-time-tracker-0.0.7/src/request_time_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: request-time-tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: Requests time tracker from being captured by proxy (e.g. nginx) till being executed by wsgi handler
 Home-page: https://github.com/razortheory/request-time-tracker
 Author: Roman Karpovich
 Author-email: roman@razortheory.com
 License: UNKNOWN
 Project-URL: Home, https://github.com/razortheory/request-time-tracker
 Project-URL: Bug Tracker, https://github.com/razortheory/request-time-tracker/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-#Queue time tracker
+# Queue time tracker
 Reads time when request was processed by nginx & send time spent in queue before it was handled by wsgi.  
 Designed mostly for autoscaling. Instance cpu is not trustworthy enough, sometimes there can be external bottlenecks, 
 so even if instance cpu is fine, application can hang in queue between nginx(for example) and gunicorn or another wsgi processor.  
 
-##Configuration
+## Configuration
 1. Add header with request timestamp.
 
    nginx:
     ```
    proxy_set_header X-RequestTime $msec;
    ```
 
@@ -68,15 +68,15 @@
     ),
 )
 
 wsgi_application = tracker(wsgi_application)
 ```
 
 
-##Cloudwatch role policy:
+## Cloudwatch role policy:
 ```
 {
     “Version”: “2012-10-17",
     “Statement”: [
         {
             “Sid”: “VisualEditor0”,
             “Effect”: “Allow”,
```

### Comparing `request-time-tracker-0.0.6/src/request_time_tracker.egg-info/SOURCES.txt` & `request-time-tracker-0.0.7/src/request_time_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/tests/base.py` & `request-time-tracker-0.0.7/src/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 
 def noop():
     pass
 
 
 def get_time_in_millis():
-    start_time = datetime.utcnow()
+    start_time = datetime.now()
     return '{0}.{1}'.format(int(start_time.timestamp()), int(start_time.microsecond / 1000))
```

### Comparing `request-time-tracker-0.0.6/src/tests/settings.py` & `request-time-tracker-0.0.7/src/tests/settings.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/tests/test_django_cache_tracker.py` & `request-time-tracker-0.0.7/src/tests/test_django_cache_tracker.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from django.test import TestCase
 
 from request_time_tracker.trackers.cache.django import DjangoCacheQueueTimeTracker
 from tests.base import DummyNotifier, DummyWSGI, get_time_in_millis, noop
 
 
 class TestCacheTracker(TestCase):
+    def test_request_duration(self):
+        tracker = partial(DjangoCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
+                          cache_name='queue-tracker-cache')
+        wsgi = tracker(DummyWSGI())
+        time_spent = wsgi.get_time_spent_in_queue({'time-header': get_time_in_millis()})
+        self.assertLess(abs(time_spent), timedelta(seconds=1))
+
     def test_wrong_cache_name(self):
         tracker = partial(DjangoCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
                           cache_name='missing')
         wsgi = tracker(DummyWSGI())
         self.assertEqual(caches['default'], wsgi.get_cache())
 
     @patch('tests.base.DummyNotifier.notify_time_spent')
@@ -29,10 +36,10 @@
         notify_mock.reset_mock()
         tracker = partial(DjangoCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
                           cache_name='queue-tracker-cache')
         wsgi = tracker(DummyWSGI())
         wsgi({'time-header': get_time_in_millis()}, noop)
         notify_mock.assert_not_called()
 
-        caches['queue-tracker-cache'].set(wsgi.get_cache_key(), datetime.utcnow() - timedelta(seconds=11))
+        caches['queue-tracker-cache'].set(wsgi.get_cache_key(), datetime.now() - timedelta(seconds=11))
         wsgi({'time-header': get_time_in_millis()}, noop)
         notify_mock.assert_called()
```

### Comparing `request-time-tracker-0.0.6/src/tests/test_legacy.py` & `request-time-tracker-0.0.7/src/tests/test_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from django.test import TestCase, override_settings
 
 from request_time_tracker.wsgi import QueueTimeTracker
 from tests.base import DummyWSGI, FakeThread, get_time_in_millis, noop
 
 
 class TestLegacyTracker(TestCase):
+    @override_settings(CLOUDWATCH_QUEUE_TIME_HEADER='time-header')
+    def test_request_duration(self):
+        wsgi = QueueTimeTracker(DummyWSGI())
+        time_spent = wsgi.get_time_spent_in_queue({'time-header': get_time_in_millis()})
+        self.assertLess(abs(time_spent), timedelta(seconds=1))
+
     @patch('request_time_tracker.notifiers.cloudwatch.CloudWatchNotifier.notify_time_spent')
     @override_settings(CLOUDWATCH_QUEUE_TIME_ACCESS_KEY='test')
     @override_settings(CLOUDWATCH_QUEUE_TIME_SECRET_KEY='test')
     @override_settings(CLOUDWATCH_QUEUE_TIME_REGION='test')
     @override_settings(CLOUDWATCH_QUEUE_TIME_NAMESPACE='test')
     @override_settings(CLOUDWATCH_QUEUE_TIME_HEADER='time-header')
     def test_functionality(self, notify_mock):
```

### Comparing `request-time-tracker-0.0.6/src/tests/test_memory_tracker.py` & `request-time-tracker-0.0.7/src/tests/test_memory_tracker.py`

 * *Files identical despite different names*

### Comparing `request-time-tracker-0.0.6/src/tests/test_redis_cache_tracker.py` & `request-time-tracker-0.0.7/src/tests/test_redis_cache_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from datetime import datetime, timedelta
 from functools import partial
 from unittest import TestCase
 from unittest.mock import patch
 
 from redis import Redis
-
 from request_time_tracker.trackers.cache.redis import RedisCacheQueueTimeTracker
 from tests.base import DummyNotifier, DummyWSGI, get_time_in_millis, noop
 
 
 class TestCacheTracker(TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         cls.redis_url = 'redis://localhost:6379/0'
 
     def setUp(self) -> None:
         Redis.from_url(self.redis_url).flushdb()
 
+    def test_request_duration(self):
+        tracker = partial(RedisCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
+                          redis_url=self.redis_url)
+        wsgi = tracker(DummyWSGI())
+        time_spent = wsgi.get_time_spent_in_queue({'time-header': get_time_in_millis()})
+        self.assertLess(abs(time_spent), timedelta(seconds=1))
+
     def test_bad_redis_url(self):
         tracker = partial(RedisCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
                           redis_url='redis://localhosssst:6379/0')
         wsgi = tracker(DummyWSGI())
         wsgi({'time-header': get_time_in_millis()}, noop)
 
     @patch('tests.base.DummyNotifier.notify_time_spent')
@@ -36,10 +42,10 @@
         notify_mock.reset_mock()
         tracker = partial(RedisCacheQueueTimeTracker, queue_time_header_name='time-header', notifier=DummyNotifier(),
                           redis_url=self.redis_url)
         wsgi = tracker(DummyWSGI())
         wsgi({'time-header': get_time_in_millis()}, noop)
         notify_mock.assert_not_called()
 
-        cache.set(wsgi.get_cache_key(), (datetime.utcnow() - timedelta(seconds=11)).timestamp())
+        cache.set(wsgi.get_cache_key(), (datetime.now() - timedelta(seconds=11)).timestamp())
         wsgi({'time-header': get_time_in_millis()}, noop)
         notify_mock.assert_called()
```

