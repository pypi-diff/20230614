# Comparing `tmp/django-dashboards-0.1.3.tar.gz` & `tmp/django-dashboards-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dashboards-0.1.3.tar", last modified: Tue May 23 11:55:44 2023, max compression
+gzip compressed data, was "django-dashboards-0.1.4.tar", last modified: Wed Jun 14 11:11:36 2023, max compression
```

## Comparing `django-dashboards-0.1.3.tar` & `django-dashboards-0.1.4.tar`

### file list

```diff
@@ -1,230 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/table/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/menus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.929654 django-dashboards-0.1.3/dashboards/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/static/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/css/
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/dashboards.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/buttons.css
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/cards.css
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/dashboards.css
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/forms.css
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/grid.css
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/layout.css
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/menu.css
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/js/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/js/dashboard.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/datatables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/alpine.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/datatables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.945654 django-dashboards-0.1.3/dashboards/templates/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/form/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/form/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/loading.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/html.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/stat.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/text.html
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/dashboard_partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/js.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/style.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/card.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/container.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/tab.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templatetags/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/django_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.953654 django-dashboards-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.953654 django-dashboards-0.1.3/docs/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.957655 django-dashboards-0.1.3/docs/dashboards/howto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/async_component.gif
--rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_add_form.png
--rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_chart_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_gauge.png
--rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_map_examples.png
--rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_table.png
--rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/dependent_table_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_basic.png
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_complex.png
--rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_chart.png
--rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_layout.png
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_component_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_loading.png
--rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_style.png
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/async.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/components/
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/included.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/dashboards.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/dynamic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/menus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/chart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/table.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/sse.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/docs_dj_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/app1/dashboards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/components/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_model_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/menu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/test_menutags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/views/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_form_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_form_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/meta/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/component/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/chart/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/form.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/component/gauge/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/gauge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/gauge/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/component/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/table/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/table/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/component/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/menus/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/menus/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.922099 django-dashboards-0.1.4/dashboards/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/static/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/static/dashboards/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/dashboards.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/buttons.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/cards.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/dashboards.css
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/gauge.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/layout.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/menu.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/css/src/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/static/dashboards/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/loading.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.922099 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.926100 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/css/datatables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.930100 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/alpine.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/datatables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/gauge.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.922099 django-dashboards-0.1.4/dashboards/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.930100 django-dashboards-0.1.4/dashboards/templates/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/chart/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/form/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/gauge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/gauge/gauge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/loading.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/map/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/table/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/table/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/components/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/text/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/text/stat.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/components/text/text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/dashboard_partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.922099 django-dashboards-0.1.4/dashboards/templates/dashboards/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/includes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/includes/static/js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/includes/static/style.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.922099 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/tabs/container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/tabs/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/tabs/tab.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/dashboards/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/templatetags/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/dashboards/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/django_dashboards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-14 11:11:36.000000 django-dashboards-0.1.4/django_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-06-14 11:11:36.000000 django-dashboards-0.1.4/django_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:11:36.000000 django-dashboards-0.1.4/django_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 11:11:36.000000 django-dashboards-0.1.4/django_dashboards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 11:11:36.000000 django-dashboards-0.1.4/django_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.934100 django-dashboards-0.1.4/docs/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.938099 django-dashboards-0.1.4/docs/dashboards/howto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/docs/dashboards/howto/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/async_component.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/components_add_form.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/components_chart_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/components_gauge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/components_map_examples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/components_table.png
+-rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/dependent_table_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/layout_basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/layout_complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/quickstart_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/quickstart_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/serializers_chart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/serializers_layout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_component_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_loading.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_style.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/async.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/docs/dashboards/howto/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/components/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/components/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/components/included.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/dashboards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/dynamic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/menus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/docs/dashboards/howto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/serializers/chart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/serializers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/serializers/table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/sse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/howto/views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/dashboards/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/docs_dj_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/app1/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/components/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/components/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.946099 django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/test_model_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/dashboard/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/tests/dashboards/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/menu/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/menu/test_menutags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/tests/dashboards/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_dashboard_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/tests/dashboards/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/tests/dashboards/views/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/snapshots/snap_test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/snapshots/snap_test_form_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/dashboards/views/test_form_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:36.950100 django-dashboards-0.1.4/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/meta/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 11:11:32.000000 django-dashboards-0.1.4/tests/utils.py
```

### Comparing `django-dashboards-0.1.3/LICENSE` & `django-dashboards-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/PKG-INFO` & `django-dashboards-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dashboards-0.1.3/README.rst` & `django-dashboards-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/base.py` & `django-dashboards-0.1.4/dashboards/component/base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/chart/chart.py` & `django-dashboards-0.1.4/dashboards/component/chart/chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/chart/serializers.py` & `django-dashboards-0.1.4/dashboards/component/chart/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,33 +58,45 @@
                 }
             }
         )
 
     @classmethod
     def serialize(cls, **kwargs) -> str:
         self = cls()
