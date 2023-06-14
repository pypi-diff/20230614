# Comparing `tmp/wagtail-links-2.5.0.tar.gz` & `tmp/wagtail-links-2.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-links-2.5.0.tar", last modified: Wed Jun 14 15:49:46 2023, max compression
+gzip compressed data, was "wagtail-links-2.5.0b1.tar", last modified: Tue Feb 14 21:09:21 2023, max compression
```

## Comparing `wagtail-links-2.5.0.tar` & `wagtail-links-2.5.0b1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.818592 wagtail-links-2.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-14 15:49:46.818592 wagtail-links-2.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-14 15:49:46.818592 wagtail-links-2.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.812592 wagtail-links-2.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.814592 wagtail-links-2.5.0/src/wagtail_links/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.812592 wagtail-links-2.5.0/src/wagtail_links/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.812592 wagtail-links-2.5.0/src/wagtail_links/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.816592 wagtail-links-2.5.0/src/wagtail_links/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     2630 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.817592 wagtail-links-2.5.0/src/wagtail_links/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py
--rw-rw-rw-   0 root         (0) root         (0)     2236 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.817592 wagtail-links-2.5.0/src/wagtail_links/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/templatetags/wagtail_links.py
--rw-rw-rw-   0 root         (0) root         (0)     3903 2023-06-14 15:49:37.000000 wagtail-links-2.5.0/src/wagtail_links/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:49:46.815592 wagtail-links-2.5.0/src/wagtail_links.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-06-14 15:49:46.000000 wagtail-links-2.5.0/src/wagtail_links.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-14 15:49:46.000000 wagtail-links-2.5.0/src/wagtail_links.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 15:49:46.000000 wagtail-links-2.5.0/src/wagtail_links.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-14 15:49:46.000000 wagtail-links-2.5.0/src/wagtail_links.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 15:49:46.000000 wagtail-links-2.5.0/src/wagtail_links.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.652846 wagtail-links-2.5.0b1/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-02-14 21:09:21.652846 wagtail-links-2.5.0b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-02-14 21:09:21.653847 wagtail-links-2.5.0b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.643836 wagtail-links-2.5.0b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.647840 wagtail-links-2.5.0b1/src/wagtail_links/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.643836 wagtail-links-2.5.0b1/src/wagtail_links/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.644837 wagtail-links-2.5.0b1/src/wagtail_links/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.650843 wagtail-links-2.5.0b1/src/wagtail_links/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.652846 wagtail-links-2.5.0b1/src/wagtail_links/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0002_auto_20170522_1552.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0003_auto_20170522_2015.py
+-rw-rw-rw-   0 root         (0) root         (0)     2236 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0004_auto_20190411_2102.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0006_auto_20200101_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/0007_auto_20200101_1658.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4938 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.652846 wagtail-links-2.5.0b1/src/wagtail_links/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/templatetags/wagtail_links.py
+-rw-rw-rw-   0 root         (0) root         (0)     3903 2023-02-14 21:09:10.000000 wagtail-links-2.5.0b1/src/wagtail_links/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 21:09:21.649842 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-02-14 21:09:21.000000 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-02-14 21:09:21.000000 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 21:09:21.000000 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-02-14 21:09:21.000000 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-14 21:09:21.000000 wagtail-links-2.5.0b1/src/wagtail_links.egg-info/top_level.txt
```

### Comparing `wagtail-links-2.5.0/PKG-INFO` & `wagtail-links-2.5.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: wagtail-links
-Version: 2.5.0
+Version: 2.5.0b1
 Summary: Wagtail links provides a consistent way to refer to links in a wagtail page.
 Home-page: https://gitlab.com/thelabnyc/wagtail-links
