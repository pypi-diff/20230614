# Comparing `tmp/pytk_net-0.1.1.tar.gz` & `tmp/pytk_net-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytk_net-0.1.1.tar", last modified: Wed Jun 14 06:05:00 2023, max compression
+gzip compressed data, was "dist\pytk_net-0.1.2.tar", last modified: Wed Jun 14 14:25:28 2023, max compression
```

## Comparing `pytk_net-0.1.1.tar` & `pytk_net-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:05:00.343256 pytk_net-0.1.1/
--rw-rw-rw-   0        0        0      966 2023-06-14 06:05:00.343256 pytk_net-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:05:00.332102 pytk_net-0.1.1/pytk_net/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.1.1/pytk_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:05:00.341405 pytk_net-0.1.1/pytk_net/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.1.1/pytk_net/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.1.1/pytk_net/icons/bootstrap-icons.woff
--rw-rw-rw-   0        0        0     2039 2023-06-09 06:17:45.000000 pytk_net-0.1.1/pytk_net/utils.py
--rw-rw-rw-   0        0        0      326 2023-06-14 03:20:06.000000 pytk_net-0.1.1/pytk_net/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:05:00.338409 pytk_net-0.1.1/pytk_net.egg-info/
--rw-rw-rw-   0        0        0      966 2023-06-14 06:05:00.000000 pytk_net-0.1.1/pytk_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-14 06:05:00.000000 pytk_net-0.1.1/pytk_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:05:00.000000 pytk_net-0.1.1/pytk_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 06:05:00.000000 pytk_net-0.1.1/pytk_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:05:00.343256 pytk_net-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-14 06:04:54.000000 pytk_net-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:25:28.317828 pytk_net-0.1.2/
+-rw-rw-rw-   0        0        0      966 2023-06-14 14:25:28.316460 pytk_net-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-14 06:03:47.000000 pytk_net-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 14:25:28.303129 pytk_net-0.1.2/pytk_net/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytk_net-0.1.2/pytk_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:25:28.312470 pytk_net-0.1.2/pytk_net/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytk_net-0.1.2/pytk_net/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytk_net-0.1.2/pytk_net/icons/bootstrap-icons.woff
+drwxrwxrwx   0        0        0        0 2023-06-14 14:25:28.315463 pytk_net-0.1.2/pytk_net/overwrite/
+-rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytk_net-0.1.2/pytk_net/overwrite/DateEntry.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytk_net-0.1.2/pytk_net/overwrite/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-06-09 06:17:45.000000 pytk_net-0.1.2/pytk_net/utils.py
+-rw-rw-rw-   0        0        0      333 2023-06-14 14:15:59.000000 pytk_net-0.1.2/pytk_net/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:25:28.309474 pytk_net-0.1.2/pytk_net.egg-info/
+-rw-rw-rw-   0        0        0      966 2023-06-14 14:25:28.000000 pytk_net-0.1.2/pytk_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-14 14:25:28.000000 pytk_net-0.1.2/pytk_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:25:28.000000 pytk_net-0.1.2/pytk_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 14:25:28.000000 pytk_net-0.1.2/pytk_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 14:25:28.317828 pytk_net-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-14 14:25:18.000000 pytk_net-0.1.2/setup.py
```

### Comparing `pytk_net-0.1.1/PKG-INFO` & `pytk_net-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk_net
-Version: 0.1.1
+Version: 0.1.2
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

### Comparing `pytk_net-0.1.1/README.md` & `pytk_net-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytk_net-0.1.1/pytk_net/icons/bootstrap-icons.json` & `pytk_net-0.1.2/pytk_net/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pytk_net-0.1.1/pytk_net/icons/bootstrap-icons.woff` & `pytk_net-0.1.2/pytk_net/icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pytk_net-0.1.1/pytk_net/utils.py` & `pytk_net-0.1.2/pytk_net/utils.py`

 * *Files identical despite different names*

### Comparing `pytk_net-0.1.1/pytk_net.egg-info/PKG-INFO` & `pytk_net-0.1.2/pytk_net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytk-net
-Version: 0.1.1
+Version: 0.1.2
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
```

