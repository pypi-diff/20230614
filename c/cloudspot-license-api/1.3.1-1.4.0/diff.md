# Comparing `tmp/cloudspot-license-api-1.3.1.tar.gz` & `tmp/cloudspot-license-api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudspot-license-api-1.3.1.tar", last modified: Wed Mar  8 12:01:09 2023, max compression
+gzip compressed data, was "dist\cloudspot-license-api-1.4.0.tar", last modified: Fri May 12 09:23:42 2023, max compression
```

## Comparing `cloudspot-license-api-1.3.1.tar` & `cloudspot-license-api-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/cloudspotlicense/
--rw-rw-rw-   0        0        0     4078 2023-03-08 11:42:20.000000 cloudspot-license-api-1.3.1/cloudspotlicense/api.py
--rw-rw-rw-   0        0        0      103 2022-10-03 14:12:11.000000 cloudspot-license-api-1.3.1/cloudspotlicense/config.py
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/cloudspotlicense/constants/
--rw-rw-rw-   0        0        0      189 2022-01-28 15:55:32.000000 cloudspot-license-api-1.3.1/cloudspotlicense/constants/errors.py
--rw-rw-rw-   0        0        0      463 2022-02-04 10:27:01.000000 cloudspot-license-api-1.3.1/cloudspotlicense/constants/responses.py
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/cloudspotlicense/endpoints/
--rw-rw-rw-   0        0        0     2819 2023-03-08 11:42:20.000000 cloudspot-license-api-1.3.1/cloudspotlicense/endpoints/auth.py
--rw-rw-rw-   0        0        0      120 2022-10-03 14:17:47.000000 cloudspot-license-api-1.3.1/cloudspotlicense/endpoints/base.py
--rw-rw-rw-   0        0        0        0 2021-04-25 10:50:21.000000 cloudspot-license-api-1.3.1/cloudspotlicense/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/cloudspotlicense/models/
--rw-rw-rw-   0        0        0     1561 2023-03-08 12:00:56.000000 cloudspot-license-api-1.3.1/cloudspotlicense/models/auth.py
--rw-rw-rw-   0        0        0     2902 2022-10-03 14:25:09.000000 cloudspot-license-api-1.3.1/cloudspotlicense/models/base.py
--rw-rw-rw-   0        0        0      144 2022-01-21 14:32:49.000000 cloudspot-license-api-1.3.1/cloudspotlicense/models/errors.py
--rw-rw-rw-   0        0        0        0 2021-04-23 14:27:21.000000 cloudspot-license-api-1.3.1/cloudspotlicense/models/__init__.py
--rw-rw-rw-   0        0        0        0 2021-04-11 13:15:48.000000 cloudspot-license-api-1.3.1/cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-08 12:01:08.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5861 2023-03-08 12:01:08.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-03-08 12:01:08.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      676 2023-03-08 12:01:08.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-03-08 12:01:08.000000 cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 cloudspot-license-api-1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2021-04-16 14:13:07.000000 cloudspot-license-api-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5861 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5070 2022-10-17 09:12:25.000000 cloudspot-license-api-1.3.1/README.md
--rw-rw-rw-   0        0        0       86 2023-03-08 12:01:09.000000 cloudspot-license-api-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-03-08 12:00:56.000000 cloudspot-license-api-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/
+-rw-rw-rw-   0        0        0     4078 2023-03-08 11:42:20.000000 cloudspot-license-api-1.4.0/cloudspotlicense/api.py
+-rw-rw-rw-   0        0        0      103 2022-10-03 14:12:11.000000 cloudspot-license-api-1.4.0/cloudspotlicense/config.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/
+-rw-rw-rw-   0        0        0      189 2022-01-28 15:55:32.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/errors.py
+-rw-rw-rw-   0        0        0      463 2022-02-04 10:27:01.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/responses.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/
+-rw-rw-rw-   0        0        0     2807 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/auth.py
+-rw-rw-rw-   0        0        0      120 2022-10-03 14:17:47.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/base.py
+-rw-rw-rw-   0        0        0        0 2021-04-25 10:50:21.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/
+-rw-rw-rw-   0        0        0     1604 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/auth.py
+-rw-rw-rw-   0        0        0     2902 2022-10-03 14:25:09.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/base.py
+-rw-rw-rw-   0        0        0      144 2022-01-21 14:32:49.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/errors.py
+-rw-rw-rw-   0        0        0        0 2021-04-23 14:27:21.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-04-11 13:15:48.000000 cloudspot-license-api-1.4.0/cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     5861 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      676 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 cloudspot-license-api-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2021-04-16 14:13:07.000000 cloudspot-license-api-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5861 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5070 2022-10-17 09:12:25.000000 cloudspot-license-api-1.4.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/setup.py
```

### Comparing `cloudspot-license-api-1.3.1/cloudspotlicense/api.py` & `cloudspot-license-api-1.4.0/cloudspotlicense/api.py`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.3.1/cloudspotlicense/endpoints/auth.py` & `cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,51 +10,51 @@
         
     def authenticate(self, username, password):
         endpoint = '{0}/{1}'.format(self.endpoint, 'authenticate')
         data = { 'username' : username, 'password' : password }
         
         status, headers, resp_json = self.api.post(endpoint, data)
         
-        if status != 200: return AuthResponse().parse_error(resp_json)
+        if status > 399: return AuthResponse().parse_error(resp_json)
         auth_resp = AuthResponse().parse(resp_json)
         
         return auth_resp
     
     def validate_impersonation(self, token):
         endpoint = '{0}/{1}'.format(self.endpoint, 'impersonation-validation')
         data = { 'token' : token }
         
         status, headers, resp_json = self.api.post(endpoint, data)
         
-        if status != 200: return ImpersonateResponse().parse_error(resp_json)
+        if status > 399: return ImpersonateResponse().parse_error(resp_json)
         impersonate_resp = ImpersonateResponse().parse(resp_json)
         
         return impersonate_resp
     
     def get_user(self):
         if not self.api.token: raise NoValidToken('No token found. Authenticate the user first to retrieve a token or supply a token to the function.')
         
         endpoint = '{0}/{1}'.format(self.endpoint, 'users/profile')
         data = None
         
         status, headers, resp_json = self.api.get(endpoint, data)
-        
-        if status != 200: return User().parse_error(resp_json)
+
+        if status > 399: return User().parse_error(resp_json)
         user_resp = User().parse(resp_json)
         
         return user_resp
     
     def get_company_permissions(self, company_id):
         if not self.api.token: raise NoValidToken('No token found. Authenticate the user first to retrieve a token or supply a token to the function.')
         endpoint = '{0}/{1}/{2}'.format(self.endpoint, 'get-company-permissions', company_id)
         data = None
         
         status, headers, resp_json = self.api.get(endpoint, data)
         
-        if status != 200: return CompanyPermissionsResponse().parse_error(resp_json)
+        if status > 399: return CompanyPermissionsResponse().parse_error(resp_json)
         resp = CompanyPermissionsResponse().parse(resp_json)
         
         return resp
 
     def get_permissions(self):
         if not self.api.token: raise NoValidToken('No token found. Authenticate the user first to retrieve a token or supply a token to the function.')
         endpoint = '{0}/{1}'.format(self.endpoint, 'get-permissions')
```

