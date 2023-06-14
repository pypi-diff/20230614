# Comparing `tmp/je_web_runner-0.0.8.tar.gz` & `tmp/je_web_runner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_web_runner-0.0.8.tar", last modified: Wed May 18 06:42:39 2022, max compression
+gzip compressed data, was "dist\je_web_runner-0.0.9.tar", last modified: Fri May 20 19:38:59 2022, max compression
```

## Comparing `je_web_runner-0.0.8.tar` & `je_web_runner-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-05-06 19:45:56.000000 je_web_runner-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      708 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-05-06 19:45:56.000000 je_web_runner-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/
--rw-rw-rw-   0        0        0     1077 2022-05-18 06:12:02.000000 je_web_runner-0.0.8/je_web_runner/__init__.py
--rw-rw-rw-   0        0        0        0 2022-05-08 23:05:18.000000 je_web_runner-0.0.8/je_web_runner/__main__.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/
--rw-rw-rw-   0        0        0       52 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/
--rw-rw-rw-   0        0        0       73 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/__init__.py
--rw-rw-rw-   0        0        0      855 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/keys/
--rw-rw-rw-   0        0        0        0 2022-05-18 06:06:23.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/keys/__init__.py
--rw-rw-rw-   0        0        0       47 2022-05-18 06:09:13.000000 je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/keys/selenium_keys.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/
--rw-rw-rw-   0        0        0       46 2022-05-10 14:12:01.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/__init__.py
--rw-rw-rw-   0        0        0      972 2022-05-18 06:23:59.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/web_element_wrapper.py
--rw-rw-rw-   0        0        0     2449 2022-05-18 02:28:40.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_manager.py
--rw-rw-rw-   0        0        0     2081 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_with_options.py
--rw-rw-rw-   0        0        0    13558 2022-05-18 06:24:39.000000 je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_wrapper.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/
--rw-rw-rw-   0        0        0       35 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/assert_value/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:50:02.000000 je_web_runner-0.0.8/je_web_runner/utils/assert_value/__init__.py
--rw-rw-rw-   0        0        0     2793 2022-05-14 03:52:14.000000 je_web_runner-0.0.8/je_web_runner/utils/assert_value/result_check.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/exception/
--rw-rw-rw-   0        0        0       45 2022-05-07 17:33:02.000000 je_web_runner-0.0.8/je_web_runner/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      698 2022-05-09 03:28:45.000000 je_web_runner-0.0.8/je_web_runner/utils/exception/exception_tag.py
--rw-rw-rw-   0        0        0      512 2022-05-13 15:16:15.000000 je_web_runner-0.0.8/je_web_runner/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/executor/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:59:45.000000 je_web_runner-0.0.8/je_web_runner/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     2821 2022-05-15 23:54:03.000000 je_web_runner-0.0.8/je_web_runner/utils/executor/executor.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/file_process/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      298 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/file_process/create_project_structure.py
--rw-rw-rw-   0        0        0      711 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/json/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1271 2022-05-09 03:28:46.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2022-05-06 19:46:48.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1094 2022-05-09 03:29:42.000000 je_web_runner-0.0.8/je_web_runner/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/
--rw-rw-rw-   0        0        0        0 2022-05-13 21:15:19.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/__init__.py
--rw-rw-rw-   0        0        0      656 2022-05-11 07:54:28.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_class.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_record/
--rw-rw-rw-   0        0        0        0 2022-05-08 22:49:43.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_record/__init__.py
--rw-rw-rw-   0        0        0      549 2022-05-13 21:16:22.000000 je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner/utils/test_record/
--rw-rw-rw-   0        0        0        0 2022-05-08 23:22:33.000000 je_web_runner-0.0.8/je_web_runner/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      197 2022-05-08 23:44:10.000000 je_web_runner-0.0.8/je_web_runner/utils/test_record/test_record.py
-drwxrwxrwx   0        0        0        0 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/
--rw-rw-rw-   0        0        0      708 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1899 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/je_web_runner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-18 06:42:39.000000 je_web_runner-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      972 2022-05-18 06:42:37.000000 je_web_runner-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-06 19:45:56.000000 je_web_runner-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1282 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2022-05-19 02:29:36.000000 je_web_runner-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/
+-rw-rw-rw-   0        0        0     1077 2022-05-18 06:12:02.000000 je_web_runner-0.0.9/je_web_runner/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:05:18.000000 je_web_runner-0.0.9/je_web_runner/__main__.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/
+-rw-rw-rw-   0        0        0       52 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/
+-rw-rw-rw-   0        0        0       73 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/__init__.py
+-rw-rw-rw-   0        0        0      855 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/keys/
+-rw-rw-rw-   0        0        0        0 2022-05-18 06:06:23.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/keys/__init__.py
+-rw-rw-rw-   0        0        0       47 2022-05-18 06:09:13.000000 je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/keys/selenium_keys.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/
+-rw-rw-rw-   0        0        0       46 2022-05-10 14:12:01.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      972 2022-05-18 06:23:59.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/web_element_wrapper.py
+-rw-rw-rw-   0        0        0     2449 2022-05-18 02:28:40.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_manager.py
+-rw-rw-rw-   0        0        0     2081 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_with_options.py
+-rw-rw-rw-   0        0        0    19751 2022-05-20 18:47:34.000000 je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_wrapper.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/
+-rw-rw-rw-   0        0        0       35 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/assert_value/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:50:02.000000 je_web_runner-0.0.9/je_web_runner/utils/assert_value/__init__.py
+-rw-rw-rw-   0        0        0     2793 2022-05-14 03:52:14.000000 je_web_runner-0.0.9/je_web_runner/utils/assert_value/result_check.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/exception/
+-rw-rw-rw-   0        0        0       45 2022-05-07 17:33:02.000000 je_web_runner-0.0.9/je_web_runner/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      698 2022-05-09 03:28:45.000000 je_web_runner-0.0.9/je_web_runner/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      512 2022-05-13 15:16:15.000000 je_web_runner-0.0.9/je_web_runner/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:59:45.000000 je_web_runner-0.0.9/je_web_runner/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6362 2022-05-20 18:47:34.000000 je_web_runner-0.0.9/je_web_runner/utils/executor/executor.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      298 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/file_process/create_project_structure.py
+-rw-rw-rw-   0        0        0      711 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1271 2022-05-09 03:28:46.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:48.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1094 2022-05-09 03:29:42.000000 je_web_runner-0.0.9/je_web_runner/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/
+-rw-rw-rw-   0        0        0        0 2022-05-13 21:15:19.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/__init__.py
+-rw-rw-rw-   0        0        0      656 2022-05-11 07:54:28.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_class.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:49:43.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_record/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-05-20 17:20:05.000000 je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:22:33.000000 je_web_runner-0.0.9/je_web_runner/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      197 2022-05-08 23:44:10.000000 je_web_runner-0.0.9/je_web_runner/utils/test_record/test_record.py
+drwxrwxrwx   0        0        0        0 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/
+-rw-rw-rw-   0        0        0     1282 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1899 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/je_web_runner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-20 19:38:59.000000 je_web_runner-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      972 2022-05-20 19:38:58.000000 je_web_runner-0.0.9/setup.py
```

### Comparing `je_web_runner-0.0.8/LICENSE` & `je_web_runner-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/__init__.py` & `je_web_runner-0.0.9/je_web_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py` & `je_web_runner-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/selenium_wrapper/web_element_wrapper.py` & `je_web_runner-0.0.9/je_web_runner/selenium_wrapper/web_element_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_manager.py` & `je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_manager.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_with_options.py` & `je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_with_options.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/selenium_wrapper/webdriver_wrapper.py` & `je_web_runner-0.0.9/je_web_runner/selenium_wrapper/webdriver_wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -217,62 +217,171 @@
     def execute_async_script(self, script: str, *args):
         self.current_webdriver.execute_async_script(script, *args)
 
     # ActionChains
     def move_to_element(self, targe_element: WebElement):
         self._action_chain.move_to_element(targe_element)
 