-Author: thelabnyc
-Author-email: thelabdev@thelabnyc.com
-License: ISC
+Author: David Burke
+Author-email: dburke@thelabnyc.com
+License: Apache License
 Keywords: django wagtail
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Provides-Extra: development
-License-File: LICENSE
 
 =============
 Wagtail Links
 =============
 
 Purpose
 =======
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: wagtail-links Version: 2.5.0 Summary: Wagtail links
-provides a consistent way to refer to links in a wagtail page. Home-page:
-https://gitlab.com/thelabnyc/wagtail-links Author: thelabnyc Author-email:
-thelabdev@thelabnyc.com License: ISC Keywords: django wagtail Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Web
-Environment Classifier: Framework :: Django Classifier: Framework :: Wagtail
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Intended Audience :: Developers Classifier: License ::
-OSI Approved :: Apache Software License Provides-Extra: development License-
-File: LICENSE ============= Wagtail Links ============= Purpose ======= Wagtail
-links has two goals: - Provide a consistent way to refer to links, which may be
-of different types, so as to reduce decision fatigue - Minimize broken links as
-much as possible. Install ======= Install wagtail-links via Pip. .. code:: bash
-pip install wagtail-links Add ``wagtail_links`` to your Django project's
+Metadata-Version: 2.1 Name: wagtail-links Version: 2.5.0b1 Summary: Wagtail
+links provides a consistent way to refer to links in a wagtail page. Home-page:
+https://gitlab.com/thelabnyc/wagtail-links Author: David Burke Author-email:
+dburke@thelabnyc.com License: Apache License Keywords: django wagtail
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
+Wagtail Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: Apache Software License Provides-Extra: development
+============= Wagtail Links ============= Purpose ======= Wagtail links has two
+goals: - Provide a consistent way to refer to links, which may be of different
+types, so as to reduce decision fatigue - Minimize broken links as much as
+possible. Install ======= Install wagtail-links via Pip. .. code:: bash pip
+install wagtail-links Add ``wagtail_links`` to your Django project's
 INSTALLED_APPS setting. Run database migrations. .. code:: bash python
 manage.py migrate Usage ===== Add a foreign key to the page you wish to add
 links to. .. code:: python my_link = models.ForeignKey( 'wagtail_links.Link',
 null=True, blank=True, on_delete=models.SET_NULL, related_name='+' ) Neat: ..
 image:: admin.png You may use it like: .. code:: html Link_here From a
 template, you can also load a link by its name: .. code:: html {% load
 get_wagtail_link_url from wagtail_links %} Link_here This is useful for global
```

### Comparing `wagtail-links-2.5.0/README.rst` & `wagtail-links-2.5.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/setup.py` & `wagtail-links-2.5.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from versiontag import get_version, cache_git_tag  # NOQA
 
 
 packages = find_packages("src")
 
 install_requires = [
-    "wagtail>=3.0,<5.1",
+    "wagtail>=3.0,<4.2",
 ]
 
 extras_require = {
     "development": [
         "flake8>=3.3.0",
         "tox>=2.7.0",
         "versiontag>=1.2.0",
@@ -46,17 +46,17 @@
         "Framework :: Wagtail",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
     ],
     keywords="django wagtail",
-    author="thelabnyc",
-    author_email="thelabdev@thelabnyc.com",
+    author="David Burke",
+    author_email="dburke@thelabnyc.com",
     url="https://gitlab.com/thelabnyc/wagtail-links",
-    license="ISC",
+    license="Apache License",
     package_dir={"": "src"},
     packages=packages,
     include_package_data=True,
     install_requires=install_requires,
     extras_require=extras_require,
 )
