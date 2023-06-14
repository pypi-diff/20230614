# Comparing `tmp/django_shopify_app-1.1.5.tar.gz` & `tmp/django_shopify_app-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_shopify_app-1.1.5.tar", last modified: Sun Jun  4 05:27:25 2023, max compression
+gzip compressed data, was "django_shopify_app-1.1.6.tar", last modified: Wed Jun 14 00:08:10 2023, max compression
```

## Comparing `django_shopify_app-1.1.5.tar` & `django_shopify_app-1.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/django_shopify_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/run_shopify_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/update_shop_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.241584 django_shopify_app-1.1.6/django_shopify_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-14 00:08:10.000000 django_shopify_app-1.1.6/django_shopify_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-14 00:08:10.000000 django_shopify_app-1.1.6/django_shopify_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:08:10.000000 django_shopify_app-1.1.6/django_shopify_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 00:08:10.000000 django_shopify_app-1.1.6/django_shopify_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 00:08:10.000000 django_shopify_app-1.1.6/django_shopify_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.241584 django_shopify_app-1.1.6/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.241584 django_shopify_app-1.1.6/shopify_app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.241584 django_shopify_app-1.1.6/shopify_app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/management/commands/run_shopify_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/management/commands/update_shop_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.241584 django_shopify_app-1.1.6/shopify_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/shopify_app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/shopify_app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/shopify_app/templates/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/templates/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/templates/shopify_app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/shopify_app/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:10.245585 django_shopify_app-1.1.6/shopify_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-14 00:08:00.000000 django_shopify_app-1.1.6/shopify_app/views.py
```

### Comparing `django_shopify_app-1.1.5/PKG-INFO` & `django_shopify_app-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_shopify_app
-Version: 1.1.5
+Version: 1.1.6
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.5/README.md` & `django_shopify_app-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/django_shopify_app.egg-info/PKG-INFO` & `django_shopify_app-1.1.6/django_shopify_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-shopify-app
-Version: 1.1.5
+Version: 1.1.6
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.5/django_shopify_app.egg-info/SOURCES.txt` & `django_shopify_app-1.1.6/django_shopify_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/apps.py` & `django_shopify_app-1.1.6/shopify_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/decorators.py` & `django_shopify_app-1.1.6/shopify_app/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
             request = args[0]
 
             authorization_header = request.META.get("HTTP_SHOPIFYAUTH")
             if (
                 not authorization_header
                 and request.user.is_authenticated
-                and request.user.is_admin
+                and request.user.is_staff
             ):
-                print('user is admin')
+                print('user is staff ')
 
             app_config = apps.get_app_config("shopify_app")
             decoded_session_token = session_token.decode_from_header(
                 authorization_header=authorization_header,
                 api_key=app_config.SHOPIFY_API_KEY,
                 secret=app_config.SHOPIFY_API_SECRET,
             )
```

### Comparing `django_shopify_app-1.1.5/shopify_app/management/commands/run_shopify_pubsub.py` & `django_shopify_app-1.1.6/shopify_app/management/commands/run_shopify_pubsub.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/management/commands/update_shop_webhooks.py` & `django_shopify_app-1.1.6/shopify_app/management/commands/update_shop_webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/models.py` & `django_shopify_app-1.1.6/shopify_app/models.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/services/webhooks.py` & `django_shopify_app-1.1.6/shopify_app/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/templates/shopify_app/index.html` & `django_shopify_app-1.1.6/shopify_app/templates/shopify_app/index.html`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/urls.py` & `django_shopify_app-1.1.6/shopify_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/utils/__init__.py` & `django_shopify_app-1.1.6/shopify_app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.5/shopify_app/views.py` & `django_shopify_app-1.1.6/shopify_app/views.py`

 * *Files identical despite different names*

