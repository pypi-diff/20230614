# Comparing `tmp/django_minify_html-1.5.0.tar.gz` & `tmp/django_minify_html-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_minify_html-1.5.0.tar", last modified: Sat Feb 25 07:22:23 2023, max compression
+gzip compressed data, was "django_minify_html-1.6.0.tar", last modified: Wed Jun 14 13:58:23 2023, max compression
```

## Comparing `django_minify_html-1.5.0.tar` & `django_minify_html-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:23.546577 django_minify_html-1.5.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      530 2023-02-25 07:22:21.000000 django_minify_html-1.5.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1056 2022-06-03 11:58:39.000000 django_minify_html-1.5.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_minify_html-1.5.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8013 2023-02-25 07:22:23.546670 django_minify_html-1.5.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     6640 2023-01-20 11:36:47.000000 django_minify_html-1.5.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      460 2023-02-15 21:55:44.000000 django_minify_html-1.5.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1668 2023-02-25 07:22:23.547035 django_minify_html-1.5.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:23.543002 django_minify_html-1.5.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:23.545244 django_minify_html-1.5.0/src/django_minify_html/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:43.000000 django_minify_html-1.5.0/src/django_minify_html/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      188 2022-06-03 11:58:43.000000 django_minify_html-1.5.0/src/django_minify_html/apps.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)      713 2022-11-04 11:24:12.000000 django_minify_html-1.5.0/src/django_minify_html/decorators.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2646 2022-11-08 23:28:02.000000 django_minify_html-1.5.0/src/django_minify_html/middleware.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:43.000000 django_minify_html-1.5.0/src/django_minify_html/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:23.546117 django_minify_html-1.5.0/src/django_minify_html.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     8013 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      540 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       24 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2023-02-25 07:22:23.000000 django_minify_html-1.5.0/src/django_minify_html.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-02-25 07:22:23.546276 django_minify_html-1.5.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2607 2022-11-08 23:28:07.000000 django_minify_html-1.5.0/tests/test_middleware.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:58:23.691770 django_minify_html-1.6.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      593 2023-06-14 13:58:21.000000 django_minify_html-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1056 2022-06-03 11:58:39.000000 django_minify_html-1.6.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-01-20 12:09:56.000000 django_minify_html-1.6.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8060 2023-06-14 13:58:23.691834 django_minify_html-1.6.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6636 2023-06-14 13:54:20.000000 django_minify_html-1.6.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-02-28 09:05:50.000000 django_minify_html-1.6.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1709 2023-06-14 13:58:23.692096 django_minify_html-1.6.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:58:23.689508 django_minify_html-1.6.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:58:23.690823 django_minify_html-1.6.0/src/django_minify_html/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:43.000000 django_minify_html-1.6.0/src/django_minify_html/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      188 2022-06-03 11:58:43.000000 django_minify_html-1.6.0/src/django_minify_html/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      713 2022-11-04 11:24:12.000000 django_minify_html-1.6.0/src/django_minify_html/decorators.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2646 2023-05-06 09:54:14.000000 django_minify_html-1.6.0/src/django_minify_html/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2022-06-03 11:58:43.000000 django_minify_html-1.6.0/src/django_minify_html/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:58:23.691526 django_minify_html-1.6.0/src/django_minify_html.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     8060 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      540 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       24 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       19 2023-06-14 13:58:23.000000 django_minify_html-1.6.0/src/django_minify_html.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-14 13:58:23.691661 django_minify_html-1.6.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2607 2022-11-08 23:28:07.000000 django_minify_html-1.6.0/tests/test_middleware.py
```

### Comparing `django_minify_html-1.5.0/CHANGELOG.rst` & `django_minify_html-1.6.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.6.0 (2023-06-14)
+------------------
+
+* Support Python 3.12.
+
 1.5.0 (2023-02-25)
 ------------------
 
 * Support Django 4.2.
 
 1.4.0 (2022-10-31)
 ------------------
```

### Comparing `django_minify_html-1.5.0/LICENSE` & `django_minify_html-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_minify_html-1.5.0/PKG-INFO` & `django_minify_html-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_minify_html
-Version: 1.5.0
+Version: 1.6.0
 Summary: Use minify-html, the extremely fast HTML + JS + CSS minifier, with Django.
 Home-page: https://github.com/adamchainz/django-minify-html
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-minify-html/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -21,14 +21,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==================
@@ -52,15 +53,15 @@
    :alt: pre-commit
 
 Use `minify-html <https://github.com/wilsonzlin/minify-html>`__, the extremely fast HTML + JS + CSS minifier, with Django.
 
 Requirements
 ------------
 
