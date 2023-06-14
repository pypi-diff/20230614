# Comparing `tmp/wagtail-nav-menus-3.9.0.tar.gz` & `tmp/wagtail-nav-menus-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-nav-menus-3.9.0.tar", last modified: Tue Jun 21 20:45:54 2022, max compression
+gzip compressed data, was "wagtail-nav-menus-3.9.2.tar", last modified: Tue Jan 24 19:40:40 2023, max compression
```

## Comparing `wagtail-nav-menus-3.9.0.tar` & `wagtail-nav-menus-3.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.692061 wagtail-nav-menus-3.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3474 2022-06-21 20:45:54.692061 wagtail-nav-menus-3.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2729 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-06-21 20:45:54.693061 wagtail-nav-menus-3.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1613 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.679059 wagtail-nav-menus-3.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.686060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/
--rw-rw-rw-   0 root         (0) root         (0)       55 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/config.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    10772 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/loading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.679059 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.680060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.689060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1600 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.690060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      929 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     4416 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/0002_auto_20190911_1745.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/0003_auto_20191111_1655.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/models.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.681059 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.691060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/
--rw-rw-rw-   0 root         (0) root         (0)      227 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/get_url.html
--rw-rw-rw-   0 root         (0) root         (0)      356 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/menu_link.html
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/nav_category.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.691060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/tags/
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templates/nav_menus/tags/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.692061 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/templatetags/nav_menu_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     9748 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/viewsets.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2022-06-21 20:45:43.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/wagtail_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-21 20:45:54.688060 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3474 2022-06-21 20:45:54.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1252 2022-06-21 20:45:54.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-21 20:45:54.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2022-06-21 20:45:54.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-06-21 20:45:54.000000 wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.206923 wagtail-nav-menus-3.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-01-24 19:40:40.206923 wagtail-nav-menus-3.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-24 19:40:40.206923 wagtail-nav-menus-3.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.194910 wagtail-nav-menus-3.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.200916 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    10752 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/loading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.194910 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.194910 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.202919 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.204921 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)    13217 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/0002_auto_20190911_1745.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/0003_auto_20191111_1655.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.195911 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.205922 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/get_url.html
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/menu_link.html
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/nav_category.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.205922 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/tags/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templates/nav_menus/tags/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.206923 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/templatetags/nav_menu_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)    10439 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/viewsets.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-01-24 19:40:30.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/wagtail_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 19:40:40.202919 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-01-24 19:40:40.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-01-24 19:40:40.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 19:40:40.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-01-24 19:40:40.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-01-24 19:40:40.000000 wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/top_level.txt
```

### Comparing `wagtail-nav-menus-3.9.0/PKG-INFO` & `wagtail-nav-menus-3.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: wagtail-nav-menus
-Version: 3.9.0
+Version: 3.9.2
 Summary: Wagtail Nav Menus is a app to provide highly customizable menus in wagtail by leveraging StreamFields.
 Home-page: https://gitlab.com/thelabnyc/wagtail-nav-menus
 Author: David Burke
 Author-email: david@thelabnyc.com
 License: Apache License
 Keywords: django wagtail
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -105,10 +104,7 @@
 ---------
 
 If using Django Rest Framework to access the menu data, this module provides some tools to get started.
 
 Add NavMenuViewSet to your Rest Framework Router. ::
 
     from wagtail_nav_menus.viewsets import NavMenuViewSet
-
-
-
```

### Comparing `wagtail-nav-menus-3.9.0/README.rst` & `wagtail-nav-menus-3.9.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,7 @@
 ---------
 
 If using Django Rest Framework to access the menu data, this module provides some tools to get started.
 
 Add NavMenuViewSet to your Rest Framework Router. ::
 
     from wagtail_nav_menus.viewsets import NavMenuViewSet
-
```

### Comparing `wagtail-nav-menus-3.9.0/setup.py` & `wagtail-nav-menus-3.9.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages, Distribution
 import codecs
 import os.path
 
 # Make sure versiontag exists before going any further
-Distribution().fetch_build_eggs('versiontag>=1.2.0')
+Distribution().fetch_build_eggs("versiontag>=1.2.0")
 
 from versiontag import get_version, cache_git_tag  # NOQA
 
 
-packages = find_packages('src')
+packages = find_packages("src")
 
 install_requires = [
-    'wagtail>=2.7,<4.0',
+    "wagtail>=2.7,<4.1",
 ]
 extras_require = {
-    'development': [
-        'flake8>=3.3.0',
-        'tox>=2.7.0',
-        'ipdb'
-    ],
+    "development": ["flake8>=3.3.0", "tox>=2.7.0", "ipdb"],
 }
 
 
 def fpath(name):
     return os.path.join(os.path.dirname(__file__), name)
 
 
 def read(fname):
-    return codecs.open(fpath(fname), encoding='utf-8').read()
+    return codecs.open(fpath(fname), encoding="utf-8").read()
 
 
 cache_git_tag()
 
 setup(
     name="wagtail-nav-menus",
     description="Wagtail Nav Menus is a app to provide highly customizable menus in wagtail by leveraging StreamFields.",
     version=get_version(pypi=True),
-    long_description=open('README.rst').read(),
+    long_description=open("README.rst").read(),
     keywords="django wagtail",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Framework :: Wagtail',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Intended Audience :: Developers',
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Framework :: Wagtail",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
     ],
     author="David Burke",
     author_email="david@thelabnyc.com",
     url="https://gitlab.com/thelabnyc/wagtail-nav-menus",
     license="Apache License",
