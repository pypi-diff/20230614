# Comparing `tmp/django_federation_auditlog-0.2.1.tar.gz` & `tmp/django_federation_auditlog-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-0.2.1.tar", max compression
+gzip compressed data, was "django_federation_auditlog-0.2.2.tar", max compression
```

## Comparing `django_federation_auditlog-0.2.1.tar` & `django_federation_auditlog-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       17 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      799 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4164 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3212 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-06-14 19:13:38.463012 django_federation_auditlog-0.2.1/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    15062 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      742 2023-06-14 19:13:38.467012 django_federation_auditlog-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4175 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3212 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    15062 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      742 2023-06-14 19:29:50.695310 django_federation_auditlog-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 django_federation_auditlog-0.2.2/PKG-INFO
```

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/admin.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/diff.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/middleware.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class AuditlogMiddleware(MiddlewareMixin):
     def __call__(self, request):
         user = SimpleLazyObject(lambda: getattr(request, "user", None))
 
         if not user.is_authenticated:
             jwt_authentication = JWTTokenUserAuthentication()
             header = jwt_authentication.get_header(request)
-            if jwt_authentication.get_raw_token(header):
+            if header and jwt_authentication.get_raw_token(header):
                 token_user, _ = jwt_authentication.authenticate(request)
                 User = get_user_model()
                 user = User(
                     username=token_user.token['user_id'],
                     email=token_user.token['user_id'],
                     is_active=True,
                 )
```

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/mixins.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/models.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/receivers.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/django_federation_auditlog/registry.py` & `django_federation_auditlog-0.2.2/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-0.2.1/pyproject.toml` & `django_federation_auditlog-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 djangorestframework = "==3.11.1"
```

### Comparing `django_federation_auditlog-0.2.1/PKG-INFO` & `django_federation_auditlog-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