-Python 3.8 to 3.11 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
@@ -110,15 +111,15 @@
 ``django_minify_html.middleware.MinifyHtmlMiddleware``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The middleware runs ``minify_html.minify()`` on the content of HTML responses.
 This function minifies HTML, and any inline JavaScript and CSS.
 
 The middleware passes keyword arguments to ``minify()`` from its ``minify_args`` attribute, a dictionary of names to values.
-These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/src/lib.template.rs>`__.
+These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/main/src/lib.rs>`__.
 By default the middleware overrides ``minify_css`` and ``minify_js`` to ``True``.
 If you need to change an argument, subclass the middleware, replace ``minify_args``, and use your subclass.
 For example, to preserve comments after minification:
 
 .. code-block:: python
 
     from django_minify_html.middleware import MinifyHtmlMiddleware
```

### Comparing `django_minify_html-1.5.0/README.rst` & `django_minify_html-1.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    :alt: pre-commit
 
 Use `minify-html <https://github.com/wilsonzlin/minify-html>`__, the extremely fast HTML + JS + CSS minifier, with Django.
 
 Requirements
 ------------
 
-Python 3.8 to 3.11 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
@@ -77,15 +77,15 @@
 ``django_minify_html.middleware.MinifyHtmlMiddleware``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The middleware runs ``minify_html.minify()`` on the content of HTML responses.
 This function minifies HTML, and any inline JavaScript and CSS.
 
 The middleware passes keyword arguments to ``minify()`` from its ``minify_args`` attribute, a dictionary of names to values.
-These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/src/lib.template.rs>`__.
+These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/main/src/lib.rs>`__.
 By default the middleware overrides ``minify_css`` and ``minify_js`` to ``True``.
 If you need to change an argument, subclass the middleware, replace ``minify_args``, and use your subclass.
 For example, to preserve comments after minification:
 
 .. code-block:: python
 
     from django_minify_html.middleware import MinifyHtmlMiddleware
```

### Comparing `django_minify_html-1.5.0/setup.cfg` & `django_minify_html-1.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = django_minify_html
-version = 1.5.0
+version = 1.6.0
 description = Use minify-html, the extremely fast HTML + JS + CSS minifier, with Django.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/django-minify-html
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
@@ -21,14 +21,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
 keywords = Django
 project_urls = 
 	Changelog = https://github.com/adamchainz/django-minify-html/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `django_minify_html-1.5.0/src/django_minify_html/decorators.py` & `django_minify_html-1.6.0/src/django_minify_html/decorators.py`

 * *Files identical despite different names*

### Comparing `django_minify_html-1.5.0/src/django_minify_html/middleware.py` & `django_minify_html-1.6.0/src/django_minify_html/middleware.py`

 * *Files identical despite different names*

### Comparing `django_minify_html-1.5.0/src/django_minify_html.egg-info/PKG-INFO` & `django_minify_html-1.6.0/src/django_minify_html.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minify-html
-Version: 1.5.0
+Version: 1.6.0
 Summary: Use minify-html, the extremely fast HTML + JS + CSS minifier, with Django.
 Home-page: https://github.com/adamchainz/django-minify-html
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-minify-html/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -21,14 +21,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==================
@@ -52,15 +53,15 @@
    :alt: pre-commit
 
 Use `minify-html <https://github.com/wilsonzlin/minify-html>`__, the extremely fast HTML + JS + CSS minifier, with Django.
 
 Requirements
 ------------
 
-Python 3.8 to 3.11 supported.
+Python 3.8 to 3.12 supported.
 
 Django 3.2 to 4.2 supported.
 
 ----
 
 **Want to work smarter and faster?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
@@ -110,15 +111,15 @@
 ``django_minify_html.middleware.MinifyHtmlMiddleware``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The middleware runs ``minify_html.minify()`` on the content of HTML responses.
 This function minifies HTML, and any inline JavaScript and CSS.
 
 The middleware passes keyword arguments to ``minify()`` from its ``minify_args`` attribute, a dictionary of names to values.
-These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/src/lib.template.rs>`__.
+These correspond to the values in the Rust library’s `Cfg structure <https://docs.rs/minify-html/latest/minify_html/struct.Cfg.html>`__, which have defaults in the Python library as visible `in the source <https://github.com/wilsonzlin/minify-html/blob/master/python/main/src/lib.rs>`__.
 By default the middleware overrides ``minify_css`` and ``minify_js`` to ``True``.
 If you need to change an argument, subclass the middleware, replace ``minify_args``, and use your subclass.
 For example, to preserve comments after minification:
 
 .. code-block:: python
 
     from django_minify_html.middleware import MinifyHtmlMiddleware
```

### Comparing `django_minify_html-1.5.0/src/django_minify_html.egg-info/SOURCES.txt` & `django_minify_html-1.6.0/src/django_minify_html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_minify_html-1.5.0/tests/test_middleware.py` & `django_minify_html-1.6.0/tests/test_middleware.py`

 * *Files identical despite different names*

