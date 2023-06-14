# Comparing `tmp/django-webpack-loader-2.0.0.tar.gz` & `tmp/django-webpack-loader-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webpack-loader-2.0.0.tar", last modified: Mon May 22 12:26:10 2023, max compression
+gzip compressed data, was "django-webpack-loader-2.0.1.tar", last modified: Wed Jun 14 12:12:58 2023, max compression
```

## Comparing `django-webpack-loader-2.0.0.tar` & `django-webpack-loader-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/
--rw-r--r--   0 renato    (1000) renato    (1000)     1078 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/LICENSE
--rw-r--r--   0 renato    (1000) renato    (1000)       34 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/MANIFEST.in
--rw-r--r--   0 renato    (1000) renato    (1000)    24842 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/PKG-INFO
--rw-r--r--   0 renato    (1000) renato    (1000)    20129 2023-05-22 12:03:11.000000 django-webpack-loader-2.0.0/README.md
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/
--rw-r--r--   0 renato    (1000) renato    (1000)    24842 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/PKG-INFO
--rw-r--r--   0 renato    (1000) renato    (1000)      589 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/SOURCES.txt
--rw-r--r--   0 renato    (1000) renato    (1000)        1 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/dependency_links.txt
--rw-r--r--   0 renato    (1000) renato    (1000)       66 2023-05-22 12:26:10.000000 django-webpack-loader-2.0.0/django_webpack_loader.egg-info/top_level.txt
--rw-r--r--   0 renato    (1000) renato    (1000)       80 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/setup.cfg
--rw-r--r--   0 renato    (1000) renato    (1000)     1731 2022-12-09 12:03:45.000000 django-webpack-loader-2.0.0/setup.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/
--rw-r--r--   0 renato    (1000) renato    (1000)      179 2023-05-22 12:03:11.000000 django-webpack-loader-2.0.0/webpack_loader/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)      744 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/apps.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1016 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/config.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/contrib/
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/contrib/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)      481 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/contrib/jinja2ext.py
--rw-r--r--   0 renato    (1000) renato    (1000)      251 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/errors.py
--rw-r--r--   0 renato    (1000) renato    (1000)      700 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/exceptions.py
--rw-r--r--   0 renato    (1000) renato    (1000)     5207 2023-05-19 19:41:04.000000 django-webpack-loader-2.0.0/webpack_loader/loader.py
--rw-r--r--   0 renato    (1000) renato    (1000)       31 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/signals.py
-drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-05-22 12:26:10.895145 django-webpack-loader-2.0.0/webpack_loader/templatetags/
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/templatetags/__init__.py
--rw-r--r--   0 renato    (1000) renato    (1000)     2141 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/templatetags/webpack_loader.py
--rw-r--r--   0 renato    (1000) renato    (1000)     3840 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.0/webpack_loader/utils.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/
+-rw-r--r--   0 renato    (1000) renato    (1000)     1078 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/LICENSE
+-rw-r--r--   0 renato    (1000) renato    (1000)       34 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/MANIFEST.in
+-rw-r--r--   0 renato    (1000) renato    (1000)    24881 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/PKG-INFO
+-rw-r--r--   0 renato    (1000) renato    (1000)    20129 2023-05-22 12:03:11.000000 django-webpack-loader-2.0.1/README.md
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/django_webpack_loader.egg-info/
+-rw-r--r--   0 renato    (1000) renato    (1000)    24881 2023-06-14 12:12:58.000000 django-webpack-loader-2.0.1/django_webpack_loader.egg-info/PKG-INFO
+-rw-r--r--   0 renato    (1000) renato    (1000)      589 2023-06-14 12:12:58.000000 django-webpack-loader-2.0.1/django_webpack_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)        1 2023-06-14 12:12:58.000000 django-webpack-loader-2.0.1/django_webpack_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)       66 2023-06-14 12:12:58.000000 django-webpack-loader-2.0.1/django_webpack_loader.egg-info/top_level.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)       80 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/setup.cfg
+-rw-r--r--   0 renato    (1000) renato    (1000)     1765 2023-06-14 12:02:46.000000 django-webpack-loader-2.0.1/setup.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/webpack_loader/
+-rw-r--r--   0 renato    (1000) renato    (1000)      179 2023-06-14 12:08:36.000000 django-webpack-loader-2.0.1/webpack_loader/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      744 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/apps.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1016 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/config.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/webpack_loader/contrib/
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/contrib/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      481 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/contrib/jinja2ext.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      251 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/errors.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      700 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/exceptions.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     5207 2023-05-19 19:41:04.000000 django-webpack-loader-2.0.1/webpack_loader/loader.py
+-rw-r--r--   0 renato    (1000) renato    (1000)       31 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/signals.py
+drwxr-xr-x   0 renato    (1000) renato    (1000)        0 2023-06-14 12:12:58.216772 django-webpack-loader-2.0.1/webpack_loader/templatetags/
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/templatetags/__init__.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     2141 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/templatetags/webpack_loader.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     3840 2022-06-20 14:57:36.000000 django-webpack-loader-2.0.1/webpack_loader/utils.py
```

### Comparing `django-webpack-loader-2.0.0/LICENSE` & `django-webpack-loader-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/PKG-INFO` & `django-webpack-loader-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-webpack-loader
-Version: 2.0.0
+Version: 2.0.1
 Summary: Transparently use webpack with django
 Home-page: https://github.com/django-webpack/django-webpack-loader
 Author: Owais Lone
 Author-email: hello@owaislone.org
 License: UNKNOWN
-Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.0
+Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.1
 Description: # django-webpack-loader
         
         [![Build Status](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master.svg?style=svg)](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master)
         [![Coverage Status](https://coveralls.io/repos/github/django-webpack/django-webpack-loader/badge.svg?branch=master)](https://coveralls.io/github/django-webpack/django-webpack-loader?branch=master)
         ![pyversions](https://img.shields.io/pypi/pyversions/django-webpack-loader)
         ![djversions](https://img.shields.io/pypi/djversions/django-webpack-loader)
         
@@ -464,10 +464,11 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `django-webpack-loader-2.0.0/README.md` & `django-webpack-loader-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/django_webpack_loader.egg-info/PKG-INFO` & `django-webpack-loader-2.0.1/django_webpack_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-webpack-loader
-Version: 2.0.0
+Version: 2.0.1
 Summary: Transparently use webpack with django
 Home-page: https://github.com/django-webpack/django-webpack-loader
 Author: Owais Lone
 Author-email: hello@owaislone.org
 License: UNKNOWN
-Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.0
+Download-URL: https://github.com/django-webpack/django-webpack-loader/tarball/2.0.1
 Description: # django-webpack-loader
         
         [![Build Status](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master.svg?style=svg)](https://circleci.com/gh/django-webpack/django-webpack-loader/tree/master)
         [![Coverage Status](https://coveralls.io/repos/github/django-webpack/django-webpack-loader/badge.svg?branch=master)](https://coveralls.io/github/django-webpack/django-webpack-loader?branch=master)
         ![pyversions](https://img.shields.io/pypi/pyversions/django-webpack-loader)
         ![djversions](https://img.shields.io/pypi/djversions/django-webpack-loader)
         
@@ -464,10 +464,11 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `django-webpack-loader-2.0.0/django_webpack_loader.egg-info/SOURCES.txt` & `django-webpack-loader-2.0.1/django_webpack_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/setup.py` & `django-webpack-loader-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,11 +41,12 @@
     'Framework :: Django :: 2.1',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Environment :: Web Environment',
     'License :: OSI Approved :: MIT License',
   ],
 )
```

### Comparing `django-webpack-loader-2.0.0/webpack_loader/apps.py` & `django-webpack-loader-2.0.1/webpack_loader/apps.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/webpack_loader/config.py` & `django-webpack-loader-2.0.1/webpack_loader/config.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/webpack_loader/exceptions.py` & `django-webpack-loader-2.0.1/webpack_loader/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/webpack_loader/loader.py` & `django-webpack-loader-2.0.1/webpack_loader/loader.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/webpack_loader/templatetags/webpack_loader.py` & `django-webpack-loader-2.0.1/webpack_loader/templatetags/webpack_loader.py`

 * *Files identical despite different names*

### Comparing `django-webpack-loader-2.0.0/webpack_loader/utils.py` & `django-webpack-loader-2.0.1/webpack_loader/utils.py`

 * *Files identical despite different names*

