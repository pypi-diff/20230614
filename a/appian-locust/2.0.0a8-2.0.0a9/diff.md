# Comparing `tmp/appian-locust-2.0.0a8.tar.gz` & `tmp/appian-locust-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a8.tar", last modified: Tue Jun 13 20:35:12 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a9.tar", last modified: Tue Jun 13 21:44:15 2023, max compression
```

## Comparing `appian-locust-2.0.0a8.tar` & `appian-locust-2.0.0a9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.254654 appian-locust-2.0.0a8/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    52246 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    16611 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)    16940 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/appianclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.255654 appian-locust-2.0.0a8/appian_locust/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/feature_flag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.256654 appian-locust-2.0.0a8/appian_locust/info/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/info/tasks_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.257654 appian-locust-2.0.0a8/appian_locust/objects/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/application.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/page.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/objects/site.py
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/system_operator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.258654 appian-locust-2.0.0a8/appian_locust/uiform/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    73478 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/uiform/uiform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/appian_locust/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/utilities/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    14863 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 20:35:12.254654 appian-locust-2.0.0a8/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1786 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 20:35:12.000000 appian-locust-2.0.0a8/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-13 20:35:12.259654 appian-locust-2.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-13 20:35:04.000000 appian-locust-2.0.0a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.763548 appian-locust-2.0.0a9/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    52246 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    16611 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)    16940 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/appianclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.764547 appian-locust-2.0.0a9/appian_locust/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/feature_flag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.765547 appian-locust-2.0.0a9/appian_locust/info/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/info/tasks_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.766548 appian-locust-2.0.0a9/appian_locust/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/application.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/page.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/objects/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/system_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.767547 appian-locust-2.0.0a9/appian_locust/uiform/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    73478 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/uiform/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/appian_locust/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/utilities/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    14863 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:44:15.764547 appian-locust-2.0.0a9/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 21:44:15.000000 appian-locust-2.0.0a9/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-13 21:44:15.768547 appian-locust-2.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-13 21:44:07.000000 appian-locust-2.0.0a9/setup.py
```

### Comparing `appian-locust-2.0.0a8/LICENSE` & `appian-locust-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/PKG-INFO` & `appian-locust-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a8/README.rst` & `appian-locust-2.0.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_actions.py` & `appian-locust-2.0.0a9/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_admin.py` & `appian-locust-2.0.0a9/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_base.py` & `appian-locust-2.0.0a9/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_design.py` & `appian-locust-2.0.0a9/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a9/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a9/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_interactor.py` & `appian-locust-2.0.0a9/appian_locust/_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a9/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_news.py` & `appian-locust-2.0.0a9/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_portals.py` & `appian-locust-2.0.0a9/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_records.py` & `appian-locust-2.0.0a9/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_records_helper.py` & `appian-locust-2.0.0a9/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_reports.py` & `appian-locust-2.0.0a9/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a9/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_sites.py` & `appian-locust-2.0.0a9/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_task_opener.py` & `appian-locust-2.0.0a9/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_tasks.py` & `appian-locust-2.0.0a9/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a9/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/appianclient.py` & `appian-locust-2.0.0a9/appian_locust/appianclient.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/exceptions/exceptions.py` & `appian-locust-2.0.0a9/appian_locust/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/feature_flag.py` & `appian-locust-2.0.0a9/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/actions_info.py` & `appian-locust-2.0.0a9/appian_locust/info/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/news_info.py` & `appian-locust-2.0.0a9/appian_locust/info/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/records_info.py` & `appian-locust-2.0.0a9/appian_locust/info/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/reports_info.py` & `appian-locust-2.0.0a9/appian_locust/info/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/sites_info.py` & `appian-locust-2.0.0a9/appian_locust/info/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/info/tasks_info.py` & `appian-locust-2.0.0a9/appian_locust/info/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/objects/design_object.py` & `appian-locust-2.0.0a9/appian_locust/objects/design_object.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/objects/page.py` & `appian-locust-2.0.0a9/appian_locust/objects/page.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/system_operator.py` & `appian-locust-2.0.0a9/appian_locust/system_operator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/application_uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/design_object_uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/design_uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/record_list_uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/record_uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/uiform/uiform.py` & `appian-locust-2.0.0a9/appian_locust/uiform/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/utilities/helper.py` & `appian-locust-2.0.0a9/appian_locust/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/utilities/loadDriverUtils.py` & `appian-locust-2.0.0a9/appian_locust/utilities/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/utilities/logger.py` & `appian-locust-2.0.0a9/appian_locust/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust/visitor.py` & `appian-locust-2.0.0a9/appian_locust/visitor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a9/appian_locust.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a8/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.0a9/appian_locust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/setup.cfg` & `appian-locust-2.0.0a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a8/setup.py` & `appian-locust-2.0.0a9/setup.py`

 * *Files identical despite different names*

