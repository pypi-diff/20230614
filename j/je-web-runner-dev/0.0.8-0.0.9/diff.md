# Comparing `tmp/je_web_runner_dev-0.0.8.tar.gz` & `tmp/je_web_runner_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_web_runner_dev-0.0.8.tar", last modified: Sat May 14 08:00:11 2022, max compression
+gzip compressed data, was "dist\je_web_runner_dev-0.0.9.tar", last modified: Sun May 15 14:01:03 2022, max compression
```

## Comparing `je_web_runner_dev-0.0.8.tar` & `je_web_runner_dev-0.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      712 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0      980 2022-05-14 08:00:09.000000 je_web_runner_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner/
--rw-rw-rw-   0        0        0      995 2022-05-14 03:49:03.000000 je_web_runner_dev-0.0.8/je_web_runner/__init__.py
--rw-rw-rw-   0        0        0        0 2022-05-08 23:05:18.000000 je_web_runner_dev-0.0.8/je_web_runner/__main__.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/
--rw-rw-rw-   0        0        0       52 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/
--rw-rw-rw-   0        0        0       73 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/__init__.py
--rw-rw-rw-   0        0        0      855 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/
--rw-rw-rw-   0        0        0       46 2022-05-10 14:12:01.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/__init__.py
--rw-rw-rw-   0        0        0      842 2022-05-14 03:51:31.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/web_element_wrapper.py
--rw-rw-rw-   0        0        0     1826 2022-05-14 02:44:04.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_manager.py
--rw-rw-rw-   0        0        0     2081 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_with_options.py
--rw-rw-rw-   0        0        0     6510 2022-05-14 03:05:39.000000 je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_wrapper.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/
--rw-rw-rw-   0        0        0       35 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/assert_value/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:50:02.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/assert_value/__init__.py
--rw-rw-rw-   0        0        0     2793 2022-05-14 03:52:14.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/assert_value/result_check.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/exception/
--rw-rw-rw-   0        0        0       45 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      698 2022-05-09 03:28:45.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/exception/exception_tag.py
--rw-rw-rw-   0        0        0      512 2022-05-13 15:16:15.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/executor/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:59:45.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     2821 2022-05-14 02:44:04.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/executor/executor.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/file_process/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      298 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/file_process/create_project_structure.py
--rw-rw-rw-   0        0        0      711 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1271 2022-05-09 03:28:46.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1094 2022-05-09 03:29:42.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/
--rw-rw-rw-   0        0        0        0 2022-05-13 21:15:19.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/__init__.py
--rw-rw-rw-   0        0        0      656 2022-05-11 07:54:28.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_class.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_record/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:49:43.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_record/__init__.py
--rw-rw-rw-   0        0        0      549 2022-05-13 21:16:22.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_record/
--rw-rw-rw-   0        0        0        0 2022-05-08 23:22:33.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      197 2022-05-08 23:44:10.000000 je_web_runner_dev-0.0.8/je_web_runner/utils/test_record/test_record.py
-drwxrwxrwx   0        0        0        0 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/
--rw-rw-rw-   0        0        0      712 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1819 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-05-14 08:00:10.000000 je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-14 08:00:11.000000 je_web_runner_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      972 2022-05-13 20:58:08.000000 je_web_runner_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      712 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      980 2022-05-15 14:01:01.000000 je_web_runner_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner/
+-rw-rw-rw-   0        0        0      995 2022-05-14 03:49:03.000000 je_web_runner_dev-0.0.9/je_web_runner/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:05:18.000000 je_web_runner_dev-0.0.9/je_web_runner/__main__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/
+-rw-rw-rw-   0        0        0       52 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/
+-rw-rw-rw-   0        0        0       73 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/__init__.py
+-rw-rw-rw-   0        0        0      855 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/
+-rw-rw-rw-   0        0        0       46 2022-05-10 14:12:01.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1513 2022-05-14 18:47:14.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/web_element_wrapper.py
+-rw-rw-rw-   0        0        0     1831 2022-05-14 19:44:19.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_manager.py
+-rw-rw-rw-   0        0        0     2081 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_with_options.py
+-rw-rw-rw-   0        0        0     8213 2022-05-14 20:07:26.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_wrapper.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/
+-rw-rw-rw-   0        0        0       35 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:50:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/__init__.py
+-rw-rw-rw-   0        0        0     2793 2022-05-14 03:52:14.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/result_check.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/
+-rw-rw-rw-   0        0        0       45 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      698 2022-05-09 03:28:45.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      512 2022-05-13 15:16:15.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:59:45.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     2821 2022-05-14 02:44:04.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/executor.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      298 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/create_project_structure.py
+-rw-rw-rw-   0        0        0      711 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1271 2022-05-09 03:28:46.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1094 2022-05-09 03:29:42.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/
+-rw-rw-rw-   0        0        0        0 2022-05-13 21:15:19.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/__init__.py
+-rw-rw-rw-   0        0        0      656 2022-05-11 07:54:28.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_class.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:49:43.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/__init__.py
+-rw-rw-rw-   0        0        0      549 2022-05-13 21:16:22.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:22:33.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      197 2022-05-08 23:44:10.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/test_record.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/
+-rw-rw-rw-   0        0        0      712 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1819 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      972 2022-05-13 20:58:08.000000 je_web_runner_dev-0.0.9/setup.py
```

### Comparing `je_web_runner_dev-0.0.8/LICENSE` & `je_web_runner_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/PKG-INFO` & `je_web_runner_dev-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_web_runner_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: selenium get_webdriver_wrapper
 Home-page: https://github.com/JE-Chen/WebRunner
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_web_runner_dev-0.0.8/dev_setup.py` & `je_web_runner_dev-0.0.9/dev_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_web_runner_dev",
-    version="0.0.08",
+    version="0.0.09",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="selenium get_webdriver_wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/WebRunner",
     packages=setuptools.find_packages(),
