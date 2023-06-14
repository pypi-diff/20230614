# Comparing `tmp/django-cloudspotlicense-6.1.1.tar.gz` & `tmp/django-cloudspotlicense-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-cloudspotlicense-6.1.1.tar", last modified: Fri Jun  9 09:41:13 2023, max compression
+gzip compressed data, was "dist\django-cloudspotlicense-6.2.0.tar", last modified: Wed Jun 14 13:38:55 2023, max compression
```

## Comparing `django-cloudspotlicense-6.1.1.tar` & `django-cloudspotlicense-6.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/
--rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/admin.py
--rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/apps.py
--rw-rw-rw-   0        0        0      244 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/config.py
--rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/context_processors.py
--rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/
--rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/__init__.py
--rw-rw-rw-   0        0        0     2987 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/mixins.py
--rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/models.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/
--rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/login.html
--rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/select_company.html
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/
--rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/license_tags.py
--rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/templatetags/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/tests.py
--rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/urls.py
--rw-rw-rw-   0        0        0      401 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/utils.py
--rw-rw-rw-   0        0        0    16199 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/views.py
--rw-rw-rw-   0        0        0       69 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    10292 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1148 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10292 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9428 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-09 09:41:13.000000 django-cloudspotlicense-6.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/
+-rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/admin.py
+-rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/apps.py
+-rw-rw-rw-   0        0        0      244 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/config.py
+-rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/context_processors.py
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/
+-rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2987 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/mixins.py
+-rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/models.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templates/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templates/auth/
+-rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templates/auth/login.html
+-rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templates/auth/select_company.html
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templatetags/
+-rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templatetags/license_tags.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/templatetags/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/tests.py
+-rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/urls.py
+-rw-rw-rw-   0        0        0      401 2023-06-07 15:51:33.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/utils.py
+-rw-rw-rw-   0        0        0    16233 2023-06-14 13:36:58.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/views.py
+-rw-rw-rw-   0        0        0       69 2023-06-09 09:39:27.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:38:54.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    10292 2023-06-14 13:38:54.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-06-14 13:38:54.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1148 2023-06-14 13:38:54.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2023-06-14 13:38:54.000000 django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-6.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-6.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10292 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9428 2023-06-09 09:19:51.000000 django-cloudspotlicense-6.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-14 13:38:55.000000 django-cloudspotlicense-6.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-06-14 13:36:58.000000 django-cloudspotlicense-6.2.0/setup.py
```

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/helpers.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/helpers.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/migrations/0001_initial.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/mixins.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/mixins.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/models.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/models.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/templates/auth/login.html` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/urls.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/urls.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense/views.py` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,20 +240,20 @@
         
         req = json.loads(request.body)
         event = req['event']
         data = req['data']
         UserModel = get_user_model()
         
         if event == 'permissions.updated':
-            token = data['token']
+            username = data['username']
             
             try:
-                user = UserModel.objects.get(license_token=token)
+                user = UserModel.objects.get(username=username)
             except UserModel.DoesNotExist:
-                return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : 'No user matched the token.' }}, status=HTTPStatus.NOT_FOUND)
+                return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : f'No user matched the username: {username}.' }}, status=HTTPStatus.NOT_FOUND)
             
             permissions = data['permissions']
             company_id = data['company_id']
             available_companies = data['available_companies']
             
             # update the companies that the user is in
             user.available_companies.clear()
@@ -265,15 +265,15 @@
                     company.save()
                 
                 user.available_companies.add(company.id)
             
             try:
                 company = CloudspotCompany.objects.get(pk=company_id)
             except CloudspotCompany.DoesNotExist:
-                return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : 'No company matched the id.' }}, status=HTTPStatus.NOT_FOUND)
+                return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : f'No company matched the id: {company_id}' }}, status=HTTPStatus.NOT_FOUND)
 
             # Only update the user permissions if the current company is the company in the request
             # Otherwise, these permissions do not apply to this user at this moment
             # When the user switches companies, the new permissions get retrieved from the License Server anyway
             if user.company == company:
                 if get_root_perm() not in permissions:
                     # if the root permission is revoked, the user is not allowed to use the app for this company anymore.
```

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/PKG-INFO` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 6.1.1
+Version: 6.2.0
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.2.0.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-6.1.1/django_cloudspotlicense.egg-info/SOURCES.txt` & `django-cloudspotlicense-6.2.0/django_cloudspotlicense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/LICENSE.txt` & `django-cloudspotlicense-6.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/PKG-INFO` & `django-cloudspotlicense-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 6.1.1
+Version: 6.2.0
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.2.0.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-6.1.1/README.md` & `django-cloudspotlicense-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-6.1.1/setup.py` & `django-cloudspotlicense-6.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'django-cloudspotlicense',         
   packages=['django_cloudspotlicense', 'django_cloudspotlicense.migrations', 'django_cloudspotlicense.templatetags'],
   include_package_data=True,
-  version = '6.1.1',
+  version = '6.2.0',
   license='GPL-3.0-or-later',
   description = 'Django package to integrate the authentication of the Cloudspot License Server in other django applications',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/django-cloudspotlicense',
-  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.1.1.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/6.2.0.tar.gz',
   keywords = ['cloudspot', 'django'],
   install_requires=[
           'requests',
           'cloudspot-license-api',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

