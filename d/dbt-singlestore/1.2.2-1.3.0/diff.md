# Comparing `tmp/dbt-singlestore-1.2.2.tar.gz` & `tmp/dbt-singlestore-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbt-singlestore-1.2.2.tar", last modified: Mon May 22 19:02:54 2023, max compression
+gzip compressed data, was "dbt-singlestore-1.3.0.tar", last modified: Wed Jun 14 14:34:00 2023, max compression
```

## Comparing `dbt-singlestore-1.2.2.tar` & `dbt-singlestore-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)    11356 2022-01-12 14:48:12.000000 dbt-singlestore-1.2.2/LICENSE
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       46 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/MANIFEST.in
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/PKG-INFO
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     3273 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/README.md
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/adapters/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      433 2022-01-12 13:59:39.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/__init__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       18 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/__version__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      751 2022-01-24 13:04:48.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/column.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     2993 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/connections.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     6075 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/impl.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      952 2022-01-25 11:30:29.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/relation.py
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       51 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/__init__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       79 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/dbt_project.yml
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1554 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/catalog.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      806 2022-06-22 14:31:34.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/columns.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     9113 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/common.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      606 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/grants.sql
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4394 2022-01-26 15:42:32.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4373 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      916 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      224 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       90 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/bool_or.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      135 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      203 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/dateadd.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      193 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/datediff.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      122 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/hash.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      624 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/listagg.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       94 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/safe_cast.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      389 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/split_part.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      482 2022-01-25 16:24:27.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/profile_template.yml
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      420 2022-01-25 16:25:45.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/sample_profiles.yml
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/PKG-INFO
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1481 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/SOURCES.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        1 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/dependency_links.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       55 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/requires.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        4 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/top_level.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       38 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/setup.cfg
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      765 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/setup.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)    11356 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/LICENSE
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       46 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/MANIFEST.in
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     3304 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/README.md
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        2 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/__init__.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/adapters/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/adapters/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      433 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       18 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/__version__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      751 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/column.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     2993 2023-06-14 14:33:19.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/connections.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     6075 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/impl.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      952 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/adapters/singlestore/relation.py
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/include/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       51 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/__init__.py
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       79 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/dbt_project.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1554 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/catalog.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      806 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/columns.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     9224 2023-06-14 09:44:17.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/common.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      606 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/grants.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.312879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.316879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4394 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     4373 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      916 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      224 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       90 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/bool_or.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      135 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      203 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/dateadd.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      193 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/datediff.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      122 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/hash.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      624 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/listagg.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       94 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/safe_cast.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      389 2023-05-25 13:50:11.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/split_part.sql
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      482 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/profile_template.yml
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      420 2023-05-19 09:49:48.000000 dbt-singlestore-1.3.0/dbt/include/singlestore/sample_profiles.yml
+drwxr-xr-x   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        0 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      321 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/PKG-INFO
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)     1497 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/SOURCES.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        1 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/dependency_links.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       55 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/requires.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)        4 2023-06-14 14:34:00.000000 dbt-singlestore-1.3.0/dbt_singlestore.egg-info/top_level.txt
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)       38 2023-06-14 14:34:00.320879 dbt-singlestore-1.3.0/setup.cfg
+-rw-r--r--   0 okramarenko-ua (185476362) okramarenko-ua (185476362)      765 2023-06-14 14:33:19.000000 dbt-singlestore-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dbt-singlestore-1.2.2/LICENSE` & `dbt-singlestore-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/README.md` & `dbt-singlestore-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 ## Testing and supported versions
 
 Default dbt [test suite](tests/test_basic.py) is used to check the adapter functionality. [Development](Development.md) overview has a section "Run tests" which contains instructions on running the tests. Currently, the tests have been successfully run for the following product versions:
 
 Singlestore | dbt-core | dbt-tests-adapter
 ------------|----------|-------------------
+8.1.1       | 1.3.0    | 1.3.0
 7.8.29      | 1.2.2    | 1.2.2
 
 Singlestore | dbt-core | pytest-dbt-adapter
 ------------|----------|-------------------
 7.8.3       | 1.1.1    | 0.6.0
 7.6.6       | 1.0.1    | 0.6.0
 7.5.12      | 1.0.1    | 0.6.0
```

### Comparing `dbt-singlestore-1.2.2/dbt/adapters/singlestore/column.py` & `dbt-singlestore-1.3.0/dbt/adapters/singlestore/column.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/adapters/singlestore/connections.py` & `dbt-singlestore-1.3.0/dbt/adapters/singlestore/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/adapters/singlestore/impl.py` & `dbt-singlestore-1.3.0/dbt/adapters/singlestore/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/adapters/singlestore/relation.py` & `dbt-singlestore-1.3.0/dbt/adapters/singlestore/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/catalog.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/columns.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/common.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/common.sql`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,19 @@
 
 
 {% macro singlestore__current_timestamp() -%}
     current_timestamp()
 {%- endmacro %}
 
 
+{%- macro singlestore__current_timestamp_in_utc_backcompat() -%}
+    UTC_TIMESTAMP()
+{%- endmacro -%}
+
+       
 {% macro singlestore__create_view_as(relation, sql) -%}
     {%- set sql_header = config.get('sql_header', none) -%}
     {{ sql_header if sql_header is not none }}
     create view {{ relation }} as
         {{ sql }}
 {%- endmacro %}
```

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/grants.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/listagg.sql` & `dbt-singlestore-1.3.0/dbt/include/singlestore/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.2.2/dbt_singlestore.egg-info/SOURCES.txt` & `dbt-singlestore-1.3.0/dbt_singlestore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+dbt/__init__.py
 dbt/adapters/singlestore/__init__.py
 dbt/adapters/singlestore/__version__.py
 dbt/adapters/singlestore/column.py
 dbt/adapters/singlestore/connections.py
 dbt/adapters/singlestore/impl.py
 dbt/adapters/singlestore/relation.py
 dbt/include/singlestore/__init__.py
```

### Comparing `dbt-singlestore-1.2.2/setup.py` & `dbt-singlestore-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-singlestore"
 # make sure this always matches dbt/adapters/singlestore/__version__.py
-package_version = "1.2.2"
+package_version = "1.3.0"
 description = """The singlestore adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
```

