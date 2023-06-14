# Comparing `tmp/ckanext-googleanalytics-2.2.1.tar.gz` & `tmp/ckanext-googleanalytics-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-googleanalytics-2.2.1.tar", last modified: Tue Jan 17 19:21:24 2023, max compression
+gzip compressed data, was "ckanext-googleanalytics-2.2.2.tar", last modified: Fri Mar  3 00:18:16 2023, max compression
```

## Comparing `ckanext-googleanalytics-2.2.1.tar` & `ckanext-googleanalytics-2.2.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34520 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/LICENSE.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7595 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.645280 ckanext-googleanalytics-2.2.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      339 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      893 2023-01-17 19:20:31.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      178 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12223 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14202 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/commands.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2295 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3998 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/controller.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2948 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/dbutil.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1683 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/ga_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1229 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2556 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      462 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      800 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      700 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      136 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/model/base.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      476 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/flask_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5160 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/pylons_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      643 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.635279 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      446 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/googleanalytics_header.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1135 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1794 2023-01-17 19:19:58.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3614 2023-01-17 19:19:58.000000 ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1985 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      140 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-01-17 19:21:24.000000 ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2075 2023-01-17 19:21:24.685280 ckanext-googleanalytics-2.2.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-01-15 15:32:34.000000 ckanext-googleanalytics-2.2.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34520 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/LICENSE.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      149 2023-03-03 00:09:49.000000 ckanext-googleanalytics-2.2.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7595 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.731446 ckanext-googleanalytics-2.2.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      339 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.731446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.731446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      893 2023-03-03 00:17:03.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      178 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12223 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14202 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/commands.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2295 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      774 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3998 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/controller.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2948 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/dbutil.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1683 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/ga_auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1229 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2556 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      462 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      800 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      700 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      136 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/model/base.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      476 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/flask_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5160 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/pylons_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      643 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.731446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2022-08-23 13:42:03.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      446 2022-08-23 14:02:56.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 14:05:09.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/googleanalytics_header.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1135 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1794 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3614 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2033 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      140 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-03 00:18:16.000000 ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-08-23 22:53:50.000000 ckanext-googleanalytics-2.2.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2075 2023-03-03 00:18:16.741446 ckanext-googleanalytics-2.2.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.2/setup.py
```

### Comparing `ckanext-googleanalytics-2.2.1/LICENSE.txt` & `ckanext-googleanalytics-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/PKG-INFO` & `ckanext-googleanalytics-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalytics
-Version: 2.2.1
+Version: 2.2.2
 Summary: Add GA tracking and reporting to CKAN instance
 Home-page: https://github.com/ckan/ckanext-googleanalytics
 Author: Seb Bacon
 Author-email: seb.bacon@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-googleanalytics-2.2.1/README.md` & `ckanext-googleanalytics-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/cli.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/commands.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/commands.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/config.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/controller.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/controller.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/dbutil.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/dbutil.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/ga_auth.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/ga_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/helpers.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/action.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/logic/schema.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/model/__init__.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/__init__.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/plugin/pylons_plugin.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/plugin/pylons_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/base.html` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/conftest.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/tests/logic/test_action.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/utils.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext/googleanalytics/views.py` & `ckanext-googleanalytics-2.2.2/ckanext/googleanalytics/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/PKG-INFO` & `ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalytics
-Version: 2.2.1
+Version: 2.2.2
 Summary: Add GA tracking and reporting to CKAN instance
 Home-page: https://github.com/ckan/ckanext-googleanalytics
 Author: Seb Bacon
 Author-email: seb.bacon@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-googleanalytics-2.2.1/ckanext_googleanalytics.egg-info/SOURCES.txt` & `ckanext-googleanalytics-2.2.2/ckanext_googleanalytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/googleanalytics/__init__.py
 ckanext/googleanalytics/cli.py
 ckanext/googleanalytics/commands.py
 ckanext/googleanalytics/config.py
+ckanext/googleanalytics/config_declaration.yaml
 ckanext/googleanalytics/controller.py
 ckanext/googleanalytics/dbutil.py
 ckanext/googleanalytics/ga_auth.py
 ckanext/googleanalytics/helpers.py
 ckanext/googleanalytics/interfaces.py
 ckanext/googleanalytics/utils.py
 ckanext/googleanalytics/views.py
```

### Comparing `ckanext-googleanalytics-2.2.1/setup.cfg` & `ckanext-googleanalytics-2.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-googleanalytics
-version = 2.2.1
+version = 2.2.2
 description = Add GA tracking and reporting to CKAN instance
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ckan/ckanext-googleanalytics
 author = Seb Bacon
 author_email = seb.bacon@gmail.com
 license = AGPL
```

