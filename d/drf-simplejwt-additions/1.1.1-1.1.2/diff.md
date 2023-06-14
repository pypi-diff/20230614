# Comparing `tmp/drf-simplejwt-additions-1.1.1.tar.gz` & `tmp/drf-simplejwt-additions-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-simplejwt-additions-1.1.1.tar", last modified: Wed Jun 14 07:23:16 2023, max compression
+gzip compressed data, was "drf-simplejwt-additions-1.1.2.tar", last modified: Wed Jun 14 07:33:33 2023, max compression
```

## Comparing `drf-simplejwt-additions-1.1.1.tar` & `drf-simplejwt-additions-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:23:16.026555 drf-simplejwt-additions-1.1.1/
--rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.1/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:23:16.026670 drf-simplejwt-additions-1.1.1/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     2601 2023-06-14 07:17:24.000000 drf-simplejwt-additions-1.1.1/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:23:16.005744 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1459 2023-06-14 06:59:58.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/middleware.py
--rw-r--r--   0 rustam     (501) staff       (20)      526 2023-06-14 07:23:05.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/serializers.py
--rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/views.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:23:16.026304 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:23:15.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      420 2023-06-14 07:23:16.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-14 07:23:15.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-14 07:23:15.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-14 07:23:15.000000 drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-14 07:23:16.027200 drf-simplejwt-additions-1.1.1/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.1/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.109520 drf-simplejwt-additions-1.1.2/
+-rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.2/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:33:33.109635 drf-simplejwt-additions-1.1.2/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     2601 2023-06-14 07:17:24.000000 drf-simplejwt-additions-1.1.2/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.107266 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-14 05:29:58.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1459 2023-06-14 06:59:58.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/middleware.py
+-rw-r--r--   0 rustam     (501) staff       (20)      552 2023-06-14 07:33:25.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/serializers.py
+-rw-r--r--   0 rustam     (501) staff       (20)      272 2023-06-14 05:37:54.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/views.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-14 07:33:33.109109 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     3716 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      420 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       62 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       24 2023-06-14 07:33:33.000000 drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1079 2023-06-14 07:33:33.110301 drf-simplejwt-additions-1.1.2/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2023-06-14 05:28:46.000000 drf-simplejwt-additions-1.1.2/setup.py
```

### Comparing `drf-simplejwt-additions-1.1.1/PKG-INFO` & `drf-simplejwt-additions-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-simplejwt-additions
-Version: 1.1.1
+Version: 1.1.2
 Summary: Additions for Django Rest Framework Simple JWT
 Home-page: https://github.com/AllYouZombies/drf-simplejwt-additions
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-simplejwt-additions-1.1.1/README.md` & `drf-simplejwt-additions-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/middleware.py` & `drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/middleware.py`

 * *Files identical despite different names*

### Comparing `drf-simplejwt-additions-1.1.1/drf_simplejwt_additions/serializers.py` & `drf-simplejwt-additions-1.1.2/drf_simplejwt_additions/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 
 
 class TokenObtainPairWithFullUserSerializer(TokenObtainPairSerializer):
     @classmethod
     def get_token(cls, user):
         token = super().get_token(user)
         user_data = {}
-        fields = (i.name for i in User._meta.fields)
+        fields = (i.name for i in User._meta.fields if i.name != 'last_login')
         for field in fields:
             user_data[field] = str(getattr(user, field))
         token['user'] = user_data
         return token
```

### Comparing `drf-simplejwt-additions-1.1.1/drf_simplejwt_additions.egg-info/PKG-INFO` & `drf-simplejwt-additions-1.1.2/drf_simplejwt_additions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-simplejwt-additions
-Version: 1.1.1
+Version: 1.1.2
 Summary: Additions for Django Rest Framework Simple JWT
 Home-page: https://github.com/AllYouZombies/drf-simplejwt-additions
 Author: Astafeev Rustam
 Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `drf-simplejwt-additions-1.1.1/setup.cfg` & `drf-simplejwt-additions-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-simplejwt-additions
-version = 1.1.1
+version = 1.1.2
 description = Additions for Django Rest Framework Simple JWT
 url = https://github.com/AllYouZombies/drf-simplejwt-additions
 author = Astafeev Rustam
 author_email = rustam@astafeev.dev
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
```

