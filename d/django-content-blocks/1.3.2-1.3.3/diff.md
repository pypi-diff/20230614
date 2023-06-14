# Comparing `tmp/django-content-blocks-1.3.2.tar.gz` & `tmp/django-content-blocks-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.3.2.tar", last modified: Wed May 24 12:01:38 2023, max compression
+gzip compressed data, was "django-content-blocks-1.3.3.tar", last modified: Mon Jun  5 17:04:46 2023, max compression
```

## Comparing `django-content-blocks-1.3.2.tar` & `django-content-blocks-1.3.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.365796 django-content-blocks-1.3.2/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4662 2023-05-24 12:01:38.366439 django-content-blocks-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.920102 django-content-blocks-1.3.2/content_blocks/
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.2/content_blocks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/abstract_models.py
--rw-r--r--   0 root         (0) root         (0)    11884 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/admin.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/admin_forms.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-05-24 11:56:52.000000 django-content-blocks-1.3.2/content_blocks/apps.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/conf.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.2/content_blocks/fields.py
--rw-r--r--   0 root         (0) root         (0)     8031 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.926445 django-content-blocks-1.3.2/content_blocks/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.2/content_blocks/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.961227 django-content-blocks-1.3.2/content_blocks/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.2/content_blocks/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/management/commands/export_content_block_templates.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.2/content_blocks/management/commands/import_content_block_templates.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/management/commands/set_content_blocks_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.977356 django-content-blocks-1.3.2/content_blocks/migrations/
--rw-r--r--   0 root         (0) root         (0)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.2/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.2/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.2/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.2/content_blocks/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22721 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.995384 django-content-blocks-1.3.2/content_blocks/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.2/content_blocks/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12032 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/services/content_block.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/services/content_block_parent.py
--rw-r--r--   0 root         (0) root         (0)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.2/content_blocks/services/content_block_template.py
--rw-r--r--   0 root         (0) root         (0)     5123 2023-05-24 11:59:52.000000 django-content-blocks-1.3.2/content_blocks/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.799731 django-content-blocks-1.3.2/content_blocks/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.001948 django-content-blocks-1.3.2/content_blocks/static/content_blocks/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.019525 django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/
--rw-r--r--   0 root         (0) root         (0)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 root         (0) root         (0)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:37.805440 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.064409 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 root         (0) root         (0)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.084828 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 root         (0) root         (0)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 root         (0) root         (0)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.112121 django-content-blocks-1.3.2/content_blocks/static/content_blocks/iframeresizer/
--rw-r--r--   0 root         (0) root         (0)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-r--r--   0 root         (0) root         (0)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.127160 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 root         (0) root         (0)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 root         (0) root         (0)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.142918 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 root         (0) root         (0)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 root         (0) root         (0)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.204748 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 root         (0) root         (0)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 root         (0) root         (0)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.218188 django-content-blocks-1.3.2/content_blocks/templates/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.2/content_blocks/templates/.DS_Store
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.236517 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.242940 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/admin/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-05 14:20:51.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.263585 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.275967 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.284639 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.309756 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.321152 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.330670 django-content-blocks-1.3.2/content_blocks/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.2/content_blocks/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.2/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.2/content_blocks/urls.py
--rw-r--r--   0 root         (0) root         (0)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.2/content_blocks/views.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.2/content_blocks/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 12:01:38.363751 django-content-blocks-1.3.2/django_content_blocks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4662 2023-05-24 12:01:37.000000 django-content-blocks-1.3.2/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4653 2023-05-24 12:01:37.000000 django-content-blocks-1.3.2/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-24 12:01:37.000000 django-content-blocks-1.3.2/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 12:01:37.000000 django-content-blocks-1.3.2/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-24 12:01:37.000000 django-content-blocks-1.3.2/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1945 2023-05-24 12:01:38.375619 django-content-blocks-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.2/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.821662 django-content-blocks-1.3.3/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     4662 2023-06-05 17:04:46.821797 django-content-blocks-1.3.3/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.795332 django-content-blocks-1.3.3/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.3/content_blocks/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/abstract_models.py
+-rw-r--r--   0 quantra    (501) staff       (20)    11872 2023-06-04 21:01:31.000000 django-content-blocks-1.3.3/content_blocks/admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/admin_forms.py
+-rw-r--r--   0 quantra    (501) staff       (20)      952 2023-06-04 20:53:17.000000 django-content-blocks-1.3.3/content_blocks/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1591 2023-06-03 20:41:24.000000 django-content-blocks-1.3.3/content_blocks/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.3/content_blocks/fields.py
+-rw-r--r--   0 quantra    (501) staff       (20)     8031 2023-05-24 23:15:33.000000 django-content-blocks-1.3.3/content_blocks/forms.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.795839 django-content-blocks-1.3.3/content_blocks/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.3/content_blocks/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.797384 django-content-blocks-1.3.3/content_blocks/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.3/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 quantra    (501) staff       (20)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/export_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1461 2023-05-24 11:55:23.000000 django-content-blocks-1.3.3/content_blocks/management/commands/import_content_block_templates.py
+-rw-r--r--   0 quantra    (501) staff       (20)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/management/commands/set_content_blocks_cache.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.798514 django-content-blocks-1.3.3/content_blocks/migrations/
+-rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.3/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.3/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.3/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.3/content_blocks/migrations/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    23959 2023-06-04 20:37:37.000000 django-content-blocks-1.3.3/content_blocks/models.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.800017 django-content-blocks-1.3.3/content_blocks/services/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.3/content_blocks/services/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12032 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/services/content_block.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/services/content_block_parent.py
+-rw-r--r--   0 quantra    (501) staff       (20)     5283 2023-05-24 11:55:40.000000 django-content-blocks-1.3.3/content_blocks/services/content_block_template.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3312 2023-06-04 21:01:31.000000 django-content-blocks-1.3.3/content_blocks/signals.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.787085 django-content-blocks-1.3.3/content_blocks/static/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.800302 django-content-blocks-1.3.3/content_blocks/static/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.801746 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 quantra    (501) staff       (20)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.788454 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.803184 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 quantra    (501) staff       (20)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 quantra    (501) staff       (20)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.804221 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.805432 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/
+-rw-r--r--   0 quantra    (501) staff       (20)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-r--r--   0 quantra    (501) staff       (20)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.806108 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 quantra    (501) staff       (20)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 quantra    (501) staff       (20)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.806747 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 quantra    (501) staff       (20)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 quantra    (501) staff       (20)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.808529 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 quantra    (501) staff       (20)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 quantra    (501) staff       (20)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 quantra    (501) staff       (20)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 quantra    (501) staff       (20)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.809154 django-content-blocks-1.3.3/content_blocks/templates/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.3/content_blocks/templates/.DS_Store
+-rw-r--r--   0 quantra    (501) staff       (20)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/base.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.810157 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/
+-rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/.DS_Store
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.810989 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/
+-rw-r--r--   0 quantra    (501) staff       (20)      317 2023-06-04 15:21:52.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+-rw-r--r--   0 quantra    (501) staff       (20)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 quantra    (501) staff       (20)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.812599 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 quantra    (501) staff       (20)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 quantra    (501) staff       (20)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 quantra    (501) staff       (20)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.813684 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 quantra    (501) staff       (20)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.814268 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 quantra    (501) staff       (20)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 quantra    (501) staff       (20)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.815251 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 quantra    (501) staff       (20)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 quantra    (501) staff       (20)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 quantra    (501) staff       (20)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 quantra    (501) staff       (20)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 quantra    (501) staff       (20)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.816106 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 quantra    (501) staff       (20)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 quantra    (501) staff       (20)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 quantra    (501) staff       (20)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.817441 django-content-blocks-1.3.3/content_blocks/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.3/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.3/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 quantra    (501) staff       (20)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.3/content_blocks/urls.py
+-rw-r--r--   0 quantra    (501) staff       (20)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.3/content_blocks/views.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.3/content_blocks/widgets.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-06-05 17:04:46.821517 django-content-blocks-1.3.3/django_content_blocks.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     4662 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     4653 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       55 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       23 2023-06-05 17:04:46.000000 django-content-blocks-1.3.3/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.3/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1945 2023-06-05 17:04:46.825328 django-content-blocks-1.3.3/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.3/setup.py
```

### Comparing `django-content-blocks-1.3.2/LICENSE` & `django-content-blocks-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/PKG-INFO` & `django-content-blocks-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.2
+Version: 1.3.3
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.2/README.rst` & `django-content-blocks-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/abstract_models.py` & `django-content-blocks-1.3.3/content_blocks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/admin.py` & `django-content-blocks-1.3.3/content_blocks/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Content blocks admin.py
 """
 from io import StringIO
 
 from adminsortable2.admin import SortableAdminMixin, SortableInlineAdminMixin
-from django.conf import settings
+from django.apps import apps
 from django.contrib import admin, messages
 from django.http import HttpResponseRedirect, StreamingHttpResponse
 from django.template import TemplateDoesNotExist
 from django.template.loader import get_template
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
 
@@ -154,15 +154,15 @@
             content_type="application/json",
             headers={
                 "Content-Disposition": 'attachment; filename="content_block_templates.json"'
             },
         )
 
 
-if "dbtemplates" in settings.INSTALLED_APPS:
+if apps.is_installed("dbtemplates"):
     from dbtemplates.models import Template
 
     admin.site.unregister(ContentBlockTemplate)
 
     @admin.register(ContentBlockTemplate)
     class ContentBlockTemplateDBTemplatesAdmin(ContentBlockTemplateAdmin):
         @property
```

### Comparing `django-content-blocks-1.3.2/content_blocks/admin_forms.py` & `django-content-blocks-1.3.3/content_blocks/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/apps.py` & `django-content-blocks-1.3.3/content_blocks/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from django.apps import AppConfig
+from django.apps import AppConfig, apps
 from django.db import OperationalError, ProgrammingError
 
 from content_blocks.conf import settings
 
 logger = logging.getLogger(__name__)
 
 
@@ -14,18 +14,15 @@
 
     def ready(self):
         from content_blocks.signals import (  # noqa
             cleanup_media_delete,
             cleanup_media_save,
         )
 
-        if not settings.CONTENT_BLOCKS_DISABLE_UPDATE_CACHE_MODEL_CHOICE:
-            from content_blocks.signals import update_cache_model_choice  # noqa
-
-        if "dbtemplates" in settings.INSTALLED_APPS:
+        if apps.is_installed("dbtemplates"):
             from content_blocks.signals import update_cache_template  # noqa
 
         if not settings.CONTENT_BLOCKS_DISABLE_CACHE_ON_START:
             try:
                 from content_blocks.services.content_block import CacheServices
 
                 CacheServices.get_or_set_cache_all()
```

### Comparing `django-content-blocks-1.3.2/content_blocks/conf.py` & `django-content-blocks-1.3.3/content_blocks/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
     # Disable caching of content blocks
     CONTENT_BLOCKS_DISABLE_CACHE = False
 
     # Disable caching of content blocks on start
     CONTENT_BLOCKS_DISABLE_CACHE_ON_START = False
 
-    # Disable updating cache on related model save
-    CONTENT_BLOCKS_DISABLE_UPDATE_CACHE_MODEL_CHOICE = False
-
     # Choose the storage backend to use for media files
     # Image, field and video storage settings are use instead of content blocks storage if set.
     CONTENT_BLOCKS_IMAGE_STORAGE = None
     CONTENT_BLOCKS_FILE_STORAGE = None
     CONTENT_BLOCKS_VIDEO_STORAGE = None
     # Use default storage if not set.
     # Support provided here for Django 3.2
```

### Comparing `django-content-blocks-1.3.2/content_blocks/fields.py` & `django-content-blocks-1.3.3/content_blocks/fields.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/forms.py` & `django-content-blocks-1.3.3/content_blocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/management/commands/export_content_block_templates.py` & `django-content-blocks-1.3.3/content_blocks/management/commands/export_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/management/commands/import_content_block_templates.py` & `django-content-blocks-1.3.3/content_blocks/management/commands/import_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.3.3/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py` & `django-content-blocks-1.3.3/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py` & `django-content-blocks-1.3.3/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/models.py` & `django-content-blocks-1.3.3/content_blocks/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Content Blocks models.py
 """
