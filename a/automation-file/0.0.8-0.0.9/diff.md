# Comparing `tmp/automation_file-0.0.8.tar.gz` & `tmp/automation_file-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file-0.0.8.tar", last modified: Tue Jun 13 07:20:16 2023, max compression
+gzip compressed data, was "automation_file-0.0.9.tar", last modified: Wed Jun 14 06:18:01 2023, max compression
```

## Comparing `automation_file-0.0.8.tar` & `automation_file-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.851022 automation_file-0.0.8/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-06-13 07:20:16.850022 automation_file-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.723709 automation_file-0.0.8/automation_file.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.727785 automation_file-0.0.8/file_automation/
--rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file-0.0.8/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.730841 automation_file-0.0.8/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.8/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.738828 automation_file-0.0.8/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.8/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.8/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.743836 automation_file-0.0.8/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.8/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.8/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.750357 automation_file-0.0.8/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.8/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file-0.0.8/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.753422 automation_file-0.0.8/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.8/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.759485 automation_file-0.0.8/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.8/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.766907 automation_file-0.0.8/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.774458 automation_file-0.0.8/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.780546 automation_file-0.0.8/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.8/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.8/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.788669 automation_file-0.0.8/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.8/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.794773 automation_file-0.0.8/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.8/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.801855 automation_file-0.0.8/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.806902 automation_file-0.0.8/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.8/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.813169 automation_file-0.0.8/file_automation/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file-0.0.8/file_automation/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file-0.0.8/file_automation/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.821801 automation_file-0.0.8/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.8/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file-0.0.8/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file-0.0.8/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.828717 automation_file-0.0.8/file_automation/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.8/file_automation/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     6741 2023-06-13 06:29:23.000000 automation_file-0.0.8/file_automation/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.834938 automation_file-0.0.8/file_automation/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.8/file_automation/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file-0.0.8/file_automation/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.841504 automation_file-0.0.8/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.8/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file-0.0.8/file_automation/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.847472 automation_file-0.0.8/file_automation/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file-0.0.8/file_automation/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py
--rw-rw-rw-   0        0        0     1004 2023-06-13 07:19:53.000000 automation_file-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 07:20:16.851022 automation_file-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.953716 automation_file-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-06-14 06:18:01.952715 automation_file-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.755597 automation_file-0.0.9/automation_file.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-06-14 06:18:01.000000 automation_file-0.0.9/automation_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2595 2023-06-14 06:18:01.000000 automation_file-0.0.9/automation_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:18:01.000000 automation_file-0.0.9/automation_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-14 06:18:01.000000 automation_file-0.0.9/automation_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 06:18:01.000000 automation_file-0.0.9/automation_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.760506 automation_file-0.0.9/file_automation/
+-rw-rw-rw-   0        0        0     2352 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.764504 automation_file-0.0.9/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.9/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.773148 automation_file-0.0.9/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.9/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.9/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.781702 automation_file-0.0.9/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.9/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-06-14 05:39:31.000000 automation_file-0.0.9/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.790515 automation_file-0.0.9/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.9/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file-0.0.9/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.793513 automation_file-0.0.9/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.9/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.802207 automation_file-0.0.9/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.9/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.812714 automation_file-0.0.9/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      654 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.819765 automation_file-0.0.9/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.828555 automation_file-0.0.9/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.9/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.835584 automation_file-0.0.9/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2326 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.844161 automation_file-0.0.9/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.852124 automation_file-0.0.9/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.9/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3859 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.855120 automation_file-0.0.9/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.9/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.861883 automation_file-0.0.9/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file-0.0.9/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     5465 2023-06-14 05:00:01.000000 automation_file-0.0.9/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.875310 automation_file-0.0.9/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.9/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file-0.0.9/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file-0.0.9/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.882376 automation_file-0.0.9/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.9/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     7324 2023-06-14 05:49:58.000000 automation_file-0.0.9/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.889284 automation_file-0.0.9/file_automation/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.9/file_automation/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-03-28 03:05:06.000000 automation_file-0.0.9/file_automation/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.897749 automation_file-0.0.9/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.9/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file-0.0.9/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.906262 automation_file-0.0.9/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.9/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file-0.0.9/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.913798 automation_file-0.0.9/file_automation/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:15:41.000000 automation_file-0.0.9/file_automation/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3543 2023-06-14 05:45:44.000000 automation_file-0.0.9/file_automation/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.920811 automation_file-0.0.9/file_automation/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 automation_file-0.0.9/file_automation/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     3063 2023-06-14 05:44:10.000000 automation_file-0.0.9/file_automation/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.933559 automation_file-0.0.9/file_automation/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 automation_file-0.0.9/file_automation/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-06-14 04:55:06.000000 automation_file-0.0.9/file_automation/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      447 2023-06-14 05:42:24.000000 automation_file-0.0.9/file_automation/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.941035 automation_file-0.0.9/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file-0.0.9/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 automation_file-0.0.9/file_automation/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:18:01.949707 automation_file-0.0.9/file_automation/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.9/file_automation/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-14 04:44:37.000000 automation_file-0.0.9/file_automation/utils/socket_server/file_automation_socket_server.py
+-rw-rw-rw-   0        0        0     1004 2023-06-14 06:17:38.000000 automation_file-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:18:01.954718 automation_file-0.0.9/setup.cfg
```

### Comparing `automation_file-0.0.8/LICENSE` & `automation_file-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/PKG-INFO` & `automation_file-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file
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

