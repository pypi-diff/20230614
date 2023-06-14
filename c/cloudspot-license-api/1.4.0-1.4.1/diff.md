# Comparing `tmp/cloudspot-license-api-1.4.0.tar.gz` & `tmp/cloudspot-license-api-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudspot-license-api-1.4.0.tar", last modified: Fri May 12 09:23:42 2023, max compression
+gzip compressed data, was "dist\cloudspot-license-api-1.4.1.tar", last modified: Wed Jun 14 13:32:37 2023, max compression
```

## Comparing `cloudspot-license-api-1.4.0.tar` & `cloudspot-license-api-1.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/
--rw-rw-rw-   0        0        0     4078 2023-03-08 11:42:20.000000 cloudspot-license-api-1.4.0/cloudspotlicense/api.py
--rw-rw-rw-   0        0        0      103 2022-10-03 14:12:11.000000 cloudspot-license-api-1.4.0/cloudspotlicense/config.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/
--rw-rw-rw-   0        0        0      189 2022-01-28 15:55:32.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/errors.py
--rw-rw-rw-   0        0        0      463 2022-02-04 10:27:01.000000 cloudspot-license-api-1.4.0/cloudspotlicense/constants/responses.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/
--rw-rw-rw-   0        0        0     2807 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/auth.py
--rw-rw-rw-   0        0        0      120 2022-10-03 14:17:47.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/base.py
--rw-rw-rw-   0        0        0        0 2021-04-25 10:50:21.000000 cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/
--rw-rw-rw-   0        0        0     1604 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/auth.py
--rw-rw-rw-   0        0        0     2902 2022-10-03 14:25:09.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/base.py
--rw-rw-rw-   0        0        0      144 2022-01-21 14:32:49.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/errors.py
--rw-rw-rw-   0        0        0        0 2021-04-23 14:27:21.000000 cloudspot-license-api-1.4.0/cloudspotlicense/models/__init__.py
--rw-rw-rw-   0        0        0        0 2021-04-11 13:15:48.000000 cloudspot-license-api-1.4.0/cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5861 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      676 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 09:23:41.000000 cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 cloudspot-license-api-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2021-04-16 14:13:07.000000 cloudspot-license-api-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5861 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5070 2022-10-17 09:12:25.000000 cloudspot-license-api-1.4.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 09:23:42.000000 cloudspot-license-api-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspotlicense/
+-rw-rw-rw-   0        0        0     4078 2023-03-08 11:42:20.000000 cloudspot-license-api-1.4.1/cloudspotlicense/api.py
+-rw-rw-rw-   0        0        0      103 2022-10-03 14:12:11.000000 cloudspot-license-api-1.4.1/cloudspotlicense/config.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspotlicense/constants/
+-rw-rw-rw-   0        0        0      189 2022-01-28 15:55:32.000000 cloudspot-license-api-1.4.1/cloudspotlicense/constants/errors.py
+-rw-rw-rw-   0        0        0      463 2022-02-04 10:27:01.000000 cloudspot-license-api-1.4.1/cloudspotlicense/constants/responses.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspotlicense/endpoints/
+-rw-rw-rw-   0        0        0     2807 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.1/cloudspotlicense/endpoints/auth.py
+-rw-rw-rw-   0        0        0      120 2022-10-03 14:17:47.000000 cloudspot-license-api-1.4.1/cloudspotlicense/endpoints/base.py
+-rw-rw-rw-   0        0        0        0 2021-04-25 10:50:21.000000 cloudspot-license-api-1.4.1/cloudspotlicense/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspotlicense/models/
+-rw-rw-rw-   0        0        0     1604 2023-05-12 09:22:22.000000 cloudspot-license-api-1.4.1/cloudspotlicense/models/auth.py
+-rw-rw-rw-   0        0        0     2953 2023-06-14 13:31:23.000000 cloudspot-license-api-1.4.1/cloudspotlicense/models/base.py
+-rw-rw-rw-   0        0        0      208 2023-06-14 13:31:23.000000 cloudspot-license-api-1.4.1/cloudspotlicense/models/errors.py
+-rw-rw-rw-   0        0        0        0 2021-04-23 14:27:21.000000 cloudspot-license-api-1.4.1/cloudspotlicense/models/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-04-11 13:15:48.000000 cloudspot-license-api-1.4.1/cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     5861 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      676 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 cloudspot-license-api-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2021-04-16 14:13:07.000000 cloudspot-license-api-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5861 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5070 2022-10-17 09:12:25.000000 cloudspot-license-api-1.4.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-14 13:32:37.000000 cloudspot-license-api-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-06-14 13:31:23.000000 cloudspot-license-api-1.4.1/setup.py
```

### Comparing `cloudspot-license-api-1.4.0/cloudspotlicense/api.py` & `cloudspot-license-api-1.4.1/cloudspotlicense/api.py`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/cloudspotlicense/endpoints/auth.py` & `cloudspot-license-api-1.4.1/cloudspotlicense/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/cloudspotlicense/models/auth.py` & `cloudspot-license-api-1.4.1/cloudspotlicense/models/auth.py`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/cloudspotlicense/models/base.py` & `cloudspot-license-api-1.4.1/cloudspotlicense/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,21 @@
     def __init__(self):
 
         self.has_error = False
         self.error = None
 
     def parse(self, json):
         for key, value in json.items():
-            attrVal = getattr(self, key)
+            attr_val = getattr(self, key, None)
 
-            if isinstance(attrVal, BaseModel):
-                setattr(self, key, attrVal.parse(value))
-            else:
-                setattr(self, key, value)
+            if attr_val:
+                if isinstance(attr_val, BaseModel):
+                    setattr(self, key, attr_val.parse(value))
+                else:
+                    setattr(self, key, value)
 
         return self
     
     def get_json(self):
 
         dikt = {}
         for k, v in self.__dict__.items():
```

### Comparing `cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/PKG-INFO` & `cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudspot-license-api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Wrapper for the Cloudspot License API endpoints
 Home-page: https://github.com/Ecosy-EU/cloudspot-license-api
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.1.tar.gz
 Keywords: cloudspot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cloudspot-license-api-1.4.0/cloudspot_license_api.egg-info/SOURCES.txt` & `cloudspot-license-api-1.4.1/cloudspot_license_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/LICENSE.txt` & `cloudspot-license-api-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/PKG-INFO` & `cloudspot-license-api-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudspot-license-api
-Version: 1.4.0
+Version: 1.4.1
 Summary: Wrapper for the Cloudspot License API endpoints
 Home-page: https://github.com/Ecosy-EU/cloudspot-license-api
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.1.tar.gz
 Keywords: cloudspot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cloudspot-license-api-1.4.0/README.md` & `cloudspot-license-api-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudspot-license-api-1.4.0/setup.py` & `cloudspot-license-api-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'cloudspot-license-api',         
   packages=['cloudspotlicense', 'cloudspotlicense.models', 'cloudspotlicense.constants', 'cloudspotlicense.endpoints'],
-  version = '1.4.0',
+  version = '1.4.1',
   license='GPL-3.0-or-later',
   description = 'Wrapper for the Cloudspot License API endpoints',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/cloudspot-license-api',
-  download_url = 'https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/cloudspot-license-api/archive/refs/tags/1.4.1.tar.gz',
   keywords = ['cloudspot'],
   install_requires=[
           'requests',
           'python-dateutil',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