+        request = kwargs.get("request")
         df = self.get_data(**kwargs)
 
         if isinstance(df, pd.DataFrame) and df.empty:
             return self.empty_chart()
 
         fig = self.to_fig(df)
-        fig = self.apply_layout(fig)
+
+        fig = self.apply_layout(
+            fig, dark=request and request.COOKIES.get("appearanceMode") == "dark"
+        )
+
         return fig.to_json()
 
     def get_fields(self) -> Optional[List[str]]:
         # TODO: for some reason mypy complains about this one line
         return self._meta.fields  # type: ignore
 
-    def apply_layout(self, fig: go.Figure):
+    def apply_layout(self, fig: go.Figure, dark=False):
         layout = self.layout or {}
 
         for attr in self.meta_layout_attrs:
             layout.setdefault(attr, getattr(self._meta, attr))
 
+        if dark:
+            fig = fig.update_layout(
+                template="plotly_dark",
+                plot_bgcolor="rgba(0,0,0,0.05)",
+                paper_bgcolor="rgba(0,0,0,0.05)",
+            )
+
         return fig.update_layout(**layout)
 
     def convert_to_df(self, data: Any, columns: Optional[List] = None) -> pd.DataFrame:
         return pd.DataFrame(data, columns=columns)
 
     def get_data(self, *args, **kwargs) -> pd.DataFrame:
         fields = self.get_fields()