```

### Comparing `wagtail-links-2.5.0/src/wagtail_links/fields.py` & `wagtail-links-2.5.0b1/src/wagtail_links/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/locale/es/LC_MESSAGES/django.po` & `wagtail-links-2.5.0b1/src/wagtail_links/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0001_initial.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0002_auto_20170522_1552.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0002_auto_20170522_1552.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0003_auto_20170522_2015.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0003_auto_20170522_2015.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0004_auto_20190411_2102.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0004_auto_20190411_2102.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0005_auto_20191203_1908_squashed_0006_auto_20191204_2129.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0006_auto_20200101_1646.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0006_auto_20200101_1646.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/migrations/0007_auto_20200101_1658.py` & `wagtail-links-2.5.0b1/src/wagtail_links/migrations/0007_auto_20200101_1658.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/models.py` & `wagtail-links-2.5.0b1/src/wagtail_links/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/templatetags/wagtail_links.py` & `wagtail-links-2.5.0b1/src/wagtail_links/templatetags/wagtail_links.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links/tests.py` & `wagtail-links-2.5.0b1/src/wagtail_links/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail-links-2.5.0/src/wagtail_links.egg-info/PKG-INFO` & `wagtail-links-2.5.0b1/src/wagtail_links.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: wagtail-links
-Version: 2.5.0
+Version: 2.5.0b1
 Summary: Wagtail links provides a consistent way to refer to links in a wagtail page.
 Home-page: https://gitlab.com/thelabnyc/wagtail-links
-Author: thelabnyc
-Author-email: thelabdev@thelabnyc.com
-License: ISC
+Author: David Burke
+Author-email: dburke@thelabnyc.com
+License: Apache License
 Keywords: django wagtail
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Provides-Extra: development
-License-File: LICENSE
 
 =============
 Wagtail Links
 =============
 
 Purpose
 =======
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: wagtail-links Version: 2.5.0 Summary: Wagtail links
-provides a consistent way to refer to links in a wagtail page. Home-page:
-https://gitlab.com/thelabnyc/wagtail-links Author: thelabnyc Author-email:
-thelabdev@thelabnyc.com License: ISC Keywords: django wagtail Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Web
-Environment Classifier: Framework :: Django Classifier: Framework :: Wagtail
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Intended Audience :: Developers Classifier: License ::
-OSI Approved :: Apache Software License Provides-Extra: development License-
-File: LICENSE ============= Wagtail Links ============= Purpose ======= Wagtail
-links has two goals: - Provide a consistent way to refer to links, which may be
-of different types, so as to reduce decision fatigue - Minimize broken links as
-much as possible. Install ======= Install wagtail-links via Pip. .. code:: bash
-pip install wagtail-links Add ``wagtail_links`` to your Django project's
+Metadata-Version: 2.1 Name: wagtail-links Version: 2.5.0b1 Summary: Wagtail
+links provides a consistent way to refer to links in a wagtail page. Home-page:
+https://gitlab.com/thelabnyc/wagtail-links Author: David Burke Author-email:
+dburke@thelabnyc.com License: Apache License Keywords: django wagtail
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
+Wagtail Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: Apache Software License Provides-Extra: development
+============= Wagtail Links ============= Purpose ======= Wagtail links has two
+goals: - Provide a consistent way to refer to links, which may be of different
+types, so as to reduce decision fatigue - Minimize broken links as much as
+possible. Install ======= Install wagtail-links via Pip. .. code:: bash pip
+install wagtail-links Add ``wagtail_links`` to your Django project's
 INSTALLED_APPS setting. Run database migrations. .. code:: bash python
 manage.py migrate Usage ===== Add a foreign key to the page you wish to add
 links to. .. code:: python my_link = models.ForeignKey( 'wagtail_links.Link',
 null=True, blank=True, on_delete=models.SET_NULL, related_name='+' ) Neat: ..
 image:: admin.png You may use it like: .. code:: html Link_here From a
 template, you can also load a link by its name: .. code:: html {% load
 get_wagtail_link_url from wagtail_links %} Link_here This is useful for global
```

### Comparing `wagtail-links-2.5.0/src/wagtail_links.egg-info/SOURCES.txt` & `wagtail-links-2.5.0b1/src/wagtail_links.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/wagtail_links/__init__.py
 src/wagtail_links/apps.py
 src/wagtail_links/fields.py
```

