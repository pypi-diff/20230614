# Comparing `tmp/dbt-fabric-1.4.0rc1.tar.gz` & `tmp/dbt-fabric-1.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.4.0rc1.tar", last modified: Thu Jun  1 04:27:22 2023, max compression
+gzip compressed data, was "dbt-fabric-1.4.0rc2.tar", last modified: Wed Jun 14 00:00:21 2023, max compression
```

## Comparing `dbt-fabric-1.4.0rc1.tar` & `dbt-fabric-1.4.0rc2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:51:02.121636 dbt-fabric-1.4.0rc1/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1087 2023-05-23 21:04:53.000000 dbt-fabric-1.4.0rc1/LICENSE
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       47 2023-05-23 21:04:53.000000 dbt-fabric-1.4.0rc1/MANIFEST.in
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     3716 2023-06-01 19:51:02.116761 dbt-fabric-1.4.0rc1/PKG-INFO
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     2552 2023-06-01 19:14:36.000000 dbt-fabric-1.4.0rc1/README.md
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:56.749227 dbt-fabric-1.4.0rc1/dbt/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:56.726820 dbt-fabric-1.4.0rc1/dbt/adapters/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:57.760132 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      682 2023-05-24 01:24:30.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/__init__.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       22 2023-06-01 19:46:41.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/__version__.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     6101 2023-05-24 22:24:53.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_adapter.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      536 2023-05-24 20:58:49.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_column.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      218 2023-05-23 21:34:03.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_configs.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)    14953 2023-06-01 03:21:58.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_connection_manager.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1891 2023-05-23 22:26:55.000000 dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_credentials.py
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:56.753234 dbt-fabric-1.4.0rc1/dbt/include/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:57.903384 dbt-fabric-1.4.0rc1/dbt/include/fabric/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       52 2023-05-23 21:04:54.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/__init__.py
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       74 2023-05-23 21:41:54.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/dbt_project.yml
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:57.038233 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:58.717041 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     3443 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/apply_grants.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     4365 2023-06-01 19:26:26.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/columns.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1094 2023-05-24 01:24:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/indexes.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     4750 2023-05-26 17:06:19.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/metadata.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      120 2023-05-23 21:04:54.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/persist_docs.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     4738 2023-06-01 19:26:26.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/relation.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1357 2023-05-26 14:49:02.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/schema.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:57.009634 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:56.923320 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:59.066406 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/incremental/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      273 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     2178 2023-05-27 05:28:40.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:59.210017 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/table/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      581 2023-05-31 09:48:56.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:59.326763 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/view/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      411 2023-05-29 21:28:14.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:59.499997 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/seeds/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1834 2023-05-27 05:29:11.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:50:59.936413 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1458 2023-05-29 21:28:14.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1064 2023-05-31 09:49:16.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      249 2023-05-24 16:45:16.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:51:00.215036 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/tests/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      449 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/tests/helpers.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     1329 2023-05-24 00:05:35.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/tests/test.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:51:01.785649 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       87 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/any_value.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      113 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/array_construct.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      162 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       88 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/concat.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      142 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/date_trunc.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      219 2023-06-01 03:13:54.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/dateadd.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      149 2023-06-01 03:14:11.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/hash.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      447 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/last_day.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       86 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/length.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      264 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/listagg.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      154 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/position.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       94 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/safe_cast.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      740 2023-05-23 21:48:30.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/split_part.sql
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)      263 2023-05-24 16:50:21.000000 dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/timestamps.sql
-drwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        0 2023-06-01 19:51:02.057394 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     3716 2023-06-01 19:50:53.000000 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/PKG-INFO
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     2225 2023-06-01 19:50:56.000000 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/SOURCES.txt
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        1 2023-06-01 19:50:53.000000 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/dependency_links.txt
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       72 2023-06-01 19:50:53.000000 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/requires.txt
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)        4 2023-06-01 19:50:53.000000 dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/top_level.txt
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)       38 2023-06-01 19:51:02.123635 dbt-fabric-1.4.0rc1/setup.cfg
--rwxrwxrwx   0 pvenkat   (1000) pvenkat   (1000)     3352 2023-06-01 03:10:46.000000 dbt-fabric-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.623928 dbt-fabric-1.4.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14953 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.615928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:00:21.619928 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 00:00:21.000000 dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:00:21.623928 dbt-fabric-1.4.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-13 23:59:34.000000 dbt-fabric-1.4.0rc2/setup.py
```

### Comparing `dbt-fabric-1.4.0rc1/LICENSE` & `dbt-fabric-1.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/PKG-INFO` & `dbt-fabric-1.4.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/microsoft/dbt-fabric/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,18 +28,17 @@
 [dbt](https://www.getdbt.com) adapter for Microsoft Fabric Synapse Data Warehouse.
 
 The adapter supports dbt-core 1.4 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
-We've bundled all documentation on the dbt docs site:
-TODO
-* [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+We've bundled all documentation on the dbt docs site
+* [Profile setup & authentication](https://docs.getdbt.com/docs/core/connect-data-platform/fabric-setup)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/fabric-configs)
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
 [macOS](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/install-microsoft-odbc-driver-sql-server-macos?view=sql-server-ver16) |
 [Linux](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16)
@@ -78,7 +78,9 @@
 ## License
 
 [![PyPI - License](https://img.shields.io/pypi/l/dbt-fabric)](https://github.com/microsoft/dbt-fabric/blob/main/LICENSE)
 
 ## Code of Conduct
 
 This project and everyone involved is expected to follow the [Microsoft Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+
+
```

### Comparing `dbt-fabric-1.4.0rc1/README.md` & `dbt-fabric-1.4.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 [dbt](https://www.getdbt.com) adapter for Microsoft Fabric Synapse Data Warehouse.
 
 The adapter supports dbt-core 1.4 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
-We've bundled all documentation on the dbt docs site:
-TODO
-* [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+We've bundled all documentation on the dbt docs site
+* [Profile setup & authentication](https://docs.getdbt.com/docs/core/connect-data-platform/fabric-setup)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/fabric-configs)
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
 [macOS](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/install-microsoft-odbc-driver-sql-server-macos?view=sql-server-ver16) |
 [Linux](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16)
```

### Comparing `dbt-fabric-1.4.0rc1/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.4.0rc2/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files 10% similar despite different names*

```diff
@@ -63,37 +63,29 @@
         INNER JOIN sys.schemas s
             ON o.schema_id = s.schema_id
             AND s.schema_id = v.schema_id
         WHERE s.name = '{{ from_relation.schema }}'
             AND v.name = '{{ from_relation.identifier }}'
             AND o.[type] = 'V';
     {% endcall %}
-    {% set view_def_full = load_result('get_view_definition')['data'][0][0] %}
-
-    {%set view_name = from_relation.identifier.replace("\"","") %}
-    {%set schema_name = from_relation.schema.replace("\"","") %}
 
-    {% set final_view_sql = modules.re.sub("create view ","",view_def_full, modules.re.I) %}
-    {%set doublequoteview = "\""~schema_name~"\""~".\""~view_name~"\" as "%}
-    {% set final_view_sql = modules.re.sub(doublequoteview,"",final_view_sql, modules.re.I) %}
+    {% set view_def_full = load_result('get_view_definition')['data'][0][0] %}
+    {# Jinja does not allow bitwise operators and we need re.I | re.M here. So calculated manually this becomes 10. #}
+    {% set final_view_sql = modules.re.sub("create\s+view\s+.*?\s+as\s+","",view_def_full, 10) %}
 
-    {%set squarebracketview = "["~schema_name~"]"~".["~view_name~"] as "%}
-    {% set final_view_sql = modules.re.sub(squarebracketview,"",final_view_sql, modules.re.I) %}
-    {%set regularview = schema_name~"."~view_name~ "as "%}
-    {% set final_view_sql = modules.re.sub(regularview,"",final_view_sql, modules.re.I) %}
     {% call statement('create_new_view') %}
         {{ create_view_as(to_relation, final_view_sql) }}
     {% endcall %}
     {% call statement('drop_old_view') %}
         EXEC('DROP VIEW IF EXISTS {{ from_relation.include(database=False) }};');
     {% endcall %}
   {% endif %}
   {% if to_relation.type == 'table' %}
       {% call statement('rename_relation') %}
-        EXEC('create table {{ to_relation.include(database=False) }} as select * from {{ from_relation.include(database=False) }};');
+        EXEC('create table {{ to_relation.include(database=False) }} as select * from {{ from_relation.include(database=False) }}');
       {%- endcall %}
       {{ fabric__drop_relation(from_relation) }}
   {% endif %}
 {% endmacro %}
 
 -- DROP fabric__truncate_relation when TRUNCATE TABLE is supported
 {% macro fabric__truncate_relation(relation) -%}
```

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/materializations/tests/test.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt/include/fabric/macros/utils/split_part.sql` & `dbt-fabric-1.4.0rc2/dbt/include/fabric/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/microsoft/dbt-fabric/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -27,18 +28,17 @@
 [dbt](https://www.getdbt.com) adapter for Microsoft Fabric Synapse Data Warehouse.
 
 The adapter supports dbt-core 1.4 or newer and follows the same versioning scheme.
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
-We've bundled all documentation on the dbt docs site:
-TODO
-* [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+We've bundled all documentation on the dbt docs site
+* [Profile setup & authentication](https://docs.getdbt.com/docs/core/connect-data-platform/fabric-setup)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/fabric-configs)
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
 [macOS](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/install-microsoft-odbc-driver-sql-server-macos?view=sql-server-ver16) |
 [Linux](https://docs.microsoft.com/nl-be/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16)
@@ -78,7 +78,9 @@
 ## License
 
 [![PyPI - License](https://img.shields.io/pypi/l/dbt-fabric)](https://github.com/microsoft/dbt-fabric/blob/main/LICENSE)
 
 ## Code of Conduct
 
 This project and everyone involved is expected to follow the [Microsoft Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+
+
```

### Comparing `dbt-fabric-1.4.0rc1/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.4.0rc2/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.4.0rc1/setup.py` & `dbt-fabric-1.4.0rc2/setup.py`

 * *Files identical despite different names*