```

### Comparing `django-dashboards-0.1.3/dashboards/component/form.py` & `django-dashboards-0.1.4/dashboards/component/form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/layout.py` & `django-dashboards-0.1.4/dashboards/component/layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/map.py` & `django-dashboards-0.1.4/dashboards/component/map.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/table/mixins.py` & `django-dashboards-0.1.4/dashboards/component/table/mixins.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/table/serializers.py` & `django-dashboards-0.1.4/dashboards/component/table/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/table/table.py` & `django-dashboards-0.1.4/dashboards/component/table/table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/component/text.py` & `django-dashboards-0.1.4/dashboards/component/text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/config.py` & `django-dashboards-0.1.4/dashboards/config.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/dashboard.py` & `django-dashboards-0.1.4/dashboards/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/forms.py` & `django-dashboards-0.1.4/dashboards/forms.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/menus/menu.py` & `django-dashboards-0.1.4/dashboards/menus/menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/meta/__init__.py` & `django-dashboards-0.1.4/dashboards/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/permissions.py` & `django-dashboards-0.1.4/dashboards/permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/registry.py` & `django-dashboards-0.1.4/dashboards/registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/dashboards.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/dashboards.css`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
   --color-light-cta-hover-background: #404040;
   --color-light-cta-text: #fafafa;
   --color-light-cta-hover-text: var(--color-light-cta-text);
   --color-light-cta-alt-background: #a3a3a3;
   --color-light-cta-alt-hover-background: #fafafa;
   --color-light-cta-alt-text: #404040;
   --color-light-cta-alt-hover-text: var(--color-light-cta-alt-text);
+  --color-light-gauge-background: #a3a3a3;
+  --color-light-gauge-fill: #0284c7;
   --light-root-background: linear-gradient(to top right, var(--color-light-background-primary), var(--color-light-background-primary), var(--color-light-border));
   
   --color-dark-background-primary: #404040;
   --color-dark-background-secondary: #525252;
   --color-dark-background-tertiary: #737373;
   --color-dark-border: #737373;
   --color-dark-text-primary: #fafafa;
@@ -30,14 +32,16 @@
   --color-dark-cta-hover-background: #fafafa;
   --color-dark-cta-text: #404040;
   --color-dark-cta-hover-text: var(--color-dark-cta-text);
   --color-dark-cta-alt-background: #737373;
   --color-dark-cta-alt-hover-background: #404040;
   --color-dark-cta-alt-text: #fafafa;
   --color-dark-cta-alt-hover-text: var(--color-dark-cta-alt-text);
+  --color-dark-gauge-background: #e5e5e5;
+  --color-dark-gauge-fill: #38bdf8;
   --dark-root-background: linear-gradient(to top right, var(--color-dark-background-primary), var(--color-dark-background-primary), var(--color-dark-background-secondary));
   
   --color-background-primary: var(--color-light-background-primary);
   --color-background-secondary: var(--color-light-background-secondary);
   --color-background-tertiary: var(--color-light-background-tertiary);
   --color-border: var(--color-light-border);
   --color-text-primary: var(--color-light-text-primary);
@@ -47,14 +51,16 @@
   --color-cta-hover-background: var(--color-light-cta-hover-background);
   --color-cta-text: var(--color-light-cta-text);
   --color-cta-hover-text: var(--color-light-cta-hover-text);
   --color-cta-alt-background: var(--color-light-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-light-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-light-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-light-cta-alt-hover-text);
+  --color-gauge-background: var(--color-light-gauge-background);
+  --color-gauge-fill: var(--color-light-gauge-fill);
   --root-background: var(--light-root-background);
 }
 
 @media (prefers-color-scheme: dark) {
   :root {
     --color-background-primary: var(--color-dark-background-primary);
     --color-background-secondary: var(--color-dark-background-secondary);
@@ -67,14 +73,16 @@
     --color-cta-hover-background: var(--color-dark-cta-hover-background);
     --color-cta-text: var(--color-dark-cta-text);
     --color-cta-hover-text: var(--color-dark-cta-hover-text);
     --color-cta-alt-background: var(--color-dark-cta-alt-background);
     --color-cta-alt-hover-background: var(--color-dark-cta-alt-hover-background);
     --color-cta-alt-text: var(--color-dark-cta-alt-text);
     --color-cta-alt-hover-text: var(--color-dark-cta-alt-hover-text);
+    --color-gauge-background: var(--color-dark-gauge-background);
+    --color-gauge-fill: var(--color-dark-gauge-fill);
     --root-background: var(--dark-root-background);
   }
 }
 
 .light {
   --color-background-primary: var(--color-light-background-primary);
   --color-background-secondary: var(--color-light-background-secondary);
@@ -87,14 +95,16 @@
   --color-cta-hover-background: var(--color-light-cta-hover-background);
   --color-cta-text: var(--color-light-cta-text);
   --color-cta-hover-text: var(--color-light-cta-hover-text);
   --color-cta-alt-background: var(--color-light-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-light-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-light-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-light-cta-alt-hover-text);
+  --color-gauge-background: var(--color-light-gauge-background);
+  --color-gauge-fill: var(--color-light-gauge-fill);
   --root-background: var(--light-root-background);
 }
 
 .dark {
   --color-background-primary: var(--color-dark-background-primary);
   --color-background-secondary: var(--color-dark-background-secondary);
   --color-background-tertiary: var(--color-dark-background-tertiary);
@@ -106,14 +116,16 @@
   --color-cta-hover-background: var(--color-dark-cta-hover-background);
   --color-cta-text: var(--color-dark-cta-text);
   --color-cta-hover-text: var(--color-dark-cta-hover-text);
   --color-cta-alt-background: var(--color-dark-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-dark-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-dark-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-dark-cta-alt-hover-text);
+  --color-gauge-background: var(--color-dark-gauge-background);
+  --color-gauge-fill: var(--color-dark-gauge-fill);
   --root-background: var(--dark-root-background);
 }
 
 .btn {
   height: 2em;
   border-radius: 1em;
   text-align: center;
@@ -492,14 +504,62 @@
 }
 
 .span-12 {
   grid-column-end: span 12;
   grid-auto-rows: min-content;
 }
 
+.gauge-container {
+  display: block;
+  margin: auto;
+  position: relative;
+  width: 100%;
+}
+
+.gauge .dial {
+  stroke: var(--color-gauge-background);
+  stroke-width: 10;
+  opacity: 0.1;
+}
+
+.gauge .value {
+  stroke: var(--color-gauge-fill);
+  stroke-dasharray: none;
+  stroke-width: 10;
+}
+
+.gauge-title-text {
+  color: var(--color-text-primary);
+  text-align: center;
+  display: inline-block;
+  width: 100%;
+  font-size: 10vw;
+}
+
+.gauge-value-text {
+  color: var(--color-text-primary);
+  text-align: center;
+  display: inline-block;
+  width: 100%;
+}
+
+.gauge-sub-text {
+  color: var(--color-text-secondary);
+  display: inline-block;
+  font-size: .8rem;
+}
+
+.gauge-content {
+  position: absolute;
+  margin: auto;
+  top: 50%;
+  left: 50%;
+  transform: translate(-50%, -50%);
+}
+
 .dashboard-container {
   display: grid;
   grid-template-columns: repeat(12, 1fr);
   grid-gap: 1rem;
   gap: 1rem;
   text-align: center;
   width: 100%;
@@ -587,7 +647,11 @@
   font-size: 0.8em;
 }
 
 .gauge-container {
   margin: auto;
   max-width: 65%;
 }
+
+.loading-img{
+  padding: 5em;
+}
```

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/buttons.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/buttons.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/cards.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/cards.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/dashboards.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/dashboards.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/forms.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/forms.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/grid.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/grid.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/layout.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/layout.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/menu.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/menu.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/theme.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/css/src/theme.css`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
   --color-light-cta-hover-background: #404040;
   --color-light-cta-text: #fafafa;
   --color-light-cta-hover-text: var(--color-light-cta-text);
   --color-light-cta-alt-background: #a3a3a3;
   --color-light-cta-alt-hover-background: #fafafa;
   --color-light-cta-alt-text: #404040;
   --color-light-cta-alt-hover-text: var(--color-light-cta-alt-text);
+  --color-light-gauge-background: #a3a3a3;
+  --color-light-gauge-fill: #0284c7;
   --light-root-background: linear-gradient(to top right, var(--color-light-background-primary), var(--color-light-background-primary), var(--color-light-border));
   
   --color-dark-background-primary: #404040;
   --color-dark-background-secondary: #525252;
   --color-dark-background-tertiary: #737373;
   --color-dark-border: #737373;
   --color-dark-text-primary: #fafafa;
@@ -30,14 +32,16 @@
   --color-dark-cta-hover-background: #fafafa;
   --color-dark-cta-text: #404040;
   --color-dark-cta-hover-text: var(--color-dark-cta-text);
   --color-dark-cta-alt-background: #737373;
   --color-dark-cta-alt-hover-background: #404040;
   --color-dark-cta-alt-text: #fafafa;
   --color-dark-cta-alt-hover-text: var(--color-dark-cta-alt-text);
+  --color-dark-gauge-background: #e5e5e5;
+  --color-dark-gauge-fill: #38bdf8;
   --dark-root-background: linear-gradient(to top right, var(--color-dark-background-primary), var(--color-dark-background-primary), var(--color-dark-background-secondary));
   
   --color-background-primary: var(--color-light-background-primary);
   --color-background-secondary: var(--color-light-background-secondary);
   --color-background-tertiary: var(--color-light-background-tertiary);
   --color-border: var(--color-light-border);
   --color-text-primary: var(--color-light-text-primary);
@@ -47,14 +51,16 @@
   --color-cta-hover-background: var(--color-light-cta-hover-background);
   --color-cta-text: var(--color-light-cta-text);
   --color-cta-hover-text: var(--color-light-cta-hover-text);
   --color-cta-alt-background: var(--color-light-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-light-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-light-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-light-cta-alt-hover-text);
+  --color-gauge-background: var(--color-light-gauge-background);
+  --color-gauge-fill: var(--color-light-gauge-fill);
   --root-background: var(--light-root-background);
 }
 
 @media (prefers-color-scheme: dark) {
   :root {
     --color-background-primary: var(--color-dark-background-primary);
     --color-background-secondary: var(--color-dark-background-secondary);
@@ -67,14 +73,16 @@
     --color-cta-hover-background: var(--color-dark-cta-hover-background);
     --color-cta-text: var(--color-dark-cta-text);
     --color-cta-hover-text: var(--color-dark-cta-hover-text);
     --color-cta-alt-background: var(--color-dark-cta-alt-background);
     --color-cta-alt-hover-background: var(--color-dark-cta-alt-hover-background);
     --color-cta-alt-text: var(--color-dark-cta-alt-text);
     --color-cta-alt-hover-text: var(--color-dark-cta-alt-hover-text);
+    --color-gauge-background: var(--color-dark-gauge-background);
+    --color-gauge-fill: var(--color-dark-gauge-fill);
     --root-background: var(--dark-root-background);
   }
 }
 
 .light {
   --color-background-primary: var(--color-light-background-primary);
   --color-background-secondary: var(--color-light-background-secondary);
@@ -87,14 +95,16 @@
   --color-cta-hover-background: var(--color-light-cta-hover-background);
   --color-cta-text: var(--color-light-cta-text);
   --color-cta-hover-text: var(--color-light-cta-hover-text);
   --color-cta-alt-background: var(--color-light-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-light-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-light-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-light-cta-alt-hover-text);
+  --color-gauge-background: var(--color-light-gauge-background);
+  --color-gauge-fill: var(--color-light-gauge-fill);
   --root-background: var(--light-root-background);
 }
 
 .dark {
   --color-background-primary: var(--color-dark-background-primary);
   --color-background-secondary: var(--color-dark-background-secondary);
   --color-background-tertiary: var(--color-dark-background-tertiary);
@@ -106,9 +116,11 @@
   --color-cta-hover-background: var(--color-dark-cta-hover-background);
   --color-cta-text: var(--color-dark-cta-text);
   --color-cta-hover-text: var(--color-dark-cta-hover-text);
   --color-cta-alt-background: var(--color-dark-cta-alt-background);
   --color-cta-alt-hover-background: var(--color-dark-cta-alt-hover-background);
   --color-cta-alt-text: var(--color-dark-cta-alt-text);
   --color-cta-alt-hover-text: var(--color-dark-cta-alt-hover-text);
+  --color-gauge-background: var(--color-dark-gauge-background);
+  --color-gauge-fill: var(--color-dark-gauge-fill);
   --root-background: var(--dark-root-background);
 }
```

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/js/dashboard.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/datatables.min.css` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/alpine.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/datatables.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.sse.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/htmx.sse.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/jquery.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/plotly.min.js` & `django-dashboards-0.1.4/dashboards/static/dashboards/vendor/js/plotly.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/base.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/base.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/chart.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/chart/chart.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/component.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/component.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/form/form.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/form/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,9 @@
           </td>
         </tr>
       {% endif %}
       </tbody>
     </table>
     {% for field in hidden_fields %}{{ field }}{% endfor %}
   </form>
-  {% endwith %}}
+  {% endwith %}
 {% endspaceless %}
```