```

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/__init__.py` & `je_web_runner_dev-0.0.9/je_web_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py` & `je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_manager.py` & `je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 from je_web_runner.selenium_wrapper.webdriver_wrapper import webdriver_wrapper
 from je_web_runner.utils.test_object.test_object_record.test_object_record_class import test_object_record
 
 
 class WebdriverManager(object):
 
     def __init__(self, **kwargs):
-        self.current_webdriver_list = list()
+        self._current_webdriver_list = list()
         self.webdriver_wrapper = webdriver_wrapper
         self.webdriver_element = web_element_wrapper
         self.current_webdriver: [WebDriver, None] = None
 
     def new_driver(self, webdriver_name: str, opera_path: str = None, **kwargs):
         self.current_webdriver = webdriver_wrapper.set_driver(webdriver_name, opera_path, **kwargs)
-        self.current_webdriver_list.append(self.current_webdriver)
+        self._current_webdriver_list.append(self.current_webdriver)
 
     def change_webdriver(self, index_of_webdriver: int):
-        self.current_webdriver = self.current_webdriver_list[index_of_webdriver]
+        self.current_webdriver = self._current_webdriver_list[index_of_webdriver]
         self.webdriver_wrapper.current_webdriver = self.current_webdriver
 
     def quit(self):
-        if self.current_webdriver_list is None:
+        if self._current_webdriver_list is None:
             raise WebDriverIsNoneException(selenium_wrapper_web_driver_not_found_error)
         test_object_record.clean_record()
-        for not_closed_webdriver in self.current_webdriver_list:
+        for not_closed_webdriver in self._current_webdriver_list:
             not_closed_webdriver.close()
         self.current_webdriver.quit()
 
 
 def get_webdriver_manager(webdriver_name: str, opera_path: str = None, **kwargs):
     web_runner.new_driver(webdriver_name, opera_path)
     return web_runner
```

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_with_options.py` & `je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_with_options.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/selenium_wrapper/webdriver_wrapper.py` & `je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium import webdriver
+from selenium.webdriver.support.wait import WebDriverWait
 
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.opera import OperaDriverManager
 from webdriver_manager.microsoft import IEDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from webdriver_manager.utils import ChromeType
@@ -56,15 +58,17 @@
 }
 
 
 class WebDriverWrapper(object):
 
     def __init__(self):
         self.current_webdriver: [WebDriver, None] = None
-        self.webdriver_name: [str, None] = None
+        self._webdriver_name: [str, None] = None
+
+    # start a new webdriver
 
     def set_driver(self, webdriver_name: str, opera_path: str = None, **kwargs):
         webdriver_name = str(webdriver_name).lower()
         webdriver_value = _webdriver_dict.get(webdriver_name)
         if webdriver_value is None:
             raise WebDriverNotFoundException(selenium_wrapper_web_driver_not_found_error)
         webdriver_install_manager = _webdriver_manager_dict.get(webdriver_name)
