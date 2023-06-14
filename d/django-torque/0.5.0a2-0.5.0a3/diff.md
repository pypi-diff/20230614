# Comparing `tmp/django-torque-0.5.0a2.tar.gz` & `tmp/django-torque-0.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-torque-0.5.0a2.tar", last modified: Sat Jun 10 11:47:21 2023, max compression
+gzip compressed data, was "django-torque-0.5.0a3.tar", last modified: Wed Jun 14 20:07:47 2023, max compression
```

## Comparing `django-torque-0.5.0a2.tar` & `django-torque-0.5.0a3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.454963 django-torque-0.5.0a2/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/django_torque.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3016 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-06-10 11:47:21.000000 django-torque-0.5.0a2/django_torque.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-06-10 11:47:21.454963 django-torque-0.5.0a2/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/apps.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/cache_rebuilder/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/cache_rebuilder/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/cache_rebuilder/apps.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6295 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/cache_rebuilder/background.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.434963 django-torque-0.5.0a2/torque/management/
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.438964 django-torque-0.5.0a2/torque/management/commands/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/management/commands/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/management/commands/remove_unattached.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-10 11:47:21.450963 django-torque-0.5.0a2/torque/migrations/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12576 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0001_initial.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      437 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0002_auto_20210321_1604.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      451 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0003_auto_20210321_1725.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      729 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0005_auto_20210323_1303.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      573 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0006_auto_20210323_1623.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      839 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0007_auto_20210406_1738.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      373 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0008_auto_20210406_1909.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0009_sheetconfig_search_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1360 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0010_tableofcontentscache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0011_auto_20210416_1739.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0012_searchcacherow_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0013_spreadsheet_last_updated.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      404 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0014_tableofcontentscache_rendered_html.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      364 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2472 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0016_auto_20210721_1444.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      661 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0017_auto_20210721_1621.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      303 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0018_delete_permissiongroup.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      825 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0019_auto_20210721_1720.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0020_tableofcontents_raw.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      326 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0021_remove_column_type.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      636 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0022_auto_20210905_1430.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      837 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0023_auto_20210905_1454.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      767 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0024_auto_20210905_1535.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      791 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0025_auto_20210905_1624.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      893 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0026_auto_20210905_1638.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1333 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0027_auto_20210905_1642.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1328 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0028_auto_20210905_1659.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2538 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0029_auto_20210905_1716.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      580 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0030_auto_20210927_1304.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      707 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0031_auto_20210930_1328.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      399 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0032_searchcachedocument_filtered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      877 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0033_csvspecification.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1643 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0034_auto_20220209_1209.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0035_template_in_config.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      803 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      472 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0037_template_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      521 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0038_wiki_linked_wiki_keys.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0039_document_attached.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      456 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/0040_value_unique_value_for_field_document.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      417 2023-03-28 11:03:24.000000 django-torque-0.5.0a2/torque/migrations/0041_searchcachedocument_explore_rank.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1245 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0042_documentdictcache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0043_documentdictcache_unique_document_dict.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      414 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0044_documentdictcache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      669 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0045_templatecachedocument_dirty_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0046_delete_templatecachedocument.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1585 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0047_templatecachedocument_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a2/torque/migrations/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    25665 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/models.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.5.0a2/torque/urls.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3489 2023-06-10 11:34:57.000000 django-torque-0.5.0a2/torque/utils.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       30 2023-06-10 11:44:02.000000 django-torque-0.5.0a2/torque/version.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    36146 2023-06-10 11:38:15.000000 django-torque-0.5.0a2/torque/views.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.998384 django-torque-0.5.0a3/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-14 20:07:46.998384 django-torque-0.5.0a3/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.998384 django-torque-0.5.0a3/django_torque.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-06-14 20:07:46.000000 django-torque-0.5.0a3/django_torque.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3016 2023-06-14 20:07:46.000000 django-torque-0.5.0a3/django_torque.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-06-14 20:07:46.000000 django-torque-0.5.0a3/django_torque.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2023-06-14 20:07:46.000000 django-torque-0.5.0a3/django_torque.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-06-14 20:07:46.000000 django-torque-0.5.0a3/django_torque.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-06-14 20:07:46.998384 django-torque-0.5.0a3/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-06-10 11:34:57.000000 django-torque-0.5.0a3/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.982384 django-torque-0.5.0a3/torque/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/apps.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.982384 django-torque-0.5.0a3/torque/cache_rebuilder/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/cache_rebuilder/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/cache_rebuilder/apps.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6668 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/cache_rebuilder/background.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.978384 django-torque-0.5.0a3/torque/management/
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.986384 django-torque-0.5.0a3/torque/management/commands/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/management/commands/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/management/commands/remove_unattached.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-06-14 20:07:46.998384 django-torque-0.5.0a3/torque/migrations/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12575 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0001_initial.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      436 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0002_auto_20210321_1604.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      450 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0003_auto_20210321_1725.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      728 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0005_auto_20210323_1303.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      572 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0006_auto_20210323_1623.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      838 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0007_auto_20210406_1738.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      372 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0008_auto_20210406_1909.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      402 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0009_sheetconfig_search_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1359 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0010_tableofcontentscache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0011_auto_20210416_1739.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0012_searchcacherow_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      397 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0013_spreadsheet_last_updated.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0014_tableofcontentscache_rendered_html.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      363 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2471 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0016_auto_20210721_1444.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      660 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0017_auto_20210721_1621.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      302 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0018_delete_permissiongroup.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      824 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0019_auto_20210721_1720.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0020_tableofcontents_raw.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0021_remove_column_type.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      635 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0022_auto_20210905_1430.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      836 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0023_auto_20210905_1454.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      766 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0024_auto_20210905_1535.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      790 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0025_auto_20210905_1624.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      892 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0026_auto_20210905_1638.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1332 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0027_auto_20210905_1642.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1327 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0028_auto_20210905_1659.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2537 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0029_auto_20210905_1716.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      579 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0030_auto_20210927_1304.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      706 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0031_auto_20210930_1328.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0032_searchcachedocument_filtered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      876 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0033_csvspecification.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1642 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0034_auto_20220209_1209.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      390 2023-06-14 20:04:53.000000 django-torque-0.5.0a3/torque/migrations/0035_template_in_config.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      802 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      471 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0037_template_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      520 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0038_wiki_linked_wiki_keys.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0039_document_attached.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      455 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0040_value_unique_value_for_field_document.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      416 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0041_searchcachedocument_explore_rank.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1244 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0042_documentdictcache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      460 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0043_documentdictcache_unique_document_dict.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      413 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0044_documentdictcache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      668 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0045_templatecachedocument_dirty_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      324 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0046_delete_templatecachedocument.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1584 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0047_templatecachedocument_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a3/torque/migrations/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    26216 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/models.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.5.0a3/torque/urls.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3524 2023-06-14 20:04:54.000000 django-torque-0.5.0a3/torque/utils.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       30 2023-06-14 20:05:25.000000 django-torque-0.5.0a3/torque/version.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    37505 2023-06-14 20:04:55.000000 django-torque-0.5.0a3/torque/views.py
```

### Comparing `django-torque-0.5.0a2/PKG-INFO` & `django-torque-0.5.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.0a2
+Version: 0.5.0a3
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.5.0a2/README.md` & `django-torque-0.5.0a3/README.md`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a2/django_torque.egg-info/PKG-INFO` & `django-torque-0.5.0a3/django_torque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.5.0a2
+Version: 0.5.0a3
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.5.0a2/django_torque.egg-info/SOURCES.txt` & `django-torque-0.5.0a3/django_torque.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a2/setup.py` & `django-torque-0.5.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a2/torque/cache_rebuilder/background.py` & `django-torque-0.5.0a3/torque/cache_rebuilder/background.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,41 +15,51 @@
         if config:
             # We do this outside of the transaction, because if someone comes
             # along and dirties it again while we're rebuilding, we want to
             # rebuild it after we're done rebuilding it.
             config.cache_dirty = False
             config.save()
 
-            print("Populating unbuilt template caches for %s in %s" % (config.group, config.wiki.wiki_key))
-            for view_template in models.Template.objects.filter(type="View", wiki=config.wiki):
+            print(
+                "Populating unbuilt template caches for %s in %s"
+                % (config.group, config.wiki.wiki_key)
+            )
+            for view_template in models.Template.objects.filter(
+                type="View", wiki=config.wiki
+            ):
                 config.populate_template_cache(view_template)
 
-            for search_template in models.Template.objects.filter(type="Search", wiki=config.wiki):
+            for search_template in models.Template.objects.filter(
+                type="Search", wiki=config.wiki
+            ):
                 config.populate_template_cache(search_template, True)
 
             print(
                 "Rebuilding search index for %s: %s"
                 % (config.wiki.wiki_key, config.group)
             )
             with transaction.atomic():
                 config.rebuild_search_index()
 
             return True
 
 
 class PropagateTemplateDirty:
     """When a template gets dirty, we need to update all the caches that depend on it"""
+
     def run(self):
         from torque import models
 
         for template in models.Template.objects.filter(dirty=True).all():
             template.dirty = False
             template.save()
 
-            models.TemplateCacheDocument.objects.filter(template=template).update(dirty=True)
+            models.TemplateCacheDocument.objects.filter(template=template).update(
+                dirty=True
+            )
 
             if template.type == "TOC":
                 models.TableOfContentsCache.objects.filter(
                     toc__in=template.collection.tables_of_contents.all()
                 ).update(dirty=True)
 
 
@@ -101,33 +111,46 @@
 
 class RebuildTemplateCacheDocuments:
     def run(self):
         from torque import models
 
         template_cache = models.TemplateCacheDocument.objects.filter(dirty=True).first()
         if template_cache:
-            print("Rebuilding template cache for (%s: %s), %s left" % (
-                template_cache.document_dict.wiki_config.wiki.wiki_key,
-                template_cache.document_dict.document.key,
-                models.TemplateCacheDocument.objects.filter(dirty=True).count()
-            ))
+            print(
+                "Rebuilding template cache for (%s: %s), %s left"
+                % (
+                    template_cache.document_dict.wiki_config.wiki.wiki_key,
+                    template_cache.document_dict.document.key,
+                    models.TemplateCacheDocument.objects.filter(dirty=True).count(),
+                )
+            )
 
-            for tc in models.TemplateCacheDocument.objects.filter(document_dict=template_cache.document_dict, dirty=True):
+            for tc in models.TemplateCacheDocument.objects.filter(
+                document_dict=template_cache.document_dict, dirty=True
+            ):
                 template_cache.rebuild()
 
             return True
 
 
 class CreateUnbuiltDocumentDicts:
     def run(self):
         from torque import models
 
         for wiki_config in models.WikiConfig.objects.all():
-            if wiki_config.valid_ids.count() != models.DocumentDictCache.objects.filter(document__in=wiki_config.valid_ids.all(), wiki_config=wiki_config).count():
-                print("Add unbuilt document dictionaries for %s in %s" % (wiki_config.group, wiki_config.wiki.wiki_key))
+            if (
+                wiki_config.valid_ids.count()
+                != models.DocumentDictCache.objects.filter(
+                    document__in=wiki_config.valid_ids.all(), wiki_config=wiki_config
+                ).count()
+            ):
+                print(
+                    "Add unbuilt document dictionaries for %s in %s"
+                    % (wiki_config.group, wiki_config.wiki.wiki_key)
+                )
                 wiki_config.rebuild_document_dict_cache()
                 return True
 
 
 class RebuildDocumentDicts:
     def run(self):
         from torque import models
@@ -150,20 +173,19 @@
 
         while True:
             try:
                 # We always want to do the dictionary caches if they exist,
                 # and for the rest of the caches, they shouldn't do very many just
                 # in case there's new document dict cache invalidation that's happened
                 (
-                    CreateUnbuiltDocumentDicts().run() or
-                    RebuildDocumentDicts().run() or
-                    RebuildWikiConfigs().run() or
-                    PropagateTemplateDirty().run() or
-                    RebuildSearchCacheDocuments().run() or
-                    RebuildTOCs().run() or
-                    RebuildTemplateCacheDocuments().run() or
-                    time.sleep(5)
+                    CreateUnbuiltDocumentDicts().run()
+                    or RebuildDocumentDicts().run()
+                    or RebuildWikiConfigs().run()
+                    or PropagateTemplateDirty().run()
+                    or RebuildSearchCacheDocuments().run()
+                    or RebuildTOCs().run()
+                    or RebuildTemplateCacheDocuments().run()
+                    or time.sleep(5)
                 )
             except:
                 print("Rebuilder failed a loop due to %s" % sys.exc_info()[0])
                 print(traceback.format_exc())
-
```