#### html2text {}

```diff
@@ -5,8 +5,8 @@
 swap="outerHTML" hx-target="#component-{{ component.template_id }}-inner"> {
 { ctx.errors }}
 {{ field.label_tag}}
 {% if field.help_text %}{{ field.help_text|safe }}{% endif %} { {{ field }}
 { errors }}
                                                                [Submit]
 {% for field in hidden_fields %}{{ field }}{% endfor %}
-{% endwith %}} {% endspaceless %}
+{% endwith %} {% endspaceless %}
```

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/map.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/map/map.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/basic.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/table/basic.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/index.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/table/index.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/stat.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/components/text/stat.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/dashboard.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/dashboard.html`

 * *Files 14% similar despite different names*

```diff
@@ -13,44 +13,50 @@
 {% endblock %}
 
 {% block content %}
 {% dashboard_menus %}
 {% if sections.items %}
 <div class="menu-card">
     <div class="bumper"></div>
+    {% block navigation %}
     <nav role="navigation">
         <ul class="menu">
             {% for section, items in sections.items %}
             <li class="{% if section == active_section %}active{% endif %}">
-                <a href="#">{{ section }}</a>
-                <ul class="dropdown">
-                    {% for item in items %}
-                    <li class="{% if item.selected %}active{% endif %}">
-                        <a href="{{ item.url }}">{{ item.title }}</a>
-                    </li>
-                    {% endfor %}
-                </ul>
+                {% if items|length > 1 %}
+                    <a href="#">{{ section }}</a>
+                    <ul class="dropdown">
+                        {% for item in items %}
+                        <li class="{% if item.selected %}active{% endif %}">
+                            <a href="{{ item.url }}">{{ item.title }}</a>
+                        </li>
+                        {% endfor %}
+                    </ul>
+                {% else %}
+                    <a href="{{ items.0.url }}">{{ section }}</a>
+                {% endif %}
             </li>
             {% endfor %}
             <li>
                 <a href="#">☼</a>
                 <ul class="dropdown">
                     <li class="{% if request.COOKIES.appearanceMode == 'light' %}active{% endif %}">
