# Comparing `tmp/wrangles-1.3.0.tar.gz` & `tmp/wrangles-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.3.0.tar", last modified: Sun Jun 11 17:40:25 2023, max compression
+gzip compressed data, was "wrangles-1.3.1.tar", last modified: Tue Jun 13 22:13:05 2023, max compression
```

## Comparing `wrangles-1.3.0.tar` & `wrangles-1.3.1.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.675200 wrangles-1.3.0/
--rw-rw-rw-   0        0        0    11558 2022-12-19 21:12:29.000000 wrangles-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4464 2023-06-11 17:40:25.675200 wrangles-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2023-03-31 00:02:07.000000 wrangles-1.3.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-11 17:40:25.676199 wrangles-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-06-11 17:16:14.000000 wrangles-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.630921 wrangles-1.3.0/wrangles/
--rw-rw-rw-   0        0        0      565 2022-06-23 01:29:50.000000 wrangles-1.3.0/wrangles/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/auth.py
--rw-rw-rw-   0        0        0      840 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/batching.py
--rw-rw-rw-   0        0        0     2069 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/classify.py
--rw-rw-rw-   0        0        0      559 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/config.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.666230 wrangles-1.3.0/wrangles/connectors/
--rw-rw-rw-   0        0        0      449 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/connectors/__init__.py
--rw-rw-rw-   0        0        0     7108 2023-06-11 17:29:44.000000 wrangles-1.3.0/wrangles/connectors/akeneo.py
--rw-rw-rw-   0        0        0    11023 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/ckan.py
--rw-rw-rw-   0        0        0     7811 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/file.py
--rw-rw-rw-   0        0        0     2498 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/http.py
--rw-rw-rw-   0        0        0     1883 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/jinja.py
--rw-rw-rw-   0        0        0     4830 2023-06-11 17:30:43.000000 wrangles-1.3.0/wrangles/connectors/mongodb.py
--rw-rw-rw-   0        0        0     6136 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/mssql.py
--rw-rw-rw-   0        0        0     4372 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/mysql.py
--rw-rw-rw-   0        0        0     6328 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/notification.py
--rw-rw-rw-   0        0        0     5892 2022-06-23 01:29:50.000000 wrangles-1.3.0/wrangles/connectors/postgres.py
--rw-rw-rw-   0        0        0    16169 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/pricefx.py
--rw-rw-rw-   0        0        0     4534 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/recipe.py
--rw-rw-rw-   0        0        0     8527 2023-06-11 17:31:29.000000 wrangles-1.3.0/wrangles/connectors/s3.py
--rw-rw-rw-   0        0        0     4754 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/connectors/salesforce.py
--rw-rw-rw-   0        0        0     4442 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/sftp.py
--rw-rw-rw-   0        0        0     2430 2022-12-19 21:12:29.000000 wrangles-1.3.0/wrangles/connectors/ssh.py
--rw-rw-rw-   0        0        0     5651 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/connectors/test.py
--rw-rw-rw-   0        0        0     8037 2023-06-11 17:20:06.000000 wrangles-1.3.0/wrangles/connectors/train.py
--rw-rw-rw-   0        0        0     1899 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/console.py
--rw-rw-rw-   0        0        0     1588 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/data.py
--rw-rw-rw-   0        0        0    10100 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/extract.py
--rw-rw-rw-   0        0        0     4412 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/format.py
--rw-rw-rw-   0        0        0    21142 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.675200 wrangles-1.3.0/wrangles/recipe_wrangles/
--rw-rw-rw-   0        0        0      585 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/convert.py
--rw-rw-rw-   0        0        0     8695 2023-06-11 17:22:18.000000 wrangles-1.3.0/wrangles/recipe_wrangles/create.py
--rw-rw-rw-   0        0        0    21176 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/extract.py
--rw-rw-rw-   0        0        0     8126 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/format.py
--rw-rw-rw-   0        0        0    27181 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/main.py
--rw-rw-rw-   0        0        0     8584 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/merge.py
--rw-rw-rw-   0        0        0     4041 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/pandas.py
--rw-rw-rw-   0        0        0     8715 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/select.py
--rw-rw-rw-   0        0        0     6791 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/recipe_wrangles/split.py
--rw-rw-rw-   0        0        0     1883 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/select.py
--rw-rw-rw-   0        0        0     2099 2023-03-31 00:02:07.000000 wrangles-1.3.0/wrangles/standardize.py
--rw-rw-rw-   0        0        0     6067 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/train.py
--rw-rw-rw-   0        0        0     3502 2023-06-11 17:16:14.000000 wrangles-1.3.0/wrangles/translate.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:40:25.652861 wrangles-1.3.0/wrangles.egg-info/
--rw-rw-rw-   0        0        0     4464 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1422 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 17:40:25.000000 wrangles-1.3.0/wrangles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.189765 wrangles-1.3.1/
+-rw-rw-rw-   0        0        0     3615 2023-06-13 22:13:05.189765 wrangles-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.166825 wrangles-1.3.1/Wrangles.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1573 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      159 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 22:13:05.190761 wrangles-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-06-13 22:13:01.000000 wrangles-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.164832 wrangles-1.3.1/wrangles/
+-rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.3.1/wrangles/__init__.py
+-rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/auth.py
+-rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/batching.py
+-rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/classify.py
+-rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.182782 wrangles-1.3.1/wrangles/connectors/
+-rw-rw-rw-   0        0        0      449 2023-05-15 15:40:44.000000 wrangles-1.3.1/wrangles/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7108 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/akeneo.py
+-rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/ckan.py
+-rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/file.py
+-rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/http.py
+-rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/jinja.py
+-rw-rw-rw-   0        0        0     4830 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/mongodb.py
+-rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/mysql.py
+-rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/notification.py
+-rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.3.1/wrangles/connectors/postgres.py
+-rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/pricefx.py
+-rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/recipe.py
+-rw-rw-rw-   0        0        0     8527 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/s3.py
+-rw-rw-rw-   0        0        0     4754 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/connectors/salesforce.py
+-rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/sftp.py
+-rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/ssh.py
+-rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/test.py
+-rw-rw-rw-   0        0        0     8037 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/train.py
+-rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/console.py
+-rw-rw-rw-   0        0        0     1588 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/data.py
+-rw-rw-rw-   0        0        0    10100 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/extract.py
+-rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/format.py
+-rw-rw-rw-   0        0        0    22513 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/recipe.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.188768 wrangles-1.3.1/wrangles/recipe_wrangles/
+-rw-rw-rw-   0        0        0      585 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/convert.py
+-rw-rw-rw-   0        0        0     8695 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/recipe_wrangles/create.py
+-rw-rw-rw-   0        0        0    21176 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/extract.py
+-rw-rw-rw-   0        0        0     8126 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/format.py
+-rw-rw-rw-   0        0        0    27181 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/main.py
+-rw-rw-rw-   0        0        0     8584 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/merge.py
+-rw-rw-rw-   0        0        0     4041 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/pandas.py
+-rw-rw-rw-   0        0        0     8715 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/select.py
+-rw-rw-rw-   0        0        0     6791 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/split.py
+-rw-rw-rw-   0        0        0     1883 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/select.py
+-rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/standardize.py
+-rw-rw-rw-   0        0        0     6067 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/train.py
+-rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.3.1/wrangles/translate.py
```

### Comparing `wrangles-1.3.0/README.md` & `wrangles-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/setup.py` & `wrangles-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.3.0',
+    version = '1.3.1',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.3.0/wrangles/__init__.py` & `wrangles-1.3.1/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/auth.py` & `wrangles-1.3.1/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/batching.py` & `wrangles-1.3.1/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/classify.py` & `wrangles-1.3.1/wrangles/classify.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/config.py` & `wrangles-1.3.1/wrangles/config.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/akeneo.py` & `wrangles-1.3.1/wrangles/connectors/akeneo.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/ckan.py` & `wrangles-1.3.1/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/file.py` & `wrangles-1.3.1/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/http.py` & `wrangles-1.3.1/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/jinja.py` & `wrangles-1.3.1/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/mongodb.py` & `wrangles-1.3.1/wrangles/connectors/mongodb.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/mssql.py` & `wrangles-1.3.1/wrangles/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/mysql.py` & `wrangles-1.3.1/wrangles/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/notification.py` & `wrangles-1.3.1/wrangles/connectors/notification.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/postgres.py` & `wrangles-1.3.1/wrangles/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/pricefx.py` & `wrangles-1.3.1/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/recipe.py` & `wrangles-1.3.1/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/s3.py` & `wrangles-1.3.1/wrangles/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/salesforce.py` & `wrangles-1.3.1/wrangles/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/sftp.py` & `wrangles-1.3.1/wrangles/connectors/sftp.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/ssh.py` & `wrangles-1.3.1/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/test.py` & `wrangles-1.3.1/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/connectors/train.py` & `wrangles-1.3.1/wrangles/connectors/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/console.py` & `wrangles-1.3.1/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/data.py` & `wrangles-1.3.1/wrangles/data.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/extract.py` & `wrangles-1.3.1/wrangles/extract.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/format.py` & `wrangles-1.3.1/wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe.py` & `wrangles-1.3.1/wrangles/recipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -288,49 +288,85 @@
                 # Execute a user's custom function
                 try:
                     custom_function = functions[wrangle[7:]]
                 except:
                     raise ValueError(f'Custom Wrangle function: "{wrangle}" not found')
 
                 # Get user's function arguments