### Comparing `django-torque-0.5.0a2/torque/management/commands/remove_unattached.py` & `django-torque-0.5.0a3/torque/management/commands/remove_unattached.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a2/torque/migrations/0001_initial.py` & `django-torque-0.5.0a3/torque/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.2 on 2020-11-25 12:31
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Cell",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0005_auto_20210323_1303.py` & `django-torque-0.5.0a3/torque/migrations/0005_auto_20210323_1303.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.contrib.postgres.indexes
 import django.contrib.postgres.search
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0003_auto_20210321_1725"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="searchcacherow",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0006_auto_20210323_1623.py` & `django-torque-0.5.0a3/torque/migrations/0006_auto_20210323_1623.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.7 on 2021-03-23 16:23
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0005_auto_20210323_1303"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="sheetconfig",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0007_auto_20210406_1738.py` & `django-torque-0.5.0a3/torque/migrations/0007_auto_20210406_1738.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.7 on 2021-04-06 17:38
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0006_auto_20210323_1623"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="celledit",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0010_tableofcontentscache.py` & `django-torque-0.5.0a3/torque/migrations/0010_tableofcontentscache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.7 on 2021-04-16 17:17
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0009_sheetconfig_search_cache_dirty"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="TableOfContentsCache",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0016_auto_20210721_1444.py` & `django-torque-0.5.0a3/torque/migrations/0016_auto_20210721_1444.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.5 on 2021-07-21 14:44
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0015_remove_tableofcontentscache_rendered_data"),
     ]
 
     def create_wikis(apps, schema_editor):
         classes = [
             apps.get_model("torque", "Template"),
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0017_auto_20210721_1621.py` & `django-torque-0.5.0a3/torque/migrations/0017_auto_20210721_1621.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.5 on 2021-07-21 16:21
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0016_auto_20210721_1444"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="celledit",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0019_auto_20210721_1720.py` & `django-torque-0.5.0a3/torque/migrations/0019_auto_20210721_1720.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.5 on 2021-07-21 17:20
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0018_delete_permissiongroup"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="wiki",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0022_auto_20210905_1430.py` & `django-torque-0.5.0a3/torque/migrations/0022_auto_20210905_1430.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2021-09-05 14:30
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0021_remove_column_type"),
     ]
 
     operations = [
         migrations.RenameModel("Cell", "Value"),
         migrations.RenameModel("CellEdit", "ValueEdit"),
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0023_auto_20210905_1454.py` & `django-torque-0.5.0a3/torque/migrations/0023_auto_20210905_1454.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2021-09-05 14:54
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0022_auto_20210905_1430"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="value",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0024_auto_20210905_1535.py` & `django-torque-0.5.0a3/torque/migrations/0024_auto_20210905_1535.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2021-09-05 15:35
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0023_auto_20210905_1454"),
     ]
 
     operations = [
         migrations.RenameField(
             model_name="spreadsheet",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0025_auto_20210905_1624.py` & `django-torque-0.5.0a3/torque/migrations/0025_auto_20210905_1624.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2021-09-05 16:24
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0024_auto_20210905_1535"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="field",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0026_auto_20210905_1638.py` & `django-torque-0.5.0a3/torque/migrations/0026_auto_20210905_1638.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.contrib.postgres.indexes
 import django.contrib.postgres.search
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0025_auto_20210905_1624"),
     ]
 
     operations = [
         migrations.RenameModel("Row", "Document"),
         migrations.RenameModel("SearchCacheRow", "SearchCacheDocument"),
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0027_auto_20210905_1642.py` & `django-torque-0.5.0a3/torque/migrations/0027_auto_20210905_1642.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.contrib.postgres.indexes
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0026_auto_20210905_1638"),
     ]
 
     operations = [
         migrations.RemoveConstraint(
             model_name="attachment",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0028_auto_20210905_1659.py` & `django-torque-0.5.0a3/torque/migrations/0028_auto_20210905_1659.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.7 on 2021-09-05 16:59
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0027_auto_20210905_1642"),
     ]
 
     operations = [
         migrations.RenameModel(
             old_name="SheetConfig",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0029_auto_20210905_1716.py` & `django-torque-0.5.0a3/torque/migrations/0029_auto_20210905_1716.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.7 on 2021-09-05 17:16
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0028_auto_20210905_1659"),
     ]
 
     operations = [
         migrations.RenameModel(
             old_name="Spreadsheet",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0030_auto_20210927_1304.py` & `django-torque-0.5.0a3/torque/migrations/0030_auto_20210927_1304.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.7 on 2021-09-27 13:04
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0029_auto_20210905_1716"),
     ]
 
     operations = [
         migrations.RemoveConstraint(
             model_name="template",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0031_auto_20210930_1328.py` & `django-torque-0.5.0a3/torque/migrations/0031_auto_20210930_1328.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.7 on 2021-09-30 13:28
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0030_auto_20210927_1304"),
     ]
 
     operations = [
         migrations.RemoveConstraint(
             model_name="document",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0033_csvspecification.py` & `django-torque-0.5.0a3/torque/migrations/0033_csvspecification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.7 on 2022-02-05 21:54
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0032_searchcachedocument_filtered_data"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="CsvSpecification",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0034_auto_20220209_1209.py` & `django-torque-0.5.0a3/torque/migrations/0034_auto_20220209_1209.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.7 on 2022-02-09 12:09
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0033_csvspecification"),
     ]
 
     operations = [
         migrations.RenameField(
             model_name="wikiconfig",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py` & `django-torque-0.5.0a3/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.0.3 on 2022-04-13 18:25
 
 import django.contrib.postgres.indexes
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0035_template_in_config"),
     ]
 
     operations = [
         migrations.RemoveIndex(
             model_name="searchcachedocument",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0038_wiki_linked_wiki_keys.py` & `django-torque-0.5.0a3/torque/migrations/0038_wiki_linked_wiki_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.0.3 on 2022-04-14 13:01
 
 import django.contrib.postgres.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0037_template_dirty"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="wiki",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0042_documentdictcache.py` & `django-torque-0.5.0a3/torque/migrations/0042_documentdictcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.1 on 2023-04-04 19:28
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0041_searchcachedocument_explore_rank"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="DocumentDictCache",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0045_templatecachedocument_dirty_and_more.py` & `django-torque-0.5.0a3/torque/migrations/0045_templatecachedocument_dirty_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1 on 2023-04-07 16:25
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0044_documentdictcache_dirty"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="templatecachedocument",
```

### Comparing `django-torque-0.5.0a2/torque/migrations/0047_templatecachedocument_and_more.py` & `django-torque-0.5.0a3/torque/migrations/0047_templatecachedocument_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.1 on 2023-04-07 18:01
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("torque", "0046_delete_templatecachedocument"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="TemplateCacheDocument",
```

### Comparing `django-torque-0.5.0a2/torque/models.py` & `django-torque-0.5.0a3/torque/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,55 +175,55 @@
     # Fortunately, that is highly unlikely, and the only real downside is that
     # the search cache has to be re-indexed, which is not a catastrophic error.
     in_config = models.BooleanField(default=False)
 
     cache_dirty = models.BooleanField(default=False)
 
     def rebuild_document_dict_cache(self):
-        values = (Value.objects.filter(
+        values = (
+            Value.objects.filter(
                 document__in=self.valid_ids.all(),
                 field__in=self.valid_fields.all(),
             )
             .prefetch_related("field")
             .prefetch_related("document")
-            .values('document_id', 'document__key', 'field__name', 'latest')
+            .values("document_id", "document__key", "field__name", "latest")
         )
         new_documents = {}
         for value in values:
             try:
-                new_documents[value['document_id']]["fields"][
-                    value['field__name']
-                ] = orjson.loads(value['latest'])
+                new_documents[value["document_id"]]["fields"][
+                    value["field__name"]
+                ] = orjson.loads(value["latest"])
             except KeyError:
-                new_documents[value['document_id']] = {
-                    "key": value['document__key'],
-                    "fields": {
-                        value['field__name']: orjson.loads(value['latest'])
-                    },
+                new_documents[value["document_id"]] = {
+                    "key": value["document__key"],
+                    "fields": {value["field__name"]: orjson.loads(value["latest"])},
                 }
 
         document_dicts = []
         for document in self.valid_ids.all():
             document_dicts.append(
                 DocumentDictCache(
                     document=document,
                     wiki_config=self,
                     dictionary=json.dumps(new_documents[document.id]),
                 )
             )
 
         DocumentDictCache.objects.bulk_create(document_dicts, ignore_conflicts=True)
 
-
     def rebuild_search_index(self):
         from django.conf import settings
 
         SearchCacheDocument.objects.filter(wiki_config=self).delete()
         sc_documents = []
-        for ddc in DocumentDictCache.objects.filter(wiki_config=self, document__in=self.valid_ids.all()):
+        for ddc in DocumentDictCache.objects.filter(
+            wiki_config=self, document__in=self.valid_ids.all()
+        ):
             document_dict = orjson.loads(ddc.dictionary)["fields"]
             filtered_data = {}
             for filter in getattr(settings, "TORQUE_FILTERS", []):
                 filtered_data[filter.name()] = filter.document_value(document_dict)
 
             explore_rank = None
             if getattr(settings, "TORQUE_EXPLORE_RANK", None):
@@ -254,24 +254,30 @@
                 template_documents.append(
                     TemplateCacheDocument(
                         document_dict=ddc,
                         template=template,
                         rendered_text="",
                     )
                 )
-            TemplateCacheDocument.objects.bulk_create(template_documents, ignore_conflicts=True)
+            TemplateCacheDocument.objects.bulk_create(
+                template_documents, ignore_conflicts=True
+            )
 
-            TemplateCacheDocument.objects.filter(template=template, document_dict__wiki_config=wiki_config).update(dirty=True)
+            TemplateCacheDocument.objects.filter(
+                template=template, document_dict__wiki_config=wiki_config
+            ).update(dirty=True)
 
         build_cache(self)
 
         if include_linked_wikis:
             for wiki_key in self.wiki.linked_wiki_keys:
                 try:
-                    linked_config = WikiConfig.objects.get(group=self.group, wiki=Wiki.objects.get(wiki_key=wiki_key))
+                    linked_config = WikiConfig.objects.get(
+                        group=self.group, wiki=Wiki.objects.get(wiki_key=wiki_key)
+                    )
                     build_cache(linked_config)
                 except WikiConfig.DoesNotExist:
                     # If there's no permission set up for the group, or the wiki doesn't actually
                     # exist, just soldier on
                     pass
 
 
@@ -290,19 +296,27 @@
     # no longer actively attached.  Instead of just removing them right away, and
     # losing any Value or ValueEdits associated, we just mark them as unattached,
     # and then we can later clean them up if we want.
     attached = models.BooleanField(default=True)
 
     def to_dict(self, config):
         try:
-            return orjson.loads(DocumentDictCache.objects.get(document=self, wiki_config=config).dictionary)
+            return orjson.loads(
+                DocumentDictCache.objects.get(
+                    document=self, wiki_config=config
+                ).dictionary
+            )
         except DocumentDictCache.DoesNotExist:
             new_document = {"key": self.key, "fields": {}}
-            for value in self.values.filter(field__in=config.valid_fields.all()).values("field__name", "latest"):
-                new_document["fields"][value["field__name"]] = orjson.loads(value["latest"])
+            for value in self.values.filter(field__in=config.valid_fields.all()).values(
+                "field__name", "latest"
+            ):
+                new_document["fields"][value["field__name"]] = orjson.loads(
+                    value["latest"]
+                )
 
             return new_document
 
     def rebuild_cache(self, config):
         try:
             ddc = DocumentDictCache.objects.get(document=self, wiki_config=config)
             if not ddc.dirty:
@@ -312,15 +326,17 @@
                 # We undirty now so that if it dirties while we're rebuilding, we rebuild again, just for safety
                 ddc.dirty = False
                 ddc.save()
         except DocumentDictCache.DoesNotExist:
             ddc = DocumentDictCache.objects.create(document=self, wiki_config=config)
 
         new_document = {"key": self.key, "fields": {}}
-        for value in self.values.filter(field__in=config.valid_fields.all()).values("field__name", "latest"):
+        for value in self.values.filter(field__in=config.valid_fields.all()).values(
+            "field__name", "latest"
+        ):
             new_document["fields"][value["field__name"]] = orjson.loads(value["latest"])
 
         ddc.dictionary = json.dumps(new_document)
         ddc.save()
 
     def __getitem__(self, key):
         try:
@@ -462,28 +478,34 @@
         global_line_template_contents = global_line_template.get_file_contents()
 
         def add_to_data(wiki_config):
             collection = wiki_config.collection
 
             if results_limit:
                 key_list = [rl[1] for rl in results_limit if rl[0] == collection.name]
-                document_limit = Document.objects.filter(key__in=key_list, collection=collection)
-                documents = [orjson.loads(ddc.dictionary)["fields"] for ddc in DocumentDictCache.objects.filter(document__in=document_limit, wiki_config=wiki_config).all()]
+                document_limit = Document.objects.filter(
+                    key__in=key_list, collection=collection
+                )
+                documents = [
+                    orjson.loads(ddc.dictionary)["fields"]
+                    for ddc in DocumentDictCache.objects.filter(
+                        document__in=document_limit, wiki_config=wiki_config
+                    ).all()
+                ]
             else:
-                documents = [orjson.loads(ddc.dictionary)["fields"]
-                        for ddc
-                        in DocumentDictCache.objects.filter(
-                            document__in=wiki_config.valid_ids.all(),
-                            wiki_config=wiki_config
-                        )
+                documents = [
+                    orjson.loads(ddc.dictionary)["fields"]
+                    for ddc in DocumentDictCache.objects.filter(
+                        document__in=wiki_config.valid_ids.all(),
+                        wiki_config=wiki_config,
+                    )
                 ]
 
             data[global_collection_data_name][collection.name] = {
-                document[collection.key_field]: document
-                for document in documents
+                document[collection.key_field]: document for document in documents
             }
             data["toc_lines"][collection.name] = {
                 document[collection.key_field]: jinja_env.from_string(
                     global_line_template_contents
                 ).render({collection.object_name: document})
                 for document in documents
             }
@@ -614,39 +636,50 @@
     document = models.ForeignKey(Document, on_delete=models.CASCADE)
     wiki_config = models.ForeignKey(WikiConfig, on_delete=models.CASCADE)
     dirty = models.BooleanField(default=False)
     dictionary = models.TextField(null=True)
 
     class Meta:
         constraints = [
-            models.UniqueConstraint(fields=["document", "wiki_config"], name="unique_document_dict"),
+            models.UniqueConstraint(
+                fields=["document", "wiki_config"], name="unique_document_dict"
+            ),
         ]
 
 
 class TemplateCacheDocument(models.Model):
     document_dict = models.ForeignKey(DocumentDictCache, on_delete=models.CASCADE)
     template = models.ForeignKey(Template, on_delete=models.CASCADE)
     rendered_text = models.TextField(null=True)
     dirty = models.BooleanField(default=False)
 
     class Meta:
         constraints = [
-            models.UniqueConstraint(fields=["document_dict", "template"], name="unique_template_cache_document"),
+            models.UniqueConstraint(
+                fields=["document_dict", "template"],
+                name="unique_template_cache_document",
+            ),
         ]
 
     def rebuild(self):
         try:
             jinja_template = jinja_env.from_string(self.template.get_file_contents())
 
             (scheme, server) = self.template.wiki.server.split("://")
-            site = mwclient.Site(server, self.template.wiki.script_path + "/", scheme=scheme)
+            site = mwclient.Site(
+                server, self.template.wiki.script_path + "/", scheme=scheme
+            )
             site.login(self.template.wiki.username, self.template.wiki.password)
 
             rendered_data = jinja_template.render(
-                {self.document_dict.document.collection.object_name: orjson.loads(self.document_dict.dictionary)["fields"]}
+                {
+                    self.document_dict.document.collection.object_name: orjson.loads(
+                        self.document_dict.dictionary
+                    )["fields"]
+                }
             )
             rendered_html = site.api(
                 "parse", text=rendered_data, contentmodel="wikitext", prop="text"
             )["parse"]["text"]["*"]
 
             self.rendered_text = rendered_html
         except Exception:
```

### Comparing `django-torque-0.5.0a2/torque/urls.py` & `django-torque-0.5.0a3/torque/urls.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.5.0a2/torque/utils.py` & `django-torque-0.5.0a3/torque/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,22 +80,27 @@
         enabled_extensions = (
             enabled_extensions + settings.TORQUE_ENABLED_JINJA_EXTENSIONS
         )
 
     env = Environment(extensions=enabled_extensions)
 
     if getattr(settings, "TORQUE_JINJA_GLOBALS", False):
-        for (key, value) in settings.TORQUE_JINJA_GLOBALS.items():
+        for key, value in settings.TORQUE_JINJA_GLOBALS.items():
             env.globals[key] = value
 
     return env
 
 
 def dirty_documents(documents, wiki_config=None):
     from torque import models
+
     if wiki_config:
-        document_dicts = models.DocumentDictCache.objects.filter(document__in=documents, wiki_config=wiki_config)
+        document_dicts = models.DocumentDictCache.objects.filter(
+            document__in=documents, wiki_config=wiki_config
+        )
     else:
         document_dicts = models.DocumentDictCache.objects.filter(document__in=documents)
 
     document_dicts.update(dirty=True)
-    models.TemplateCacheDocument.objects.filter(document_dict__in=document_dicts).update(dirty=True)
+    models.TemplateCacheDocument.objects.filter(
+        document_dict__in=document_dicts
+    ).update(dirty=True)
```

### Comparing `django-torque-0.5.0a2/torque/views.py` & `django-torque-0.5.0a3/torque/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,87 +59,98 @@
 def search_data(qs, filters, wiki_configs, documents_limited_to):
     data_vector_q = Q()
     if qs:
         for q in qs:
             data_vector_q |= Q(data_vector=q)
 
     document_limit_or = Q()
-    for (collection, document) in documents_limited_to:
+    for collection, document in documents_limited_to:
         document_limit_or |= Q(collection__name=collection, document__key=document)
 
     results = (
         models.SearchCacheDocument.objects.filter(
             data_vector_q,
             document_limit_or,
             collection__in=wiki_configs.values_list("collection", flat=True),
             wiki__wiki_key__in=wiki_configs.values_list("wiki__wiki_key", flat=True),
             group__in=wiki_configs.values_list("group", flat=True),
             wiki_config__in=wiki_configs,
         )
         .select_related("document")
         .select_related("collection")
     )
+
     filter_results = []
     torque_filters_by_name = {
         f.name(): f for f in getattr(settings, "TORQUE_FILTERS", [])
     }
+    test_torque_filters_by_name = {
+        f.name(): f for f in getattr(settings, "TORQUE_FILTERS", [])
+    }
+    results_filtered_data = []
+    for result in results.values("filtered_data"):
+        results_filtered_data.append(result["filtered_data"])
+
     for filter in getattr(settings, "TORQUE_FILTERS", []):
-        additional_filters = []
-        for name, values in filters.items():
-            if name != filter.name():
-                q_objects = Q()
-                for value in values:
-                    if torque_filters_by_name[name].is_list():
-                        key = "filtered_data__%s__contains" % name
-                    else:
-                        key = "filtered_data__%s" % name
-                    q_dict = {key: value}
-                    q_objects |= Q(**q_dict)
-                additional_filters.append(q_objects)
+        selected_objects = []
+
+        def result_filtered_data_addable(result_filtered_data):
+            for name, values in filters.items():
+                if name != filter.name() and values:
+                    filter_passed = False
+                    for value in values:
+                        if name in result_filtered_data.keys():
+                            if (
+                                torque_filters_by_name[name].is_list()
+                                and value in result_filtered_data[name]
+                            ):
+                                filter_passed = True
+                                break
+                            elif (
+                                not torque_filters_by_name[name].is_list()
+                                and value == result_filtered_data[name]
+                            ):
+                                filter_passed = True
+                                break
+                    if not filter_passed:
+                        return False
+            return True
+
+        selected_objects = [
+            result_filtered_data
+            for result_filtered_data in results_filtered_data
+            if result_filtered_data_addable(result_filtered_data)
+        ]
+
+        counts = {}
+        for selected_object in selected_objects:
+            if filter.name() in selected_object:
+                if filter.is_list():
+                    for value in selected_object[filter.name()]:
+                        if value not in filter.ignored_values():
+                            if value not in counts:
+                                counts[value] = {"name": value, "total": 0}
+
+                            counts[value]["total"] += 1
+                else:
+                    value = selected_object[filter.name()]
+                    if value not in filter.ignored_values():
+                        if value not in counts:
+                            counts[value] = {"name": value, "total": 0}
+
+                        counts[value]["total"] += 1
+
         filter_result = {
             "name": filter.name(),
             "display": filter.display_name(),
             "primary": filter.is_primary(),
-            "counts": {},
+            "counts": {name: counts[name] for name in filter.sort(list(counts.keys()))},
         }
 
-        grouped_results = (
-            results.filter(*additional_filters)
-            .values("filtered_data__%s" % filter.name())
-            .annotate(total=Count("id"))
-        )
-        for result in grouped_results:
-            name = result["filtered_data__%s" % filter.name()]
-            if name:
-                if filter.is_list():
-                    for item in name:
-                        if item not in filter_result["counts"]:
-                            filter_result["counts"][item] = {
-                                "name": item,
-                                "total": 0,
-                            }
-
-                        filter_result["counts"][item]["total"] += result["total"]
-                else:
-                    filter_result["counts"][name] = {
-                        "name": name,
-                        "total": result["total"],
-                    }
-
-        names = list(filter_result["counts"].keys())
-        names = filter.sort(names)
-        filter_result["counts"] = [
-            filter_result["counts"][name]
-            for name in names
-            if name not in filter.ignored_values()
-        ]
-
-        # If the only values returned are ignored ones, then we don't want to show the filter at all!
-        if len(filter_result["counts"]) > 0:
-            filter_results.append(filter_result)
+        filter_results.append(filter_result)
 
     additional_filters = []
     for name, values in filters.items():
         q_objects = Q()
         if torque_filters_by_name[name].is_list():
             key = "filtered_data__%s__contains" % name
         else:
@@ -179,25 +190,28 @@
     # be worth being more clear about what we're doing here via the interface.
     #
     # This has gotten weird because the results are actually html from cached
     # results
     if fmt == "mwiki":
         mwiki_text = ""
 
-        template = models.Template.objects.get(name="Search", collection=template_config.collection)
+        template = models.Template.objects.get(
+            type="Search", collection=template_config.collection
+        )
 
         cache_or = Q()
         for r in returned_results[offset : (offset + 20)]:
-            cache_or |= Q(document_dict__wiki_config=r.wiki_config, document_dict__document=r.document)
+            cache_or |= Q(
+                document_dict__wiki_config=r.wiki_config,
+                document_dict__document=r.document,
+            )
 
         cached_results = models.TemplateCacheDocument.objects.filter(
             template=template,
-        ).filter(
-            cache_or
-        )
+        ).filter(cache_or)
 
         for cached_result in cached_results.filter(dirty=True):
             cached_result.rebuild()
 
         mwiki_text = "\n".join([c.rendered_text for c in cached_results])
 
         return JsonResponse(
@@ -262,89 +276,111 @@
     configs = models.WikiConfig.objects.filter(
         collection__name=collection_name, wiki=wiki, group=group
     )
     return search(q, f, offset, configs.first(), configs, results_limit, fmt)
 
 
 def explore(
-    qs, filters, offset, template_name, template_config, wiki_configs, results_limit
+    qs,
+    filters,
+    offset,
+    template_name,
+    template_config,
+    wiki_configs,
+    results_limit,
+    filters_only=False,
 ):
+    import time
+
+    start = time.perf_counter()
     (returned_results, filter_results) = search_data(
         qs, filters, wiki_configs, results_limit
     )
 
-    mwiki_text = ""
+    response = {
+        "num_results": returned_results.count(),
+        "filter_results": filter_results,
+    }
 
-    result_set = [
-        orjson.loads(models.DocumentDictCache.objects.get(document=r.document, wiki_config__group=r.group).dictionary)["fields"] for r in returned_results[offset : (offset + 100)]
-    ]
-    explore_templates = models.Template.objects.filter(
-        type="Explore",
-        collection=template_config.collection,
-    )
-    if explore_templates:
-        if template_name:
-            template = jinja_env.from_string(
-                explore_templates.get(name=template_name).get_file_contents()
-            )
-        else:
-            template = jinja_env.from_string(
-                explore_templates.get(is_default=True).get_file_contents()
-            )
-        mwiki_text += template.render(
-            {template_config.collection.object_data_name(): result_set}
-        )
-    else:
-        for result in result_set:
-            template = jinja_env.from_string(
-                models.Template.objects.get(
-                    name="Search", collection=template_config.collection
-                ).get_file_contents()
-            )
+    if not filters_only:
+        mwiki_text = ""
+
+        result_set = [
+            orjson.loads(
+                models.DocumentDictCache.objects.get(
+                    document=r.document, wiki_config__group=r.group
+                ).dictionary
+            )["fields"]
+            for r in returned_results[offset : (offset + 100)]
+        ]
+        explore_templates = models.Template.objects.filter(
+            type="Explore",
+            collection=template_config.collection,
+        )
+        if explore_templates:
+            if template_name:
+                template = jinja_env.from_string(
+                    explore_templates.get(name=template_name).get_file_contents()
+                )
+            else:
+                template = jinja_env.from_string(
+                    explore_templates.get(is_default=True).get_file_contents()
+                )
             mwiki_text += template.render(
-                {template_config.collection.object_name: result}
+                {template_config.collection.object_data_name(): result_set}
             )
-            mwiki_text += "\n\n"
+        else:
+            for result in result_set:
+                template = jinja_env.from_string(
+                    models.Template.objects.get(
+                        name="Search", collection=template_config.collection
+                    ).get_file_contents()
+                )
+                mwiki_text += template.render(
+                    {template_config.collection.object_name: result}
+                )
+                mwiki_text += "\n\n"
 
-    return JsonResponse(
-        {
-            "num_results": returned_results.count(),
-            "results": [(r["collection__name"], r["document__key"]) for r in returned_results.values("collection__name", "document__key")],
-            "mwiki_text": mwiki_text,
-            "filter_results": filter_results,
-        },
-        safe=False,
-    )
+        response["results"] = [
+            (r["collection__name"], r["document__key"])
+            for r in returned_results.values("collection__name", "document__key")
+        ]
+        response["mwiki_text"] = mwiki_text
+
+    return JsonResponse(response, safe=False)
 
 
 def explore_global(request):
     qs = (
         json.loads(request.GET["qs"])
         if "qs" in request.GET and request.GET["qs"]
         else []
     )
     f = json.loads(request.GET["f"]) if "f" in request.GET and request.GET["f"] else {}
-    template_name = request.GET["template"]
+    template_name = request.GET.get("template")
     results_limit_json = json.loads(request.body) if request.body else None
     results_limit = results_limit_json if results_limit_json else []
     offset = int(request.GET.get("offset", 0))
     group = request.GET["group"]
     global_wiki_key = request.GET["wiki_key"]
     global_collection_name = request.GET["collection_name"]
+    filter_only = request.GET.get("filter_only", False)
     wiki_keys = request.GET["wiki_keys"].split(",")
     collection_names = request.GET["collection_names"].split(",")
     global_config = models.WikiConfig.objects.get(
         collection__name=global_collection_name,
         wiki__wiki_key=global_wiki_key,
         group=group,
     )
     configs = models.WikiConfig.objects.filter(
         collection__name__in=collection_names, wiki__wiki_key__in=wiki_keys, group=group
     ).all()
-    return explore(qs, f, offset, template_name, global_config, configs, results_limit)
+    return explore(
+        qs, f, offset, template_name, global_config, configs, results_limit, filter_only
+    )
 
 
 def explore_collection(request, collection_name):
     qs = (
         json.loads(request.GET["qs"])
         if "qs" in request.GET and request.GET["qs"]
         else []
@@ -352,23 +388,31 @@
     results_limit_json = json.loads(request.body) if request.body else None
     results_limit = (
         [[collection_name, key] for key in results_limit_json]
         if results_limit_json
         else []
     )
     f = json.loads(request.GET["f"]) if "f" in request.GET and request.GET["f"] else {}
-    template_name = request.GET["template"]
+    template_name = request.GET.get("template")
     offset = int(request.GET.get("offset", 0))
     group = request.GET["group"]
+    filter_only = request.GET.get("filter_only", False)
     wiki = get_wiki_from_request(request, collection_name)
     configs = models.WikiConfig.objects.filter(
         collection__name=collection_name, wiki=wiki, group=group
     )
     return explore(
-        qs, f, offset, template_name, configs.first(), configs, results_limit
+        qs,
+        f,
+        offset,
+        template_name,
+        configs.first(),
+        configs,
+        results_limit,
+        filter_only,
     )
 
 
 def edit_record(collection_name, key, group, wiki, field, new_value):
     collection = models.Collection.objects.get(name=collection_name)
     document = models.Document.objects.get(collection=collection, key=key)
     wiki_config = models.WikiConfig.objects.get(
@@ -413,15 +457,20 @@
     models.TableOfContentsCache.objects.filter(
         toc__in=collection.tables_of_contents.all()
     ).update(dirty=True)
     utils.dirty_documents([document])
     # Rebuild immediately because whoever is doing the editing probably
     # wants to see the fruits of their efforts.
     document.rebuild_cache(wiki_config)
-    [t.rebuild() for t in models.TemplateCacheDocument.objects.filter(document_dict__wiki_config=wiki_config, document_dict__document=document).all()]
+    [
+        t.rebuild()
+        for t in models.TemplateCacheDocument.objects.filter(
+            document_dict__wiki_config=wiki_config, document_dict__document=document
+        ).all()
+    ]
 
     wiki.invalidate_linked_wiki_toc_cache()
     models.SearchCacheDocument.objects.filter(document=document).update(dirty=True)
 
     # This is overkill, but that's ok.  There's a bit of work to make it so
     # the individaul template cache documents have a dirty method
     collection.templates.update(dirty=True)
@@ -545,15 +594,14 @@
     )["fields"]
 
     if fmt == "json":
         return JsonResponse(document)
     elif fmt == "dict":
         return document
 
-
     templates = models.Template.objects.filter(
         collection=collection,
         wiki=wiki,
         type="View",
     )
 
     if view is not None:
@@ -573,16 +621,21 @@
     if fmt == "mwiki":
         rendered_template = jinja_env.from_string(template.get_file_contents()).render(
             {collection.object_name: document}
         )
         return HttpResponse(rendered_template)
     elif fmt == "html":
         try:
-            ddc = models.DocumentDictCache.objects.get(wiki_config=wiki_config, document=wiki_config.valid_ids.get(key=key, collection=collection))
-            cache = models.TemplateCacheDocument.objects.get(template=template, document_dict=ddc)
+            ddc = models.DocumentDictCache.objects.get(
+                wiki_config=wiki_config,
+                document=wiki_config.valid_ids.get(key=key, collection=collection),
+            )
+            cache = models.TemplateCacheDocument.objects.get(
+                template=template, document_dict=ddc
+            )
             if cache.dirty:
                 cache.rebuild()
             return HttpResponse(cache.rendered_text)
         except models.TemplateCacheDocument.DoesNotExist:
             return HttpResponse("")
     else:
         raise Exception(f"Invalid format {fmt}")
@@ -1025,15 +1078,19 @@
                 ):
                     row.extend(
                         settings.TORQUE_CSV_PROCESSORS[field_name].process_value(
                             python_value
                         )
                     )
                 elif field_name in getattr(settings, "TORQUE_CSV_PROCESSORS", {}):
-                    row.extend(settings.TORQUE_CSV_PROCESSORS[field_name].default_value(field_name))
+                    row.extend(
+                        settings.TORQUE_CSV_PROCESSORS[field_name].default_value(
+                            field_name
+                        )
+                    )
                 elif python_value:
                     row.append(python_value)
                 else:
                     row.append("")
             writer.writerow(row)
 
         return response
```

