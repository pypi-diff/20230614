# Comparing `tmp/django_federation_auditlog-0.2.0.tar.gz` & `tmp/django_federation_auditlog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.2.0.tar", max compression
+gzip compressed data, was "django_federation_auditlog-0.2.1.tar", max compression
```

## Comparing `django_federation_auditlog-0.2.0.tar` & `django_federation_auditlog-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       17 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      817 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4164 2023-06-14 18:56:24.735575 django_federation_auditlog-0.2.0/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      665 2023-06-14 18:56:24.739575 django_federation_auditlog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4164 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3212 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    15062 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      742 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.1/PKG-INFO
```

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/admin.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib import admin
 
 from django_federation_auditlog.models import LogEntry
 from django_federation_auditlog.mixins import LogEntryAdminMixin
-from django_federation_auditlog.filters import ResourceTypeFilter
+from auditlog.filters import ResourceTypeFilter
 
 
 @admin.register(LogEntry)
 class LogEntryAdmin(admin.ModelAdmin, LogEntryAdminMixin):
     list_display = [
         "created",
         "resource_url",
```

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/diff.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/middleware.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/mixins.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/models.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/receivers.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/django_federation_auditlog/registry.py` & `django_federation_auditlog-0.2.1/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.0/pyproject.toml` & `django_federation_auditlog-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-django-auditlog = "1.0.0"
+djangorestframework = "==3.11.1"
+djangorestframework-simplejwt = "==5.0.0"
+django-auditlog = "==1.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8b1"
 flake8 = "^3.8.3"
 
 
 [tool.black]
```

### Comparing `django_federation_auditlog-0.2.0/PKG-INFO` & `django_federation_auditlog-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-auditlog (==1.0.0)
+Requires-Dist: djangorestframework (==3.11.1)
+Requires-Dist: djangorestframework-simplejwt (==5.0.0)
 Description-Content-Type: text/markdown
 
 # Django Auditlog
```