-                function_args = _inspect.getfullargspec(custom_function).args
-                # Drop params from function_args
-                for arg in function_args:
-                    if arg in params.keys():
-                        function_args.remove(arg)
+                fn_argspec = _inspect.getfullargspec(custom_function)
 
                 # Check for function_args and df
-                if len(function_args) > 0 and 'df' in function_args:
+                if 'df' in fn_argspec.args:
                     # If user's first argument is df, pass them the whole dataframe
-                    df = functions[wrangle[7:]](df=df, **params)
+                    df = custom_function(df=df, **params)
 
                 # Dealing with no function_args
                 else:
+                    # Use a temp copy of dataframe as not to affect original
                     df_temp = df
 
+                    # If user specifies an input, reduce dataframe down as required
                     if 'input' in params:
-                        params['input'] = _wildcard_expansion(all_columns=df.columns.tolist(), selected_columns=params['input'])
-                        df_temp = df_temp[params['input']]
-                    # Drop columns from df_temp that are not in function_args
-                    if function_args:
-                        try:
-                            df_temp = df_temp[function_args]
-                        except:
-                            raise KeyError(f"input/output passed without df. Pass df as a function variable or use the column header in place of input/output to fix this issue. See https://wrangles.io/python/recipes/custom-functions/wrangles for more information")
-                    # Create params_temp and drop input/output
+                        df_temp = df_temp[
+                            _wildcard_expansion(
+                                all_columns=df.columns.tolist(),
+                                selected_columns=params['input']
+                            )
+                        ]
+
+                    # If the user hasn't explicitly requested input or output
+                    # then remove them so they will not be included in kwargs
                     params_temp = params.copy()
