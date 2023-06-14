# Comparing `tmp/azunyan-4.8.2.tar.gz` & `tmp/azunyan-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azunyan-4.8.2.tar", last modified: Wed Mar 15 16:38:26 2023, max compression
+gzip compressed data, was "azunyan-4.8.3.tar", last modified: Thu May 11 10:18:01 2023, max compression
```

## Comparing `azunyan-4.8.2.tar` & `azunyan-4.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 16:38:26.334313 azunyan-4.8.2/
--rw-rw-rw-   0        0        0    35148 2020-02-22 15:30:19.000000 azunyan-4.8.2/LICENSE
--rw-rw-rw-   0        0        0      768 2023-03-15 16:38:26.333813 azunyan-4.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      218 2021-03-08 21:56:37.000000 azunyan-4.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-15 16:38:26.334313 azunyan-4.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1265 2023-03-15 16:38:21.000000 azunyan-4.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 16:38:26.324535 azunyan-4.8.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-15 16:38:26.330770 azunyan-4.8.2/src/JK/
--rw-rw-rw-   0        0        0        0 2023-03-13 17:02:41.000000 azunyan-4.8.2/src/JK/__init__.py
--rw-rw-rw-   0        0        0     4334 2023-03-15 15:58:04.000000 azunyan-4.8.2/src/JK/db.py
--rw-rw-rw-   0        0        0     1607 2023-03-15 15:50:12.000000 azunyan-4.8.2/src/JK/file.py
--rw-rw-rw-   0        0        0      267 2023-03-15 15:50:13.000000 azunyan-4.8.2/src/JK/func.py
--rw-rw-rw-   0        0        0     1680 2023-03-15 15:50:15.000000 azunyan-4.8.2/src/JK/image.py
--rw-rw-rw-   0        0        0     1264 2023-03-15 16:38:17.000000 azunyan-4.8.2/src/JK/telegram_bot.py
--rw-rw-rw-   0        0        0     2418 2023-03-15 15:50:17.000000 azunyan-4.8.2/src/JK/web.py
-drwxrwxrwx   0        0        0        0 2023-03-15 16:38:26.333311 azunyan-4.8.2/src/azunyan.egg-info/
--rw-rw-rw-   0        0        0      768 2023-03-15 16:38:26.000000 azunyan-4.8.2/src/azunyan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-03-15 16:38:26.000000 azunyan-4.8.2/src/azunyan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 16:38:26.000000 azunyan-4.8.2/src/azunyan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-03-15 16:38:26.000000 azunyan-4.8.2/src/azunyan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 10:18:01.876732 azunyan-4.8.3/
+-rw-rw-rw-   0        0        0    35148 2020-02-22 15:30:19.000000 azunyan-4.8.3/LICENSE
+-rw-rw-rw-   0        0        0      768 2023-05-11 10:18:01.876222 azunyan-4.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2021-03-08 21:56:37.000000 azunyan-4.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-11 10:18:01.876732 azunyan-4.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2023-05-11 10:17:46.000000 azunyan-4.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:18:01.866031 azunyan-4.8.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-11 10:18:01.872671 azunyan-4.8.3/src/JK/
+-rw-rw-rw-   0        0        0        0 2023-03-13 17:02:41.000000 azunyan-4.8.3/src/JK/__init__.py
+-rw-rw-rw-   0        0        0     4310 2023-05-11 10:16:49.000000 azunyan-4.8.3/src/JK/db.py
+-rw-rw-rw-   0        0        0     1607 2023-03-15 15:50:12.000000 azunyan-4.8.3/src/JK/file.py
+-rw-rw-rw-   0        0        0      267 2023-03-15 15:50:13.000000 azunyan-4.8.3/src/JK/func.py
+-rw-rw-rw-   0        0        0     1680 2023-03-15 15:50:15.000000 azunyan-4.8.3/src/JK/image.py
+-rw-rw-rw-   0        0        0     1264 2023-03-15 16:38:17.000000 azunyan-4.8.3/src/JK/telegram_bot.py
+-rw-rw-rw-   0        0        0     2418 2023-03-15 15:50:17.000000 azunyan-4.8.3/src/JK/web.py
+drwxrwxrwx   0        0        0        0 2023-05-11 10:18:01.875711 azunyan-4.8.3/src/azunyan.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-05-11 10:18:01.000000 azunyan-4.8.3/src/azunyan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-05-11 10:18:01.000000 azunyan-4.8.3/src/azunyan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 10:18:01.000000 azunyan-4.8.3/src/azunyan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-11 10:18:01.000000 azunyan-4.8.3/src/azunyan.egg-info/top_level.txt
```

### Comparing `azunyan-4.8.2/LICENSE` & `azunyan-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azunyan-4.8.2/PKG-INFO` & `azunyan-4.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azunyan
-Version: 4.8.2
+Version: 4.8.3
 Summary: Some simple functions I packed for self usage
 Home-page: https://github.com/Elypha/azunyan
 Author: Elypha
 Author-email: i@elypha.com
 Project-URL: Bug Tracker, https://github.com/Elypha/azunyan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `azunyan-4.8.2/setup.py` & `azunyan-4.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="azunyan",
-    version="4.8.2",
+    version="4.8.3",
     author="Elypha",
     author_email="i@elypha.com",
     description="Some simple functions I packed for self usage",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Elypha/azunyan",
     project_urls={
```

### Comparing `azunyan-4.8.2/src/JK/db.py` & `azunyan-4.8.3/src/JK/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 import mysql.connector
 from loguru import logger
 
 
 class SQLite:
     def __init__(
         self,
-        path: str,
-        database: str
+        path: str
     ):
         """
         SQLite3 database connection class.
 
         - `path` str\n
             - e.g., `'/home/user/database.db'`
         - `database` str\n
             - e.g., `'config'`
         """
         try:
             self.db = sqlite3.connect(path, check_same_thread=False)
-            self.cur = database.cursor()
+            self.cur = self.db.cursor()
             logger.info(f'Connected to SQLite3 database via "{path}"')
         except Exception as err:
             logger.error(f'SQLite3 database connection failed: {err}')
             quit()
 
     def query(self, SQL):
         try:
```

### Comparing `azunyan-4.8.2/src/JK/file.py` & `azunyan-4.8.3/src/JK/file.py`

 * *Files identical despite different names*

### Comparing `azunyan-4.8.2/src/JK/image.py` & `azunyan-4.8.3/src/JK/image.py`

 * *Files identical despite different names*

### Comparing `azunyan-4.8.2/src/JK/telegram_bot.py` & `azunyan-4.8.3/src/JK/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `azunyan-4.8.2/src/JK/web.py` & `azunyan-4.8.3/src/JK/web.py`

 * *Files identical despite different names*

### Comparing `azunyan-4.8.2/src/azunyan.egg-info/PKG-INFO` & `azunyan-4.8.3/src/azunyan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azunyan
-Version: 4.8.2
+Version: 4.8.3
 Summary: Some simple functions I packed for self usage
 Home-page: https://github.com/Elypha/azunyan
 Author: Elypha
 Author-email: i@elypha.com
 Project-URL: Bug Tracker, https://github.com/Elypha/azunyan/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