-                        <a href="#" onclick="Dashboard.setAppearance('light')">☼ light</a>
+                        <a href="#" onclick="Dashboard.setAppearance('light'); location.reload();">☼ light</a>
                     </li>
                     <li class="{% if request.COOKIES.appearanceMode == 'dark' %}active{% endif %}">
-                        <a href="#" onclick="Dashboard.setAppearance('dark')">☾ dark</a>
+                        <a href="#" onclick="Dashboard.setAppearance('dark'); location.reload();">☾ dark</a>
                     </li>
                     <li class="{% if not request.COOKIES.appearanceMode %}active{% endif %}">
-                        <a href="#" onclick="Dashboard.setAppearance(null)">🖳 system</a>
+                        <a href="#" onclick="Dashboard.setAppearance(null); location.reload();">🖳 system</a>
                     </li>
                 </ul>
             </li>
         </ul>
     </nav>
+    {% endblock navigation %}
     <div class="bumper"></div>
 </div>
 {% endif %}
 <div class="dashboard-container">
     {% render_dashboard dashboard %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
 {% extends "dashboards/base.html" %} {% load static %} {% load dashboards %} {%
 block dashboards_js %} {{ block.super }} {% include "dashboards/includes/
 static/js.html" %} {% endblock %} {% block dashboards_style %} {{ block.super
 }} {% include "dashboards/includes/static/style.html" %} {% endblock %} {%
 block content %} {% dashboard_menus %} {% if sections.items %}
