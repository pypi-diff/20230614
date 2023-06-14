# Comparing `tmp/django_federation_auditlog-0.1.0.tar.gz` & `tmp/django_federation_auditlog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.1.0.tar", max compression
+gzip compressed data, was "django_federation_auditlog-0.2.0.tar", max compression
```

## Comparing `django_federation_auditlog-0.1.0.tar` & `django_federation_auditlog-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       17 2023-06-14 18:39:01.988085 django_federation_auditlog-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 18:39:01.988085 django_federation_auditlog-0.1.0/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      783 2023-06-14 18:39:01.988085 django_federation_auditlog-0.1.0/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0       93 2023-06-14 18:39:01.988085 django_federation_auditlog-0.1.0/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5479 2023-06-14 18:39:01.988085 django_federation_auditlog-0.1.0/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4147 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2356 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2050 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4654 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      665 2023-06-14 18:39:01.992085 django_federation_auditlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 django_federation_auditlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4164 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3212 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    15062 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      665 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.0/PKG-INFO
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/admin.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib import admin
 
-from iauditlog.models import LogEntry
-from iauditlog.mixins import LogEntryAdminMixin
+from django_federation_auditlog.models import LogEntry
+from django_federation_auditlog.mixins import LogEntryAdminMixin
 from django_federation_auditlog.filters import ResourceTypeFilter
 
 
 @admin.register(LogEntry)
 class LogEntryAdmin(admin.ModelAdmin, LogEntryAdminMixin):
     list_display = [
         "created",
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/diff.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Untracked fields are many-to-many relations and relations to the Auditlog LogEntry model.
 
     :param field: The field to check.
     :type field: Field
     :return: Whether the given field should be tracked.
     :rtype: bool
     """
-    from iauditlog.models import LogEntry
+    from django_federation_auditlog.models import LogEntry
 
     # Do not track many to many relations
     if field.many_to_many:
         return False
 
     # Do not track relations to LogEntry
     if (
@@ -96,15 +96,15 @@
     :param fields_to_check: An iterable of the field names to restrict the diff to, while ignoring the rest of
         the model's fields. This is used to pass the `update_fields` kwarg from the model's `save` method.
     :type fields_to_check: Iterable
     :return: A dictionary with the names of the changed fields as keys and a two tuple of the old and new field values
              as value.
     :rtype: dict
     """
-    from iauditlog.registry import auditlog
+    from django_federation_auditlog.registry import auditlog
 
     if not (old is None or isinstance(old, Model)):
         raise TypeError(
             "The supplied old instance is not a valid model instance."
         )
     if not (new is None or isinstance(new, Model)):
         raise TypeError(
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/middleware.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import threading
 import time
 from functools import partial
 
-from iauditlog.models import LogEntry
+from django_federation_auditlog.models import LogEntry
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db.models.signals import pre_save
 from django.utils.deprecation import MiddlewareMixin
 from django.utils.functional import SimpleLazyObject
 from rest_framework_simplejwt.authentication import JWTTokenUserAuthentication
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/mixins.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django import urls as urlresolvers
 from django.conf import settings
 from django.urls.exceptions import NoReverseMatch
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 
-from iauditlog.models import LogEntry
+from django_federation_auditlog.models import LogEntry
 
 MAX = 75
 
 
 class LogEntryAdminMixin:
     def created(self, obj):
         return obj.timestamp.strftime("%Y-%m-%d %H:%M:%S")
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/models.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/receivers.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/receivers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from iauditlog.diff import model_instance_diff
-from iauditlog.models import LogEntry
+from django_federation_auditlog.diff import model_instance_diff
+from django_federation_auditlog.models import LogEntry
 
 
 def log_create(sender, instance, created, **kwargs):
     """
     Signal receiver that creates a log entry when a model instance is first saved to the database.
 
     Direct use is discouraged, connect your model through :py:func:`auditlog.registry.register` instead.
```

### Comparing `django_federation_auditlog-0.1.0/django_federation_auditlog/registry.py` & `django_federation_auditlog-0.2.0/django_federation_auditlog/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     def __init__(
         self,
         create: bool = True,
         update: bool = True,
         delete: bool = True,
         custom: Optional[Dict[ModelSignal, Callable]] = None,
     ):
-        from iauditlog.receivers import log_create, log_delete, log_update
+        from django_federation_auditlog.receivers import (
+            log_create,
+            log_delete,
+            log_update,
+        )
 
         self._registry = {}
         self._signals = {}
 
         if create:
             self._signals[post_save] = log_create
         if update:
```

### Comparing `django_federation_auditlog-0.1.0/pyproject.toml` & `django_federation_auditlog-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 django-auditlog = "1.0.0"
```

### Comparing `django_federation_auditlog-0.1.0/PKG-INFO` & `django_federation_auditlog-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

