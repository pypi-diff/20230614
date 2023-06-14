# Comparing `tmp/wagtailsnippetscopy-0.5.1.tar.gz` & `tmp/wagtailsnippetscopy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailsnippetscopy-0.5.1.tar", max compression
+gzip compressed data, was "wagtailsnippetscopy-0.5.2.tar", max compression
```

## Comparing `wagtailsnippetscopy-0.5.1.tar` & `wagtailsnippetscopy-0.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1707 2023-06-14 09:34:23.280389 wagtailsnippetscopy-0.5.1/README.md
--rw-r--r--   0        0        0      990 2023-06-14 09:45:01.611943 wagtailsnippetscopy-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 09:34:23.280577 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/__init__.py
--rw-r--r--   0        0        0      583 2023-06-14 09:34:23.280685 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/admin.py
--rw-r--r--   0        0        0      113 2023-06-14 09:34:23.280761 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/apps.py
--rw-r--r--   0        0        0     1090 2023-06-14 09:34:23.280835 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/forms.py
--rw-r--r--   0        0        0      365 2023-06-14 09:34:23.280923 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/models.py
--rw-r--r--   0        0        0      576 2023-06-14 09:34:23.281009 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/registry.py
--rw-r--r--   0        0        0      882 2023-06-14 09:34:23.281191 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
--rw-r--r--   0        0        0     2936 2023-06-14 09:43:56.576469 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/views.py
--rw-r--r--   0        0        0      414 2023-06-14 09:35:23.143684 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/wagtail_hooks.py
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 wagtailsnippetscopy-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1707 2023-06-14 09:34:23.280389 wagtailsnippetscopy-0.5.2/README.md
+-rw-r--r--   0        0        0      990 2023-06-14 13:36:24.588383 wagtailsnippetscopy-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 09:34:23.280577 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-14 09:34:23.280685 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/admin.py
+-rw-r--r--   0        0        0      113 2023-06-14 09:34:23.280761 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/apps.py
+-rw-r--r--   0        0        0     1090 2023-06-14 09:34:23.280835 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/forms.py
+-rw-r--r--   0        0        0      365 2023-06-14 09:34:23.280923 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/models.py
+-rw-r--r--   0        0        0      576 2023-06-14 09:34:23.281009 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/registry.py
+-rw-r--r--   0        0        0      882 2023-06-14 09:34:23.281191 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
+-rw-r--r--   0        0        0     2936 2023-06-14 09:43:56.576469 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/views.py
+-rw-r--r--   0        0        0      414 2023-06-14 09:35:23.143684 wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/wagtail_hooks.py
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 wagtailsnippetscopy-0.5.2/PKG-INFO
```

### Comparing `wagtailsnippetscopy-0.5.1/README.md` & `wagtailsnippetscopy-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/pyproject.toml` & `wagtailsnippetscopy-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtailsnippetscopy"
-version = "0.5.1"
+version = "0.5.2"
 description = "Copy A Snippet Feature for Wagtail CMS"
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 license = "The MIT License (MIT)"
 readme = "README.md"
 homepage = "https://timonweb.com"
 repository = "https://github.com/timonweb/wagtailsnippetscopy"
 classifiers = [
```

### Comparing `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/admin.py` & `wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/admin.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/forms.py` & `wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/registry.py` & `wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/registry.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html` & `wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/views.py` & `wagtailsnippetscopy-0.5.2/wagtailsnippetscopy/views.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.1/PKG-INFO` & `wagtailsnippetscopy-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailsnippetscopy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Copy A Snippet Feature for Wagtail CMS
 Home-page: https://timonweb.com
 License: The MIT License (MIT)
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