+    def move_to_element_with_test_object(self, element_name: str):
+        element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(element_name).test_object_name
+        )
+        self._action_chain.move_to_element(element)
+
     def move_to_element_with_offset(self, target_element: WebElement, x: int, y: int):
         self._action_chain.move_to_element_with_offset(target_element, x, y)
 
+    def move_to_element_with_offset_and_test_object(self, element_name: str, x: int, y: int):
+        element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(element_name).test_object_name
+        )
+        self._action_chain.move_to_element_with_offset(element, x, y)
+
     def drag_and_drop(self, web_element: WebElement, targe_element: WebElement):
         self._action_chain.drag_and_drop(web_element, targe_element)
 
+    def drag_and_drop_with_test_object(self, element_name: str, target_element_name: str):
+        element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(element_name).test_object_name
+        )
+        another_element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(target_element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(target_element_name).test_object_name
+        )
+        self._action_chain.drag_and_drop(element, another_element)
+
     def drag_and_drop_offset(self, web_element: WebElement, target_x: int, target_y: int):
         self._action_chain.drag_and_drop_by_offset(web_element, target_x, target_y)
 
+    def drag_and_drop_offset_with_test_object(self, element_name: str, target_x: int, target_y: int):
+        element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(element_name).test_object_name
+        )
+        self._action_chain.drag_and_drop_by_offset(element, target_x, target_y)
+
     def perform(self):
         self._action_chain.perform()
 
     def reset_actions(self):
         self._action_chain.reset_actions()
 
     def left_click(self, on_element: WebElement = None):
         self._action_chain.click(on_element)
 
+    def left_click_with_test_object(self, element_name: str = None):
+        if element_name is None:
+            self._action_chain.click(None)
+        else:
+            element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.click(element)
+
     def left_click_and_hold(self, on_element: WebElement = None):
         self._action_chain.click_and_hold(on_element)
 
