# Comparing `tmp/ckanext-googleanalytics-2.2.3.tar.gz` & `tmp/ckanext-googleanalytics-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-googleanalytics-2.2.3.tar", last modified: Wed Jun 14 12:52:24 2023, max compression
+gzip compressed data, was "ckanext-googleanalytics-2.3.0.tar", last modified: Wed Jun 14 17:30:14 2023, max compression
```

## Comparing `ckanext-googleanalytics-2.2.3.tar` & `ckanext-googleanalytics-2.3.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34520 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/LICENSE.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      149 2023-03-03 00:09:49.000000 ckanext-googleanalytics-2.2.3/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7595 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.216556 ckanext-googleanalytics-2.2.3/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      339 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.216556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.216556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      893 2023-03-03 00:17:03.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      178 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12223 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14202 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/commands.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2759 2023-06-14 12:49:44.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1823 2023-06-14 12:44:58.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3998 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/controller.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2948 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/dbutil.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1683 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/ga_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1229 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2556 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      462 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      800 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      700 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      136 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/model/base.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2141 2023-06-14 12:35:50.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      476 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/flask_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5160 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/pylons_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      643 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.216556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2022-08-23 13:42:03.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      666 2023-06-14 12:10:32.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 14:05:09.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/googleanalytics_header.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1135 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1794 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3556 2023-06-14 12:24:57.000000 ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2033 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      140 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 12:52:24.000000 ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-08-23 22:53:50.000000 ckanext-googleanalytics-2.2.3/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2075 2023-06-14 12:52:24.226556 ckanext-googleanalytics-2.2.3/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.2.3/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34520 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/LICENSE.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      149 2023-03-03 00:09:49.000000 ckanext-googleanalytics-2.3.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7595 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      339 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      893 2023-03-03 00:17:03.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      178 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12223 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14202 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/commands.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3080 2023-06-14 16:39:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1929 2023-06-14 15:27:28.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3998 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/controller.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2948 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/dbutil.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1683 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/ga_auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1338 2023-06-14 15:18:56.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2022-12-13 02:17:08.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2556 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      462 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      800 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      700 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      136 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/model/base.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2141 2023-06-14 12:35:50.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      476 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/flask_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5160 2022-10-14 07:43:46.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/pylons_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      643 2023-06-14 15:22:48.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.978816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2022-08-23 13:42:03.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      666 2023-06-14 12:10:32.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      430 2023-06-14 15:15:40.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtm.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 14:05:09.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/googleanalytics_header.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      618 2023-06-14 15:23:16.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1135 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1299 2022-08-23 22:54:33.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      397 2023-06-14 17:28:09.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/test_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1064 2023-06-14 17:26:09.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/test_view.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2288 2023-06-14 15:44:13.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3715 2023-06-14 15:43:18.000000 ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2234 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      279 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      140 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-14 17:30:13.000000 ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-08-23 22:53:50.000000 ckanext-googleanalytics-2.3.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       89 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2075 2023-06-14 17:30:13.988816 ckanext-googleanalytics-2.3.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-08-23 11:41:12.000000 ckanext-googleanalytics-2.3.0/setup.py
```

### Comparing `ckanext-googleanalytics-2.2.3/LICENSE.txt` & `ckanext-googleanalytics-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/PKG-INFO` & `ckanext-googleanalytics-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalytics
-Version: 2.2.3
+Version: 2.3.0
 Summary: Add GA tracking and reporting to CKAN instance
 Home-page: https://github.com/ckan/ckanext-googleanalytics
 Author: Seb Bacon
 Author-email: seb.bacon@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-googleanalytics-2.2.3/README.md` & `ckanext-googleanalytics-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/assets/googleanalytics_event_tracking.js`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/cli.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/commands.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/commands.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/config.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import ast
 import logging
 
 from werkzeug.utils import import_string
 
 import ckan.plugins.toolkit as tk
 
+CONFIG_TRACKING_ID = "googleanalytics.id"
 CONFIG_HANDLER_PATH = "googleanalytics.download_handler"
+CONFIG_TRACKING_MODE = "googleanalytics.tracking_mode"
 
 DEFAULT_RESOURCE_URL_TAG = "/downloads/"
 DEFAULT_RECENT_VIEW_DAYS = 14
 
 
 log = logging.getLogger(__name__)
 
@@ -26,29 +28,32 @@
     else:
         handler = None
         log.warning(("Missing {} config option.").format(CONFIG_HANDLER_PATH))
 
     return handler
 
 
-
 def tracking_mode():
-    # type: () -> Literal["ga", "gtag"]
-    type_ = tk.config.get("googleanalytics.tracking_mode")
+    # type: () -> Literal["ga", "gtag", "gtm"]
+    type_ = tk.config.get(CONFIG_TRACKING_MODE)
     if type_:
         return type_
 
     id_ = tracking_id()
 
     if id_.startswith("UA-"):
         return "ga"
 
     if id_.startswith("G-"):
         return "gtag"
 
+    if id_.startswith("GTM-"):
+        return "gtm"
+
+
     return "ga"
 
 
 def measurement_id():
     # type: () -> str
     """Set the MeasurementID for tracking API actions. By default,
     `googleanalytics.id` is used.
@@ -67,14 +72,21 @@
     return tk.config.get("googleanalytics.measurement_protocol.client_id")
 
 
 def measurement_protocol_client_secret():
     return tk.config.get("googleanalytics.measurement_protocol.client_secret")
 
 
+def measurement_protocol_track_downloads():
+    # type: () -> bool
+    return tk.asbool(
+        tk.config.get("googleanalytics.measurement_protocol.track_downloads")
+    )
+
+
 def account():
     return tk.config.get("googleanalytics.account")
 
 
 def profile_id():
     return tk.config.get("googleanalytics.profile_id")
```

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/controller.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/controller.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/dbutil.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/dbutil.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/ga_auth.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/ga_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/helpers.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import ckan.plugins.toolkit as tk
 from ckanext.googleanalytics import config
 
 
 def get_helpers():
     return {
         "googleanalytics_header": googleanalytics_header,
+        "googleanalytics_id": googleanalytics_id,
         "googleanalytics_resource_prefix": googleanalytics_resource_prefix,
         "googleanalytics_tracking_mode": googleanalytics_tracking_mode,
     }
 
 
 def googleanalytics_resource_prefix():
 