### Comparing `automation_file-0.0.8/README.md` & `automation_file-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/automation_file.egg-info/PKG-INFO` & `automation_file-0.0.9/automation_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file
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

### Comparing `automation_file-0.0.8/automation_file.egg-info/SOURCES.txt` & `automation_file-0.0.9/automation_file.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -33,13 +33,24 @@
 file_automation/utils/callback/__init__.py
 file_automation/utils/callback/callback_function_executor.py
 file_automation/utils/exception/__init__.py
 file_automation/utils/exception/exception_tags.py
 file_automation/utils/exception/exceptions.py
 file_automation/utils/executor/__init__.py
 file_automation/utils/executor/action_executor.py
+file_automation/utils/file_process/__init__.py
+file_automation/utils/file_process/get_dir_file_list.py
 file_automation/utils/json/__init__.py
 file_automation/utils/json/json_file.py
 file_automation/utils/logging/__init__.py
 file_automation/utils/logging/loggin_instance.py
+file_automation/utils/package_manager/__init__.py
+file_automation/utils/package_manager/package_manager_class.py
+file_automation/utils/project/__init__.py
+file_automation/utils/project/create_project_structure.py
+file_automation/utils/project/template/__init__.py
+file_automation/utils/project/template/template_executor.py
+file_automation/utils/project/template/template_keyword.py
 file_automation/utils/scheduler/__init__.py
-file_automation/utils/scheduler/extend_apscheduler.py
+file_automation/utils/scheduler/extend_apscheduler.py
+file_automation/utils/socket_server/__init__.py
+file_automation/utils/socket_server/file_automation_socket_server.py
```

### Comparing `automation_file-0.0.8/file_automation/local/dir/dir_process.py` & `automation_file-0.0.9/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/local/file/file_process.py` & `automation_file-0.0.9/file_automation/local/file/file_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,7 +82,12 @@
 
 
 def remove_file(file_path: str):
     file_path = Path(file_path)
     if file_path.exists() and file_path.is_file():
         file_path.unlink(missing_ok=True)
         file_automation_logger.info(f"Remove file, file path: {file_path}")