@@ -78,24 +82,23 @@
                 executable_path=_webdriver_manager_dict.get(webdriver_name)().install(), options=opera_options, **kwargs
             )
         else:
             webdriver_service = _webdriver_service_dict.get(webdriver_name)(
                 webdriver_install_manager().install(),
             )
             self.current_webdriver = webdriver_value(service=webdriver_service, **kwargs)
-            self.webdriver_name = webdriver_name
+            self._webdriver_name = webdriver_name
         return self.current_webdriver
 
-    def to_url(self, url: str):
-        self.current_webdriver.get(url)
-
     def set_webdriver_options_capability(self, key_and_vale_dict: dict):
-        if self.webdriver_name is None:
+        if self._webdriver_name is None:
             raise WebDriverIsNoneException(selenium_wrapper_web_driver_not_found_error)
-        set_webdriver_options_capability_wrapper(self.webdriver_name, key_and_vale_dict)
+        set_webdriver_options_capability_wrapper(self._webdriver_name, key_and_vale_dict)
+
+    # web element
 
     def find_element(self, test_object: TestObject):
         if self.current_webdriver is None:
             raise WebDriverIsNoneException(selenium_wrapper_web_driver_not_found_error)
         web_element_wrapper.current_web_element = self.current_webdriver.find_element(
             test_object.test_object_type, test_object.test_object_name)
         return web_element_wrapper.current_web_element
@@ -121,17 +124,56 @@
             raise WebDriverIsNoneException(selenium_wrapper_web_driver_not_found_error)
         web_element_wrapper.current_web_element_list = self.current_webdriver.find_elements(
             test_object_record.test_object_record_dict.get(element_name).test_object_type,
             test_object_record.test_object_record_dict.get(element_name).test_object_name
         )
         return web_element_wrapper.current_web_element
 
+    # wait
+
     def wait_implicitly(self, time_to_wait: int):
         self.current_webdriver.implicitly_wait(time_to_wait)
 
+    def explict_wait(self, wait_time: int, statement, until_type: bool = True):
+        if until_type:
+            return WebDriverWait(self.current_webdriver, wait_time).until(statement)
+        else:
+            return WebDriverWait(self.current_webdriver, wait_time).until_not(statement)
+
+    # webdriver url redirect
+
+    def to_url(self, url: str):
+        self.current_webdriver.get(url)
+
+    # webdriver new page
+    def switch(self, switch_type: str, switchy_target_name: str = None):
+        switch_type = switch_type.lower()
+        switch_type_dict = {
+            "active_element": self.current_webdriver.switch_to.active_element,
+            "default_content": self.current_webdriver.switch_to.default_content,
+            "frame": self.current_webdriver.switch_to.frame,
+            "parent_frame": self.current_webdriver.switch_to.parent_frame,
+            "window": self.current_webdriver.switch_to.window,
+        }
+        try:
+            switch_type_dict.update(
+                {"alert": self.current_webdriver.switch_to.alert}
+            )
+        except NoAlertPresentException as error:
+            switch_type_dict.update(
+                {"alert": None}
+            )
+        if switch_type in ["active_element", "alert"]:
+            return switch_type_dict.get(switch_type)
+        elif switch_type in ["default_content", "parent_frame"]:
+            return switch_type_dict.get(switch_type)()
+        else:
+            return switch_type_dict.get(switch_type)(switchy_target_name)
+
+    # webdriver wrapper add function
     def check_current_webdriver(self, check_dict: dict):
         check_webdriver(self.current_webdriver, check_dict)
 
     def quit(self):
         test_object_record.clean_record()
         self.current_webdriver.quit()
```

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/assert_value/result_check.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/result_check.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/exception/exception_tag.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exception_tag.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/exception/exceptions.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/executor/executor.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/executor/executor.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/file_process/get_dir_file_list.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_file/json_file.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/json/json_format/json_process.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_class.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_class.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/PKG-INFO` & `je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-web-runner-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: selenium get_webdriver_wrapper
 Home-page: https://github.com/JE-Chen/WebRunner
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_web_runner_dev-0.0.8/je_web_runner_dev.egg-info/SOURCES.txt` & `je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_web_runner_dev-0.0.8/setup.py` & `je_web_runner_dev-0.0.9/setup.py`

 * *Files identical despite different names*

