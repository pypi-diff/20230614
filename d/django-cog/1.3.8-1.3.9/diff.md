# Comparing `tmp/django-cog-1.3.8.tar.gz` & `tmp/django-cog-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cog-1.3.8.tar", last modified: Wed Mar 29 19:49:57 2023, max compression
+gzip compressed data, was "django-cog-1.3.9.tar", last modified: Wed Jun 14 16:02:15 2023, max compression
```

## Comparing `django-cog-1.3.8.tar` & `django-cog-1.3.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 19:49:57.852118 django-cog-1.3.8/
--rwxr-xr-x   0 david     (1000) david     (1000)       62 2022-07-29 13:57:20.000000 django-cog-1.3.8/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    16176 2023-03-29 19:49:57.852118 django-cog-1.3.8/PKG-INFO
--rwxr-xr-x   0 david     (1000) david     (1000)    15596 2022-07-29 13:57:20.000000 django-cog-1.3.8/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 19:49:57.848118 django-cog-1.3.8/django_cog/
--rwxr-xr-x   0 david     (1000) david     (1000)    10726 2022-07-29 13:57:47.000000 django-cog-1.3.8/django_cog/__init__.py
--rwxr-xr-x   0 david     (1000) david     (1000)     5066 2022-07-29 13:57:47.000000 django-cog-1.3.8/django_cog/admin.py
--rwxr-xr-x   0 david     (1000) david     (1000)     1883 2022-07-29 13:57:47.000000 django-cog-1.3.8/django_cog/apps.py
--rwxr-xr-x   0 david     (1000) david     (1000)      177 2022-07-29 13:57:47.000000 django-cog-1.3.8/django_cog/celery.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 19:49:57.852118 django-cog-1.3.8/django_cog/migrations/
--rwxr-xr-x   0 david     (1000) david     (1000)     5998 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0001_initial.py
--rwxr-xr-x   0 david     (1000) david     (1000)     1003 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0002_auto_20210519_0824.py
--rwxr-xr-x   0 david     (1000) david     (1000)      532 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0003_task_queue.py
--rwxr-xr-x   0 david     (1000) david     (1000)      559 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0004_auto_20210519_0931.py
--rwxr-xr-x   0 david     (1000) david     (1000)      422 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0005_auto_20210519_1006.py
--rwxr-xr-x   0 david     (1000) david     (1000)      611 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0006_auto_20210525_0809.py
--rwxr-xr-x   0 david     (1000) david     (1000)      522 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0007_auto_20210525_0810.py
--rwxr-xr-x   0 david     (1000) david     (1000)      390 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0008_task_critical.py
--rwxr-xr-x   0 david     (1000) david     (1000)      379 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0009_taskrun_success.py
--rwxr-xr-x   0 david     (1000) david     (1000)      533 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0010_auto_20210914_1500.py
--rwxr-xr-x   0 david     (1000) david     (1000)      757 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0011_cogerrorhandler.py
--rwxr-xr-x   0 david     (1000) david     (1000)     1005 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0012_cogerror.py
--rwxr-xr-x   0 david     (1000) david     (1000)      526 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0013_task_error_handler.py
--rwxr-xr-x   0 david     (1000) david     (1000)      529 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0014_auto_20210915_1035.py
--rwxr-xr-x   0 david     (1000) david     (1000)      419 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0015_cogerror_error_type.py
--rwxr-xr-x   0 david     (1000) david     (1000)      423 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0016_auto_20210915_1042.py
--rwxr-xr-x   0 david     (1000) david     (1000)      935 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0017_auto_20210915_1533.py
--rwxr-xr-x   0 david     (1000) david     (1000)      554 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/0018_auto_20210915_1544.py
--rw-r--r--   0 david     (1000) david     (1000)      704 2023-03-29 19:48:08.000000 django-cog-1.3.8/django_cog/migrations/0019_auto_20230329_1547.py
--rwxr-xr-x   0 david     (1000) david     (1000)        0 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/migrations/__init__.py
--rwxr-xr-x   0 david     (1000) david     (1000)    13228 2023-03-29 19:47:53.000000 django-cog-1.3.8/django_cog/models.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 19:49:57.852118 django-cog-1.3.8/django_cog/templates/
--rwxr-xr-x   0 david     (1000) david     (1000)      320 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/templates/cancel_run.html
--rwxr-xr-x   0 david     (1000) david     (1000)      198 2022-07-29 13:59:51.000000 django-cog-1.3.8/django_cog/templates/change_form.html
--rwxr-xr-x   0 david     (1000) david     (1000)     1006 2022-07-29 13:57:47.000000 django-cog-1.3.8/django_cog/tests.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 19:49:57.848118 django-cog-1.3.8/django_cog.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    16176 2023-03-29 19:49:57.000000 django-cog-1.3.8/django_cog.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1324 2023-03-29 19:49:57.000000 django-cog-1.3.8/django_cog.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-29 19:49:57.000000 django-cog-1.3.8/django_cog.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       61 2023-03-29 19:49:57.000000 django-cog-1.3.8/django_cog.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-03-29 19:49:57.000000 django-cog-1.3.8/django_cog.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-03-29 19:49:57.852118 django-cog-1.3.8/setup.cfg
--rwxr-xr-x   0 david     (1000) david     (1000)     1050 2023-03-29 19:49:12.000000 django-cog-1.3.8/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-14 16:02:15.498781 django-cog-1.3.9/
+-rwxr-xr-x   0 david     (1000) david     (1000)       62 2022-07-29 13:57:20.000000 django-cog-1.3.9/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)    16177 2023-06-14 16:02:15.498781 django-cog-1.3.9/PKG-INFO
+-rwxr-xr-x   0 david     (1000) david     (1000)    15596 2022-07-29 13:57:20.000000 django-cog-1.3.9/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-14 16:02:15.498781 django-cog-1.3.9/django_cog/
+-rwxr-xr-x   0 david     (1000) david     (1000)    10726 2022-07-29 13:57:47.000000 django-cog-1.3.9/django_cog/__init__.py
+-rwxr-xr-x   0 david     (1000) david     (1000)     5066 2022-07-29 13:57:47.000000 django-cog-1.3.9/django_cog/admin.py
+-rwxr-xr-x   0 david     (1000) david     (1000)     1883 2022-07-29 13:57:47.000000 django-cog-1.3.9/django_cog/apps.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      177 2022-07-29 13:57:47.000000 django-cog-1.3.9/django_cog/celery.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-14 16:02:15.498781 django-cog-1.3.9/django_cog/migrations/
+-rwxr-xr-x   0 david     (1000) david     (1000)     5998 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0001_initial.py
+-rwxr-xr-x   0 david     (1000) david     (1000)     1003 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0002_auto_20210519_0824.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      532 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0003_task_queue.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      559 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0004_auto_20210519_0931.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      422 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0005_auto_20210519_1006.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      611 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0006_auto_20210525_0809.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      522 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0007_auto_20210525_0810.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      390 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0008_task_critical.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      379 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0009_taskrun_success.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      533 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0010_auto_20210914_1500.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      757 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0011_cogerrorhandler.py
+-rwxr-xr-x   0 david     (1000) david     (1000)     1005 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0012_cogerror.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      526 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0013_task_error_handler.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      529 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0014_auto_20210915_1035.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      419 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0015_cogerror_error_type.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      423 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0016_auto_20210915_1042.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      935 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0017_auto_20210915_1533.py
+-rwxr-xr-x   0 david     (1000) david     (1000)      554 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/0018_auto_20210915_1544.py
+-rw-r--r--   0 david     (1000) david     (1000)      704 2023-03-29 19:48:08.000000 django-cog-1.3.9/django_cog/migrations/0019_auto_20230329_1547.py
+-rwxr-xr-x   0 david     (1000) david     (1000)        0 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/migrations/__init__.py
+-rwxr-xr-x   0 david     (1000) david     (1000)    13602 2023-06-14 16:00:36.000000 django-cog-1.3.9/django_cog/models.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-14 16:02:15.498781 django-cog-1.3.9/django_cog/templates/
+-rwxr-xr-x   0 david     (1000) david     (1000)      320 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/templates/cancel_run.html
+-rwxr-xr-x   0 david     (1000) david     (1000)      198 2022-07-29 13:59:51.000000 django-cog-1.3.9/django_cog/templates/change_form.html
+-rwxr-xr-x   0 david     (1000) david     (1000)     1006 2022-07-29 13:57:47.000000 django-cog-1.3.9/django_cog/tests.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-14 16:02:15.498781 django-cog-1.3.9/django_cog.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    16177 2023-06-14 16:02:15.000000 django-cog-1.3.9/django_cog.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1324 2023-06-14 16:02:15.000000 django-cog-1.3.9/django_cog.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-14 16:02:15.000000 django-cog-1.3.9/django_cog.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       61 2023-06-14 16:02:15.000000 django-cog-1.3.9/django_cog.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-06-14 16:02:15.000000 django-cog-1.3.9/django_cog.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-14 16:02:15.498781 django-cog-1.3.9/setup.cfg
+-rwxr-xr-x   0 david     (1000) david     (1000)     1051 2023-06-14 16:01:53.000000 django-cog-1.3.9/setup.py
```

### Comparing `django-cog-1.3.8/PKG-INFO` & `django-cog-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-cog
-Version: 1.3.8
+Version: 1.3.9
 Summary: Django library for launching pipelines of multiple stages and parallel tasks.
 Home-page: https://github.com/david-pettifor-nd/django_cog.git
 Author: David W Pettifor
 Author-email: dpettifo@nd.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Description-Content-Type: text/markdown
 
 # Django-Cog
 A [django-celery-beat](https://github.com/celery/django-celery-beat) extension to build pipelines of chronological stages and parallel tasks.
```

### Comparing `django-cog-1.3.8/README.md` & `django-cog-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/__init__.py` & `django-cog-1.3.9/django_cog/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/admin.py` & `django-cog-1.3.9/django_cog/admin.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/apps.py` & `django-cog-1.3.9/django_cog/apps.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0001_initial.py` & `django-cog-1.3.9/django_cog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0002_auto_20210519_0824.py` & `django-cog-1.3.9/django_cog/migrations/0002_auto_20210519_0824.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0003_task_queue.py` & `django-cog-1.3.9/django_cog/migrations/0003_task_queue.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0004_auto_20210519_0931.py` & `django-cog-1.3.9/django_cog/migrations/0004_auto_20210519_0931.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0006_auto_20210525_0809.py` & `django-cog-1.3.9/django_cog/migrations/0006_auto_20210525_0809.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0007_auto_20210525_0810.py` & `django-cog-1.3.9/django_cog/migrations/0007_auto_20210525_0810.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0010_auto_20210914_1500.py` & `django-cog-1.3.9/django_cog/migrations/0010_auto_20210914_1500.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0011_cogerrorhandler.py` & `django-cog-1.3.9/django_cog/migrations/0011_cogerrorhandler.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0012_cogerror.py` & `django-cog-1.3.9/django_cog/migrations/0012_cogerror.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0013_task_error_handler.py` & `django-cog-1.3.9/django_cog/migrations/0013_task_error_handler.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0014_auto_20210915_1035.py` & `django-cog-1.3.9/django_cog/migrations/0014_auto_20210915_1035.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0017_auto_20210915_1533.py` & `django-cog-1.3.9/django_cog/migrations/0017_auto_20210915_1533.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0018_auto_20210915_1544.py` & `django-cog-1.3.9/django_cog/migrations/0018_auto_20210915_1544.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/migrations/0019_auto_20230329_1547.py` & `django-cog-1.3.9/django_cog/migrations/0019_auto_20230329_1547.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog/models.py` & `django-cog-1.3.9/django_cog/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,18 +196,23 @@
     pipeline = models.ForeignKey(Pipeline, related_name='runs', on_delete=models.CASCADE)
     success = models.BooleanField(null=True)
 
     def __str__(self):
         return f"{str(self.pipeline)} {self.__str_runtimes__()}"
     
     def save(self, *args, **kwargs):
+        # do we have an ID yet?  if not, this means we're on our first stage
+        if not self.id:
+            super().save(*args, **kwargs)
+        
         # how many tasks need to be completed?
         required = self.pipeline.stages.all().count()
-        completed = self.stage_runs.filter(
-            completed_on__isnull=False
+        completed = StageRun.objects.filter(
+            completed_on__isnull=False,
+            pipeline_run=self
         ).count()
         if required == completed:
             self.completed_on = datetime.datetime.now(tz=pytz.UTC)
 
             # did we complete successfully?  if we're here and haven't been set to false yet,
             # then we can assume it's all good
             if self.success is None:
@@ -242,32 +247,38 @@
                         average_weight = task.runs.filter(
                             task__enabled=True
                         )[:sample_size].annotate(
                             runtime=duration
                         ).aggregate(models.Avg('runtime'))['runtime__avg'].total_seconds()
                         task.weight  = average_weight
                         task.save()
+        
         super(PipelineRun, self).save(*args, **kwargs)
 
 class StageRun(EntityRun):
     """
     Specific execution run of a stage.
     """
     pipeline_run = models.ForeignKey(PipelineRun, related_name='stage_runs', on_delete=models.CASCADE)
     stage = models.ForeignKey(Stage, related_name='runs', on_delete=models.CASCADE)
     success = models.BooleanField(null=True)
 
     def __str__(self):
         return f"{str(self.stage)} {self.__str_runtimes__()}"
     
     def save(self, *args, **kwargs):
+        # do we have an ID yet?  if not, this means we're on our first stage
+        if not self.id:
+            super().save(*args, **kwargs)
+        
         # how many tasks need to be completed?
         required = self.stage.assigned_tasks.filter(enabled=True).count()
-        completed = self.task_runs.filter(
-            completed_on__isnull=False
+        completed = TaskRun.objects.filter(
+            completed_on__isnull=False,
+            stage_run=self
         ).count()
         if required == completed and self.completed_on is None:
             self.completed_on = datetime.datetime.now(tz=pytz.UTC)
 
             # did we complete it successfully?  default is yes unless we've been set
             # to false by a failed task already
             if self.success is None:
```

### Comparing `django-cog-1.3.8/django_cog/tests.py` & `django-cog-1.3.9/django_cog/tests.py`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/django_cog.egg-info/PKG-INFO` & `django-cog-1.3.9/django_cog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-cog
-Version: 1.3.8
+Version: 1.3.9
 Summary: Django library for launching pipelines of multiple stages and parallel tasks.
 Home-page: https://github.com/david-pettifor-nd/django_cog.git
 Author: David W Pettifor
 Author-email: dpettifo@nd.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Description-Content-Type: text/markdown
 
 # Django-Cog
 A [django-celery-beat](https://github.com/celery/django-celery-beat) extension to build pipelines of chronological stages and parallel tasks.
```

### Comparing `django-cog-1.3.8/django_cog.egg-info/SOURCES.txt` & `django-cog-1.3.9/django_cog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cog-1.3.8/setup.py` & `django-cog-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-cog",
-    version="1.3.8",
+    version="1.3.9",
     description="Django library for launching pipelines of multiple stages and parallel tasks.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/david-pettifor-nd/django_cog.git",
     author="David W Pettifor",
     author_email="dpettifo@nd.edu",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.1",
     ],
     packages=["django_cog"],
     include_package_data=True,
     install_requires=["celery==5.2.7", "django-celery-beat", "django-nested-inline>=0.4.2"]
```

