# Comparing `tmp/wagtail-icon-chooser-0.0.1.tar.gz` & `tmp/wagtail-icon-chooser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-icon-chooser-0.0.1.tar", last modified: Thu May 18 17:23:23 2023, max compression
+gzip compressed data, was "wagtail-icon-chooser-0.0.2.tar", last modified: Wed Jun 14 13:53:15 2023, max compression
```

## Comparing `wagtail-icon-chooser-0.0.1.tar` & `wagtail-icon-chooser-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.192157 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-18 17:23:23.000000 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-18 17:23:23.000000 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:23:23.000000 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 17:23:23.000000 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 17:23:23.000000 wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.188157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.192157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/css/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/js/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.192157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.192157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/templates/wagtailiconchooser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:23.196157 wagtail-icon-chooser-0.0.1/wagtailiconchooser/templates/wagtailiconchooser/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 17:23:04.000000 wagtail-icon-chooser-0.0.1/wagtailiconchooser/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-14 13:53:15.505971 wagtail-icon-chooser-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 13:53:15.000000 wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.497971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:53:15.501971 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-14 13:52:58.000000 wagtail-icon-chooser-0.0.2/wagtailiconchooser/widgets.py
```

### Comparing `wagtail-icon-chooser-0.0.1/PKG-INFO` & `wagtail-icon-chooser-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -74,16 +74,39 @@
 
 - Icon List Modal
 
 ![Icon Modal](screenshots/icon-list-modal.png)
 
 # Showing icons on your frontend templates
 
-The Icons can be used out of the box in templates rendered on the Wagtail admin, without any configuration. To use them
-on your frontend templates, one way to do it is to use the following approach:
+The Icons can be used out of the box in templates rendered on the Wagtail admin, without any custom configuration.
+
+Below are two possible ways of getting your svg icon to show on your custom frontend template:
+
+### 1. Including individual SVG markup
+
+You can use the `svg_icon` template tag as below:
+
+```html
+{% load wagtailiconchooser_tags %}
+
+....
+
+{% block content %}
+
+<div>
+    {% svg_icon name=page.icon classname="your-custom-class" %}
+</div>
+
+{% endblock content %}
+
+.....
+```
+
+### 2. Using SVG Sprites
 
 - Add all icons to your template's context, and have them as a svg sprite. Wagtail provides a way to get all the admin
   icons as a svg sprite, using a view found at `wagtail.admin.views.home.icons`
 - Add the svg sprite to your template
 - use the `icon` template tag from `wagtailadmin_tags` to render your svg, which will the link with the icon from the
   svg sprite
 - or directly render the svg to the template
@@ -130,20 +153,24 @@
 
 {% endblock content %}
 
 
 .....
 ```
 
-You can also directly render your icon without using the `icon` template tag.
+You can also directly render your icon without using the `icon` from `wagtailadmin_tags` template tag,
+since`wagtailadmin_tags` is clearly meant to be used on the admin side of things.
 
 Just replace `{% icon name=page.icon %}` with
 
 ```html
 
 {{ icons_svg_sprite|safe }}
 
 <svg class="icon">
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
+`NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
+have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
+might not use all the icons.
```

### Comparing `wagtail-icon-chooser-0.0.1/README.md` & `wagtail-icon-chooser-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -53,16 +53,39 @@
 
 - Icon List Modal
 
 ![Icon Modal](screenshots/icon-list-modal.png)
 
 # Showing icons on your frontend templates
 
-The Icons can be used out of the box in templates rendered on the Wagtail admin, without any configuration. To use them
-on your frontend templates, one way to do it is to use the following approach:
+The Icons can be used out of the box in templates rendered on the Wagtail admin, without any custom configuration.
+
+Below are two possible ways of getting your svg icon to show on your custom frontend template:
+
+### 1. Including individual SVG markup
+
+You can use the `svg_icon` template tag as below:
+
+```html
+{% load wagtailiconchooser_tags %}
+
+....
+
+{% block content %}
+
+<div>
+    {% svg_icon name=page.icon classname="your-custom-class" %}
+</div>
+
+{% endblock content %}
+
+.....
+```
+
+### 2. Using SVG Sprites
 
 - Add all icons to your template's context, and have them as a svg sprite. Wagtail provides a way to get all the admin
   icons as a svg sprite, using a view found at `wagtail.admin.views.home.icons`
 - Add the svg sprite to your template
 - use the `icon` template tag from `wagtailadmin_tags` to render your svg, which will the link with the icon from the
   svg sprite
 - or directly render the svg to the template
