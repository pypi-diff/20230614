# Comparing `tmp/wagtailsnippetscopy-0.4.2.tar.gz` & `tmp/wagtailsnippetscopy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailsnippetscopy-0.4.2.tar", max compression
+gzip compressed data, was "wagtailsnippetscopy-0.5.0.tar", max compression
```

## Comparing `wagtailsnippetscopy-0.4.2.tar` & `wagtailsnippetscopy-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1707 2020-12-10 16:22:32.227033 wagtailsnippetscopy-0.4.2/README.md
--rw-r--r--   0        0        0      991 2022-02-19 19:03:57.990650 wagtailsnippetscopy-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-12-10 16:22:32.227263 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/__init__.py
--rw-r--r--   0        0        0      583 2020-12-10 16:22:32.227382 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/admin.py
--rw-r--r--   0        0        0      113 2020-12-10 16:22:32.227495 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/apps.py
--rw-r--r--   0        0        0     1090 2022-02-18 20:10:28.855046 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/forms.py
--rw-r--r--   0        0        0      365 2020-12-10 16:22:32.227772 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/models.py
--rw-r--r--   0        0        0      576 2020-12-10 16:22:32.227887 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/registry.py
--rw-r--r--   0        0        0      882 2020-12-10 16:22:32.228113 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
--rw-r--r--   0        0        0     2876 2022-02-18 20:10:17.751264 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/views.py
--rw-r--r--   0        0        0      355 2022-02-19 19:02:50.229502 wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/wagtail_hooks.py
--rw-r--r--   0        0        0     2496 2022-02-19 19:04:27.448359 wagtailsnippetscopy-0.4.2/setup.py
--rw-r--r--   0        0        0     2793 2022-02-19 19:04:27.448634 wagtailsnippetscopy-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1707 2023-06-14 09:34:23.280389 wagtailsnippetscopy-0.5.0/README.md
+-rw-r--r--   0        0        0      990 2023-06-14 09:36:00.777115 wagtailsnippetscopy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 09:34:23.280577 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-14 09:34:23.280685 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/admin.py
+-rw-r--r--   0        0        0      113 2023-06-14 09:34:23.280761 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/apps.py
+-rw-r--r--   0        0        0     1090 2023-06-14 09:34:23.280835 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/forms.py
+-rw-r--r--   0        0        0      365 2023-06-14 09:34:23.280923 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/models.py
+-rw-r--r--   0        0        0      576 2023-06-14 09:34:23.281009 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/registry.py
+-rw-r--r--   0        0        0      882 2023-06-14 09:34:23.281191 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
+-rw-r--r--   0        0        0     2876 2023-06-14 09:34:23.281298 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/views.py
+-rw-r--r--   0        0        0      414 2023-06-14 09:35:23.143684 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/wagtail_hooks.py
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 wagtailsnippetscopy-0.5.0/PKG-INFO
```

### Comparing `wagtailsnippetscopy-0.4.2/README.md` & `wagtailsnippetscopy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/pyproject.toml` & `wagtailsnippetscopy-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtailsnippetscopy"
-version = "0.4.2"
+version = "0.5.0"
 description = "Copy A Snippet Feature for Wagtail CMS"
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 license = "The MIT License (MIT)"
 readme = "README.md"
 homepage = "https://timonweb.com"
 repository = "https://github.com/timonweb/wagtailsnippetscopy"
 classifiers = [
@@ -20,13 +20,13 @@
     "Topic :: Utilities",
     "Environment :: Web Environment",
     "Framework :: Django",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-django = ">=2.2"
-wagtail = ">=2.11"
+django = ">=4.0"
+wagtail = ">=4.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/admin.py` & `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/admin.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/forms.py` & `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/registry.py` & `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/registry.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html` & `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/wagtailsnippetscopy/views.py` & `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/views.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.4.2/PKG-INFO` & `wagtailsnippetscopy-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: wagtailsnippetscopy
-Version: 0.4.2
+Version: 0.5.0
 Summary: Copy A Snippet Feature for Wagtail CMS
 Home-page: https://timonweb.com
 License: The MIT License (MIT)
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: django (>=2.2)
-Requires-Dist: wagtail (>=2.11)
+Requires-Dist: django (>=4.0)
+Requires-Dist: wagtail (>=4.0)
 Project-URL: Repository, https://github.com/timonweb/wagtailsnippetscopy
 Description-Content-Type: text/markdown
 
 # 'Copy A Snippet' Feature for Wagtail CMS
 
 You can now "copy" snippets (non-page models) in Wagtail CMS
```