### Comparing `cloudspot-license-api-1.3.1/cloudspotlicense/models/auth.py` & `cloudspot-license-api-1.4.0/cloudspotlicense/models/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,22 +46,24 @@
         self.permissions = permissions if permissions else AuthPermissions()
 
 class User(BaseModel):
     
     def __init__(self,
         first_name=None,
         last_name=None,
-        email=None
+        email=None,
+        pin=None
     ):
         
         super().__init__()
         
         self.first_name = first_name
         self.last_name = last_name
         self.email = email
+        self.pin = pin
 
 class CompanyPermissionsResponse(BaseModel):
     def __init__(self,
         permissions=None
     ):
 
         super().__init__()
```

### Comparing `cloudspot-license-api-1.3.1/cloudspotlicense/models/base.py` & `cloudspot-license-api-1.4.0/cloudspotlicense/models/base.py`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/PKG-INFO` & `cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudspot-license-api
-Version: 1.3.1
+Version: 1.4.0
 Summary: Wrapper for the Cloudspot License API endpoints
 Home-page: https://github.com/Ecosy-EU/cloudspot-license-api
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.3.1.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz
 Keywords: cloudspot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cloudspot-license-api-1.3.1/cloudspot_license_api.egg-info/SOURCES.txt` & `cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.3.1/LICENSE.txt` & `cloudspot-license-api-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.3.1/PKG-INFO` & `cloudspot-license-api-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudspot-license-api
-Version: 1.3.1
+Version: 1.4.0
 Summary: Wrapper for the Cloudspot License API endpoints
 Home-page: https://github.com/Ecosy-EU/cloudspot-license-api
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.3.1.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz
 Keywords: cloudspot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cloudspot-license-api-1.3.1/README.md` & `cloudspot-license-api-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.3.1/setup.py` & `cloudspot-license-api-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'cloudspot-license-api',         
   packages=['cloudspotlicense', 'cloudspotlicense.models', 'cloudspotlicense.constants', 'cloudspotlicense.endpoints'],
-  version = '1.3.1',
+  version = '1.4.0',
   license='GPL-3.0-or-later',
   description = 'Wrapper for the Cloudspot License API endpoints',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/cloudspot-license-api',
-  download_url = 'https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.3.1.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz',
   keywords = ['cloudspot'],
   install_requires=[
           'requests',
           'python-dateutil',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