+import functools
 import json
 import logging
 
 from django import forms
+from django.apps import apps
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.files.storage import get_storage_class
 from django.core.validators import RegexValidator
 from django.db import models
 from django.forms.utils import pretty_name
 from django.template.exceptions import TemplateDoesNotExist
@@ -29,25 +31,30 @@
     SVGAndImageFieldFormField,
     VideoField,
 )
 from content_blocks.widgets import FileWidget
 
 logger = logging.getLogger(__name__)
 
-if (
-    "django_cleanup" in settings.INSTALLED_APPS
-    or "django_cleanup.apps.CleanupConfig" in settings.INSTALLED_APPS
+if apps.is_installed("django_cleanup") or apps.is_installed(
+    "django_cleanup.apps.CleanupConfig"
 ):
     from django_cleanup.cleanup import cleanup_ignore
 else:
     # noop shim for when django_cleanup isn't installed
     def cleanup_ignore(cls):  # pragma: no cover (covered in settings specific tests)
         return cls
 
 
+class PolymorphError(Exception):
+    """
+    Raised should polymorph fail.
+    """
+
+
 class ContentBlockFields(models.TextChoices):
     TEXT_FIELD = "TextField"
     CONTENT_FIELD = "ContentField"
     IMAGE_FIELD = "ImageField"
     NESTED_FIELD = "NestedField"
     CHECKBOX_FIELD = "CheckboxField"
     CHOICE_FIELD = "ChoiceField"
@@ -136,25 +143,14 @@
 
     template_name = "content_blocks/partials/fields/default.html"
     preview_template_name = None
 
     class Meta:
         ordering = ["template_field__position"]
 
-    def __init__(self, *args, **kwargs):
-        """
-        Polymorph to the appropriate subclass proxy model.
-        """
-        super().__init__(*args, **kwargs)
-
-        for _class in ContentBlockField.__subclasses__():
-            if self.field_type == _class.__name__:
-                self.__class__ = _class
-                break
-
     def __init_subclass__(subcls):
         """
         Wrap all subclass form_field.__get__ methods with form_field_wrapper
         """
         super.__init_subclass__()
 
         new_property = property(
@@ -163,21 +159,54 @@
         )
         setattr(
             subcls,
             "form_field",
             new_property,
         )
 
+    def __getattribute__(self, item):
+        """
+        Lazy polymorphism.  Only polymorph when accessing certain attrs.
+        """
+        polymorph_attrs = [
+            "form_field",
+            "context_value",
+            "save_value",
+            "template_name",
+            "preview_template_name",
+            "label",
+        ]
+        if item in polymorph_attrs:
+            self.polymorph()
+
+        return super().__getattribute__(item)
+
+    def polymorph(self):
+        """
+        Polymorph this model into a proxy model subclass.
+        """
+        if self.__class__ != ContentBlockField:
+            # Don't polymorph more than once.
+            return
+
+        for subclass in ContentBlockField.__subclasses__():
+            if self.field_type == subclass.__name__:
+                self.__class__ = subclass
+                return
+
+        raise PolymorphError(f"{self} has no subclass {self.field_type}.")
+
     @staticmethod
     def form_field_wrapper(form_field):
         """
         Wraps the form_field.__get__ method and adds common attributes to all fields.
         :param form_field: the form_field.__get__ method we are wrapping
         """
 
+        @functools.wraps(form_field)
         def wrapper(self):
             field = form_field(self)
             if field is not None:
                 field.cb_field = self
 
             return field
 
@@ -464,54 +493,68 @@
     def context_value(self):
         """
         :return: Nested content blocks which we can then call render or access context on.
         """
         return self.content_blocks.nested()
 
 
-class ContentBlockManager(VisibleManager):
-    # todo consider moving some of these to service classes. Only need to keep those used in templates here?
-    def get_queryset(self):
-        """
-        Basic optimisation.
-        """
+def optimise_queryset(func):
+    """
+    Decorator to optimise queryset.
+    Moved from ContentBlockManager.get_queryset to here such that dumpdata can run without the select_related which
+    causes it to fail when using natural_keys.
+    """
+
+    @functools.wraps(func)
+    def wrapper(self):
         return (
-            super()
-            .get_queryset()
+            func(self)
             .prefetch_related("content_block_fields")
             .select_related("content_block_template")
         )
 
+    return wrapper
+
+
+class ContentBlockManager(VisibleManager):
+    # todo consider moving some of these to service classes. Only need to keep those used in templates here?
+    #   Could also take more care with optimisation and only apply it when needed.
+
+    @optimise_queryset
     def visible(self):
         """
         Visible published only.
         Used in templates to render published content blocks.
         """
         return super().visible().filter(draft=False)
 
+    @optimise_queryset
     def previews(self):
         """
         Visible drafts only. Exclude those which haven't been saved via the editor yet (empties).
         Can be used in page previews.
         """
         return super().visible().filter(draft=True, saved=True)
 
+    @optimise_queryset
     def nested(self):
         """
         Used in the context for NestedField objects. Visible but with unsaved excluded.
         """
         return super().visible().filter(draft=False, saved=True)
 
+    @optimise_queryset
     def published(self):
         """
         All published including visible=False.
         Used by the publishing/reset mechanism.
         """
         return self.get_queryset().filter(draft=False)
 
+    @optimise_queryset
     def drafts(self):
         """
         All drafts including visible=False.
         Used by the editor and publishing/reset mechanism.
         """
         return self.get_queryset().filter(draft=True)
 
@@ -654,16 +697,18 @@
     @property
     def template(self):
         if self.template_filename:
             return f"content_blocks/content_blocks/{self.template_filename}"
 
 
 class ContentBlockTemplateFieldManager(models.Manager):
-    def get_by_natural_key(self, key, content_block_template):
-        return self.get(key=key, content_block_template=content_block_template)
+    def get_by_natural_key(self, key, content_block_template_name):
+        return self.get(
+            key=key, content_block_template__name=content_block_template_name
+        )
 
 
 class ContentBlockTemplateField(PositionModel):
     """
     Content Block Template Field model.
     Used to define content block types.
     """
@@ -726,18 +771,17 @@
             )
         ]
 
     def __str__(self):
         return self.key or super().__str__()
 
     def natural_key(self):