@@ -39,7 +40,10 @@
     return tk.render_snippet(
         "googleanalytics/snippets/googleanalytics_header.html", data
     )
 
 
 def googleanalytics_tracking_mode():
     return config.tracking_mode()
+
+def googleanalytics_id():
+    return config.tracking_id()
```

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/action.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/logic/schema.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/model/__init__.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/__init__.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/plugin/pylons_plugin.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/plugin/pylons_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/base.html` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/conftest.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/tests/logic/test_action.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/utils.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,58 +5,77 @@
 from six.moves.urllib.parse import urlencode
 from ckanext.googleanalytics import config
 
 
 log = logging.getLogger(__name__)
 
 EVENT_API = "CKAN API Request"
+EVENT_DOWNLOAD = "CKAN Resource Download Request"
 
 
 def send_event(data):
     if isinstance(data, MeasurementProtocolData):
-        if data["event"] != EVENT_API:
-            log.warning("Only API event supported by Measurement Protocol at the moment")
-            return
-
-        return _mp_api_handler({
-            "action": data["object"],
-            "payload": data["payload"],
-        })
+        if data["event"] == EVENT_API:
+            return _mp_api_handler({
+                "action": data["object"],
+                "payload": data["payload"],
+            })
+
+        if data["event"] == EVENT_DOWNLOAD:
+            return _mp_download_handler({"payload": {
+                "resource_id": data["id"],
+            }})
 
+        log.warning("Only API and Download events supported by Measurement Protocol at the moment")
+        return
 
     return _ga_handler(data)
 
 
 class SafeJSONEncoder(json.JSONEncoder):
     def default(self, _):
         return None
 
 
 def _mp_api_handler(data_dict):
-
     log.debug(
         "Sending API event to Google Analytics using the Measurement Protocol: %s",
         data_dict
     )
+    _mp_event({
+        "name": data_dict["action"],
+        "params": data_dict["payload"]
+    })
+
+
+def _mp_download_handler(data_dict):
+    log.debug(
+        "Sending Downlaod event to Google Analytics using the Measurement Protocol: %s",
+        data_dict
+    )
+    _mp_event({
+        "name": "file_download",
+        "params": data_dict["payload"],
+    })
+
+
+def _mp_event(event):
     resp = requests.post(
         "https://www.google-analytics.com/mp/collect",
         params={
             "api_secret": config.measurement_protocol_client_secret(),
             "measurement_id": config.measurement_id()
         },
         data=json.dumps({
             "client_id": config.measurement_protocol_client_id(),
             "non_personalized_ads": False,
-            "events":[{
-                "name": data_dict["action"],
-                "params": data_dict["payload"]
-            }]
+            "events":[event]
         }, cls=SafeJSONEncoder)
     )
