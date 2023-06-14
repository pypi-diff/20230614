# Comparing `tmp/automation_file_dev-0.0.8.tar.gz` & `tmp/automation_file_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.8.tar", last modified: Mon Jun 12 07:23:55 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.9.tar", last modified: Tue Jun 13 07:12:36 2023, max compression
```

## Comparing `automation_file_dev-0.0.8.tar` & `automation_file_dev-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.109984 automation_file_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1306 2023-06-12 07:23:55.107828 automation_file_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.678664 automation_file_dev-0.0.8/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0     1306 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2012 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.686170 automation_file_dev-0.0.8/file_automation/
--rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file_dev-0.0.8/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.690159 automation_file_dev-0.0.8/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.8/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.704669 automation_file_dev-0.0.8/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.8/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.8/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.719534 automation_file_dev-0.0.8/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.8/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.8/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.737631 automation_file_dev-0.0.8/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.8/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file_dev-0.0.8/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.742955 automation_file_dev-0.0.8/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.8/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.758392 automation_file_dev-0.0.8/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.769185 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.780173 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.796716 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.823542 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.842802 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.864909 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.876174 automation_file_dev-0.0.8/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.8/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.909659 automation_file_dev-0.0.8/file_automation/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file_dev-0.0.8/file_automation/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file_dev-0.0.8/file_automation/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.956895 automation_file_dev-0.0.8/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.8/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file_dev-0.0.8/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file_dev-0.0.8/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.003159 automation_file_dev-0.0.8/file_automation/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.8/file_automation/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     6611 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.022084 automation_file_dev-0.0.8/file_automation/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.8/file_automation/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.040159 automation_file_dev-0.0.8/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.8/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file_dev-0.0.8/file_automation/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.096452 automation_file_dev-0.0.8/file_automation/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file_dev-0.0.8/file_automation/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py
--rw-rw-rw-   0        0        0     1008 2023-06-12 07:23:00.000000 automation_file_dev-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 07:23:55.120437 automation_file_dev-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.927899 automation_file_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1306 2023-06-13 07:12:36.926899 automation_file_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.629758 automation_file_dev-0.0.9/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1306 2023-06-13 07:12:36.000000 automation_file_dev-0.0.9/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2012 2023-06-13 07:12:36.000000 automation_file_dev-0.0.9/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:12:36.000000 automation_file_dev-0.0.9/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 07:12:36.000000 automation_file_dev-0.0.9/automation_file_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 07:12:36.000000 automation_file_dev-0.0.9/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.639162 automation_file_dev-0.0.9/file_automation/
+-rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file_dev-0.0.9/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.641164 automation_file_dev-0.0.9/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.9/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.656675 automation_file_dev-0.0.9/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.9/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.9/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.671866 automation_file_dev-0.0.9/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.9/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.9/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.693904 automation_file_dev-0.0.9/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.9/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file_dev-0.0.9/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.700928 automation_file_dev-0.0.9/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.9/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.716760 automation_file_dev-0.0.9/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.730069 automation_file_dev-0.0.9/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.743566 automation_file_dev-0.0.9/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.758654 automation_file_dev-0.0.9/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.774595 automation_file_dev-0.0.9/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.794795 automation_file_dev-0.0.9/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.809847 automation_file_dev-0.0.9/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.9/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.815020 automation_file_dev-0.0.9/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.9/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.831446 automation_file_dev-0.0.9/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file_dev-0.0.9/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file_dev-0.0.9/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.859360 automation_file_dev-0.0.9/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.9/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file_dev-0.0.9/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file_dev-0.0.9/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.878945 automation_file_dev-0.0.9/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.9/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6741 2023-06-13 06:29:23.000000 automation_file_dev-0.0.9/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.893598 automation_file_dev-0.0.9/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.9/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file_dev-0.0.9/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.907088 automation_file_dev-0.0.9/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.9/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file_dev-0.0.9/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:12:36.923257 automation_file_dev-0.0.9/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file_dev-0.0.9/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file_dev-0.0.9/file_automation/utils/scheduler/extend_apscheduler.py
+-rw-rw-rw-   0        0        0     1008 2023-06-13 07:12:02.000000 automation_file_dev-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:12:36.927899 automation_file_dev-0.0.9/setup.cfg
```

### Comparing `automation_file_dev-0.0.8/LICENSE` & `automation_file_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/PKG-INFO` & `automation_file_dev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file_dev
-Version: 0.0.8
+Version: 0.0.9
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.8/README.md` & `automation_file_dev-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/automation_file_dev.egg-info/PKG-INFO` & `automation_file_dev-0.0.9/automation_file_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file-dev
-Version: 0.0.8
+Version: 0.0.9
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.8/automation_file_dev.egg-info/SOURCES.txt` & `automation_file_dev-0.0.9/automation_file_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/__init__.py` & `automation_file_dev-0.0.9/file_automation/__init__.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/local/dir/dir_process.py` & `automation_file_dev-0.0.9/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/local/file/file_process.py` & `automation_file_dev-0.0.9/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/local/zip/zip_process.py` & `automation_file_dev-0.0.9/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/download/download_file.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/download/download_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/driver_instance.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/search/search_drive.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/search/search_drive.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/share/share_file.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/share/share_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file_dev-0.0.9/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/callback/callback_function_executor.py` & `automation_file_dev-0.0.9/file_automation/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/exception/exception_tags.py` & `automation_file_dev-0.0.9/file_automation/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/exception/exceptions.py` & `automation_file_dev-0.0.9/file_automation/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/executor/action_executor.py` & `automation_file_dev-0.0.9/file_automation/utils/executor/action_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
                 execute_record_dict.update({execute_record: event_response})
             except Exception as error:
                 file_automation_logger.error(
                     f"Execute {action} failed. {repr(error)}"
                 )
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
+        for key, value in execute_record_dict.items():
+            print(key, flush=True)
+            print(value, flush=True)
         return execute_record_dict
 
     def execute_files(self, execute_files_list: list) -> list:
         """
         :param execute_files_list: list include execute files path
         :return: every execute detail as list
         """
```

### Comparing `automation_file_dev-0.0.8/file_automation/utils/json/json_file.py` & `automation_file_dev-0.0.9/file_automation/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/logging/loggin_instance.py` & `automation_file_dev-0.0.9/file_automation/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py` & `automation_file_dev-0.0.9/file_automation/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.8/pyproject.toml` & `automation_file_dev-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