-        return (
-            self.key,
-            self.content_block_template,
-        )
+        return (self.key,) + self.content_block_template.natural_key()
+
+    natural_key.dependencies = ["content_blocks.contentblocktemplate"]
 
 
 class ContentBlockAvailability(AutoDateModel):
     """
     Used to set which content block templates can be added to a model.
     """
```

### Comparing `django-content-blocks-1.3.2/content_blocks/services/content_block.py` & `django-content-blocks-1.3.3/content_blocks/services/content_block.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/services/content_block_parent.py` & `django-content-blocks-1.3.3/content_blocks/services/content_block_parent.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/services/content_block_template.py` & `django-content-blocks-1.3.3/content_blocks/services/content_block_template.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/content_block_template_admin.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_block_template_admin.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/css/content_blocks.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/css/content_blocks.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.3.3/content_blocks/static/content_blocks/js/popup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/.DS_Store` & `django-content-blocks-1.3.3/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/.DS_Store` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/base.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.3.3/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.3.3/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.3.3/content_blocks/templatetags/content_blocks.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/urls.py` & `django-content-blocks-1.3.3/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/views.py` & `django-content-blocks-1.3.3/content_blocks/views.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/content_blocks/widgets.py` & `django-content-blocks-1.3.3/content_blocks/widgets.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/django_content_blocks.egg-info/PKG-INFO` & `django-content-blocks-1.3.3/django_content_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.2
+Version: 1.3.3
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.2/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.3.3/django_content_blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.2/setup.cfg` & `django-content-blocks-1.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-content-blocks
-version = 1.3.2
+version = 1.3.3
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

