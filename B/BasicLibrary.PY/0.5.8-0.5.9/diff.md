# Comparing `tmp/BasicLibrary.PY-0.5.8.tar.gz` & `tmp/BasicLibrary.PY-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BasicLibrary.PY-0.5.8.tar", last modified: Thu Jun  8 08:15:40 2023, max compression
+gzip compressed data, was "BasicLibrary.PY-0.5.9.tar", last modified: Thu Jun  8 08:49:15 2023, max compression
```

## Comparing `BasicLibrary.PY-0.5.8.tar` & `BasicLibrary.PY-0.5.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.294949 BasicLibrary.PY-0.5.8/
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.198712 BasicLibrary.PY-0.5.8/BasicLibrary/
--rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/__init__.py
--rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.8/BasicLibrary/__projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.250712 BasicLibrary.PY-0.5.8/BasicLibrary/biz/
--rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.8/BasicLibrary/biz/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.8/BasicLibrary/biz/stockHelper.py
--rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.8/BasicLibrary/biz/tencentHelper.py
--rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.8/BasicLibrary/configHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.519714 BasicLibrary.PY-0.5.8/BasicLibrary/data/
--rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/collectionHelper.py
--rw-rw-rw-   0        0        0     5753 2023-06-08 02:21:21.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/dateTimeHelper.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/dictHelper.py
--rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/htmlHelper.py
--rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/listHelper.py
--rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/numberHelper.py
--rw-rw-rw-   0        0        0     2728 2023-06-08 02:17:54.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/objectHelper.py
--rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/pandasHelper.py
--rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/randomHelper.py
--rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/reflectHelper.py
--rw-rw-rw-   0        0        0     1621 2023-06-08 07:12:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/regexHelper.py
--rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/setHelper.py
--rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/data/stringHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.703714 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.772710 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/helper.py
--rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/mate.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.831710 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/ddl.py
--rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/mate.py
--rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/pool.py
--rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseClient.py
--rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseDDL.py
--rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseEnum.py
--rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseHelper.py
--rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseMate.py
--rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseUnitTest.py
--rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.8/BasicLibrary/enums.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.865715 BasicLibrary.PY-0.5.8/BasicLibrary/environment/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.8/BasicLibrary/environment/__init__.py
--rw-rw-rw-   0        0        0     1593 2023-06-08 04:36:05.000000 BasicLibrary.PY-0.5.8/BasicLibrary/environment/consoleHelper.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/environment/envHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.972365 BasicLibrary.PY-0.5.8/BasicLibrary/io/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.8/BasicLibrary/io/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.8/BasicLibrary/io/dirHelper.py
--rw-rw-rw-   0        0        0     6306 2023-06-08 08:13:46.000000 BasicLibrary.PY-0.5.8/BasicLibrary/io/fileHelper.py
--rw-rw-rw-   0        0        0     1463 2023-06-08 04:03:25.000000 BasicLibrary.PY-0.5.8/BasicLibrary/io/ioHelper.py
--rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.8/BasicLibrary/io/pathHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.052643 BasicLibrary.PY-0.5.8/BasicLibrary/model/
--rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.8/BasicLibrary/model/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.8/BasicLibrary/model/container.py
--rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.8/BasicLibrary/model/dataCompare.py
--rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.8/BasicLibrary/model/kvPair.py
--rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.8/BasicLibrary/model/stopWatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.116948 BasicLibrary.PY-0.5.8/BasicLibrary/office/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.8/BasicLibrary/office/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.8/BasicLibrary/office/excelBookMate.py
--rw-rw-rw-   0        0        0     2458 2023-06-07 11:39:53.000000 BasicLibrary.PY-0.5.8/BasicLibrary/office/excelHelper.py
--rw-rw-rw-   0        0        0     3375 2023-06-07 11:44:09.000000 BasicLibrary.PY-0.5.8/BasicLibrary/office/excelMisc.py
--rw-rw-rw-   0        0        0    11164 2023-06-07 14:03:03.000000 BasicLibrary.PY-0.5.8/BasicLibrary/office/excelSheetMate.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.146954 BasicLibrary.PY-0.5.8/BasicLibrary/pattern/
--rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.8/BasicLibrary/pattern/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.8/BasicLibrary/pattern/singleton.py
--rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.8/BasicLibrary/projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.156950 BasicLibrary.PY-0.5.8/BasicLibrary/syntax/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.8/BasicLibrary/syntax/__init__.py
--rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.8/BasicLibrary/syntax/switch.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:40.272949 BasicLibrary.PY-0.5.8/BasicLibrary/web/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.8/BasicLibrary/web/__init__.py
--rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.8/BasicLibrary/web/beautifulSoupHelper.py
--rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.8/BasicLibrary/web/requestHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 08:15:39.217715 BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/
--rw-rw-rw-   0        0        0     2896 2023-06-08 08:15:38.000000 BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-08 08:15:39.000000 BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 08:15:38.000000 BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 08:15:38.000000 BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2896 2023-06-08 08:15:40.292951 BasicLibrary.PY-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 08:15:40.295949 BasicLibrary.PY-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     4280 2023-06-08 08:15:01.000000 BasicLibrary.PY-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:15.052917 BasicLibrary.PY-0.5.9/
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.150921 BasicLibrary.PY-0.5.9/BasicLibrary/
+-rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/__init__.py
+-rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.9/BasicLibrary/__projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.209917 BasicLibrary.PY-0.5.9/BasicLibrary/biz/
+-rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.9/BasicLibrary/biz/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.9/BasicLibrary/biz/stockHelper.py
+-rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.9/BasicLibrary/biz/tencentHelper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.9/BasicLibrary/configHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.481922 BasicLibrary.PY-0.5.9/BasicLibrary/data/
+-rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/collectionHelper.py
+-rw-rw-rw-   0        0        0     5753 2023-06-08 02:21:21.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/dateTimeHelper.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/dictHelper.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/htmlHelper.py
+-rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/listHelper.py
+-rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/numberHelper.py
+-rw-rw-rw-   0        0        0     2728 2023-06-08 02:17:54.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/objectHelper.py
+-rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/pandasHelper.py
+-rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/randomHelper.py
+-rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/reflectHelper.py
+-rw-rw-rw-   0        0        0     1621 2023-06-08 07:12:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/regexHelper.py
+-rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/setHelper.py
+-rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/data/stringHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.584919 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.643920 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/mate.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.701920 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/ddl.py
+-rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/mate.py
+-rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/pool.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseClient.py
+-rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseDDL.py
+-rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseEnum.py
+-rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseHelper.py
+-rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseMate.py
+-rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.9/BasicLibrary/enums.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.733938 BasicLibrary.PY-0.5.9/BasicLibrary/environment/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.9/BasicLibrary/environment/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-06-08 04:36:05.000000 BasicLibrary.PY-0.5.9/BasicLibrary/environment/consoleHelper.py
+-rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/environment/envHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.796918 BasicLibrary.PY-0.5.9/BasicLibrary/io/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.9/BasicLibrary/io/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.9/BasicLibrary/io/dirHelper.py
+-rw-rw-rw-   0        0        0     6306 2023-06-08 08:13:46.000000 BasicLibrary.PY-0.5.9/BasicLibrary/io/fileHelper.py
+-rw-rw-rw-   0        0        0     1713 2023-06-08 08:46:08.000000 BasicLibrary.PY-0.5.9/BasicLibrary/io/ioHelper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.9/BasicLibrary/io/pathHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.876959 BasicLibrary.PY-0.5.9/BasicLibrary/model/
+-rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.9/BasicLibrary/model/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.9/BasicLibrary/model/container.py
+-rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.9/BasicLibrary/model/dataCompare.py
+-rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.9/BasicLibrary/model/kvPair.py
+-rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.9/BasicLibrary/model/stopWatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.940938 BasicLibrary.PY-0.5.9/BasicLibrary/office/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.9/BasicLibrary/office/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.9/BasicLibrary/office/excelBookMate.py
+-rw-rw-rw-   0        0        0     2458 2023-06-07 11:39:53.000000 BasicLibrary.PY-0.5.9/BasicLibrary/office/excelHelper.py
+-rw-rw-rw-   0        0        0     3375 2023-06-07 11:44:09.000000 BasicLibrary.PY-0.5.9/BasicLibrary/office/excelMisc.py
+-rw-rw-rw-   0        0        0    11164 2023-06-07 14:03:03.000000 BasicLibrary.PY-0.5.9/BasicLibrary/office/excelSheetMate.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.968937 BasicLibrary.PY-0.5.9/BasicLibrary/pattern/
+-rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.9/BasicLibrary/pattern/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.9/BasicLibrary/pattern/singleton.py
+-rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.9/BasicLibrary/projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.977918 BasicLibrary.PY-0.5.9/BasicLibrary/syntax/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.9/BasicLibrary/syntax/__init__.py
+-rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.9/BasicLibrary/syntax/switch.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:15.032919 BasicLibrary.PY-0.5.9/BasicLibrary/web/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.9/BasicLibrary/web/__init__.py
+-rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.9/BasicLibrary/web/beautifulSoupHelper.py
+-rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.9/BasicLibrary/web/requestHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:49:14.171916 BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/
+-rw-rw-rw-   0        0        0     2896 2023-06-08 08:49:13.000000 BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-08 08:49:13.000000 BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:49:13.000000 BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 08:49:13.000000 BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2896 2023-06-08 08:49:15.050916 BasicLibrary.PY-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:49:15.054917 BasicLibrary.PY-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     4280 2023-06-08 08:49:00.000000 BasicLibrary.PY-0.5.9/setup.py
```

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/__init__.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/__projectHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/biz/stockHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/biz/stockHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/configHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/collectionHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/dateTimeHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/dateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/dictHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/listHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/numberHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/objectHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/objectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/pandasHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/randomHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/reflectHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/regexHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/data/stringHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/ddl.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/helper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MongoDB/mate.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/ddl.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/mate.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/MySql/pool.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseClient.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseDDL.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseMate.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/dataBase/databaseUnitTest.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/environment/consoleHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/environment/envHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/io/dirHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/io/fileHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/io/fileHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/io/pathHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/model/container.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/model/dataCompare.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/model/kvPair.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/office/excelBookMate.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/office/excelHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/office/excelHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/office/excelMisc.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/office/excelMisc.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/office/excelSheetMate.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/office/excelSheetMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/syntax/switch.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/web/beautifulSoupHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary/web/requestHelper.py` & `BasicLibrary.PY-0.5.9/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/PKG-INFO` & `BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.8
+Version: 0.5.9
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.8/BasicLibrary.PY.egg-info/SOURCES.txt` & `BasicLibrary.PY-0.5.9/BasicLibrary.PY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/PKG-INFO` & `BasicLibrary.PY-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.8
+Version: 0.5.9
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.8/README.md` & `BasicLibrary.PY-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.8/setup.py` & `BasicLibrary.PY-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NAME = 'BasicLibrary.PY'
 DESCRIPTION = '企业级的 PYTHON 库'
 URL = 'https://github.com/notinmood/BasicLibrary.PY'
 EMAIL = '9727005@qq.com'
 AUTHOR = 'xiedali'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.8'
+VERSION = '0.5.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