-    package_dir={'': 'src'},
+    package_dir={"": "src"},
     packages=packages,
     include_package_data=True,
     install_requires=install_requires,
     extras_require=extras_require,
 )
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/loading.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pass
 
 
 class ClassNotFoundError(Exception):
     pass
 
 
-def get_class(module_label, classname, module_prefix='oscar.apps'):
+def get_class(module_label, classname, module_prefix="oscar.apps"):
     """
     Dynamically import a single class from the given module.
 
     This is a simple wrapper around `get_classes` for the case of loading a
     single class.
 
     Args:
@@ -36,15 +36,15 @@
 
     Returns:
         The requested class object or `None` if it can't be found
     """
     return get_classes(module_label, [classname], module_prefix)[0]
 
 
-def get_classes(module_label, classnames, module_prefix='oscar.apps'):
+def get_classes(module_label, classnames, module_prefix="oscar.apps"):
     """
     Dynamically import a list of classes from the given module.
 
     This works by looping over ``INSTALLED_APPS`` and looking for a match
     against the passed module label.  If the requested class can't be found in
     the matching module, then we attempt to import it from the corresponding
     core app.
@@ -79,38 +79,37 @@
 
         AppNotFoundError: If no app is found in ``INSTALLED_APPS`` that matches
             the passed module label.
 
         ImportError: If the attempted import of a class raises an
             ``ImportError``, it is re-raised
     """
-    if '.' not in module_label:
+    if "." not in module_label:
         # Importing from top-level modules is not supported, e.g.
         # get_class('shipping', 'Scale'). That should be easy to fix,
         # but @maikhoepfel had a stab and could not get it working reliably.
         # Overridable classes in a __init__.py might not be a good idea anyway.
-        raise ValueError(
-            "Importing from top-level modules is not supported")
+        raise ValueError("Importing from top-level modules is not supported")
 
     # import from Oscar package (should succeed in most cases)
     # e.g. 'oscar.apps.dashboard.catalogue.forms'
     oscar_module_label = "%s.%s" % (module_prefix, module_label)
     oscar_module = _import_module(oscar_module_label, classnames)
 
     # returns e.g. 'oscar.apps.dashboard.catalogue',
     # 'yourproject.apps.dashboard.catalogue' or 'dashboard.catalogue',
     # depending on what is set in INSTALLED_APPS
     installed_apps_entry, app_name = _find_installed_apps_entry(module_label)
-    if installed_apps_entry.startswith('%s.' % module_prefix):
+    if installed_apps_entry.startswith("%s." % module_prefix):
         # The entry is obviously an Oscar one, we don't import again
         local_module = None
     else:
         # Attempt to import the classes from the local module
         # e.g. 'yourproject.dashboard.catalogue.forms'