-    # breakpoint()
+
     if resp.status_code >= 300:
         log.error("Cannot post event: %s", resp)
 
 
 def _ga_handler(data_dict):
     data = urlencode(data_dict)
     log.debug("Sending API event to Google Analytics: %s", data)
```

### Comparing `ckanext-googleanalytics-2.2.3/ckanext/googleanalytics/views.py` & `ckanext-googleanalytics-2.3.0/ckanext/googleanalytics/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def download(id, resource_id, filename=None, package_type="dataset"):
     handler = config.download_handler()
     if not handler:
         log.debug("Use default CKAN callback for resource.download")
         handler = resource.download
     _post_analytics(
         g.user,
-        "CKAN Resource Download Request",
+        utils.EVENT_DOWNLOAD,
         "Resource",
         "Download",
         resource_id,
     )
     return handler(
         package_type=package_type,
         id=id,
@@ -86,22 +86,27 @@
         request_obj_type, request_function,
         request_id, request_payload=None
 ):
 
     from ckanext.googleanalytics.plugin import GoogleAnalyticsPlugin
 
     if config.tracking_id():
-        if config.measurement_protocol_client_id() and event_type == utils.EVENT_API:
+        mp_client_id = config.measurement_protocol_client_id()
+        if mp_client_id and (
+                event_type == utils.EVENT_API
+                or (event_type == utils.EVENT_DOWNLOAD and config.measurement_protocol_track_downloads())
+        ):
             data_dict = utils.MeasurementProtocolData({
                 "event": event_type,
                 "object": request_obj_type,
                 "function": request_function,
                 "id": request_id,
                 "payload": request_payload,
             })
+
         else:
             data_dict = utils.UniversalAnalyticsData({
                 "v": 1,
                 "tid": config.tracking_id(),
                 "cid": hashlib.md5(six.ensure_binary(tk.c.user)).hexdigest(),
                 # customer id should be obfuscated
                 "t": "event",
```

### Comparing `ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/PKG-INFO` & `ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-googleanalytics
-Version: 2.2.3
+Version: 2.3.0
 Summary: Add GA tracking and reporting to CKAN instance
 Home-page: https://github.com/ckan/ckanext-googleanalytics
 Author: Seb Bacon
 Author-email: seb.bacon@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ckanext-googleanalytics-2.2.3/ckanext_googleanalytics.egg-info/SOURCES.txt` & `ckanext-googleanalytics-2.3.0/ckanext_googleanalytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,26 @@
 ckanext/googleanalytics/logic/schema.py
 ckanext/googleanalytics/model/__init__.py
 ckanext/googleanalytics/model/base.py
 ckanext/googleanalytics/plugin/__init__.py
 ckanext/googleanalytics/plugin/flask_plugin.py
 ckanext/googleanalytics/plugin/pylons_plugin.py
 ckanext/googleanalytics/templates/base.html
+ckanext/googleanalytics/templates/page.html
 ckanext/googleanalytics/templates/googleanalytics/snippets/_ga.html
 ckanext/googleanalytics/templates/googleanalytics/snippets/_gtag.html
+ckanext/googleanalytics/templates/googleanalytics/snippets/_gtm.html
 ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_asset.html
 ckanext/googleanalytics/templates/googleanalytics/snippets/event_tracking_resource.html
 ckanext/googleanalytics/templates/googleanalytics/snippets/googleanalytics_header.html
 ckanext/googleanalytics/tests/__init__.py
 ckanext/googleanalytics/tests/conftest.py
+ckanext/googleanalytics/tests/test_config.py
 ckanext/googleanalytics/tests/test_plugin.py
+ckanext/googleanalytics/tests/test_view.py
 ckanext/googleanalytics/tests/logic/__init__.py
 ckanext/googleanalytics/tests/logic/test_action.py
 ckanext_googleanalytics.egg-info/PKG-INFO
 ckanext_googleanalytics.egg-info/SOURCES.txt
 ckanext_googleanalytics.egg-info/dependency_links.txt
 ckanext_googleanalytics.egg-info/entry_points.txt
 ckanext_googleanalytics.egg-info/namespace_packages.txt
```

### Comparing `ckanext-googleanalytics-2.2.3/setup.cfg` & `ckanext-googleanalytics-2.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-googleanalytics
-version = 2.2.3
+version = 2.3.0
 description = Add GA tracking and reporting to CKAN instance
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ckan/ckanext-googleanalytics
 author = Seb Bacon
 author_email = seb.bacon@gmail.com
 license = AGPL
```