@@ -109,20 +132,24 @@
 
 {% endblock content %}
 
 
 .....
 ```
 
-You can also directly render your icon without using the `icon` template tag.
+You can also directly render your icon without using the `icon` from `wagtailadmin_tags` template tag,
+since`wagtailadmin_tags` is clearly meant to be used on the admin side of things.
 
 Just replace `{% icon name=page.icon %}` with
 
 ```html
 
 {{ icons_svg_sprite|safe }}
 
 <svg class="icon">
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
+`NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
+have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
+might not use all the icons.
```

### Comparing `wagtail-icon-chooser-0.0.1/setup.cfg` & `wagtail-icon-chooser-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-icon-chooser
-version = 0.0.1
+version = 0.0.2
 description = Wagtail Icon Chooser
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-icon-chooser
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/PKG-INFO` & `wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-icon-chooser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wagtail Icon Chooser
 Home-page: https://github.com/wmo-raf/wagtail-icon-chooser
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
@@ -74,16 +74,39 @@
 
 - Icon List Modal
 
 ![Icon Modal](screenshots/icon-list-modal.png)
 
 # Showing icons on your frontend templates
 
-The Icons can be used out of the box in templates rendered on the Wagtail admin, without any configuration. To use them
-on your frontend templates, one way to do it is to use the following approach:
+The Icons can be used out of the box in templates rendered on the Wagtail admin, without any custom configuration.
+
+Below are two possible ways of getting your svg icon to show on your custom frontend template:
+
+### 1. Including individual SVG markup
+
+You can use the `svg_icon` template tag as below:
+
+```html
+{% load wagtailiconchooser_tags %}
+
+....
+
+{% block content %}
+
+<div>
+    {% svg_icon name=page.icon classname="your-custom-class" %}
+</div>
+
+{% endblock content %}
+
+.....
+```
+
+### 2. Using SVG Sprites
 
 - Add all icons to your template's context, and have them as a svg sprite. Wagtail provides a way to get all the admin
   icons as a svg sprite, using a view found at `wagtail.admin.views.home.icons`
 - Add the svg sprite to your template
 - use the `icon` template tag from `wagtailadmin_tags` to render your svg, which will the link with the icon from the
   svg sprite
 - or directly render the svg to the template
@@ -130,20 +153,24 @@
 
 {% endblock content %}
 
 
 .....
 ```
 
-You can also directly render your icon without using the `icon` template tag.
+You can also directly render your icon without using the `icon` from `wagtailadmin_tags` template tag,
+since`wagtailadmin_tags` is clearly meant to be used on the admin side of things.
 
 Just replace `{% icon name=page.icon %}` with
 
 ```html
 
 {{ icons_svg_sprite|safe }}
 
 <svg class="icon">
     <use href="#icon-{{ page.icon }}"></use>
 </svg>
 ```
 
+`NOTE` This approach will load all the icons added to Wagtail (using the `register_icons` hook) to your template. If you
+have registered many SVG icons, this might increase your page's loading bandwidth and might not be efficient since you
+might not use all the icons.
```

### Comparing `wagtail-icon-chooser-0.0.1/wagtail_icon_chooser.egg-info/SOURCES.txt` & `wagtail-icon-chooser-0.0.2/wagtail_icon_chooser.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 wagtail_icon_chooser.egg-info/top_level.txt
 wagtailiconchooser/__init__.py
 wagtailiconchooser/admin.py
 wagtailiconchooser/apps.py
 wagtailiconchooser/blocks.py
 wagtailiconchooser/models.py
 wagtailiconchooser/tests.py
+wagtailiconchooser/utils.py
 wagtailiconchooser/views.py
 wagtailiconchooser/widgets.py
 wagtailiconchooser/migrations/__init__.py
 wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css
 wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget-telepath.js
 wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js
-wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html
+wagtailiconchooser/templatetags/__init__.py
+wagtailiconchooser/templatetags/wagtailiconchooser_tags.py
```

### Comparing `wagtail-icon-chooser-0.0.1/wagtailiconchooser/blocks.py` & `wagtail-icon-chooser-0.0.2/wagtailiconchooser/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css` & `wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/css/icon-chooser-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.1/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js` & `wagtail-icon-chooser-0.0.2/wagtailiconchooser/static/wagtailiconchooser/js/icon-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.1/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html` & `wagtail-icon-chooser-0.0.2/wagtailiconchooser/templates/wagtailiconchooser/widgets/icon-chooser-widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-icon-chooser-0.0.1/wagtailiconchooser/widgets.py` & `wagtail-icon-chooser-0.0.2/wagtailiconchooser/widgets.py`

 * *Files identical despite different names*