-        sub_module = module_label.replace(app_name, '', 1)
+        sub_module = module_label.replace(app_name, "", 1)
         local_module_label = installed_apps_entry + sub_module
         local_module = _import_module(local_module_label, classnames)
 
     if oscar_module is local_module is None:
         # This intentionally doesn't raise an ImportError, because ImportError
         # can get masked in complex circular import scenarios.
         raise ModuleNotFoundError(
@@ -160,79 +159,78 @@
         klass = None
         for module in modules:
             if hasattr(module, classname):
                 klass = getattr(module, classname)
                 break
         if not klass:
             packages = [m.__name__ for m in modules if m is not None]
-            raise ClassNotFoundError("No class '%s' found in %s" % (
-                classname, ", ".join(packages)))
+            raise ClassNotFoundError(
+                "No class '%s' found in %s" % (classname, ", ".join(packages))
+            )
         klasses.append(klass)
     return klasses
 
 
 def _get_installed_apps_entry(app_name):
     """
     Given an app name (e.g. 'catalogue'), walk through INSTALLED_APPS
     and return the first match, or None.
     This does depend on the order of INSTALLED_APPS and will break if
     e.g. 'dashboard.catalogue' comes before 'catalogue' in INSTALLED_APPS.
     """
     for installed_app in settings.INSTALLED_APPS:
         # match root-level apps ('catalogue') or apps with same name at end
         # ('shop.catalogue'), but don't match 'fancy_catalogue'
-        if installed_app == app_name or installed_app.endswith('.' + app_name):
+        if installed_app == app_name or installed_app.endswith("." + app_name):
             return installed_app
     return None
 
 
 def _find_installed_apps_entry(module_label):
     """
     Given a module label, finds the best matching INSTALLED_APPS entry.
 
     This is made trickier by the fact that we don't know what part of the
     module_label is part of the INSTALLED_APPS entry. So we try all possible
     combinations, trying the longer versions first. E.g. for
     'dashboard.catalogue.forms', 'dashboard.catalogue' is attempted before
     'dashboard'
     """
-    modules = module_label.split('.')
+    modules = module_label.split(".")
     # if module_label is 'dashboard.catalogue.forms.widgets', combinations
     # will be ['dashboard.catalogue.forms', 'dashboard.catalogue', 'dashboard']
-    combinations = [
-        '.'.join(modules[:-count]) for count in range(1, len(modules))]
+    combinations = [".".join(modules[:-count]) for count in range(1, len(modules))]
     for app_name in combinations:
         entry = _get_installed_apps_entry(app_name)
         if entry:
             return entry, app_name
-    raise AppNotFoundError(
-        "Couldn't find an app to import %s from" % module_label)
+    raise AppNotFoundError("Couldn't find an app to import %s from" % module_label)
 
 
 def get_profile_class():
     """
     Return the profile model class
     """
     # The AUTH_PROFILE_MODULE setting was deprecated in Django 1.5, but it
     # makes sense for Oscar to continue to use it. Projects built on Django
     # 1.4 are likely to have used a profile class and it's very difficult to
     # upgrade to a single user model. Hence, we should continue to support
     # having a separate profile class even if Django doesn't.
-    setting = getattr(settings, 'AUTH_PROFILE_MODULE', None)
+    setting = getattr(settings, "AUTH_PROFILE_MODULE", None)
     if setting is None:
         return None
-    app_label, model_name = settings.AUTH_PROFILE_MODULE.split('.')
+    app_label, model_name = settings.AUTH_PROFILE_MODULE.split(".")
     return get_model(app_label, model_name)
 
 
 def feature_hidden(feature_name):
     """
     Test if a certain Oscar feature is disabled.
     """
-    return (feature_name is not None and feature_name in settings.OSCAR_HIDDEN_FEATURES)
+    return feature_name is not None and feature_name in settings.OSCAR_HIDDEN_FEATURES
 
 
 def get_model(app_label, model_name):
     """
     Fetches a Django model using the app registry.
 
     This doesn't require that an app with the given app label exists,
@@ -250,15 +248,15 @@
             # target model has been imported and try looking the model up
             # in the app registry. This effectively emulates
             # `from path.to.app.models import Model` where we use
             # `Model = get_model('app', 'Model')` instead.
             app_config = apps.get_app_config(app_label)
             # `app_config.import_models()` cannot be used here because it
             # would interfere with `apps.populate()`.
-            import_module('%s.%s' % (app_config.name, MODELS_MODULE_NAME))
+            import_module("%s.%s" % (app_config.name, MODELS_MODULE_NAME))
             # In order to account for case-insensitivity of model_name,
             # look up the model through a private API of the app registry.
             return apps.get_registered_model(app_label, model_name)
         else:
             # This must be a different case (e.g. the model really doesn't
             # exist). We just re-raise the exception.
             raise
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.po` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/locale/es/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -4,60 +4,60 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-03-18 18:05+0000\n"
+"POT-Creation-Date: 2022-09-15 19:05+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. Translators: Backend Library Name
-#: wagtail_nav_menus/config.py:8
+#: wagtail_nav_menus/apps.py:8
 msgid "Wagtail Navigation Menus"
 msgstr ""
 
 #. Translators: Navigation Menu Item Type
-#: wagtail_nav_menus/models.py:40
+#: wagtail_nav_menus/models.py:46
 msgid "Internal Page Block"
 msgstr ""
 
 #. Translators: Navigation Menu Item Type
-#: wagtail_nav_menus/models.py:55
+#: wagtail_nav_menus/models.py:61
 msgid "External Page Block"
 msgstr ""
 
 #. Translators: Navigation Menu Item Type
-#: wagtail_nav_menus/models.py:65
+#: wagtail_nav_menus/models.py:71
 msgid "Django URL Block"
 msgstr ""
 
 #. Translators: Navigation Menu Item Type
-#: wagtail_nav_menus/models.py:87
+#: wagtail_nav_menus/models.py:93
 msgid "Relative URL Block"
 msgstr ""
 
 #. Translators: Content Block Name
 #: wagtail_nav_menus/models.py:123
 msgid "Navigation Menu Category Block"
 msgstr ""
 
 #. Translators: Model Name (singular)
-#: wagtail_nav_menus/models.py:160
+#: wagtail_nav_menus/models.py:163
 msgid "Navigation Menu"
 msgstr ""
 
 #. Translators: Model Name (plural)
-#: wagtail_nav_menus/models.py:162
+#: wagtail_nav_menus/models.py:165
 msgid "Navigation Menus"
 msgstr ""
 
-#: wagtail_nav_menus/wagtail_hooks.py:9
+#: wagtail_nav_menus/wagtail_hooks.py:8
 msgid "Nav Menu"
 msgstr ""
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/0001_initial.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/0001_initial.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,20 +8,46 @@
 import wagtail.images.blocks
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='NavMenu',
+            name="NavMenu",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(choices=[('top', 'Top'), ('footer', 'Footer')], max_length=50, unique=True)),
-                ('menu', wagtail.core.fields.StreamField((('heading', wagtail.core.blocks.CharBlock(classname='full title')), ('paragraph', wagtail.core.blocks.RichTextBlock()), ('image', wagtail.images.blocks.ImageChooserBlock())))),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        choices=[("top", "Top"), ("footer", "Footer")],
+                        max_length=50,
+                        unique=True,
+                    ),
+                ),
+                (
+                    "menu",
+                    wagtail.core.fields.StreamField(
+                        (
+                            (
+                                "heading",
+                                wagtail.core.blocks.CharBlock(classname="full title"),
+                            ),
+                            ("paragraph", wagtail.core.blocks.RichTextBlock()),
+                            ("image", wagtail.images.blocks.ImageChooserBlock()),
+                        )
+                    ),
+                ),
             ],
         ),
     ]
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/migrations/0003_auto_20191111_1655.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/migrations/0003_auto_20191111_1655.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 import django.db.models.deletion
 import wagtail_nav_menus.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('wagtail_nav_menus', '0002_auto_20190911_1745'),
+        ("wagtail_nav_menus", "0002_auto_20190911_1745"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='navmenu',
-            name='site',
-            field=models.ForeignKey(default=wagtail_nav_menus.models.site_default_id, on_delete=django.db.models.deletion.CASCADE, to='wagtailcore.Site'),
+            model_name="navmenu",
+            name="site",
+            field=models.ForeignKey(
+                default=wagtail_nav_menus.models.site_default_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="wagtailcore.Site",
+            ),
         ),
     ]
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/models.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,206 @@
 import json
 from django.db import models
 from django.conf import settings
 from django.urls import reverse
 from django.urls import NoReverseMatch
 from django.utils.translation import gettext_lazy as _
+from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.core.fields import StreamField
 from wagtail.core import blocks
 from wagtail.core.models import Site
-from wagtail.admin.edit_handlers import FieldPanel, StreamFieldPanel
+from wagtail.admin.edit_handlers import FieldPanel
 from .loading import get_class
 from .utils import date_handler
 from .defaults import (
     WAGTAIL_NAV_MENU_TYPES_DEFAULT,
     WAGTAIL_NAV_MENU_CHOICES_DEFAULT,
 )
 
+# See "Removal of special-purpose field panel types"
+# https://docs.wagtail.org/en/stable/releases/3.0.html#removal-of-special-purpose-field-panel-types
+if WAGTAIL_VERSION[0] >= 3:
+    from wagtail.admin.panels import FieldPanel as StreamFieldPanel  # NOQA
+else:
+    from wagtail.admin.edit_handlers import StreamFieldPanel  # NOQA
+
 
 NAV_MENU_CHOICES = getattr(
-    settings,
-    'WAGTAIL_NAV_MENU_CHOICES',
-    WAGTAIL_NAV_MENU_CHOICES_DEFAULT
+    settings, "WAGTAIL_NAV_MENU_CHOICES", WAGTAIL_NAV_MENU_CHOICES_DEFAULT
 )
 
 
 class AbstractPageBlock(blocks.StructBlock):
     override_title = blocks.CharBlock(required=False)
     open_in_new_tab = blocks.BooleanBlock(required=False)
 
     class Meta:
-        icon = 'link'
-        template = 'nav_menus/menu_link.html'
+        icon = "link"
+        template = "nav_menus/menu_link.html"
 
 
 class InternalPageBlock(AbstractPageBlock):
     page = blocks.PageChooserBlock()
 
     class Meta:
         # Translators: Navigation Menu Item Type
-        verbose_name = _('Internal Page Block')
+        verbose_name = _("Internal Page Block")
 
     def get_serializable_data(self, obj):
-        page = obj['page']
+        page = obj["page"]
         result = obj
-        result['page'] = page.serializable_data()
-        result['page']['url'] = page.url
+        result["page"] = page.serializable_data()
+        result["page"]["url"] = page.url
         return result
 
 
 class ExternalPageBlock(AbstractPageBlock):
     link = blocks.URLBlock()
 
     class Meta:
         # Translators: Navigation Menu Item Type
-        verbose_name = _('External Page Block')
+        verbose_name = _("External Page Block")
 
 
 class DjangoURLBlock(AbstractPageBlock):
-    """ A link that is generated from a Django reverse URL lookup
-    """
+    """A link that is generated from a Django reverse URL lookup"""
+
     url_name = blocks.CharBlock()
 
     class Meta:
         # Translators: Navigation Menu Item Type
-        verbose_name = _('Django URL Block')
+        verbose_name = _("Django URL Block")
 
     def get_serializable_data(self, obj):
-        url_name = obj['url_name']
+        url_name = obj["url_name"]
         result = obj
         try:
-            result['url'] = reverse(url_name)
+            result["url"] = reverse(url_name)
         except NoReverseMatch:
-            result['url'] = "Not Found"
+            result["url"] = "Not Found"
         return result
 
 
-URL_REGEX = r'^(?!www\.|(?:http|ftp)s?://|[A-Za-z]:\\|//).*'
+URL_REGEX = r"^(?!www\.|(?:http|ftp)s?://|[A-Za-z]:\\|//).*"
 
 
 class RelativeURLBlock(AbstractPageBlock):
-    link = blocks.RegexBlock(regex=URL_REGEX, error_mesage={
-        'invalid': "Not a relative URL"
-    })
+    link = blocks.RegexBlock(
+        regex=URL_REGEX, error_mesage={"invalid": "Not a relative URL"}
+    )
 
     class Meta:
         # Translators: Navigation Menu Item Type
-        verbose_name = _('Relative URL Block')
+        verbose_name = _("Relative URL Block")
 
 
 NAV_MENU_TYPES = getattr(
-    settings,
-    'WAGTAIL_NAV_MENU_TYPES',
-    WAGTAIL_NAV_MENU_TYPES_DEFAULT
+    settings, "WAGTAIL_NAV_MENU_TYPES", WAGTAIL_NAV_MENU_TYPES_DEFAULT
 )
 
 nav_content = []
 for name, module_label, class_name in NAV_MENU_TYPES:
     nav_content.append(
         (name, get_class(module_label, class_name)()),
     )
 
 
-NAV_CATEGORY_TYPES = getattr(
-    settings,
-    'WAGTAIL_NAV_MENU_CATEGORY_TYPES',
-    []
-)
+NAV_CATEGORY_TYPES = getattr(settings, "WAGTAIL_NAV_MENU_CATEGORY_TYPES", [])
 custom_category_content = []
 for name, module_label, class_name in NAV_CATEGORY_TYPES:
     custom_category_content.append(
         (name, get_class(module_label, class_name)()),
     )
 
 
 class NavCategoryBlock(blocks.StructBlock):
     title = blocks.CharBlock()
     sub_nav = blocks.StreamBlock(nav_content + custom_category_content)
 
     class Meta:
-        icon = 'list-ul'
-        template = 'nav_menus/nav_category.html'
+        icon = "list-ul"
+        template = "nav_menus/nav_category.html"
         # Translators: Content Block Name
-        verbose_name = _('Navigation Menu Category Block')
+        verbose_name = _("Navigation Menu Category Block")
 
 
 def site_default():
     return Site.objects.filter(is_default_site=True).first()
 
 
 def site_default_id():
-    """ Not sure why this is needed for migrations, there is probably a better way. """
+    """Not sure why this is needed for migrations, there is probably a better way."""
     site = site_default()
     if site:
         return site.id
 
 
 class AbstractNavMenu(models.Model):
     site = models.ForeignKey(
-        'wagtailcore.Site',
+        "wagtailcore.Site",
         db_index=True,
         on_delete=models.CASCADE,
-        default=site_default_id
+        default=site_default_id,
     )
     name = models.CharField(
         max_length=50,
         choices=NAV_MENU_CHOICES,
     )
-    menu = StreamField([
-        ('nav_category', NavCategoryBlock()),
-    ] + nav_content)
+    menu = StreamField(
+        [
+            ("nav_category", NavCategoryBlock()),
+        ]
+        + nav_content
+    )
 
     panels = [
-        FieldPanel('site'),
-        FieldPanel('name'),
-        StreamFieldPanel('menu'),
+        FieldPanel("site"),
+        FieldPanel("name"),
+        StreamFieldPanel("menu"),
     ]
 
     class Meta:
         # Translators: Model Name (singular)
-        verbose_name = _('Navigation Menu')
+        verbose_name = _("Navigation Menu")
         # Translators: Model Name (plural)
-        verbose_name_plural = _('Navigation Menus')
-        unique_together = ('site', 'name',)
+        verbose_name_plural = _("Navigation Menus")
+        unique_together = (
+            "site",
+            "name",
+        )
         abstract = True
-        app_label = 'wagtail_nav_menus'
+        app_label = "wagtail_nav_menus"
 
     def __str__(self):
         return self.name
 
     def stream_field_to_json(self, stream_field):
-        """ Recursive function to turn the menu stream field into json """
+        """Recursive function to turn the menu stream field into json"""
         row = {}
-        row['type'] = stream_field.block_type
-        if hasattr(stream_field.block, 'get_serializable_data'):
-            row['value'] = stream_field.block.get_serializable_data(
-                stream_field.value)
+        row["type"] = stream_field.block_type
+        if hasattr(stream_field.block, "get_serializable_data"):
+            row["value"] = stream_field.block.get_serializable_data(stream_field.value)
         else:
-            row['value'] = stream_field.value
-        if row['type'] == "image" and row['value']:
-            image = row['value']
-            row['value'] = {
+            row["value"] = stream_field.value
+        if row["type"] == "image" and row["value"]:
+            image = row["value"]
+            row["value"] = {
                 "id": image.pk,
                 "title": image.title,
                 "url": image.file.url,
             }
-        elif row['type'] == "nav_category":
+        elif row["type"] == "nav_category":
             sub_nav = []
-            for sub_stream_field in stream_field.value['sub_nav']:
+            for sub_stream_field in stream_field.value["sub_nav"]:
                 sub_nav.append(self.stream_field_to_json(sub_stream_field))
-            row['value']['sub_nav'] = sub_nav
+            row["value"]["sub_nav"] = sub_nav
         return row
 
     def to_json(self):
-        """ JSON representation of menu stream field """
+        """JSON representation of menu stream field"""
         result = []
         for stream_field in self.menu:
             result.append(self.stream_field_to_json(stream_field))
         return json.dumps(result, default=date_handler)
 
 
 class NavMenu(AbstractNavMenu):
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/tests.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,238 +6,265 @@
 import json
 import wagtail
 
 
 class NavMenuTestCase(TestCase):
     def setUp(self):
         self.json_menu = [
-            {'type': 'external_link', 'value': {'open_in_new_tab': True,
-                                                'link': 'http://www.google.com', 'override_title': 'TITLE'}},
-            {'type': 'page_link', 'value': {
-                'open_in_new_tab': False, 'page': 2, 'override_title': ''}},
-            {'type': 'image', 'value': 1},
-            {'type': 'html', 'value': '<div> html is here </div>'},
-            {'type': 'nav_category', 'value': {'title': 'a nav cat', 'sub_nav': [
-                {'type': 'page_link', 'value': {
-                    'open_in_new_tab': False, 'page': 1, 'override_title': ''}},
-            ]}},
+            {
+                "type": "external_link",
+                "value": {
+                    "open_in_new_tab": True,
+                    "link": "http://www.google.com",
+                    "override_title": "TITLE",
+                },
+            },
+            {
+                "type": "page_link",
+                "value": {"open_in_new_tab": False, "page": 2, "override_title": ""},
+            },
+            {"type": "image", "value": 1},
+            {"type": "html", "value": "<div> html is here </div>"},
+            {
+                "type": "nav_category",
+                "value": {
+                    "title": "a nav cat",
+                    "sub_nav": [
+                        {
+                            "type": "page_link",
+                            "value": {
+                                "open_in_new_tab": False,
+                                "page": 1,
+                                "override_title": "",
+                            },
+                        },
+                    ],
+                },
+            },
         ]
         self.maxDiff = None
 
     def json_after_create_menu(self, json_for_create):
-        menu = NavMenu.objects.create(
-            name="top",
-            menu=json.dumps([json_for_create])
-        )
+        menu = NavMenu.objects.create(name="top", menu=json.dumps([json_for_create]))
         output_json = menu.to_json()
         return json.loads(output_json)[0]
 
     def test_external_link(self):
         source = {
-            'type': 'external_link',
-            'value': {
-                'open_in_new_tab': True,
-                'link': 'http://www.google.com',
-                'override_title': 'TITLE'
-            }
+            "type": "external_link",
+            "value": {
+                "open_in_new_tab": True,
+                "link": "http://www.google.com",
+                "override_title": "TITLE",
+            },
         }
         expected = source
         result = self.json_after_create_menu(source)
         self.assertDictEqual(result, expected)
 
     def test_image(self):
-        source = {'type': 'image', 'value': 1}
-        expected = {'type': 'image', 'value': None}
+        source = {"type": "image", "value": 1}
+        expected = {"type": "image", "value": None}
         result = self.json_after_create_menu(source)
         self.assertDictEqual(result, expected)
 
     def test_html(self):
-        source = {'type': 'html', 'value': '<div> html is here </div>'}
-        expected = {'type': 'html', 'value': '<div> html is here </div>'}
+        source = {"type": "html", "value": "<div> html is here </div>"}
+        expected = {"type": "html", "value": "<div> html is here </div>"}
         result = self.json_after_create_menu(source)
         self.assertDictEqual(result, expected)
 
     def test_page_link(self):
         source = {
-            'type': 'page_link',
-            'value': {
-                'open_in_new_tab': False,
-                'page': 2,
-                'override_title': ''
-            }
+            "type": "page_link",
+            "value": {"open_in_new_tab": False, "page": 2, "override_title": ""},
         }
         expected = {
-            'type': 'page_link',
-            'value': {
-                'page': {
-                    'slug': 'home',
-                    'live': True,
-                    'content_type': 1,
-                    'pk': 2,
-                    'first_published_at': None,
-                    'search_description': '',
-                    'numchild': 0,
-                    'latest_revision_created_at': None,
-                    'locked': False,
-                    'expire_at': None,
-                    'url': '/',
-                    'show_in_menus': False,
-                    'title': 'Welcome to your new Wagtail site!',
-                    'seo_title': '',
-                    'url_path': '/home/',
-                    'depth': 2,
-                    'owner': None,
-                    'path': '00010001',
-                    'has_unpublished_changes': False,
-                    'draft_title': 'Welcome to your new Wagtail site!',
-                    'expired': False,
-                    'go_live_at': None,
-                    'last_published_at': None,
-                    'live_revision': None,
+            "type": "page_link",
+            "value": {
+                "page": {
+                    "slug": "home",
+                    "live": True,
+                    "content_type": 1,
+                    "pk": 2,
+                    "first_published_at": None,
+                    "search_description": "",
+                    "numchild": 0,
+                    "latest_revision_created_at": None,
+                    "locked": False,
+                    "expire_at": None,
+                    "url": "/",
+                    "show_in_menus": False,
+                    "title": "Welcome to your new Wagtail site!",
+                    "seo_title": "",
+                    "url_path": "/home/",
+                    "depth": 2,
+                    "owner": None,
+                    "path": "00010001",
+                    "has_unpublished_changes": False,
+                    "draft_title": "Welcome to your new Wagtail site!",
+                    "expired": False,
+                    "go_live_at": None,
+                    "last_published_at": None,
+                    "live_revision": None,
                 },
-                'open_in_new_tab': False,
-                'override_title': ''}
+                "open_in_new_tab": False,
+                "override_title": "",
+            },
         }
         result = self.json_after_create_menu(source)
         self.assertEqual(result["type"], expected["type"])
-        self.assertEqual(result["value"]["open_in_new_tab"], expected["value"]["open_in_new_tab"])
-        self.assertEqual(result["value"]["override_title"], expected["value"]["override_title"])
-        self.assertEqual(result["value"]["page"]["slug"], expected["value"]["page"]["slug"])
+        self.assertEqual(
+            result["value"]["open_in_new_tab"], expected["value"]["open_in_new_tab"]
+        )
+        self.assertEqual(
+            result["value"]["override_title"], expected["value"]["override_title"]
+        )
+        self.assertEqual(
+            result["value"]["page"]["slug"], expected["value"]["page"]["slug"]
+        )
 
     def test_nav_category(self):
         source = {
-            'type': 'nav_category',
-            'value': {
-                'title': 'a nav cat',
-                'sub_nav': [{
-                    'type': 'page_link',
-                    'value': {
-                        'open_in_new_tab': False,
-                        'page': 1,
-                        'override_title': ''
+            "type": "nav_category",
+            "value": {
+                "title": "a nav cat",
+                "sub_nav": [
+                    {
+                        "type": "page_link",
+                        "value": {
+                            "open_in_new_tab": False,
+                            "page": 1,
+                            "override_title": "",
+                        },
                     }
-                }]
-            }
+                ],
+            },
         }
         expected = {
-            'type': 'nav_category',
-            'value': {
-                'title': 'a nav cat',
-                'sub_nav': [{
-                    'type': 'page_link',
-                    'value': {
-                        'page': {
-                            'slug': 'root',
-                            'live': True,
-                            'content_type': 1,
-                            'pk': 1,
-                            'first_published_at': None,
-                            'search_description': '',
-                            'numchild': 1,
-                            'latest_revision_created_at': None,
-                            'locked': False,
-                            'expire_at': None,
-                            'show_in_menus': False,
-                            'title': 'Root',
-                            'seo_title': '',
-                            'url_path': '/',
-                            'depth': 1,
-                            'owner': None,
-                            'path': '0001',
-                            'has_unpublished_changes': False,
-                            'draft_title': 'Root',
-                            'url': None,
-                            'expired': False,
-                            'go_live_at': None,
-                            'last_published_at': None,
-                            'live_revision': None,
+            "type": "nav_category",
+            "value": {
+                "title": "a nav cat",
+                "sub_nav": [
+                    {
+                        "type": "page_link",
+                        "value": {
+                            "page": {
+                                "slug": "root",
+                                "live": True,
+                                "content_type": 1,
+                                "pk": 1,
+                                "first_published_at": None,
+                                "search_description": "",
+                                "numchild": 1,
+                                "latest_revision_created_at": None,
+                                "locked": False,
+                                "expire_at": None,
+                                "show_in_menus": False,
+                                "title": "Root",
+                                "seo_title": "",
+                                "url_path": "/",
+                                "depth": 1,
+                                "owner": None,
+                                "path": "0001",
+                                "has_unpublished_changes": False,
+                                "draft_title": "Root",
+                                "url": None,
+                                "expired": False,
+                                "go_live_at": None,
+                                "last_published_at": None,
+                                "live_revision": None,
+                            },
+                            "open_in_new_tab": False,
+                            "override_title": "",
                         },
-                        'open_in_new_tab': False,
-                        'override_title': ''
                     }
-                }]
-            }
+                ],
+            },
         }
         # Page schema added a few fields in Wagtail 2.8
         if wagtail.VERSION[0] == 2 and wagtail.VERSION[1] >= 8:
-            expected['value']['sub_nav'][0]['value']['page']['locked_at'] = None
-            expected['value']['sub_nav'][0]['value']['page']['locked_by'] = None
+            expected["value"]["sub_nav"][0]["value"]["page"]["locked_at"] = None
+            expected["value"]["sub_nav"][0]["value"]["page"]["locked_by"] = None
         result = self.json_after_create_menu(source)
         self.assertEqual(result["type"], expected["type"])
         self.assertEqual(result["value"]["title"], expected["value"]["title"])
-        self.assertEqual(result["value"]["sub_nav"][0]["type"], expected["value"]["sub_nav"][0]["type"])
+        self.assertEqual(
+            result["value"]["sub_nav"][0]["type"],
+            expected["value"]["sub_nav"][0]["type"],
+        )
         self.assertEqual(
             result["value"]["sub_nav"][0]["value"]["open_in_new_tab"],
-            expected["value"]["sub_nav"][0]["value"]["open_in_new_tab"]
+            expected["value"]["sub_nav"][0]["value"]["open_in_new_tab"],
         )
         self.assertEqual(
             result["value"]["sub_nav"][0]["value"]["page"]["slug"],
-            expected["value"]["sub_nav"][0]["value"]["page"]["slug"]
+            expected["value"]["sub_nav"][0]["value"]["page"]["slug"],
         )
 
     def test_menu_json(self):
-        """ Test serializing and deserializing the menu json """
-        menu = NavMenu.objects.create(
-            name="top",
-            menu=json.dumps(self.json_menu)
-        )
+        """Test serializing and deserializing the menu json"""
+        menu = NavMenu.objects.create(name="top", menu=json.dumps(self.json_menu))
 
         output_json = menu.to_json()
         output = json.loads(output_json)
 
-        self.assertEqual(output[0]['type'], "external_link")
-        self.assertEqual(output[0]['value']['link'], "http://www.google.com")
+        self.assertEqual(output[0]["type"], "external_link")
+        self.assertEqual(output[0]["value"]["link"], "http://www.google.com")
 
     def test_render_menu(self):
         json_menu = json.dumps(self.json_menu)
         NavMenu.objects.create(name="top", menu=json_menu)
         NavMenu.objects.create(name="bottom", menu=json_menu)
-        res = self.client.get('/')
+        res = self.client.get("/")
         self.assertEqual(res.status_code, 200)
 
 
-
 class NavMenuViewSetTestCase(TestCase):
     def test_nav_menu_viewset(self):
         request = APIRequestFactory().get("")
-        nav_detail = NavMenuViewSet.as_view({'get': 'retrieve'})
+        nav_detail = NavMenuViewSet.as_view({"get": "retrieve"})
         nav = NavMenu.objects.create(name="top")
         response = nav_detail(request, pk=nav.pk)
         self.assertContains(response, nav.name)
 
     def test_nav_menu_viewset_site(self):
         """
         Nav API should support Wagtail Sites and return only sites as specific
         """
         page = Page.objects.all().last()
         default_site = Site.objects.all().first()
-        other_site = Site.objects.create(hostname="example.com", port=80, root_page=page)
+        other_site = Site.objects.create(
+            hostname="example.com", port=80, root_page=page
+        )
         rdata = {
-            'SERVER_NAME': other_site.hostname,
+            "SERVER_NAME": other_site.hostname,
         }
         rfactory = APIRequestFactory(**rdata)
         request = rfactory.get("")
-        nav_detail = NavMenuViewSet.as_view({'get': 'list'})
+        nav_detail = NavMenuViewSet.as_view({"get": "list"})
         nav_default_site = NavMenu.objects.create(name="default", site=default_site)
         nav_other_site = NavMenu.objects.create(name="other", site=other_site)
         response = nav_detail(request)
         self.assertContains(response, nav_other_site.name)
         self.assertNotContains(response, nav_default_site.name)
 
     def test_nav_menu_viewset_site_filter(self):
         """
         Nav API should allow site filter override
         """
         page = Page.objects.all().last()
         default_site = Site.objects.all().first()
-        other_site = Site.objects.create(hostname="example.com", port=80, root_page=page)
+        other_site = Site.objects.create(
+            hostname="example.com", port=80, root_page=page
+        )
         rdata = {
-            'SERVER_NAME': other_site.hostname,
+            "SERVER_NAME": other_site.hostname,
         }
         rfactory = APIRequestFactory(**rdata)
         request = rfactory.get("?site=2")
-        nav_detail = NavMenuViewSet.as_view({'get': 'list'})
+        nav_detail = NavMenuViewSet.as_view({"get": "list"})
         nav_default_site = NavMenu.objects.create(name="default", site=default_site)
         nav_other_site = NavMenu.objects.create(name="other", site=other_site)
         response = nav_detail(request)
         self.assertContains(response, nav_other_site.name)
         self.assertNotContains(response, nav_default_site.name)
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus/viewsets.py` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus/viewsets.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class NavMenuViewSet(viewsets.ReadOnlyModelViewSet):
     queryset = NavMenu.objects.all()
     serializer_class = NavMenuSerializer
 
     def get_queryset(self):
-        site_id = self.request.GET.get('site', None)
+        site_id = self.request.GET.get("site", None)
         site = Site.find_for_request(self.request)
         if site_id:
             try:
                 site = Site.objects.get(id=site_id)
             except Site.DoesNotExist:
                 pass
         qs = super().get_queryset()
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/PKG-INFO` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: wagtail-nav-menus
-Version: 3.9.0
+Version: 3.9.2
 Summary: Wagtail Nav Menus is a app to provide highly customizable menus in wagtail by leveraging StreamFields.
 Home-page: https://gitlab.com/thelabnyc/wagtail-nav-menus
 Author: David Burke
 Author-email: david@thelabnyc.com
 License: Apache License
 Keywords: django wagtail
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -105,10 +104,7 @@
 ---------
 
 If using Django Rest Framework to access the menu data, this module provides some tools to get started.
 
 Add NavMenuViewSet to your Rest Framework Router. ::
 
     from wagtail_nav_menus.viewsets import NavMenuViewSet
-
-
-
```

### Comparing `wagtail-nav-menus-3.9.0/src/wagtail_nav_menus.egg-info/SOURCES.txt` & `wagtail-nav-menus-3.9.2/src/wagtail_nav_menus.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/wagtail_nav_menus/__init__.py
-src/wagtail_nav_menus/config.py
+src/wagtail_nav_menus/apps.py
 src/wagtail_nav_menus/defaults.py
 src/wagtail_nav_menus/loading.py
 src/wagtail_nav_menus/models.py
 src/wagtail_nav_menus/serializers.py
 src/wagtail_nav_menus/tests.py
 src/wagtail_nav_menus/utils.py
 src/wagtail_nav_menus/viewsets.py
```