+{% block navigation %}
     * {% for section, items in sections.items %}
-    * {{_section_}}
+    * {% if items|length > 1 %} {{_section_}}
           o {% for item in items %}
           o {{_item.title_}}
           o {% endfor %}
+      {% else %} {{_section_}} {% endif %}
     * {% endfor %}
     * â¼
           o â¼_light
           o â¾_dark
           o ð³_system
+ {% endblock navigation %}
 {% endif %}
 {% render_dashboard dashboard %}
 {% endblock %}
```

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/js.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/includes/static/js.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load static %}
 <script src="{% static 'dashboards/js/dashboard.js' %}"></script>
 <script src="{% static 'dashboards/vendor/js/htmx.min.js' %}"></script>
 <script src="{% static 'dashboards/vendor/js/htmx.sse.min.js' %}"></script>
 <script src="{% static 'dashboards/vendor/js/alpine.min.js' %}" defer></script>
 <script src="{% static 'dashboards/vendor/js/plotly.min.js' %}"></script>
 <script src="{% static 'dashboards/vendor/js/jquery.min.js' %}"></script>
-<script src="{% static 'dashboards/vendor/js/datatables.min.js' %}"></script>
+<script src="{% static 'dashboards/vendor/js/datatables.min.js' %}"></script>
+<script src="{% static 'dashboards/vendor/js/gauge.min.js' %}"></script>
```

### Comparing `django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/card.html` & `django-dashboards-0.1.4/dashboards/templates/dashboards/layout/components/card.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/templatetags/dashboards.py` & `django-dashboards-0.1.4/dashboards/templatetags/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/urls.py` & `django-dashboards-0.1.4/dashboards/urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/dashboards/views.py` & `django-dashboards-0.1.4/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/django_dashboards.egg-info/PKG-INFO` & `django-dashboards-0.1.4/django_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dashboards-0.1.3/django_dashboards.egg-info/SOURCES.txt` & `django-dashboards-0.1.4/django_dashboards.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,48 +22,54 @@
 dashboards/component/form.py
 dashboards/component/layout.py
 dashboards/component/map.py
 dashboards/component/text.py
 dashboards/component/chart/__init__.py
 dashboards/component/chart/chart.py
 dashboards/component/chart/serializers.py
+dashboards/component/gauge/__init__.py
+dashboards/component/gauge/gauge.py
 dashboards/component/table/__init__.py
 dashboards/component/table/mixins.py
 dashboards/component/table/serializers.py
 dashboards/component/table/table.py
 dashboards/menus/__init__.py
 dashboards/menus/menu.py
 dashboards/menus/registry.py
 dashboards/meta/__init__.py
+dashboards/static/dashboards/loading.svg
 dashboards/static/dashboards/css/dashboards.css
 dashboards/static/dashboards/css/src/buttons.css
 dashboards/static/dashboards/css/src/cards.css
 dashboards/static/dashboards/css/src/dashboards.css
 dashboards/static/dashboards/css/src/forms.css
+dashboards/static/dashboards/css/src/gauge.css
 dashboards/static/dashboards/css/src/grid.css
 dashboards/static/dashboards/css/src/index.css
 dashboards/static/dashboards/css/src/layout.css
 dashboards/static/dashboards/css/src/menu.css
 dashboards/static/dashboards/css/src/theme.css
 dashboards/static/dashboards/js/dashboard.js
 dashboards/static/dashboards/vendor/css/datatables.min.css
 dashboards/static/dashboards/vendor/js/alpine.min.js
 dashboards/static/dashboards/vendor/js/datatables.min.js
+dashboards/static/dashboards/vendor/js/gauge.min.js
 dashboards/static/dashboards/vendor/js/htmx.min.js
 dashboards/static/dashboards/vendor/js/htmx.sse.min.js
 dashboards/static/dashboards/vendor/js/jquery.min.js
 dashboards/static/dashboards/vendor/js/plotly.min.js
 dashboards/templates/dashboards/base.html
 dashboards/templates/dashboards/dashboard.html
 dashboards/templates/dashboards/dashboard_partial.html
 dashboards/templates/dashboards/components/component.html
 dashboards/templates/dashboards/components/loading.html
 dashboards/templates/dashboards/components/partial.html
 dashboards/templates/dashboards/components/chart/chart.html
 dashboards/templates/dashboards/components/form/form.html
