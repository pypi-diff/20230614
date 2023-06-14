# Comparing `tmp/afex-sso-0.0.56.tar.gz` & `tmp/afex-sso-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.56.tar", last modified: Tue Jun 13 20:23:58 2023, max compression
+gzip compressed data, was "afex-sso-0.0.57.tar", last modified: Wed Jun 14 09:17:52 2023, max compression
```

## Comparing `afex-sso-0.0.56.tar` & `afex-sso-0.0.57.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 20:23:58.612654 afex-sso-0.0.56/
--rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.56/LICENSE
--rw-rw-rw-   0        0        0     2315 2023-06-13 20:23:58.612654 afex-sso-0.0.56/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 20:23:58.565278 afex-sso-0.0.56/app/
-drwxrwxrwx   0        0        0        0 2023-06-13 20:23:58.580313 afex-sso-0.0.56/app/AFEX_SSO/
--rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.56/app/AFEX_SSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:23:58.596833 afex-sso-0.0.56/app/AFEX_SSO/src/
--rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.56/app/AFEX_SSO/src/__init__.py
--rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.56/app/AFEX_SSO/src/get_hash_key.py
--rw-rw-rw-   0        0        0     2155 2023-06-08 16:53:35.000000 afex-sso-0.0.56/app/AFEX_SSO/src/sso.py
--rw-rw-rw-   0        0        0     1562 2023-06-13 20:21:54.000000 afex-sso-0.0.56/app/AFEX_SSO/src/views.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:23:58.612654 afex-sso-0.0.56/app/afex_sso.egg-info/
--rw-rw-rw-   0        0        0     2315 2023-06-13 20:23:57.000000 afex-sso-0.0.56/app/afex_sso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-13 20:23:58.000000 afex-sso-0.0.56/app/afex_sso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 20:23:57.000000 afex-sso-0.0.56/app/afex_sso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-13 20:23:57.000000 afex-sso-0.0.56/app/afex_sso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 20:23:57.000000 afex-sso-0.0.56/app/afex_sso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.56/pyproject.toml
--rw-rw-rw-   0        0        0      497 2023-06-13 20:23:58.612654 afex-sso-0.0.56/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-06-13 20:22:09.000000 afex-sso-0.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:17:52.848835 afex-sso-0.0.57/
+-rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.57/LICENSE
+-rw-rw-rw-   0        0        0     2315 2023-06-14 09:17:52.848835 afex-sso-0.0.57/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.57/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:17:52.817578 afex-sso-0.0.57/app/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:17:52.833226 afex-sso-0.0.57/app/AFEX_SSO/
+-rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.57/app/AFEX_SSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:17:52.833226 afex-sso-0.0.57/app/AFEX_SSO/src/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.57/app/AFEX_SSO/src/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.57/app/AFEX_SSO/src/get_hash_key.py
+-rw-rw-rw-   0        0        0     2155 2023-06-08 16:53:35.000000 afex-sso-0.0.57/app/AFEX_SSO/src/sso.py
+-rw-rw-rw-   0        0        0     1933 2023-06-14 09:12:41.000000 afex-sso-0.0.57/app/AFEX_SSO/src/views.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:17:52.848835 afex-sso-0.0.57/app/afex_sso.egg-info/
+-rw-rw-rw-   0        0        0     2315 2023-06-14 09:17:52.000000 afex-sso-0.0.57/app/afex_sso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-14 09:17:52.000000 afex-sso-0.0.57/app/afex_sso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:17:52.000000 afex-sso-0.0.57/app/afex_sso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-14 09:17:52.000000 afex-sso-0.0.57/app/afex_sso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 09:17:52.000000 afex-sso-0.0.57/app/afex_sso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.57/pyproject.toml
+-rw-rw-rw-   0        0        0      497 2023-06-14 09:17:52.848835 afex-sso-0.0.57/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-06-14 09:16:08.000000 afex-sso-0.0.57/setup.py
```

### Comparing `afex-sso-0.0.56/LICENSE` & `afex-sso-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.56/PKG-INFO` & `afex-sso-0.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.56
+Version: 0.0.57
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.56/README.md` & `afex-sso-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.56/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.57/app/AFEX_SSO/src/sso.py`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.56/app/AFEX_SSO/src/views.py` & `afex-sso-0.0.57/app/AFEX_SSO/src/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 import base64
 
 from django.conf import settings as app_settings
+from django.contrib.auth import get_user_model, login
 from django.shortcuts import redirect
 from django.views import View
 from .get_hash_key import get_hash_key
 from .sso import SSO
 
 
 sso = SSO()
 sso_url = app_settings.SSO_URL
+UserModel = get_user_model()
+
 
 
 class LoginView(View):
 
     def get(self, request, *kwargs):
         request_url = base64.b64encode(
             request.build_absolute_uri().encode('utf-8')
         ).decode('utf-8')
-        if 'q' in request.GET.keys():
-            ses_id = request.GET.get('q')
+        if 'q' in request.GET.keys() or request.session.get('state'):
+            ses_id = request.GET.get('q') or request.session.get('state')
+            if not request.session.get('state'):
+                request.session['state'] = ses_id
             validate_sso = sso.check_credentials(session_key=ses_id)
             try:
                 response_data = validate_sso['data']
             except:
                 return redirect(f"{sso_url}?qz={request_url}")
 
             user_data = response_data.get('user')
-            if user_data.get('email') and not User.objects.filter(email=user_data.get('email')).exists():
-                user = User.objects.create(
+            if user_data.get('email') and not UserModel.objects.filter(email=user_data.get('email')).exists():
+                user = UserModel.objects.create(
                     email=user_data.get('email'),
                     username=user_data.get('email'),
                     first_name=user_data.get('first_name'),
                     last_name=user_data.get('last_name'),
                 )
             else:
-                user = User.objects.get(email=user_data.get('email'))
+                user = UserModel.objects.get(email=user_data.get('email'))
+
+            if not user.is_staff:
+                user.is_staff = True
+                user.save()
             login(request, user)
 
             return redirect("admin:index")
 
         elif 'ec' in request.GET.keys() or 'next' in request.GET.keys():
             return redirect(f"/?ec={request.GET.get('ec')}")
         return redirect(f"{sso_url}?qz={request_url}")
```

### Comparing `afex-sso-0.0.56/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.57/app/afex_sso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.56
+Version: 0.0.57
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Description: 
         # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.56/setup.py` & `afex-sso-0.0.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.56",
+    version="0.0.57",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
```

