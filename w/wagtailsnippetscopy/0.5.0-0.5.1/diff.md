# Comparing `tmp/wagtailsnippetscopy-0.5.0.tar.gz` & `tmp/wagtailsnippetscopy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailsnippetscopy-0.5.0.tar", max compression
+gzip compressed data, was "wagtailsnippetscopy-0.5.1.tar", max compression
```

## Comparing `wagtailsnippetscopy-0.5.0.tar` & `wagtailsnippetscopy-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1707 2023-06-14 09:34:23.280389 wagtailsnippetscopy-0.5.0/README.md
--rw-r--r--   0        0        0      990 2023-06-14 09:36:00.777115 wagtailsnippetscopy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 09:34:23.280577 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/__init__.py
--rw-r--r--   0        0        0      583 2023-06-14 09:34:23.280685 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/admin.py
--rw-r--r--   0        0        0      113 2023-06-14 09:34:23.280761 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/apps.py
--rw-r--r--   0        0        0     1090 2023-06-14 09:34:23.280835 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/forms.py
--rw-r--r--   0        0        0      365 2023-06-14 09:34:23.280923 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/models.py
--rw-r--r--   0        0        0      576 2023-06-14 09:34:23.281009 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/registry.py
--rw-r--r--   0        0        0      882 2023-06-14 09:34:23.281191 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
--rw-r--r--   0        0        0     2876 2023-06-14 09:34:23.281298 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/views.py
--rw-r--r--   0        0        0      414 2023-06-14 09:35:23.143684 wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/wagtail_hooks.py
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 wagtailsnippetscopy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1707 2023-06-14 09:34:23.280389 wagtailsnippetscopy-0.5.1/README.md
+-rw-r--r--   0        0        0      990 2023-06-14 09:45:01.611943 wagtailsnippetscopy-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 09:34:23.280577 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-14 09:34:23.280685 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/admin.py
+-rw-r--r--   0        0        0      113 2023-06-14 09:34:23.280761 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/apps.py
+-rw-r--r--   0        0        0     1090 2023-06-14 09:34:23.280835 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/forms.py
+-rw-r--r--   0        0        0      365 2023-06-14 09:34:23.280923 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/models.py
+-rw-r--r--   0        0        0      576 2023-06-14 09:34:23.281009 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/registry.py
+-rw-r--r--   0        0        0      882 2023-06-14 09:34:23.281191 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html
+-rw-r--r--   0        0        0     2936 2023-06-14 09:43:56.576469 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/views.py
+-rw-r--r--   0        0        0      414 2023-06-14 09:35:23.143684 wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/wagtail_hooks.py
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 wagtailsnippetscopy-0.5.1/PKG-INFO
```

### Comparing `wagtailsnippetscopy-0.5.0/README.md` & `wagtailsnippetscopy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.0/pyproject.toml` & `wagtailsnippetscopy-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtailsnippetscopy"
-version = "0.5.0"
+version = "0.5.1"
 description = "Copy A Snippet Feature for Wagtail CMS"
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 license = "The MIT License (MIT)"
 readme = "README.md"
 homepage = "https://timonweb.com"
 repository = "https://github.com/timonweb/wagtailsnippetscopy"
 classifiers = [
```

### Comparing `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/admin.py` & `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/admin.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/forms.py` & `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/registry.py` & `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/registry.py`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html` & `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/templates/wagtailsnippetscopy/copy.html`

 * *Files identical despite different names*

### Comparing `wagtailsnippetscopy-0.5.0/wagtailsnippetscopy/views.py` & `wagtailsnippetscopy-0.5.1/wagtailsnippetscopy/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 except ImportError:
     from django.utils.translation import gettext_lazy as _
 
 from wagtail.admin import messages
 from wagtail.admin.auth import user_passes_test, user_has_any_page_permission, permission_denied
 from wagtail.admin.views.pages.utils import get_valid_next_url_from_request
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
-from wagtail.core import hooks
-from wagtail.snippets.permissions import get_permission_name
 
+try:
+    from wagtail import hooks
+except ImportError:
+    from wagtail.core import hooks
+
+from wagtail.snippets.permissions import get_permission_name
 from .registry import snippet_copy_registry
 
 
 @user_passes_test(user_has_any_page_permission)
 def copy(request, app_label, model_name, id):
     # Validate snippet has been registered and title_field is set.
     meta = snippet_copy_registry.get(app_label, model_name)
```

### Comparing `wagtailsnippetscopy-0.5.0/PKG-INFO` & `wagtailsnippetscopy-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailsnippetscopy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Copy A Snippet Feature for Wagtail CMS
 Home-page: https://timonweb.com
 License: The MIT License (MIT)
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

