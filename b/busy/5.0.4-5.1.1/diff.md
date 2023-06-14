# Comparing `tmp/busy-5.0.4.tar.gz` & `tmp/busy-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.0.4.tar", last modified: Sun Jun  4 05:54:01 2023, max compression
+gzip compressed data, was "busy-5.1.1.tar", last modified: Wed Jun 14 07:21:39 2023, max compression
```

## Comparing `busy-5.0.4.tar` & `busy-5.1.1.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.816333 busy-5.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-04 05:53:42.000000 busy-5.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22714 2023-06-04 05:54:01.816333 busy-5.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22464 2023-06-04 05:53:42.000000 busy-5.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.805333 busy-5.0.4/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 05:53:42.000000 busy-5.0.4/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-04 05:53:42.000000 busy-5.0.4/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.810333 busy-5.0.4/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6844 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-04 05:53:42.000000 busy-5.0.4/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3551 2023-06-04 05:53:42.000000 busy-5.0.4/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.811333 busy-5.0.4/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.812333 busy-5.0.4/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-06-04 05:53:42.000000 busy-5.0.4/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.813333 busy-5.0.4/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-04 05:53:42.000000 busy-5.0.4/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-04 05:53:42.000000 busy-5.0.4/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.814333 busy-5.0.4/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6589 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.814333 busy-5.0.4/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-06-04 05:53:42.000000 busy-5.0.4/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.816333 busy-5.0.4/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/selector.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-04 05:53:42.000000 busy-5.0.4/busy/util/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 05:54:01.806333 busy-5.0.4/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22714 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1383 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-04 05:54:01.000000 busy-5.0.4/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-06-04 05:53:42.000000 busy-5.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 05:54:01.816333 busy-5.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-06-04 05:53:42.000000 busy-5.0.4/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.441178 busy-5.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-14 07:21:22.000000 busy-5.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-06-14 07:21:39.441178 busy-5.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-06-14 07:21:22.000000 busy-5.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.433178 busy-5.1.1/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:21:22.000000 busy-5.1.1/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-14 07:21:22.000000 busy-5.1.1/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.437178 busy-5.1.1/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6844 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/print_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-14 07:21:22.000000 busy-5.1.1/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2023-06-14 07:21:22.000000 busy-5.1.1/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.437178 busy-5.1.1/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.438178 busy-5.1.1/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-06-14 07:21:22.000000 busy-5.1.1/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.438178 busy-5.1.1/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-14 07:21:22.000000 busy-5.1.1/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-14 07:21:22.000000 busy-5.1.1/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.439178 busy-5.1.1/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.439178 busy-5.1.1/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-06-14 07:21:22.000000 busy-5.1.1/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.441178 busy-5.1.1/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/checklist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-14 07:21:22.000000 busy-5.1.1/busy/util/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:21:39.434178 busy-5.1.1/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 07:21:39.000000 busy-5.1.1/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-06-14 07:21:22.000000 busy-5.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 07:21:39.441178 busy-5.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-06-14 07:21:22.000000 busy-5.1.1/version
```

### Comparing `busy-5.0.4/LICENSE` & `busy-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/PKG-INFO` & `busy-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.0.4
+Version: 5.1.1
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.0.4/README.md` & `busy-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/activate_command.py` & `busy-5.1.1/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/add_command.py` & `busy-5.1.1/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/command.py` & `busy-5.1.1/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/defer_command.py` & `busy-5.1.1/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/delete_command.py` & `busy-5.1.1/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/drop_and_pop_command.py` & `busy-5.1.1/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/edit_command.py` & `busy-5.1.1/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/finish_command.py` & `busy-5.1.1/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/list_command.py` & `busy-5.1.1/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/command/switch_command.py` & `busy-5.1.1/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/handler.py` & `busy-5.1.1/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/model/collection/__init__.py` & `busy-5.1.1/busy/model/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/model/item.py` & `busy-5.1.1/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/storage/file_storage.py` & `busy-5.1.1/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/ui/curses_ui.py` & `busy-5.1.1/busy/ui/curses_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/ui/shell_ui.py` & `busy-5.1.1/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.1.1/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.1.1/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/ui/ui.py` & `busy-5.1.1/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/util/class_family.py` & `busy-5.1.1/busy/util/class_family.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/util/date_util.py` & `busy-5.1.1/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/util/selector.py` & `busy-5.1.1/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy/util/super_wrapper.py` & `busy-5.1.1/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.4/busy.egg-info/PKG-INFO` & `busy-5.1.1/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.0.4
+Version: 5.1.1
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.0.4/busy.egg-info/SOURCES.txt` & `busy-5.1.1/busy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 busy/command/curses_command.py
 busy/command/defer_command.py
 busy/command/delete_command.py
 busy/command/drop_and_pop_command.py
 busy/command/edit_command.py
 busy/command/finish_command.py
 busy/command/list_command.py
+busy/command/print_command.py
 busy/command/queues_command.py
 busy/command/resource_command.py
 busy/command/show_command.py
 busy/command/switch_command.py
 busy/command/tags_command.py
 busy/model/__init__.py
 busy/model/item.py
@@ -41,12 +42,13 @@
 busy/ui/curses_ui.py
 busy/ui/shell_ui.py
 busy/ui/ui.py
 busy/ui/tcl_ui/__init__.py
 busy/ui/tcl_ui/edit_task_widget.py
 busy/ui/tcl_ui/get_item_widget.py
 busy/util/__init__.py
+busy/util/checklist.py
 busy/util/class_family.py
 busy/util/date_util.py
 busy/util/python_version.py
 busy/util/selector.py
 busy/util/super_wrapper.py
```

### Comparing `busy-5.0.4/pyproject.toml` & `busy-5.1.1/pyproject.toml`

 * *Files identical despite different names*

