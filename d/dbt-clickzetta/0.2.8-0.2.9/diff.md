# Comparing `tmp/dbt-clickzetta-0.2.8.tar.gz` & `tmp/dbt-clickzetta-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.2.8.tar", last modified: Tue Jun  6 09:21:07 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.2.9.tar", last modified: Tue Jun  6 09:34:41 2023, max compression
```

## Comparing `dbt-clickzetta-0.2.8.tar` & `dbt-clickzetta-0.2.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.542231 dbt-clickzetta-0.2.8/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-06 09:21:07.542082 dbt-clickzetta-0.2.8/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.536194 dbt-clickzetta-0.2.8/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.535462 dbt-clickzetta-0.2.8/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.537572 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7206 2023-06-06 09:13:22.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6958 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      698 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.535553 dbt-clickzetta-0.2.8/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.537990 dbt-clickzetta-0.2.8/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.538204 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14274 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.538694 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.539189 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.541265 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      368 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/nullcheck.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.8/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:21:07.541924 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1898 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-06 09:21:07.000000 dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-06 09:21:07.542274 dbt-clickzetta-0.2.8/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-06 09:20:24.000000 dbt-clickzetta-0.2.8/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.566952 dbt-clickzetta-0.2.9/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-06 09:34:41.566821 dbt-clickzetta-0.2.9/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.560892 dbt-clickzetta-0.2.9/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.560093 dbt-clickzetta-0.2.9/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.562010 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7206 2023-06-06 09:13:22.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6958 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      698 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.560193 dbt-clickzetta-0.2.9/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.562529 dbt-clickzetta-0.2.9/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.562754 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14274 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.563275 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.563834 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.565959 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      368 2023-06-06 06:31:22.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/nullcheck.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.9/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 09:34:41.566655 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1898 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-06 09:34:41.000000 dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-06 09:34:41.566998 dbt-clickzetta-0.2.9/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-06 09:32:45.000000 dbt-clickzetta-0.2.9/setup.py
```

### Comparing `dbt-clickzetta-0.2.8/PKG-INFO` & `dbt-clickzetta-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.2.8
+Version: 0.2.9
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.2.9/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.2.9/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/PKG-INFO` & `dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.2.8
+Version: 0.2.9
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.2.8/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.2.9/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.8/setup.py` & `dbt-clickzetta-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.2.8"
+package_version = "0.2.9"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -64,15 +64,15 @@
     author="clickzetta",
     author_email="",
     url="",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "clickzetta-connector~=0.8.8",
+        "clickzetta-connector~=0.8.9",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```