-                    if 'input' in params_temp.keys():
-                        params_temp.pop('input')
-                    if 'output' in params_temp.keys():
-                        params_temp.pop('output')
-                    # {**x, **params_temp} deals with columns in function args and **params_temp without columns
+                    for special_parameter in ['input', 'output']:
+                        if special_parameter in params_temp and special_parameter not in fn_argspec.args:
+                            params_temp.pop(special_parameter)
+
+                    # If the user's custom function does not have kwargs available
+                    # then we need to remove any unmatched function arguments
+                    # from the parameters or the columns
+                    if not fn_argspec.varkw:
+                        params_temp2 = params_temp.copy()
+                        for param in params_temp2.keys():
+                            if param not in fn_argspec.args:
+                                params_temp.pop(param)
+
+                        cols = [
+                            col for col in 
+                            df_temp.columns.to_list()
+                            if col in fn_argspec.args
+                        ]
+
+                        # Ensure we don't remove all columns
+                        # if user hasn't specified any
+                        if cols:
+                            df_temp = df_temp[cols]
+                    
+                    # If user specifies multiple outputs, expand any list output
+                    # across the columns else return as a single column
+                    if isinstance(params['output'], list) and len(params['output']) > 1:
+                        result_type = 'expand'
+                    else:
+                        result_type = 'reduce'
+
+                    # {**x, **params_temp} deals with columns in 
+                    # function args and  **params_temp without columns
+                    # There may be no columns in the case that the user
+                    # does not specify any columns in their function parameters
                     try:
-                        df[params['output']] = df_temp.apply(lambda x: custom_function(**{**x, **params_temp}), axis=1, result_type='expand')
-                    except:    
-                        df[params['output']] = df_temp.apply(lambda x: custom_function(**params_temp), axis=1, result_type='expand')
+                        df[params['output']] = df_temp.apply(
+                            lambda x: custom_function(**{**x, **params_temp}),
+                            axis=1,
+                            result_type=result_type
+                        )
+                    except:
+                        df[params['output']] = df_temp.apply(
+                            lambda _: custom_function(**params_temp),
+                            axis=1,
+                            result_type=result_type
+                        )
 
             else:
                 # Blacklist of Wrangles not to allow wildcards for
                 if wrangle not in ['math', 'maths', 'merge.key_value_pairs', 'split.text', 'split.list', 'split.dictionary'] and 'input' in params:
                     # Expand out any wildcards or regex in column names
                     params['input'] = _wildcard_expansion(all_columns=df.columns.tolist(), selected_columns=params['input'])
```

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/convert.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/convert.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/create.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/create.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/extract.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/extract.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/format.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/main.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/main.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/merge.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/merge.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/pandas.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/pandas.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/select.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/recipe_wrangles/split.py` & `wrangles-1.3.1/wrangles/recipe_wrangles/split.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/select.py` & `wrangles-1.3.1/wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/standardize.py` & `wrangles-1.3.1/wrangles/standardize.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/train.py` & `wrangles-1.3.1/wrangles/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.0/wrangles/translate.py` & `wrangles-1.3.1/wrangles/translate.py`

 * *Files identical despite different names*