+dashboards/templates/dashboards/components/gauge/gauge.html
 dashboards/templates/dashboards/components/map/map.html
 dashboards/templates/dashboards/components/table/basic.html
 dashboards/templates/dashboards/components/table/index.html
 dashboards/templates/dashboards/components/text/html.html
 dashboards/templates/dashboards/components/text/stat.html
 dashboards/templates/dashboards/components/text/text.html
 dashboards/templates/dashboards/includes/static/js.html
@@ -139,20 +145,22 @@
 tests/dashboards/test_urls.py
 tests/dashboards/app1/__init__.py
 tests/dashboards/app1/dashboards.py
 tests/dashboards/components/__init__.py
 tests/dashboards/components/test_base.py
 tests/dashboards/components/test_chart.py
 tests/dashboards/components/test_form.py
+tests/dashboards/components/test_gauge.py
 tests/dashboards/components/test_table.py
 tests/dashboards/components/test_text.py
 tests/dashboards/components/snapshots/__init__.py
 tests/dashboards/components/snapshots/snap_test_base.py
 tests/dashboards/components/snapshots/snap_test_chart.py
 tests/dashboards/components/snapshots/snap_test_form.py
+tests/dashboards/components/snapshots/snap_test_gauge.py
 tests/dashboards/components/snapshots/snap_test_table.py
 tests/dashboards/components/snapshots/snap_test_text.py
 tests/dashboards/dashboard/__init__.py
 tests/dashboards/dashboard/test_dashboard.py
 tests/dashboards/dashboard/test_form.py
 tests/dashboards/dashboard/test_layout.py
 tests/dashboards/dashboard/test_model_dashboard.py
```

### Comparing `django-dashboards-0.1.3/docs/Makefile` & `django-dashboards-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/conf.py` & `django-dashboards-0.1.4/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "django-dashboards"
 copyright = "2023, Wildfish"
 author = "Wildfish"
-release = "0.1.3"
+release = "0.1.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
```

### Comparing `django-dashboards-0.1.3/docs/contributing.rst` & `django-dashboards-0.1.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/async_component.gif` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/async_component.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_add_form.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/components_add_form.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_chart_example.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/components_chart_example.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_gauge.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/components_gauge.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_map_examples.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/components_map_examples.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_table.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/components_table.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/demo.gif` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/dependent_table_dashboard.gif` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/dependent_table_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_basic.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/layout_basic.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_complex.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/layout_complex.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.gif` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/quickstart_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/quickstart_dashboard.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_chart.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/serializers_chart.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_layout.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/serializers_layout.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_component_template.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_component_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_loading.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_loading.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_template.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_custom_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_style.png` & `django-dashboards-0.1.4/docs/dashboards/howto/_images/templates_style.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/async.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/async.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/components/attributes.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/components/attributes.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/components/custom.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/components/custom.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/components/included.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/components/included.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/components/index.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/components/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/dashboards.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/dashboards.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/demo.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/demo.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/dynamic.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/dynamic.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/layout.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/layout.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/menus.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/menus.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/permissions.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/quickstart.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/serializers/chart.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/serializers/chart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/serializers/table.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/serializers/table.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/settings.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/settings.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/sse.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/sse.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/templates.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/templates.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/howto/views.rst` & `django-dashboards-0.1.4/docs/dashboards/howto/views.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/dashboards/index.rst` & `django-dashboards-0.1.4/docs/dashboards/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/docs_dj_settings.py` & `django-dashboards-0.1.4/docs/docs_dj_settings.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/index.rst` & `django-dashboards-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/make.bat` & `django-dashboards-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/docs/requirements.txt` & `django-dashboards-0.1.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/setup.cfg` & `django-dashboards-0.1.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dashboards
-version = 0.1.3
+version = 0.1.4
 description = Tools for building data dashboards with Django
 long_description = file: README.rst
 url = https://github.com/wildfish/django-dashboards
 author = Wildfish
 author_email = developers@wildfish.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-dashboards-0.1.3/tests/conftest.py` & `django-dashboards-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/app1/dashboards.py` & `django-dashboards-0.1.4/tests/dashboards/app1/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_base.py` & `django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -308,15 +308,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
