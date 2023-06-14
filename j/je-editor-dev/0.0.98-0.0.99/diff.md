# Comparing `tmp/je_editor_dev-0.0.98.tar.gz` & `tmp/je_editor_dev-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.98.tar", last modified: Wed May  3 09:48:13 2023, max compression
+gzip compressed data, was "je_editor_dev-0.0.99.tar", last modified: Wed May  3 10:06:33 2023, max compression
```

## Comparing `je_editor_dev-0.0.98.tar` & `je_editor_dev-0.0.99.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.970224 je_editor_dev-0.0.98/
--rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/LICENSE
--rw-rw-rw-   0        0        0     3097 2023-05-03 09:48:13.969221 je_editor_dev-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.98/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.700687 je_editor_dev-0.0.98/je_editor/
--rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.98/je_editor/__init__.py
--rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.705692 je_editor_dev-0.0.98/je_editor/pyside_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.712717 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/__init__.py
--rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/auto_save_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.736865 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/
--rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/__init__.py
--rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.743976 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/__init__.py
--rw-rw-rw-   0        0        0     7891 2023-05-03 09:43:32.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/code_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.752139 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/
--rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/__init__.py
--rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/code_record.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.757148 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/
--rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/colors/global_color.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.768159 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/open_file_dialog.py
--rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/save_file_dialog.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.771154 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.778212 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0     7183 2023-05-03 09:19:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.785169 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/ui_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.789356 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.796363 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/
--rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.804369 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
--rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.812362 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
--rw-rw-rw-   0        0        0     1307 2023-05-03 09:35:31.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.820361 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/
--rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.828365 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/
--rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
--rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
--rw-rw-rw-   0        0        0     1317 2023-05-03 09:36:21.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.839357 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:33:51.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/__init__.py
--rw-rw-rw-   0        0        0     2740 2023-05-03 09:46:50.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/venv_menu/build_venv_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.853389 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/
--rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_error_box.py
--rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_text_box.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.861360 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/
--rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/__init__.py
--rw-rw-rw-   0        0        0     6278 2023-05-03 09:33:27.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/shell_exec.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.870356 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/python_syntax.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.875737 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.880810 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.885813 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/__init__.py
--rw-rw-rw-   0        0        0      664 2023-05-03 09:19:02.000000 je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/user_setting_file.py
--rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.98/je_editor/start_editor.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.890697 je_editor_dev-0.0.98/je_editor/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.896711 je_editor_dev-0.0.98/je_editor/utils/encodings/
--rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.98/je_editor/utils/encodings/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.98/je_editor/utils/encodings/python_encodings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.904707 je_editor_dev-0.0.98/je_editor/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.98/je_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.908340 je_editor_dev-0.0.98/je_editor/utils/file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.912773 je_editor_dev-0.0.98/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.98/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.917772 je_editor_dev-0.0.98/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.98/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.924775 je_editor_dev-0.0.98/je_editor/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.98/je_editor/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.98/je_editor/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.929296 je_editor_dev-0.0.98/je_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.933316 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.98/je_editor/utils/redirect_manager/redirect_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:13.966230 je_editor_dev-0.0.98/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     3097 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 09:48:13.000000 je_editor_dev-0.0.98/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1134 2023-05-03 09:47:47.000000 je_editor_dev-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 09:48:13.971227 je_editor_dev-0.0.98/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.466696 je_editor_dev-0.0.99/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0     3097 2023-05-03 10:06:33.464700 je_editor_dev-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.152972 je_editor_dev-0.0.99/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.99/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.160051 je_editor_dev-0.0.99/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.165967 je_editor_dev-0.0.99/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.176246 je_editor_dev-0.0.99/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.183633 je_editor_dev-0.0.99/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     7891 2023-05-03 09:43:32.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.193035 je_editor_dev-0.0.99/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.200050 je_editor_dev-0.0.99/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.214096 je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.217382 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.225312 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     7183 2023-05-03 09:19:02.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.233141 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.239152 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.247149 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.257162 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.264363 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-03 09:35:31.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.270360 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.277374 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4058 2023-05-03 05:07:29.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1317 2023-05-03 09:36:21.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.284368 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/venv_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:33:51.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/venv_menu/__init__.py
+-rw-rw-rw-   0        0        0     5459 2023-05-03 10:02:52.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/venv_menu/build_venv_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.295805 je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.303062 je_editor_dev-0.0.99/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     6278 2023-05-03 09:33:27.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.311169 je_editor_dev-0.0.99/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.314083 je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.323929 je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.331900 je_editor_dev-0.0.99/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-05-03 09:19:02.000000 je_editor_dev-0.0.99/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      505 2023-05-02 08:43:36.000000 je_editor_dev-0.0.99/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.337202 je_editor_dev-0.0.99/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.346833 je_editor_dev-0.0.99/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.99/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.99/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.362610 je_editor_dev-0.0.99/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.99/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.366610 je_editor_dev-0.0.99/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.377010 je_editor_dev-0.0.99/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.99/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.384974 je_editor_dev-0.0.99/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.99/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.395007 je_editor_dev-0.0.99/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.99/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.99/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.409371 je_editor_dev-0.0.99/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.418292 je_editor_dev-0.0.99/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.99/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.99/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:06:33.461696 je_editor_dev-0.0.99/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     3097 2023-05-03 10:06:33.000000 je_editor_dev-0.0.99/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-05-03 10:06:33.000000 je_editor_dev-0.0.99/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:06:33.000000 je_editor_dev-0.0.99/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 10:06:33.000000 je_editor_dev-0.0.99/je_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 10:06:33.000000 je_editor_dev-0.0.99/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1134 2023-05-03 10:05:27.000000 je_editor_dev-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:06:33.467773 je_editor_dev-0.0.99/setup.cfg
```

### Comparing `je_editor_dev-0.0.98/LICENSE` & `je_editor_dev-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/PKG-INFO` & `je_editor_dev-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor_dev
-Version: 0.0.98
+Version: 0.0.99
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.98/README.md` & `je_editor_dev-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/__init__.py` & `je_editor_dev-0.0.99/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/__main__.py` & `je_editor_dev-0.0.99/je_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/auto_save/auto_save_thread.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/auto_save/auto_save_thread.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/code_editor/code_edit_plaintext.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/code_editor/code_edit_plaintext.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/code_process/code_exec.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/code_result/code_record.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/code_result/code_record.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/open_file_dialog.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/open_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/file_dialog/save_file_dialog.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/file_dialog/save_file_dialog.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/main_ui_setting/ui_setting.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/main_ui_setting/ui_setting.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_error_box.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/search_error_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/search_ui/search_text_box.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/search_ui/search_text_box.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/shell_process/shell_exec.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/shell_process/shell_exec.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/syntax/python_syntax.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/syntax/python_syntax.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/pyside_ui/user_setting/user_setting_file.py` & `je_editor_dev-0.0.99/je_editor/pyside_ui/user_setting/user_setting_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/encodings/python_encodings.py` & `je_editor_dev-0.0.99/je_editor/utils/encodings/python_encodings.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/exception/exception_tags.py` & `je_editor_dev-0.0.99/je_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/file/open/open_file.py` & `je_editor_dev-0.0.99/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/file/save/save_file.py` & `je_editor_dev-0.0.99/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/json/json_file.py` & `je_editor_dev-0.0.99/je_editor/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/json_format/json_process.py` & `je_editor_dev-0.0.99/je_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor/utils/redirect_manager/redirect_manager_class.py` & `je_editor_dev-0.0.99/je_editor/utils/redirect_manager/redirect_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/je_editor_dev.egg-info/PKG-INFO` & `je_editor_dev-0.0.99/je_editor_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor-dev
-Version: 0.0.98
+Version: 0.0.99
 Summary: JEditor is basic but powerful editor for python
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/je_editor
 Project-URL: Documentation, https://je-editor.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/JE-Chen/je_editor
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_editor_dev-0.0.98/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.99/je_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.98/pyproject.toml` & `je_editor_dev-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_editor_dev"
-version = "0.0.98"
+version = "0.0.99"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "JEditor is basic but powerful editor for python"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