+
+
+def create_file(file_path: str, content: str):
+    with open(file_path, "w+") as file:
+        file.write(content)
```

### Comparing `automation_file-0.0.8/file_automation/local/zip/zip_process.py` & `automation_file-0.0.9/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file-0.0.9/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from googleapiclient.errors import HttpError
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def delete_file(file_id: str) -> Union[dict, None]:
+def drive_delete_file(file_id: str) -> Union[dict, None]:
     try:
         file = driver_instance.service.files().delete(fileId=file_id).execute()
         file_automation_logger.info(f"Delete drive file: {file_id}")
         return file
     except HttpError as error:
         file_automation_logger.error(
             f"Delete file failed,"
```

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file-0.0.9/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from googleapiclient.errors import HttpError
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def add_folder(folder_name: str) -> Union[dict, None]:
+def drive_add_folder(folder_name: str) -> Union[dict, None]:
     try:
         file_metadata = {
             "name": folder_name,
             "mimeType": "application/vnd.google-apps.folder"
         }
         file = driver_instance.service.files().create(
             body=file_metadata,
```

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/download/download_file.py` & `automation_file-0.0.9/file_automation/remote/google_drive/download/download_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaIoBaseDownload
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def download_file(file_id: str, file_name: str) -> BytesIO:
+def drive_download_file(file_id: str, file_name: str) -> BytesIO:
     try:
         request = driver_instance.service.files().get_media(fileId=file_id)
         file = io.BytesIO()
         downloader = MediaIoBaseDownload(file, request)
         done = False
         while done is False:
             status, done = downloader.next_chunk()
@@ -30,27 +30,27 @@
         output_file.write(file.getbuffer())
     file_automation_logger.info(
         f"Download file: {file_id} with name: {file_name}"
     )
     return file
 
 
-def download_file_from_folder(folder_name: str) -> Union[dict, None]:
+def drive_download_file_from_folder(folder_name: str) -> Union[dict, None]:
     try:
         files = dict()
         response = driver_instance.service.files().list(
             q=f"mimeType = 'application/vnd.google-apps.folder' and name = '{folder_name}'"
         ).execute()
         folder = response.get("files", [])[0]
         folder_id = folder.get("id")
         response = driver_instance.service.files().list(
             q=f"'{folder_id}' in parents"
         ).execute()
         for file in response.get("files", []):
-            download_file(file.get("id"), file.get("name"))
+            drive_download_file(file.get("id"), file.get("name"))
             files.update({file.get("name"): file.get("id")})
         file_automation_logger.info(
             f"Download all file on {folder_name} done."
         )
         return files
     except HttpError as error:
         file_automation_logger.error(
```

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/driver_instance.py` & `automation_file-0.0.9/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/search/search_drive.py` & `automation_file-0.0.9/file_automation/remote/google_drive/search/search_drive.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from googleapiclient.errors import HttpError
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def search_all_file() -> Union[dict, None]:
+def drive_search_all_file() -> Union[dict, None]:
     try:
         item = dict()
         response = driver_instance.service.files().list().execute()
         for file in response.get("files", []):
             item.update({file.get("name"): file.get("id")})
         file_automation_logger.info(
             f"Search all file on drive"
@@ -20,15 +20,15 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def search_file_mimetype(mime_type: str) -> Union[dict, None]:
+def drive_search_file_mimetype(mime_type: str) -> Union[dict, None]:
     try:
         files = dict()
         page_token = None
         while True:
             # pylint: disable=maybe-no-member
             response = driver_instance.service.files().list(
                 q=f"mimeType='{mime_type}'",
@@ -47,15 +47,15 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def search_field(field_pattern: str) -> Union[dict, None]:
+def drive_search_field(field_pattern: str) -> Union[dict, None]:
     try:
         files = dict()
         response = driver_instance.service.files().list(fields=field_pattern).execute()
         for file in response.get("files", []):
             files.update({file.get("name"): file.get("id")})
         file_automation_logger.info(
             f"Search all {field_pattern}"
```

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/share/share_file.py` & `automation_file-0.0.9/file_automation/remote/google_drive/share/share_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from googleapiclient.errors import HttpError
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def share_file_to_user(
+def drive_share_file_to_user(
         file_id: str, user: str, user_role: str = "writer") -> Union[dict, None]:
     try:
         service = driver_instance.service
         user_permission = {
             "type": "user",
             "role": user_role,
             "emailAddress": user
@@ -28,15 +28,15 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def share_file_to_anyone(file_id: str, share_role: str = "reader") -> Union[dict, None]:
+def drive_share_file_to_anyone(file_id: str, share_role: str = "reader") -> Union[dict, None]:
     try:
         service = driver_instance.service
         user_permission = {
             "type": "anyone",
             "value": "anyone",
             "role": share_role
         }
@@ -51,15 +51,15 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def share_file_to_domain(
+def drive_share_file_to_domain(
         file_id: str, domain: str, domain_role: str = "reader") -> Union[dict, None]:
     try:
         service = driver_instance.service
         domain_permission = {
             "type": "domain",
             "role": domain_role,
             "domain": domain
```

### Comparing `automation_file-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file-0.0.9/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from googleapiclient.errors import HttpError
 from googleapiclient.http import MediaFileUpload
 
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
-def upload_to_drive(file_path: str, file_name: str = None) -> Union[dict, None]:
+def drive_upload_to_drive(file_path: str, file_name: str = None) -> Union[dict, None]:
     try:
         file_path = Path(file_path)
         if file_path.is_file():
             file_metadata = {
                 "name": file_path.name if file_name is None else file_name,
                 "mimeType": "*/*"
             }
@@ -39,15 +39,15 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def upload_to_folder(folder_id: str, file_path: str, file_name: str = None) -> Union[dict, None]:
+def drive_upload_to_folder(folder_id: str, file_path: str, file_name: str = None) -> Union[dict, None]:
     try:
         file_path = Path(file_path)
         if file_path.is_file():
             file_metadata = {
                 "name": file_path.name if file_name is None else file_name,
                 "mimeType": "*/*",
                 "parents": [f"{folder_id}"]
@@ -76,40 +76,40 @@
         file_automation_logger.error(
             f"Delete file failed,"
             f"error: {error}"
         )
         return None
 
 
-def upload_dir_to_drive(dir_path: str) -> List[Optional[set]]:
+def drive_upload_dir_to_drive(dir_path: str) -> List[Optional[set]]:
     dir_path = Path(dir_path)
     ids = list()
     if dir_path.is_dir():
         path_list = dir_path.iterdir()
         for path in path_list:
             if path.is_file():
-                ids.append(upload_to_drive(str(path.absolute()), path.name))
+                ids.append(drive_upload_to_drive(str(path.absolute()), path.name))
         file_automation_logger.info(
             f"Upload all file on dir: {dir_path} to drive"
         )
         return ids
     else:
         file_automation_logger.error(
             FileNotFoundError
         )
 
 
-def upload_dir_to_folder(folder_id: str, dir_path: str) -> List[Optional[set]]:
+def drive_upload_dir_to_folder(folder_id: str, dir_path: str) -> List[Optional[set]]:
     dir_path = Path(dir_path)
     ids = list()
     if dir_path.is_dir():
         path_list = dir_path.iterdir()
         for path in path_list:
             if path.is_file():
-                ids.append(upload_to_folder(folder_id, str(path.absolute()), path.name))
+                ids.append(drive_upload_to_folder(folder_id, str(path.absolute()), path.name))
         file_automation_logger.info(
             f"Upload all file on dir: {dir_path} to folder: {folder_id}"
         )
         return ids
     else:
         file_automation_logger.error(
             FileNotFoundError
```

### Comparing `automation_file-0.0.8/file_automation/utils/callback/callback_function_executor.py` & `automation_file-0.0.9/file_automation/utils/callback/callback_function_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 
 from file_automation.local.dir.dir_process import copy_dir, create_dir, remove_dir_tree
 from file_automation.local.file.file_process import copy_file, remove_file, rename_file, copy_specify_extension_file, \
     copy_all_file_to_dir
 from file_automation.local.zip.zip_process import zip_dir, zip_file, zip_info, zip_file_info, set_zip_password, \
     read_zip_file, unzip_file, unzip_all
-from file_automation.remote.google_drive.delete.delete_manager import delete_file
-from file_automation.remote.google_drive.dir.folder_manager import add_folder
-from file_automation.remote.google_drive.download.download_file import download_file, download_file_from_folder
+from file_automation.remote.google_drive.delete.delete_manager import drive_delete_file
+from file_automation.remote.google_drive.dir.folder_manager import drive_add_folder
+from file_automation.remote.google_drive.download.download_file import drive_download_file, drive_download_file_from_folder
 from file_automation.remote.google_drive.driver_instance import driver_instance
 from file_automation.remote.google_drive.search.search_drive import \
-    search_all_file, search_field, search_file_mimetype
+    drive_search_all_file, drive_search_field, drive_search_file_mimetype
 from file_automation.remote.google_drive.share.share_file import \
-    share_file_to_anyone, share_file_to_domain, share_file_to_user
+    drive_share_file_to_anyone, drive_share_file_to_domain, drive_share_file_to_user
 from file_automation.remote.google_drive.upload.upload_to_driver import \
-    upload_dir_to_folder, upload_to_folder, upload_dir_to_drive, upload_to_drive
+    drive_upload_dir_to_folder, drive_upload_to_folder, drive_upload_dir_to_drive, drive_upload_to_drive
 from file_automation.utils.exception.exception_tags import get_bad_trigger_function, get_bad_trigger_method
 from file_automation.utils.exception.exceptions import CallbackExecutorException
 from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
 class CallbackFunctionExecutor(object):
 
@@ -37,28 +37,28 @@
             "zip_info": zip_info,
             "zip_file_info": zip_file_info,
             "set_zip_password": set_zip_password,
             "unzip_file": unzip_file,
             "read_zip_file": read_zip_file,
             "unzip_all": unzip_all,
             "driver_instance": driver_instance,
-            "search_all_file": search_all_file,
-            "search_field": search_field,
-            "search_file_mimetype": search_file_mimetype,
-            "upload_dir_to_folder": upload_dir_to_folder,
-            "upload_to_folder": upload_to_folder,
-            "upload_dir_to_drive": upload_dir_to_drive,
-            "upload_to_drive": upload_to_drive,
-            "add_folder": add_folder,
-            "share_file_to_anyone": share_file_to_anyone,
-            "share_file_to_domain": share_file_to_domain,
-            "share_file_to_user": share_file_to_user,
-            "delete_file": delete_file,
-            "download_file": download_file,
-            "download_file_from_folder": download_file_from_folder
+            "search_all_file": drive_search_all_file,
+            "search_field": drive_search_field,
+            "search_file_mimetype": drive_search_file_mimetype,
+            "upload_dir_to_folder": drive_upload_dir_to_folder,
+            "upload_to_folder": drive_upload_to_folder,
+            "upload_dir_to_drive": drive_upload_dir_to_drive,
+            "upload_to_drive": drive_upload_to_drive,
+            "add_folder": drive_add_folder,
+            "share_file_to_anyone": drive_share_file_to_anyone,
+            "share_file_to_domain": drive_share_file_to_domain,
+            "share_file_to_user": drive_share_file_to_user,
+            "delete_file": drive_delete_file,
+            "download_file": drive_download_file,
+            "download_file_from_folder": drive_download_file_from_folder
         }
 
     def callback_function(
             self,
             trigger_function_name: str,
             callback_function: typing.Callable,
             callback_function_param: [dict, None] = None,
```

### Comparing `automation_file-0.0.8/file_automation/utils/exception/exception_tags.py` & `automation_file-0.0.9/file_automation/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/utils/exception/exceptions.py` & `automation_file-0.0.9/file_automation/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/utils/executor/action_executor.py` & `automation_file-0.0.9/file_automation/utils/executor/action_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 import builtins
-import sys
 import types
 from inspect import getmembers, isbuiltin
 
 from file_automation.local.dir.dir_process import copy_dir, create_dir, remove_dir_tree
 from file_automation.local.file.file_process import copy_file, remove_file, rename_file, copy_specify_extension_file, \
-    copy_all_file_to_dir
+    copy_all_file_to_dir, create_file
 from file_automation.local.zip.zip_process import zip_dir, zip_file, zip_info, zip_file_info, set_zip_password, \
     read_zip_file, unzip_file, unzip_all
-from file_automation.remote.google_drive.delete.delete_manager import delete_file
-from file_automation.remote.google_drive.dir.folder_manager import add_folder
-from file_automation.remote.google_drive.download.download_file import download_file, download_file_from_folder
-from file_automation.remote.google_drive.driver_instance import driver_instance
+from file_automation.remote.google_drive.delete.delete_manager import drive_delete_file
+from file_automation.remote.google_drive.dir.folder_manager import drive_add_folder
+from file_automation.remote.google_drive.download.download_file import drive_download_file, \
+    drive_download_file_from_folder
 from file_automation.remote.google_drive.search.search_drive import \
-    search_all_file, search_field, search_file_mimetype
+    drive_search_all_file, drive_search_field, drive_search_file_mimetype
 from file_automation.remote.google_drive.share.share_file import \
-    share_file_to_anyone, share_file_to_domain, share_file_to_user
+    drive_share_file_to_anyone, drive_share_file_to_domain, drive_share_file_to_user
 from file_automation.remote.google_drive.upload.upload_to_driver import \
-    upload_dir_to_folder, upload_to_folder, upload_dir_to_drive, upload_to_drive
+    drive_upload_dir_to_folder, drive_upload_to_folder, drive_upload_dir_to_drive, drive_upload_to_drive
 from file_automation.utils.exception.exception_tags import add_command_exception, executor_list_error, \
     action_is_null_error, cant_execute_action_error
 from file_automation.utils.exception.exceptions import ExecuteActionException, AddCommandException
 from file_automation.utils.json.json_file import read_action_json
 from file_automation.utils.logging.loggin_instance import file_automation_logger
+from file_automation.utils.package_manager.package_manager_class import package_manager
 
 
 class Executor(object):
 
     def __init__(self):
         self.event_dict: dict = {
+            # File
+            "create_file": create_file,
             "copy_file": copy_file,
             "rename_file": rename_file,
             "remove_file": remove_file,
+            # Dir
             "copy_all_file_to_dir": copy_all_file_to_dir,
             "copy_specify_extension_file": copy_specify_extension_file,
             "copy_dir": copy_dir,
             "create_dir": create_dir,
             "remove_dir_tree": remove_dir_tree,
+            # Zip
             "zip_dir": zip_dir,
             "zip_file": zip_file,
             "zip_info": zip_info,
             "zip_file_info": zip_file_info,
             "set_zip_password": set_zip_password,
             "unzip_file": unzip_file,
             "read_zip_file": read_zip_file,
             "unzip_all": unzip_all,
-            "driver_instance": driver_instance,
-            "search_all_file": search_all_file,
-            "search_field": search_field,
-            "search_file_mimetype": search_file_mimetype,
-            "upload_dir_to_folder": upload_dir_to_folder,
-            "upload_to_folder": upload_to_folder,
-            "upload_dir_to_drive": upload_dir_to_drive,
-            "upload_to_drive": upload_to_drive,
-            "add_folder": add_folder,
-            "share_file_to_anyone": share_file_to_anyone,
-            "share_file_to_domain": share_file_to_domain,
-            "share_file_to_user": share_file_to_user,
-            "delete_file": delete_file,
-            "download_file": download_file,
-            "download_file_from_folder": download_file_from_folder
+            # Drive
+            "drive_search_all_file": drive_search_all_file,
+            "drive_search_field": drive_search_field,
+            "drive_search_file_mimetype": drive_search_file_mimetype,
+            "drive_upload_dir_to_folder": drive_upload_dir_to_folder,
+            "drive_upload_to_folder": drive_upload_to_folder,
+            "drive_upload_dir_to_drive": drive_upload_dir_to_drive,
+            "drive_upload_to_drive": drive_upload_to_drive,
+            "drive_add_folder": drive_add_folder,
+            "drive_share_file_to_anyone": drive_share_file_to_anyone,
+            "drive_share_file_to_domain": drive_share_file_to_domain,
+            "drive_share_file_to_user": drive_share_file_to_user,
+            "drive_delete_file": drive_delete_file,
+            "drive_download_file": drive_download_file,
+            "drive_download_file_from_folder": drive_download_file_from_folder,
+            # execute
+            "execute_action": self.execute_action,
+            "execute_files": self.execute_files,
+            "add_package_to_executor": package_manager.add_package_to_executor,
         }
         # get all builtin function and add to event dict
         for function in getmembers(builtins, isbuiltin):
             self.event_dict.update({str(function[0]): function[1]})
 
     def _execute_event(self, action: list):
         event = self.event_dict.get(action[0])
@@ -124,14 +132,15 @@
         execute_detail_list: list = list()
         for file in execute_files_list:
             execute_detail_list.append(self.execute_action(read_action_json(file)))
         return execute_detail_list
 
 
 executor = Executor()
+package_manager.executor = executor
 
 
 def add_command_to_executor(command_dict: dict):
     """
     :param command_dict: dict include command we want to add to event_dict
     """
     file_automation_logger.info(
```

### Comparing `automation_file-0.0.8/file_automation/utils/json/json_file.py` & `automation_file-0.0.9/file_automation/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/utils/logging/loggin_instance.py` & `automation_file-0.0.9/file_automation/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py` & `automation_file-0.0.9/file_automation/utils/scheduler/extend_apscheduler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Callable
 
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.schedulers.blocking import BlockingScheduler
 from apscheduler.util import undefined
 
-from file_automation.utils.logging.loggin_instance import file_automation_logger
-
 
 class SchedulerManager(object):
 
     def __init__(self):
         self._blocking_schedulers: BlockingScheduler = BlockingScheduler()
         self._background_schedulers: BackgroundScheduler = BackgroundScheduler()
 
@@ -36,23 +34,17 @@
     def get_blocking_scheduler(self):
         return self._blocking_schedulers
 
     def get_nonblocking_scheduler(self):
         return self._background_schedulers
 
     def start_block_scheduler(self, *args, **kwargs):
-        file_automation_logger.info(
-            f"Start blocking scheduler with {args}, {kwargs}"
-        )
         self._blocking_schedulers.start(*args, **kwargs)
 
     def start_nonblocking_scheduler(self, *args, **kwargs):
-        file_automation_logger.info(
-            f"Start background scheduler with {args}, {kwargs}"
-        )
         self._background_schedulers.start(*args, **kwargs)
 
     def start_all_scheduler(self, *args, **kwargs):
         self._blocking_schedulers.start(*args, **kwargs)
         self._background_schedulers.start(*args, **kwargs)
 
     def add_interval_blocking_secondly(
@@ -120,29 +112,17 @@
         self.add_blocking_job(func=function, id=id, trigger="cron", **trigger_args)
 
     def add_cron_nonblocking(
             self, function: Callable, id: str = None, **trigger_args):
         self.add_nonblocking_job(func=function, id=id, trigger="cron", **trigger_args)
 
     def remove_blocking_job(self, id: str, jobstore: str = 'default'):
-        file_automation_logger.info(
-            f"Remove blocking job {id}, store on {jobstore}"
-        )
         self._blocking_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def remove_nonblocking_job(self, id: str, jobstore: str = 'default'):
-        file_automation_logger.info(
-            f"Remove nonblocking job {id}, store on {jobstore}"
-        )
         self._background_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def shutdown_blocking_scheduler(self, wait: bool = False):
-        file_automation_logger.info(
-            f"Shutdown blocking scheduler wait = {wait}"
-        )
         self._blocking_schedulers.shutdown(wait=wait)
 
     def shutdown_nonblocking_scheduler(self, wait: bool = False):
-        file_automation_logger.info(
-            f"Shutdown nonblocking scheduler wait = {wait}"
-        )
         self._background_schedulers.shutdown(wait=wait)
```

### Comparing `automation_file-0.0.8/pyproject.toml` & `automation_file-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file"
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