@@ -324,15 +327,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
@@ -340,15 +346,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
```

#### html2text {}

```diff
@@ -13,17 +13,17 @@
 """ snapshots[ "test_render[False-component_kwargs2-Text] 1" ] = """
 value
 """ snapshots[ "test_render[True-component_kwargs0-Chart] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs0-Stat] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs0-Text] 1" ] = """
 value
 """ snapshots[ "test_render[True-component_kwargs1-Chart] 1" ] = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_render[True-component_kwargs1-Stat] 1" ] = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_render[True-component_kwargs1-Text] 1" ] = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_render[True-component_kwargs2-Chart] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs2-Stat] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs2-Text] 1" ] = """
 value
 """
```

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_chart.py` & `django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_form.py` & `django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 
     
         <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             
 <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><td><label for="id_number">Number:</label><br></td><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
-  }
         </div>
     
 
 
 """
 
 snapshots[
@@ -30,13 +29,12 @@
 
 
 
     
         <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             
 <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><td><label for="id_number">Number:</label><br></td><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
-  }
         </div>
     
 
 
 """
```

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_table.py` & `django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
@@ -353,15 +356,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 """ snapshots[ "test_render[False-component_kwargs1-BasicTable] 1" ] = """
 """ snapshots[ "test_render[False-component_kwargs1-Table] 1" ] = """
 """ snapshots[ "test_render[False-component_kwargs2-BasicTable] 1" ] = """
 """ snapshots[ "test_render[False-component_kwargs2-Table] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs0-BasicTable] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs0-Table] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs1-BasicTable] 1" ] = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_render[True-component_kwargs1-Table] 1" ] = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_render[True-component_kwargs2-BasicTable] 1" ] = """
 """ snapshots[ "test_render[True-component_kwargs2-Table] 1" ] = """
 """
```

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_text.py` & `django-dashboards-0.1.4/tests/dashboards/components/snapshots/snap_test_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,15 +148,18 @@
 ] = """
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/test/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
```

#### html2text {}

```diff
@@ -18,13 +18,13 @@
  ↑ Change  increase
 """ snapshots[ "test_stat_component__renders_value[True-component_kwargs0] 1" ]
 = """
 ***** 100% *****
 increase
 """ snapshots[ "test_stat_component__renders_value[True-component_kwargs1] 1" ]
 = """
-Loading...
+[/static/dashboards/loading.svg]
 """ snapshots[ "test_stat_component__renders_value[True-component_kwargs2] 1" ]
 = """
 ***** 100% *****
  ↑ Change  increase
 """
```

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/test_base.py` & `django-dashboards-0.1.4/tests/dashboards/components/test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/test_chart.py` & `django-dashboards-0.1.4/tests/dashboards/components/test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/test_form.py` & `django-dashboards-0.1.4/tests/dashboards/components/test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/test_table.py` & `django-dashboards-0.1.4/tests/dashboards/components/test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/components/test_text.py` & `django-dashboards-0.1.4/tests/dashboards/components/test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_form.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/snap_test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_layout.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/snapshots/snap_test_layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,18 @@
   
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/component_2/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 
 </div>
 </div>"""
@@ -184,15 +187,18 @@
 
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/component_2/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
 
 
 """
 
 snapshots[
@@ -213,15 +219,18 @@
 
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/component_2/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
-            Loading...
+            
+<div class="loading-img">
+    <img src="/static/dashboards/loading.svg" />
+</div>
         </div>
     </div>
```

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/test_dashboard.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/test_layout.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/test_model_dashboard.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/test_model_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/dashboard/test_permissions.py` & `django-dashboards-0.1.4/tests/dashboards/dashboard/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/fixtures.py` & `django-dashboards-0.1.4/tests/dashboards/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/menu/test_menu.py` & `django-dashboards-0.1.4/tests/dashboards/menu/test_menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/menu/test_menutags.py` & `django-dashboards-0.1.4/tests/dashboards/menu/test_menutags.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard_form.py` & `django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_dashboard_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_layout.py` & `django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_schema.py` & `django-dashboards-0.1.4/tests/dashboards/snapshots/snap_test_schema.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/test_registry.py` & `django-dashboards-0.1.4/tests/dashboards/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/test_urls.py` & `django-dashboards-0.1.4/tests/dashboards/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_component.py` & `django-dashboards-0.1.4/tests/dashboards/views/snapshots/snap_test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_dashboard.py` & `django-dashboards-0.1.4/tests/dashboards/views/snapshots/snap_test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/views/test_component.py` & `django-dashboards-0.1.4/tests/dashboards/views/test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/views/test_dashboard.py` & `django-dashboards-0.1.4/tests/dashboards/views/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/dashboards/views/test_form_component.py` & `django-dashboards-0.1.4/tests/dashboards/views/test_form_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/meta/test_meta.py` & `django-dashboards-0.1.4/tests/meta/test_meta.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.3/tests/settings.py` & `django-dashboards-0.1.4/tests/settings.py`

 * *Files identical despite different names*