+    def left_click_and_hold_with_test_object(self, element_name: str = None):
+        if element_name is None:
+            self._action_chain.click_and_hold(None)
+        else:
+            element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.click_and_hold(element)
+
     def right_click(self, on_element: WebElement = None):
         self._action_chain.context_click(on_element)
 
+    def right_click_with_test_object(self, element_name: str = None):
+        if element_name is None:
+            self._action_chain.context_click(None)
+        else:
+            element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.context_click(element)
+
     def left_double_click(self, on_element: WebElement = None):
         self._action_chain.double_click(on_element)
 
+    def left_double_click_with_test_object(self, element_name: str = None):
+        if element_name is None:
+            self._action_chain.double_click(None)
+        else:
+            web_element_wrapper.current_web_element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.double_click(web_element_wrapper.current_web_element)
+
     def release(self, on_element: WebElement = None):
         self._action_chain.release(on_element)
 
+    def release_with_test_object(self, element_name: str = None):
+        if element_name is None:
+            self._action_chain.release(None)
+        else:
+            web_element_wrapper.current_web_element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.release(web_element_wrapper.current_web_element)
+
     def press_key(self, keycode_on_key_class, on_element: WebElement = None):
         self._action_chain.key_down(keycode_on_key_class, on_element)
 
+    def press_key_with_test_object(self, keycode_on_key_class, element_name: str = None):
+        if element_name is None:
+            self._action_chain.key_down(keycode_on_key_class, None)
+        else:
+            web_element_wrapper.current_web_element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.key_down(keycode_on_key_class, web_element_wrapper.current_web_element)
+
     def release_key(self, keycode_on_key_class, on_element: WebElement = None):
         self._action_chain.key_up(keycode_on_key_class, on_element)
 
+    def release_key_with_test_object(self, keycode_on_key_class, element_name: str = None):
+        if element_name is None:
+            self._action_chain.key_up(keycode_on_key_class, None)
+        else:
+            web_element_wrapper.current_web_element = self.current_webdriver.find_element(
+                test_object_record.test_object_record_dict.get(element_name).test_object_type,
+                test_object_record.test_object_record_dict.get(element_name).test_object_name
+            )
+            self._action_chain.key_up(keycode_on_key_class, web_element_wrapper.current_web_element)
+
     def move_by_offset(self, x: int, y: int):
         self._action_chain.move_by_offset(x, y)
 
     def pause(self, seconds: int):
         self._action_chain.pause(seconds)
 
-    def send_keys(self, *keys_to_send):
+    def send_keys(self, keys_to_send):
         self._action_chain.send_keys(*keys_to_send)
 
-    def send_keys_to_element(self, element: WebElement, *keys_to_send):
+    def send_keys_to_element(self, element: WebElement, keys_to_send):
         self._action_chain.send_keys_to_element(element, *keys_to_send)
 
+    def send_keys_to_element_with_test_object(self, element_name: str, keys_to_send):
+        web_element_wrapper.current_web_element = self.current_webdriver.find_element(
+            test_object_record.test_object_record_dict.get(element_name).test_object_type,
+            test_object_record.test_object_record_dict.get(element_name).test_object_name
+        )
+        self._action_chain.send_keys_to_element(web_element_wrapper.current_web_element, *keys_to_send)
+
     def scroll(self, x: int, y: int, delta_x: int, delta_y: int, duration: int = 0, origin: str = "viewport"):
         self._action_chain.scroll(x, y, delta_x, delta_y, duration, origin)
 
     # webdriver wrapper add function
     def check_current_webdriver(self, check_dict: dict):
         check_webdriver(self.current_webdriver, check_dict)
```

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/assert_value/result_check.py` & `je_web_runner-0.0.9/je_web_runner/utils/assert_value/result_check.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/exception/exception_tag.py` & `je_web_runner-0.0.9/je_web_runner/utils/exception/exception_tag.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/exception/exceptions.py` & `je_web_runner-0.0.9/je_web_runner/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/file_process/get_dir_file_list.py` & `je_web_runner-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/json/json_file/json_file.py` & `je_web_runner-0.0.9/je_web_runner/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/json/json_format/json_process.py` & `je_web_runner-0.0.9/je_web_runner/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_class.py` & `je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_class.py`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py` & `je_web_runner-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,12 @@
     def clean_record(self):
         self.test_object_record_dict = dict()
 
     def save_test_object(self, test_object_name: str, object_type=None, **kwargs):
         test_object = TestObject(test_object_name, object_type)
         self.test_object_record_dict.update({test_object.test_object_name: test_object})
 
+    def remove_test_object(self, test_object_name: str):
+        return self.test_object_record_dict.pop(test_object_name, False)
+
 
 test_object_record = TestObjectRecord()
```

### Comparing `je_web_runner-0.0.8/je_web_runner.egg-info/SOURCES.txt` & `je_web_runner-0.0.9/je_web_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_web_runner-0.0.8/setup.py` & `je_web_runner-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_web_runner",
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

