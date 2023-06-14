# Comparing `tmp/wagtail-draftail-plugins-0.2.1.tar.gz` & `tmp/wagtail-draftail-plugins-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-draftail-plugins-0.2.1.tar", last modified: Thu Dec 12 21:56:57 2019, max compression
+gzip compressed data, was "dist/wagtail-draftail-plugins-0.2.2.tar", last modified: Wed Dec 18 19:22:42 2019, max compression
```

## Comparing `wagtail-draftail-plugins-0.2.1.tar` & `wagtail-draftail-plugins-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/
--rw-r--r--   0 crgwbr     (501) staff       (20)       89 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.1/MANIFEST.in
--rw-r--r--   0 crgwbr     (501) staff       (20)     1395 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/PKG-INFO
--rw-r--r--   0 crgwbr     (501) staff       (20)      482 2019-12-12 21:56:29.000000 wagtail-draftail-plugins-0.2.1/README.rst
--rw-r--r--   0 crgwbr     (501) staff       (20)       99 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/setup.cfg
--rw-r--r--   0 crgwbr     (501) staff       (20)     1699 2018-11-28 18:08:15.000000 wagtail-draftail-plugins-0.2.1/setup.py
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/
--rw-r--r--   0 crgwbr     (501) staff       (20)        0 2018-06-27 15:23:06.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/__init__.py
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/es/
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/
--rw-r--r--   0 crgwbr     (501) staff       (20)      380 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 crgwbr     (501) staff       (20)      892 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 crgwbr     (501) staff       (20)     4752 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/wagtail_hooks.py
-drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/
--rw-rw-r--   0 crgwbr     (501) staff       (20)     1395 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/PKG-INFO
--rw-rw-r--   0 crgwbr     (501) staff       (20)      521 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 crgwbr     (501) staff       (20)        1 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 crgwbr     (501) staff       (20)       71 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/requires.txt
--rw-rw-r--   0 crgwbr     (501) staff       (20)       25 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/top_level.txt
--rw-r--r--   0 crgwbr     (501) staff       (20)        6 2019-12-12 21:56:57.000000 wagtail-draftail-plugins-0.2.1/version.txt
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/
+-rw-r--r--   0 crgwbr     (501) staff       (20)       89 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.2/MANIFEST.in
+-rw-r--r--   0 crgwbr     (501) staff       (20)     1395 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/PKG-INFO
+-rw-r--r--   0 crgwbr     (501) staff       (20)      482 2019-12-12 21:56:29.000000 wagtail-draftail-plugins-0.2.2/README.rst
+-rw-r--r--   0 crgwbr     (501) staff       (20)       99 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/setup.cfg
+-rw-r--r--   0 crgwbr     (501) staff       (20)     1699 2018-11-28 18:08:15.000000 wagtail-draftail-plugins-0.2.2/setup.py
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/
+-rw-r--r--   0 crgwbr     (501) staff       (20)        0 2018-06-27 15:23:06.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/__init__.py
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/es/
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/
+-rw-r--r--   0 crgwbr     (501) staff       (20)      380 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 crgwbr     (501) staff       (20)      892 2019-11-22 17:58:03.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 crgwbr     (501) staff       (20)     4747 2019-12-18 19:21:07.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/wagtail_hooks.py
+drwxr-xr-x   0 crgwbr     (501) staff       (20)        0 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/
+-rw-rw-r--   0 crgwbr     (501) staff       (20)     1395 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 crgwbr     (501) staff       (20)      521 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 crgwbr     (501) staff       (20)        1 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 crgwbr     (501) staff       (20)       71 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/requires.txt
+-rw-rw-r--   0 crgwbr     (501) staff       (20)       25 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/top_level.txt
+-rw-r--r--   0 crgwbr     (501) staff       (20)        6 2019-12-18 19:22:42.000000 wagtail-draftail-plugins-0.2.2/version.txt
```

### Comparing `wagtail-draftail-plugins-0.2.1/PKG-INFO` & `wagtail-draftail-plugins-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-draftail-plugins
-Version: 0.2.1
+Version: 0.2.2
 Summary: Commonly used extensions to Wagtail's Draftail editor.
 Home-page: https://gitlab.com/thelabnyc/wagtail-draftail-plugins
 Author: Craig Weber
 Author-email: crgwbr@gmail.com
 License: ISC
 Description: ===============================
         Wagtail Draftail Editor Plugins
```

### Comparing `wagtail-draftail-plugins-0.2.1/setup.py` & `wagtail-draftail-plugins-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.po` & `wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins/wagtail_hooks.py` & `wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins/wagtail_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from wagtail.core import hooks
 from wagtail.admin.rich_text.converters.html_to_contentstate import BlockElementHandler
 from wagtail.admin.rich_text.converters.html_to_contentstate import InlineStyleElementHandler
-from django.utils.translation import gettext_lazy as _
+from django.utils.translation import gettext as _
 from collections import namedtuple
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 
 
 EditorPlugin = namedtuple('BlockPlugin', (
     'feature_name',
     'type',
```

### Comparing `wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/PKG-INFO` & `wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-draftail-plugins
-Version: 0.2.1
+Version: 0.2.2
 Summary: Commonly used extensions to Wagtail's Draftail editor.
 Home-page: https://gitlab.com/thelabnyc/wagtail-draftail-plugins
 Author: Craig Weber
 Author-email: crgwbr@gmail.com
 License: ISC
 Description: ===============================
         Wagtail Draftail Editor Plugins
```

### Comparing `wagtail-draftail-plugins-0.2.1/src/wagtail_draftail_plugins.egg-info/SOURCES.txt` & `wagtail-draftail-plugins-0.2.2/src/wagtail_draftail_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

