# Comparing `tmp/weaviate-client-3.9.0.dev2.tar.gz` & `tmp/weaviate-client-3.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate-client-3.9.0.dev2.tar", last modified: Mon Oct  3 12:30:33 2022, max compression
+gzip compressed data, was "dist/weaviate-client-3.9.0b0.tar", last modified: Fri Oct 28 19:02:12 2022, max compression
```

## Comparing `weaviate-client-3.9.0.dev2.tar` & `weaviate-client-3.9.0b0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.350964 weaviate-client-3.9.0.dev2/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1547 2022-09-21 15:57:14.000000 weaviate-client-3.9.0.dev2/LICENSE.md
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2874 2022-10-03 12:30:33.350837 weaviate-client-3.9.0.dev2/PKG-INFO
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2621 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/README.rst
--rw-r--r--   0 bobvanluijt   (501) staff       (20)       38 2022-10-03 12:30:33.351005 weaviate-client-3.9.0.dev2/setup.cfg
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1599 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/setup.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.342968 weaviate-client-3.9.0.dev2/test/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1037 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/test/test_auth.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     8006 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/test/test_client.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1744 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/test/test_exceptions.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    38765 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/test/test_util.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      276 2022-10-03 12:30:09.000000 weaviate-client-3.9.0.dev2/test/test_version.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.344080 weaviate-client-3.9.0.dev2/weaviate/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1730 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2549 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/auth.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.344309 weaviate-client-3.9.0.dev2/weaviate/backup/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      106 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/backup/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    14147 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/backup/backup.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.345195 weaviate-client-3.9.0.dev2/weaviate/batch/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      128 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/batch/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    48537 2022-10-03 12:28:37.000000 weaviate-client-3.9.0.dev2/weaviate/batch/crud_batch.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     7024 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/batch/requests.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.345764 weaviate-client-3.9.0.dev2/weaviate/classification/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      162 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/classification/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     4307 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/classification/classification.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     7910 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/classification/config_builder.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     8959 2022-10-02 10:05:50.000000 weaviate-client-3.9.0.dev2/weaviate/client.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.346010 weaviate-client-3.9.0.dev2/weaviate/connect/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      166 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/connect/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    19101 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/connect/connection.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.346303 weaviate-client-3.9.0.dev2/weaviate/contextionary/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      160 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/contextionary/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     5183 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.346564 weaviate-client-3.9.0.dev2/weaviate/data/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      144 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/data/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    31155 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/data/crud_data.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.347334 weaviate-client-3.9.0.dev2/weaviate/data/references/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      145 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/data/references/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    27985 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/data/references/crud_references.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2212 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/exceptions.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.348460 weaviate-client-3.9.0.dev2/weaviate/gql/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      143 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/gql/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    12099 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/gql/aggregate.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    25929 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/gql/filter.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    34010 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/gql/get.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     4284 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/gql/query.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.349124 weaviate-client-3.9.0.dev2/weaviate/schema/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)       98 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/schema/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    25659 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.349418 weaviate-client-3.9.0.dev2/weaviate/schema/properties/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      116 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/schema/properties/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2633 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     4808 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/schema/validate_schema.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    14800 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/util.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)       68 2022-10-03 12:30:00.000000 weaviate-client-3.9.0.dev2/weaviate/version.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.349760 weaviate-client-3.9.0.dev2/weaviate/wcs/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)      111 2022-09-21 15:57:14.000000 weaviate-client-3.9.0.dev2/weaviate/wcs/__init__.py
--rw-r--r--   0 bobvanluijt   (501) staff       (20)    21300 2022-09-24 18:04:06.000000 weaviate-client-3.9.0.dev2/weaviate/wcs/crud_wcs.py
-drwxr-xr-x   0 bobvanluijt   (501) staff       (20)        0 2022-10-03 12:30:33.350679 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1547 2022-09-21 15:57:14.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/LICENSE.md
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     2874 2022-10-03 12:30:33.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 bobvanluijt   (501) staff       (20)     1354 2022-10-03 12:30:33.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 bobvanluijt   (501) staff       (20)        1 2022-10-03 12:30:33.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 bobvanluijt   (501) staff       (20)       72 2022-10-03 12:30:33.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 bobvanluijt   (501) staff       (20)        9 2022-10-03 12:30:33.000000 weaviate-client-3.9.0.dev2/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1547 2022-09-07 15:57:04.000000 weaviate-client-3.9.0b0/LICENSE.md
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2871 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/PKG-INFO
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2621 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/README.rst
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       38 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/setup.cfg
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1626 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/setup.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/test/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1037 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/test/test_auth.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     7984 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/test/test_client.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1744 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/test/test_exceptions.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    38765 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/test/test_util.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      278 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/test/test_version.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1730 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2549 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/auth.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/backup/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       95 2022-10-19 07:42:59.000000 weaviate-client-3.9.0b0/weaviate/backup/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    14088 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/backup/backup.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/batch/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      128 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/batch/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    54236 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/batch/crud_batch.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     7115 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/batch/requests.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/classification/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      162 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/classification/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     4306 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/classification/classification.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     7910 2022-10-17 20:11:50.000000 weaviate-client-3.9.0b0/weaviate/classification/config_builder.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     8855 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/client.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/cluster/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      118 2022-10-27 12:40:16.000000 weaviate-client-3.9.0b0/weaviate/cluster/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1687 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/cluster/cluster.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/connect/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      166 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/connect/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    19240 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/connect/connection.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/contextionary/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      160 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/contextionary/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     5183 2022-10-17 20:10:21.000000 weaviate-client-3.9.0b0/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/data/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      144 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/data/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    29382 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/data/crud_data.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/data/references/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      145 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/data/references/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    25264 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/data/references/crud_references.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     4454 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/error_msgs.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2349 2022-10-27 13:21:49.000000 weaviate-client-3.9.0b0/weaviate/exceptions.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/gql/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      143 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/gql/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    12099 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/gql/aggregate.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    25699 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/gql/filter.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    34010 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/gql/get.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     4284 2022-10-17 20:08:35.000000 weaviate-client-3.9.0b0/weaviate/gql/query.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/schema/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       98 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/schema/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    25661 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/schema/properties/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      116 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2633 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     4808 2022-10-17 07:49:00.000000 weaviate-client-3.9.0b0/weaviate/schema/validate_schema.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    14543 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/util.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       70 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/version.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate/wcs/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)      111 2021-08-17 08:32:50.000000 weaviate-client-3.9.0b0/weaviate/wcs/__init__.py
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)    21300 2022-10-28 19:01:56.000000 weaviate-client-3.9.0b0/weaviate/wcs/crud_wcs.py
+drwxr-xr-x   0 stefanbogdan   (501) staff       (20)        0 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     2871 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)     1398 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        1 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)       72 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 stefanbogdan   (501) staff       (20)        9 2022-10-28 19:02:12.000000 weaviate-client-3.9.0b0/weaviate_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `weaviate-client-3.9.0.dev2/LICENSE.md` & `weaviate-client-3.9.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/PKG-INFO` & `weaviate-client-3.9.0b0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: weaviate-client
-Version: 3.9.0.dev2
-Summary: A python native weaviate client
-Author: SeMI Technologies
-Author-email: hello@semi.technology
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-
 Weaviate python client
 ======================
 .. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
     :width: 180
     :align: right
     :alt: Weaviate logo
```

### Comparing `weaviate-client-3.9.0.dev2/README.rst` & `weaviate-client-3.9.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: weaviate-client
+Version: 3.9.0b0
+Summary: A python native weaviate client
+Author: SeMI Technologies
+Author-email: hello@semi.technology
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+
 Weaviate python client
 ======================
 .. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
     :width: 180
     :align: right
     :alt: Weaviate logo
```

### Comparing `weaviate-client-3.9.0.dev2/setup.py` & `weaviate-client-3.9.0b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from builtins import open
 from os import path
+
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
+
 from weaviate.version import __version__
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
@@ -40,17 +42,18 @@
     "weaviate.backup",
     "weaviate.classification",
     "weaviate.contextionary",
     "weaviate.data",
     "weaviate.data.references",
     "weaviate.gql",
     "weaviate.wcs",
+    "weaviate.cluster",
   ],
-  python_requires='>=3.6',
+  python_requires='>=3.7',
   install_requires=[
-    "requests>=2.23.0,<2.28.0",
+    "requests>=2.23.0,<2.29.0",
     "validators>=0.18.2,<0.19.0",
-    "tqdm>=4.59.0,<5.0.0"
+    "tqdm>=4.59.0,<5.0.0",
   ],
   license_files = ('LICENSE.md',),
   cmdclass = {'egg_info': egg_info_ex},
 )
```

### Comparing `weaviate-client-3.9.0.dev2/test/test_auth.py` & `weaviate-client-3.9.0b0/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/test/test_client.py` & `weaviate-client-3.9.0b0/test/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from unittest.mock import patch, Mock
 from weaviate import Client
 from weaviate.exceptions import RequestsConnectionError, UnexpectedStatusCodeException
-from test.util import mock_connection_method, check_error_message
+from test.util import mock_connection_func, check_error_message
 
 
 
 @patch('weaviate.client.Connection', Mock)
 class TestWeaviateClient(unittest.TestCase):
 
     @patch('weaviate.client.Client.get_meta', return_value={'version': '1.13.2'})
@@ -90,76 +90,76 @@
     def test_is_ready(self, mock_get_meta_method):
         """
         Test the `is_ready` method.
         """
 
         client = Client("http://localhost:8080")
         # Request to weaviate returns 200
-        connection_mock = mock_connection_method('get')
+        connection_mock = mock_connection_func('get')
         client._connection = connection_mock
         self.assertTrue(client.is_ready())  # Should be true
         connection_mock.get.assert_called_with(
             path="/.well-known/ready"
         )
 
         # Request to weaviate returns 404
-        connection_mock = mock_connection_method('get', status_code=404)
+        connection_mock = mock_connection_func('get', status_code=404)
         client._connection = connection_mock
         self.assertFalse(client.is_ready())  # Should be false
         connection_mock.get.assert_called_with(
             path="/.well-known/ready"
         )
 
         # Test exception in connect
-        connection_mock = mock_connection_method('get', side_effect=RequestsConnectionError("Test"))
+        connection_mock = mock_connection_func('get', side_effect=RequestsConnectionError("Test"))
         client._connection = connection_mock
         self.assertFalse(client.is_ready())
         connection_mock.get.assert_called_with(
             path="/.well-known/ready"
         )
 
     @patch('weaviate.client.Client.get_meta', return_value={'version': '1.13.2'})
     def test_is_live(self, mock_get_meta):
         """
         Test the `is_live` method.
         """
 
         client = Client("http://localhost:8080")
         # Request to weaviate returns 200
-        connection_mock = mock_connection_method('get')
+        connection_mock = mock_connection_func('get')
         client._connection = connection_mock
         self.assertTrue(client.is_live())  # Should be true
         connection_mock.get.assert_called_with(
             path="/.well-known/live"
         )
 
         # Request to weaviate returns 404
-        connection_mock = mock_connection_method('get', status_code=404)
+        connection_mock = mock_connection_func('get', status_code=404)
         client._connection = connection_mock
         self.assertFalse(client.is_live())  # Should be false
         connection_mock.get.assert_called_with(
             path="/.well-known/live"
         )
 
     def test_get_meta(self):
         """
         Test the `get_meta` method.
         """
 
         # client = Client("http://localhost:8080")
         # # Request to weaviate returns 200
-        # connection_mock = mock_connection_method('get', return_json="OK!")
+        # connection_mock = mock_connection_func('get', return_json="OK!")
         # client._connection = connection_mock
         # self.assertEqual(client.get_meta(), "OK!")
         # connection_mock.get.assert_called_with(
         #     path="/meta"
         # )
 
         # # Request to weaviate returns 404
-        # connection_mock = mock_connection_method('get', status_code=404)
+        # connection_mock = mock_connection_func('get', status_code=404)
         # client._connection = connection_mock
         # with self.assertRaises(UnexpectedStatusCodeException) as error:
         #     client.get_meta()
         # error_message = "Meta endpoint! Unexpected status code: 404, with response body: None"
         # check_error_message(self, error, error_message)
         # connection_mock.get.assert_called_with(
         #     path="/meta"
@@ -169,32 +169,32 @@
     def test_get_open_id_configuration(self, mock_get_meta):
         """
         Test the `get_open_id_configuration` method.
         """
 
         client = Client("http://localhost:8080")
         # Request to weaviate returns 200
-        connection_mock = mock_connection_method('get', return_json="OK!")
+        connection_mock = mock_connection_func('get', return_json="OK!")
         client._connection = connection_mock
         self.assertEqual(client.get_open_id_configuration(), "OK!")
         connection_mock.get.assert_called_with(
             path="/.well-known/openid-configuration"
         )
 
         
         # Request to weaviate returns 404
-        connection_mock = mock_connection_method('get', status_code=404)
+        connection_mock = mock_connection_func('get', status_code=404)
         client._connection = connection_mock
         self.assertIsNone(client.get_open_id_configuration())
         connection_mock.get.assert_called_with(
             path="/.well-known/openid-configuration"
         )
 
         # Request to weaviate returns 204
-        connection_mock = mock_connection_method('get', status_code=204)
+        connection_mock = mock_connection_func('get', status_code=204)
         client._connection = connection_mock
         with self.assertRaises(UnexpectedStatusCodeException) as error:
             client.get_open_id_configuration()
         error_message = f"Meta endpoint! Unexpected status code: 204, with response body: None"
         check_error_message(self, error, error_message)
         connection_mock.get.assert_called_with(
             path="/.well-known/openid-configuration"
```

### Comparing `weaviate-client-3.9.0.dev2/test/test_exceptions.py` & `weaviate-client-3.9.0b0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/test/test_util.py` & `weaviate-client-3.9.0b0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/__init__.py` & `weaviate-client-3.9.0b0/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/auth.py` & `weaviate-client-3.9.0b0/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/backup/backup.py` & `weaviate-client-3.9.0b0/weaviate/backup/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         """
 
         self._connection = connection
 
     def create(self,
             backup_id: str,
             backend: str,
-            include_classes: Union[List[str], str, None]=None,
-            exclude_classes: Union[List[str], str, None]=None,
-            wait_for_completion: bool=False,
-        ) -> dict:
+            include_classes: Union[List[str], str, None] = None,
+            exclude_classes: Union[List[str], str, None] = None,
+            wait_for_completion: bool = False,
+            ) -> dict:
         """
         Create a backup of all/per class Weaviate objects.
 
         Parameters
         ----------
         backup_id : str
             The identifier name of the backup.
@@ -113,28 +113,27 @@
             raise RequestsConnectionError(
                 'Backup creation failed due to connection error.'
             ) from conn_err
         if response.status_code != 200:
             raise UnexpectedStatusCodeException("Backup creation", response)
 
         create_status: dict = response.json()
-        
+
         if wait_for_completion:
             while True:
                 status: dict = self.get_create_status(
                     backup_id=backup_id,
                     backend=backend,
                 )
                 create_status.update(status)
                 if status['status'] == 'SUCCESS':
                     break
-                elif status['status'] == 'FAILED':
+                if status['status'] == 'FAILED':
                     raise BackupFailedException(f'Backup failed: {create_status}')
-                else:
-                    sleep(1)
+                sleep(1)
         return create_status
 
     def get_create_status(self, backup_id: str, backend: str) -> bool:
         """
         Checks if a started classification job has completed.
 
         Parameters
@@ -223,15 +222,15 @@
             backup_id=backup_id,
             backend=backend,
             include_classes=include_classes,
             exclude_classes=exclude_classes,
             wait_for_completion=wait_for_completion,
         )
 
-        payload = { 
+        payload = {
             "config": {},
             "include": include_classes,
             "exclude": exclude_classes,
         }
         path = f'/backups/{backend}/{backup_id}/restore'
 
         try:
@@ -253,18 +252,17 @@
                 status: dict = self.get_restore_status(
                     backup_id=backup_id,
                     backend=backend,
                 )
                 restore_status.update(status)
                 if status['status'] == 'SUCCESS':
                     break
-                elif status['status'] == 'FAILED':
+                if status['status'] == 'FAILED':
                     raise BackupFailedException(f'Backup restore failed: {restore_status}')
-                else:
-                    sleep(1)
+                sleep(1)
         return restore_status
 
     def get_restore_status(self, backup_id: str, backend: str) -> bool:
         """
         Checks if a started classification job has completed.
 
         Parameters
@@ -304,15 +302,15 @@
 
 def _get_and_validate_create_restore_arguments(
         backup_id: str,
         backend: str,
         include_classes: Union[List[str], str, None],
         exclude_classes: Union[List[str], str, None],
         wait_for_completion: bool,
-    ) -> Tuple[str, str, List[str], List[str]]:
+        ) -> Tuple[str, str, List[str], List[str]]:
     """
     Validate and return the Backup.create/Backup.restore arguments.
 
     Parameters
     ----------
     backup_id : str
         The identifier name of the backup.
@@ -377,15 +375,15 @@
     else:
         exclude_classes = []
 
     if include_classes and exclude_classes:
         raise TypeError(
             "Either 'include_classes' OR 'exclude_classes' can be set, not both."
         )
-    
+
     include_classes = [_capitalize_first_letter(cls) for cls in include_classes]
     exclude_classes = [_capitalize_first_letter(cls) for cls in exclude_classes]
 
     return (backup_id.lower(), backend.lower(), include_classes, exclude_classes)
 
 
 def _get_and_validate_get_status(backup_id: str, backend: str) -> Tuple[str, str]:
@@ -418,9 +416,9 @@
             f"'backup_id' must be of type str. Given type: {type(backup_id)}."
         )
     if backend not in STORAGE_NAMES:
         raise ValueError(
             f"'backend' must have one of these values: {STORAGE_NAMES}. "
             f"Given value: {backend}."
         )
-    
+
     return (backup_id.lower(), backend.lower())
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/batch/crud_batch.py` & `weaviate-client-3.9.0b0/weaviate/batch/crud_batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 """
 Batch class definitions.
 """
-import asyncio
 import os
 import sys
 import time
-from numbers import Real
+import warnings
 from collections import deque
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from numbers import Real
 from typing import Tuple, Callable, Optional, Sequence
+
 from requests import ReadTimeout, Response
-from weaviate.exceptions import RequestsConnectionError, UnexpectedStatusCodeException
+
 from weaviate.connect import Connection
+from weaviate.error_msgs import (
+    BATCH_MANUAL_USE_W,
+    BATCH_REF_DEPRECATION_NEW_V14_CLS_NS_W,
+    BATCH_REF_DEPRECATION_OLD_V14_CLS_NS_W,
+    BATCH_EXECUTOR_SHUTDOWN_W,
+)
+from weaviate.exceptions import RequestsConnectionError, UnexpectedStatusCodeException
 from weaviate.util import (
     _capitalize_first_letter,
-    deprecation,
     check_batch_result,
 )
 from .requests import BatchRequest, ObjectsBatchRequest, ReferenceBatchRequest
 
+OS_CPU_COUNT = os.cpu_count()
+
+
+class BatchExecutor(ThreadPoolExecutor):
+    """
+    Weaviate Batch Executor to run batch requests in separate thread.
+    This class implements an additional method `is_shutdown` that us used my the context manager.
+    """
+
+    def is_shutdown(self) -> bool:
+        """
+        Check if executor is shutdown.
+
+        Returns
+        -------
+        bool
+            Whether the BatchExecutor is shutdown.
+        """
+
+        return self._shutdown
+
 
 class Batch:
     """
     Batch class used to add multiple objects or object references at once into weaviate.
     To add data to the Batch use these methods of this class: `add_data_object` and
     `add_reference`. This object also stores 2 recommended batch size variables, one for objects
     and one for references. The recommended batch size is updated with every batch creation, and
@@ -163,53 +192,49 @@
             Connection object to an active and running weaviate instance.
         """
 
         # set all protected attributes
         self._connection = connection
         self._objects_batch = ObjectsBatchRequest()
         self._reference_batch = ReferenceBatchRequest()
-        self._objects_per_second_frame = deque(
-            maxlen=5
+        # do not keep too many past values, so it is a better estimation of the throughput
+        # the throughput is computed for 1 second
+        self._objects_throughput_frame = deque(
+            maxlen=max(5, OS_CPU_COUNT),
         )
-        self._references_per_second_frame = deque(
-            maxlen=5
+        self._references_throughput_frame = deque(
+            maxlen=max(5, OS_CPU_COUNT),
         )
+        self._future_pool = []
+        self._reference_batch_queue = []
+        self._thread_creation_time = self._connection.timeout_config[1] / OS_CPU_COUNT
 
-        ## user configurable, need to be public should implement a setter/getter
+        # user configurable, need to be public should implement a setter/getter
         self._recommended_num_objects = None
         self._recommended_num_references = None
         self._callback = check_batch_result
         self._batch_size = None
         self._creation_time = 10.0
-        self._timeout_retries = 12
+        self._timeout_retries = 3
+        self._connection_error_retries = 3
         self._batching_type = None
-        self._max_threads = os.cpu_count()
+        self._num_workers = OS_CPU_COUNT
 
-        # create empty queue
-        self._queue = []
-        self._non_thread_message = False # Send when manual batching is enabled
-
-        # set loop
-        if sys.version_info < (3, 10):
-            self._loop = asyncio.get_event_loop()
-        else:
-            try:
-                self._loop = asyncio.get_running_loop()
-            except RuntimeError:
-                self._loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(self._loop)
+        # thread pool executor
+        self._executor: Optional[BatchExecutor] = None
 
     def configure(self,
-            batch_size: Optional[int]=None,
-            creation_time: Real=10,
-            timeout_retries: int=12,
-            callback: Optional[Callable[[dict], None]]=check_batch_result,
-            dynamic: bool=False,
-            max_threads: int=os.cpu_count()
-        ) -> 'Batch':
+            batch_size: Optional[int] = None,
+            creation_time: Real = 10,
+            timeout_retries: int = 3,
+            connection_error_retries: int = 3,
+            callback: Optional[Callable[[dict], None]] = check_batch_result,
+            dynamic: bool = False,
+            num_workers: int = OS_CPU_COUNT,
+            ) -> 'Batch':
         """
         Configure the instance to your needs. (`__call__` and `configure` methods are the same).
         NOTE: It has default values and if you want to change only one use a setter instead, or
         provide all the configurations.
 
         Parameters
         ----------
@@ -220,22 +245,26 @@
             is False -> the number of data in the Batch (sum of objects and references) when to
             auto-create; 2) in case `dynamic` is True -> the initial value for both
             `recommended_num_objects` and `recommended_num_references`, by default None
         creation_time : Real, optional
             The time interval it should take the Batch to be created, used ONLY for computing
             `recommended_num_objects` and `recommended_num_references`, by default 10
         timeout_retries : int, optional
-            Number of times to retry to create a Batch that failed with TimeOut error, by default 0
+            Number of retries to create a Batch that failed with ReadTimeout, by default 3
+        connection_error_retries : int, optional
+            Number of retries to create a Batch that failed with ConnectionError, by default 3
         callback : Optional[Callable[[dict], None]], optional
             A callback function on the results of each (objects and references) batch types.
             By default `weaviate.util.check_batch_result`.
         dynamic : bool, optional
             Whether to use dynamic batching or not, by default False
-        max_threads : int, optional
-            Max number of threads, by default 16
+        num_workers : int, optional
+            The maximal number of concurrent threads to run batch import. Only used for non-MANUAL
+            batching. i.e. is used only with AUTO or DYNAMIC batching.
+            By default, os.cpu_count()
 
         Returns
         -------
         Batch
             Updated self.
 
         Raises
@@ -246,27 +275,29 @@
             If the value of one of the arguments is wrong.
         """
 
         return self.__call__(
             batch_size=batch_size,
             creation_time=creation_time,
             timeout_retries=timeout_retries,
+            connection_error_retries=connection_error_retries,
             callback=callback,
             dynamic=dynamic,
-            max_threads=max_threads
+            num_workers=num_workers,
         )
 
     def __call__(self,
-            batch_size: Optional[int]=None,
-            creation_time: Real=10,
-            timeout_retries: int=0,
-            callback: Optional[Callable[[dict], None]]=check_batch_result,
-            dynamic: bool=False,
-            max_threads: int=os.cpu_count()
-        ) -> 'Batch':
+            batch_size: Optional[int] = None,
+            creation_time: Real = 10,
+            timeout_retries: int = 3,
+            connection_error_retries: int = 3,
+            callback: Optional[Callable[[dict], None]] = check_batch_result,
+            dynamic: bool = False,
+            num_workers: int = OS_CPU_COUNT,
+            ) -> 'Batch':
         """
         Configure the instance to your needs. (`__call__` and `configure` methods are the same).
         NOTE: It has default values and if you want to change only one use a setter instead, or
         provide all the configurations.
 
         Parameters
         ----------
@@ -277,20 +308,26 @@
             is False -> the number of data in the Batch (sum of objects and references) when to
             auto-create; 2) in case `dynamic` is True -> the initial value for both
             `recommended_num_objects` and `recommended_num_references`, by default None
         creation_time : Real, optional
             The time interval it should take the Batch to be created, used ONLY for computing
             `recommended_num_objects` and `recommended_num_references`, by default 10
         timeout_retries : int, optional
-            Number of times to retry to create a Batch that failed with TimeOut error, by default 0
+            Number of retries to create a Batch that failed with ReadTimeout, by default 3
+        connection_error_retries : int, optional
+            Number of retries to create a Batch that failed with ConnectionError, by default 3
         callback : Optional[Callable[[dict], None]], optional
             A callback function on the results of each (objects and references) batch types.
             By default `weaviate.util.check_batch_result`
         dynamic : bool, optional
             Whether to use dynamic batching or not, by default False
+        num_workers : int, optional
+            The maximal number of concurrent threads to run batch import. Only used for non-MANUAL
+            batching. i.e. is used only with AUTO or DYNAMIC batching.
+            By default, os.cpu_count()
 
         Returns
         -------
         Batch
             Updated self.
 
         Raises
@@ -299,48 +336,55 @@
             If one of the arguments is of a wrong type.
         ValueError
             If the value of one of the arguments is wrong.
         """
 
         _check_positive_num(creation_time, 'creation_time', Real)
         _check_non_negative(timeout_retries, 'timeout_retries', int)
+        _check_non_negative(connection_error_retries, 'connection_error_retries', int)
+
+        self._callback = callback
+        self._creation_time = creation_time
+        self._timeout_retries = timeout_retries
+        self._connection_error_retries = connection_error_retries
 
         # set Batch to manual import
         if batch_size is None:
-            self._callback = callback
             self._batch_size = None
-            self._creation_time = creation_time
-            self._timeout_retries = timeout_retries
             self._batching_type = None
             return self
 
         _check_positive_num(batch_size, 'batch_size', int)
+        _check_positive_num(num_workers, 'num_workers', int)
         _check_bool(dynamic, 'dynamic')
 
-        self._callback = callback
         self._batch_size = batch_size
-        self._creation_time = creation_time
-        self._timeout_retries = timeout_retries
-        self._max_threads = max_threads
 
-        if dynamic is False: # set Batch to auto-commit with fixed batch_size
+        if self._num_workers != num_workers:
+            self.flush()
+            self.shutdown()
+            self._num_workers = num_workers
+            self.start()
+            self._thread_creation_time = self._connection.timeout_config[1] / num_workers
+
+        if dynamic is False:  # set Batch to auto-commit with fixed batch_size
             self._batching_type = 'fixed'
-        else: # else set to 'dynamic'
+        else:  # else set to 'dynamic'
             self._batching_type = 'dynamic'
             self._recommended_num_objects = batch_size
             self._recommended_num_references = batch_size
         self._auto_create()
         return self
 
     def add_data_object(self,
             data_object: dict,
             class_name: str,
-            uuid: Optional[str]=None,
-            vector: Optional[Sequence]=None
-        ) -> str:
+            uuid: Optional[str] = None,
+            vector: Optional[Sequence] = None
+            ) -> str:
         """
         Add one object to this batch.
         NOTE: If the UUID of one of the objects already exists then the existing object will be
         replaced by the new object.
 
         Parameters
         ----------
@@ -382,16 +426,16 @@
         return uuid
 
     def add_reference(self,
             from_object_uuid: str,
             from_object_class_name: str,
             from_property_name: str,
             to_object_uuid: str,
-            to_object_class_name: Optional[str]=None,
-        ) -> None:
+            to_object_class_name: Optional[str] = None,
+            ) -> None:
         """
         Add one reference to this batch.
 
         Parameters
         ----------
         from_object_uuid : str
             The UUID or URL of the object that should reference another object.
@@ -416,29 +460,25 @@
         ValueError
             If 'uuid' is not valid or cannot be extracted.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if to_object_class_name is None and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "beacons, please specify the `to_object_class_name` argument for this. The "
-                "non-class namespaced beacons (None value for `to_object_class_name`) are going "
-                "to be removed in the future versions of the Weaviate Server and Weaviate Python "
-                "Client."
+            warnings.warn(
+                message=BATCH_REF_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if to_object_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. The "
-                    "non-class namespaced APIs calls are going to be made instead (None value for "
-                    "`class_name`). The non-class namespaced APIs are going to be removed in "
-                    "future versions of the Weaviate Server and Weaviate Python Client. "
-                    "Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=BATCH_REF_DEPRECATION_OLD_V14_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
                 to_object_class_name = None
             if is_server_version_14:
                 if not isinstance(to_object_class_name, str):
                     raise TypeError(
                         "'to_object_class_name' must be of type str or None. "
                         f"Given type: {type(to_object_class_name)}"
@@ -455,15 +495,15 @@
 
         if self._batching_type:
             self._auto_create()
 
     def _create_data(self,
             data_type: str,
             batch_request: BatchRequest,
-        ) -> Response:
+            ) -> Response:
         """
         Create data in batches, either Objects or References. This does NOT guarantee
         that each batch item (only Objects) is added/created. This can lead to a successful
         batch creation but unsuccessful per batch item creation. See the Examples below.
 
         Parameters
         ----------
@@ -478,35 +518,44 @@
         Returns
         -------
         requests.Response
             The requests response.
 
         Raises
         ------
+        requests.ReadTimeout
+            If the request time-outed.
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
         """
 
         try:
-            for i in range(self._timeout_retries + 1):
+            timeout_count = connection_count = 0
+            while True:
                 try:
                     response = self._connection.post(
                         path='/batch/' + data_type,
                         weaviate_object=batch_request.get_request_body()
                     )
-                except ReadTimeout:
-                    if i == self._timeout_retries:
-                        raise
-                    print(
-                        f'[ERROR] Batch ReadTimeout Exception occurred! Retrying in {(i+1)*2}s. '
-                        f'[{i+1}/{self._timeout_retries}]', file=sys.stderr
+                except ReadTimeout as error:
+                    _batch_create_error_handler(
+                        retry=timeout_count,
+                        max_retries=self._timeout_retries,
+                        error=error,
+                    )
+                    timeout_count += 1
+                except RequestsConnectionError as error:
+                    _batch_create_error_handler(
+                        retry=connection_count,
+                        max_retries=self._connection_error_retries,
+                        error=error,
                     )
-                    time.sleep((i + 1) * 2)
+                    connection_count += 1
                 else:
                     break
         except RequestsConnectionError as conn_err:
             raise RequestsConnectionError('Batch was not added to weaviate.') from conn_err
         except ReadTimeout:
             message = (
                 f"The '{data_type}' creation was cancelled because it took "
@@ -515,15 +564,15 @@
                 "Aim to on average complete batch request within less than 10s"
             )
             raise ReadTimeout(message) from None
         if response.status_code == 200:
             return response
         raise UnexpectedStatusCodeException(f"Create {data_type} in batch", response)
 
-    def create_objects(self, queue_c = None) -> list:
+    def create_objects(self) -> list:
         """
         Creates multiple Objects at once in Weaviate. This does not guarantee that each batch item
         is added/created to the Weaviate server. This can lead to a successful batch creation but
         unsuccessful per batch item creation. See the example bellow.
         NOTE: If the UUID of one of the objects already exists then the existing object will be
         replaced by the new object.
 
@@ -601,51 +650,36 @@
         ------
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
         """
 
-        # If queue_c == None, run the import without threads
-        if queue_c == None:
-
-            if self._non_thread_message == False:
-                print(f'[INFO] You are manually batching this means you are not using the client\'s built-in multi-threading. Setting `batch_size` in `client.batch.configure()` to an int value will enabled this. Also see: https://weaviate.io/developers/weaviate/current/restful-api-references/batch.html#example-request-1')
-                self._non_thread_message = True
+        if len(self._objects_batch) != 0:
+            warnings.warn(
+                message=BATCH_MANUAL_USE_W,
+                category=RuntimeWarning,
+                stacklevel=1,
+            )
 
             response = self._create_data(
                 data_type='objects',
                 batch_request=self._objects_batch,
             )
-            self._objects_per_second_frame.append(
+            self._objects_throughput_frame.append(
                 len(self._objects_batch) / response.elapsed.total_seconds()
             )
 
-            obj_per_second = sum(self._objects_per_second_frame)/len(self._objects_per_second_frame)
+            obj_per_second = sum(self._objects_throughput_frame)/len(self._objects_throughput_frame)
             self._recommended_num_objects = round(obj_per_second * self._creation_time)
             self._objects_batch = ObjectsBatchRequest()
             return response.json()
-
-        # If queue_c == int, run the import with threads
-        if len(self._queue[queue_c]['_objects_batch']) != 0:
-            response = self._create_data(
-                data_type='objects',
-                batch_request=self._queue[queue_c]['_objects_batch'],
-            )
-            self._objects_per_second_frame.append(
-                len(self._queue[queue_c]['_objects_batch']) / response.elapsed.total_seconds()
-            )
-
-            obj_per_second = sum(self._objects_per_second_frame)/len(self._objects_per_second_frame)
-            self._recommended_num_objects = round(obj_per_second * self._creation_time)
-            self._queue[queue_c]['_objects_batch'] = ObjectsBatchRequest()
-            return response.json()
         return []
 
-    def create_references(self, queue_c) -> list:
+    def create_references(self) -> list:
         """
         Creates multiple References at once in Weaviate.
         Adding References in batch is faster but it ignores validations like class name
         and property name, resulting in a SUCCESSFUL reference creation of a nonexistent object
         types and/or a nonexistent properties. If the consistency of the References is wanted
         use 'client.data_object.reference.add' to have additional validation against the
         weaviate schema. See Examples below.
@@ -711,110 +745,190 @@
         ------
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
         """
 
-        if len(self._queue[queue_c]['_reference_batch']) != 0:
+        if len(self._reference_batch) != 0:
+            warnings.warn(
+                message=BATCH_MANUAL_USE_W,
+                category=RuntimeWarning,
+                stacklevel=1,
+            )
+
             response = self._create_data(
                 data_type='references',
-                batch_request=self._queue[queue_c]['_reference_batch'],
+                batch_request=self._reference_batch,
             )
-            self._references_per_second_frame.append(
-                len(self._queue[queue_c]['_reference_batch']) / response.elapsed.total_seconds()
+            self._references_throughput_frame.append(
+                len(self._reference_batch) / response.elapsed.total_seconds()
             )
 
             ref_per_sec = (
-                sum(self._references_per_second_frame)/len(self._references_per_second_frame)
+                sum(self._references_throughput_frame)/len(self._references_throughput_frame)
             )
             self._recommended_num_references = round(ref_per_sec * self._creation_time)
-            self._queue[queue_c]['_reference_batch'] = ReferenceBatchRequest()
+            self._reference_batch = ReferenceBatchRequest()
             return response.json()
         return []
 
-    async def _run_queue(self) -> None:
+    def _flush_in_thread(self,
+            data_type: str,
+            batch_request: BatchRequest,
+            ) -> Tuple[Response, int]:
         """
-        Runs the async queue.
+        Flush BatchRequest in current thread/process.
+
+        Parameters
+        ----------
+        data_type : str
+            The data type of the BatchRequest, used to save time for not checking the type of the
+            BatchRequest.
+        batch_request : weaviate.batch.BatchRequest
+            Contains all the data objects that should be added in one batch.
+            Note: Should be a sub-class of BatchRequest since BatchRequest
+            is just an abstract class, e.g. ObjectsBatchRequest, ReferenceBatchRequest
+
+        Returns
+        -------
+        Tuple[requests.Response, int]
+            The request response and number of items sent with the BatchRequest as tuple.
         """
 
-        coroutine_list = {}
-        
-        # create the async tasks
-        c = 0
-        while c < len(self._queue):
-            coroutine_list[c] = asyncio.create_task(self.flush(c))
-            c+=1
-
-        # await the async tasks
-        c = 0
-        while c < len(self._queue):
-            await coroutine_list[c]
-            c+=1
+        if len(batch_request) != 0:
+            response = self._create_data(
+                data_type=data_type,
+                batch_request=batch_request,
+            )
+            return response, len(batch_request)
+        return None, 0
 
-        self._queue = []
+    def _send_batch_requests(self, force_wait: bool) -> None:
+        """
+        Send BatchRequest in a separate thread/process. This methods submits a task to create only
+        the ObjectsBatchRequests to the BatchExecutor and adds the ReferencesBatchRequests to a
+        queue, then it carries on in the main thread until `num_workers` tasks have been submitted.
+        When we have reached number of tasks to be equal to `num_workers` it waits for all the
+        tasks to finish and handles the responses. After all ObjectsBatchRequests have been handled
+        it created separate tasks for each ReferencesBatchRequests, then it handles their responses
+        as well. This mechanism of creating References after Objects is constructed in this manner
+        to eliminate potential error when creating references from a object that does not yet
+        exists (object that is part of another task).
+
+        Parameters
+        ----------
+        force_wait : bool
+            Whether to wait on all created tasks even if we do not have `num_workers` tasks created
+        """
+        if self._executor is None:
+            self.start()
+        elif self._executor.is_shutdown():
+            warnings.warn(
+                message=BATCH_EXECUTOR_SHUTDOWN_W,
+                category=RuntimeWarning,
+                stacklevel=1,
+            )
+            self.start()
+
+        future = self._executor.submit(
+            self._flush_in_thread,
+            data_type='objects',
+            batch_request=self._objects_batch,
+        )
+        self._future_pool.append(future)
+        if len(self._reference_batch) > 0:
+            self._reference_batch_queue.append(
+                self._reference_batch
+            )
+        self._objects_batch = ObjectsBatchRequest()
+        self._reference_batch = ReferenceBatchRequest()
+
+        if not force_wait and len(self._future_pool) < self._num_workers:
+            return
+
+        for done_future in as_completed(self._future_pool):
+
+            response_objects, nr_objects = done_future.result()
+
+            # handle objects response
+            if response_objects:
+                self._objects_throughput_frame.append(
+                    nr_objects / response_objects.elapsed.total_seconds()
+                )
+                if self._callback:
+                    self._callback(response_objects.json())
+
+        if len(self._objects_throughput_frame) != 0:
+            obj_per_second = (
+                sum(self._objects_throughput_frame)/len(self._objects_throughput_frame)
+            )
+            self._recommended_num_objects = round(obj_per_second * self._thread_creation_time)
+        # Create references after all the objects have been created
+        reference_future_pool = []
+        for reference_batch in self._reference_batch_queue:
+            future = self._executor.submit(
+                self._flush_in_thread,
+                data_type='references',
+                batch_request=reference_batch,
+            )
+            reference_future_pool.append(future)
+
+        for done_future in as_completed(reference_future_pool):
+
+            response_references, nr_references = done_future.result()
+
+            # handle references response
+            if response_references:
+                self._references_throughput_frame.append(
+                    nr_references / response_references.elapsed.total_seconds()
+                )
+                if self._callback:
+                    self._callback(response_references.json())
+
+        if len(self._references_throughput_frame) != 0:
+            ref_per_sec = (
+                sum(self._references_throughput_frame)/len(self._references_throughput_frame)
+            )
+            self._recommended_num_references = round(ref_per_sec * self._thread_creation_time)
+
+        self._future_pool = []
+        self._reference_batch_queue = []
+        return
 
     def _auto_create(self) -> None:
         """
         Auto create both objects and references in the batch. This protected method works with a
-        fixed batch size and with dynamic batching. FOr a 'fixed' batching type it auto-creates
+        fixed batch size and with dynamic batching. For a 'fixed' batching type it auto-creates
         when the sum of both objects and references equals batch_size. For dynamic batching it
         creates both batch requests when only one is full.
         """
 
         # greater or equal in case the self._batch_size is changed manually
         if self._batching_type == 'fixed':
             if sum(self.shape) >= self._batch_size:
-                self._queue.append({
-                    '_objects_batch': self._objects_batch,
-                    '_reference_batch': self._reference_batch
-                })
-                self._objects_batch = ObjectsBatchRequest()
-                self._reference_batch = ReferenceBatchRequest()
-                if len(self._queue) >= self._max_threads:
-                    asyncio.run(self._run_queue())
+                self._send_batch_requests(force_wait=False)
             return
         if self._batching_type == 'dynamic':
             if (
-                self.num_objects() >= self._recommended_num_objects
-                or self.num_references() >= self._recommended_num_references
+                    self.num_objects() >= self._recommended_num_objects
+                    or self.num_references() >= self._recommended_num_references
             ):
-                self._queue.append({
-                    '_objects_batch': self._objects_batch,
-                    '_reference_batch': self._reference_batch
-                })
-                self._objects_batch = ObjectsBatchRequest()
-                self._reference_batch = ReferenceBatchRequest()
-                if len(self._queue) >= self._max_threads:
-                    asyncio.run(self._run_queue())
+                self._send_batch_requests(force_wait=False)
             return
         # just in case
         raise ValueError(f'Unsupported batching type "{self._batching_type}"')
 
-    async def flush(self, queue_c) -> None:
+    def flush(self) -> None:
         """
         Flush both objects and references to the Weaviate server and call the callback function
         if one is provided. (See the docs for `configure` or `__call__` for how to set one.)
-        The function is async and will directly retry if it fails
         """
 
-        try:
-            loop = asyncio.get_running_loop()
-            result_objects_action = loop.run_in_executor(None, self.create_objects, queue_c)
-            result_references_action = loop.run_in_executor(None, self.create_references, queue_c)
-            result_objects = await result_objects_action
-            result_references = await result_references_action
-            if self._callback is not None:
-                if result_objects:
-                    self._callback(result_objects)
-                if result_references:
-                    self._callback(result_references)
-        except:
-            print(f'[WARNING] Connection closed by peer! Retry to decreasing threads if this keeps happening.')
-            await self.flush(queue_c)
+        self._send_batch_requests(force_wait=True)
 
     def delete_objects(self,
             class_name: str,
             where: dict,
             output: str='minimal',
             dry_run: bool=False,
         ) -> dict:
@@ -949,15 +1063,15 @@
         -------
         int
             The number of references in the batch.
         """
 
         return len(self._reference_batch)
 
-    def pop_object(self, index: int=-1) -> dict:
+    def pop_object(self, index: int = -1) -> dict:
         """
         Remove and return the object at index (default last).
 
         Parameters
         ----------
         index : int, optional
             The index of the object to pop, by default -1 (last item).
@@ -971,15 +1085,15 @@
         -------
         IndexError
             If batch is empty or index is out of range.
         """
 
         return self._objects_batch.pop(index)
 
-    def pop_reference(self, index: int=-1) -> dict:
+    def pop_reference(self, index: int = -1) -> dict:
         """
         Remove and return the reference at index (default last).
 
         Parameters
         ----------
         index : int, optional
             The index of the reference to pop, by default -1 (last item).
@@ -1159,24 +1273,41 @@
         -------
         Optional[int]
             The recommended number of references per batch. If None then it could not be computed.
         """
 
         return self._recommended_num_references
 
-    def __enter__(self):
+    def start(self) -> 'Batch':
+        """
+        Start the BatchExecutor if it was closed.
+
+        Returns
+        -------
+        Batch
+            Updated self.
+        """
+
+        if self._executor is None or self._executor.is_shutdown():
+            self._executor = BatchExecutor(max_workers=self._num_workers)
         return self
 
+    def shutdown(self) -> None:
+        """
+        Shutdown the BatchExecutor.
+        """
+
+        self._executor.shutdown()
+
+    def __enter__(self) -> 'Batch':
+        return self.start()
+
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._queue.append({
-            '_objects_batch': self._objects_batch,
-            '_reference_batch': self._reference_batch
-        })
-        asyncio.run(self._run_queue())
-        self._loop.close()
+        self.flush()
+        self.shutdown()
 
     @property
     def creation_time(self) -> Real:
         """
         Setter and Getter for `creation_time`.
 
         Parameters
@@ -1244,14 +1375,45 @@
 
     @timeout_retries.setter
     def timeout_retries(self, value: int) -> None:
 
         _check_non_negative(value, 'timeout_retries', int)
         self._timeout_retries = value
 
+    @property
+    def connection_error_retries(self) -> int:
+        """
+        Setter and Getter for `connection_error_retries`.
+
+        Properties
+        ----------
+        value : int
+            Setter ONLY: The new value for `connection_error_retries`.
+
+        Returns
+        -------
+        int
+            Getter ONLY: The `connection_error_retries` value.
+
+        Raises
+        ------
+        TypeError
+            Setter ONLY: If the new value is not of type int.
+        ValueError
+            Setter ONLY: If the new value has a non positive value.
+        """
+
+        return self._connection_error_retries
+
+    @connection_error_retries.setter
+    def connection_error_retries(self, value: int) -> None:
+
+        _check_non_negative(value, 'connection_error_retries', int)
+        self._connection_error_retries = value
+
 
 def _check_positive_num(value: Real, arg_name: str, data_type: type) -> None:
     """
     Check if the `value` of the `arg_name` is a positive number.
 
     Parameters
     ----------
@@ -1318,7 +1480,37 @@
     ------
     TypeError
         If the `value` is not of type bool.
     """
 
     if not isinstance(value, bool):
         raise TypeError(f"'{arg_name}' must be of type bool.")
+
+
+def _batch_create_error_handler(retry: int, max_retries: int, error: Exception) -> None:
+    """
+    Handle errors that occur in Batch creation. This function is going to re-raise the error if
+    number of re-tries was reached.
+
+    Parameters
+    ----------
+    retry : int
+        Current number of attempted request calls.
+    max_retries : int
+        Maximum number of attempted request calls.
+    error : Exception
+        The exception that occurred (to be re-raised if needed).
+
+    Raises
+    ------
+    Exception
+        The caught exception.
+    """
+
+    if retry >= max_retries:
+        raise error
+    print(
+        f'[ERROR] Batch {error.__class__.__name__} Exception occurred! Retrying in '
+        f'{(retry + 1) * 2}s. [{retry + 1}/{max_retries}]',
+        file=sys.stderr,
+    )
+    time.sleep((retry + 1) * 2)
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/batch/requests.py` & `weaviate-client-3.9.0b0/weaviate/batch/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def empty(self) -> None:
         """
         Remove all the items from the BatchRequest.
         """
 
         self._items = []
 
-    def pop(self, index: int=-1) -> dict:
+    def pop(self, index: int = -1) -> dict:
         """
         Remove and return item at index (default last).
 
         Parameters
         ----------
         index : int, optional
             The index of the item to pop, by default -1 (last item).
@@ -80,16 +80,16 @@
     """
 
     def add(self,
             from_object_class_name: str,
             from_object_uuid: str,
             from_property_name: str,
             to_object_uuid: str,
-            to_object_class_name: Optional[str]=None,
-        ) -> None:
+            to_object_class_name: Optional[str] = None,
+            ) -> None:
         """
         Add one Weaviate-object reference to this batch. Does NOT validate the consistency of the
         reference against the class schema. Checks the arguments' type and UUIDs' format.
 
         Parameters
         ----------
         from_object_class_name : str
@@ -113,39 +113,38 @@
         TypeError
             If arguments are not of type str.
         ValueError
             If 'uuid' is not valid or cannot be extracted.
         """
 
         if (
-            not isinstance(from_object_class_name, str)
-            or not isinstance(from_object_uuid, str)
-            or not isinstance(from_property_name, str)
-            or not isinstance(to_object_uuid, str)
+                not isinstance(from_object_class_name, str)
+                or not isinstance(from_object_uuid, str)
+                or not isinstance(from_property_name, str)
+                or not isinstance(to_object_uuid, str)
         ):
             raise TypeError('All arguments must be of type string')
 
+        to_object_uuid = get_valid_uuid(to_object_uuid)
+        from_object_uuid = get_valid_uuid(from_object_uuid)
+
         if to_object_class_name is not None:
             to_beacon = f'weaviate://localhost/{to_object_class_name}/{to_object_uuid}'
         else:
             to_beacon = f'weaviate://localhost/{to_object_uuid}'
 
-
-        from_object_uuid = get_valid_uuid(from_object_uuid)
-        to_object_uuid = get_valid_uuid(to_object_uuid)
-
         self._items.append(
             {
-            'from': 'weaviate://localhost/'
-                + from_object_class_name
-                + '/'
-                + from_object_uuid
-                + '/'
-                + from_property_name,
-            'to': to_beacon
+                'from': 'weaviate://localhost/'
+                        + from_object_class_name
+                        + '/'
+                        + from_object_uuid
+                        + '/'
+                        + from_property_name,
+                'to': to_beacon
             }
         )
 
     def get_request_body(self) -> List[dict]:
         """
         Get request body as a list of dictionaries, where each dictionary
         is a Weaviate-object reference.
@@ -164,17 +163,17 @@
     Collect objects for one batch request to weaviate.
     Caution this batch will not be validated through weaviate.
     """
 
     def add(self,
             data_object: dict,
             class_name: str,
-            uuid: Optional[str]=None,
-            vector: Optional[Sequence]=None,
-        ) -> str:
+            uuid: Optional[str] = None,
+            vector: Optional[Sequence] = None,
+            ) -> str:
         """
         Add one object to this batch. Does NOT validate the consistency of the object against
         the client's schema. Checks the arguments' type and UUIDs' format.
 
         Parameters
         ----------
         class_name : str
@@ -210,15 +209,15 @@
         batch_item = {
             "class": class_name,
             "properties": copy.deepcopy(data_object)
         }
         if uuid is not None:
             batch_item["id"] = get_valid_uuid(uuid)
         else:
-            batch_item["id"] = uuid4().hex
+            batch_item["id"] = get_valid_uuid(uuid4())
 
         if vector is not None:
             batch_item["vector"] = get_vector(vector)
 
         self._items.append(batch_item)
 
         return batch_item["id"]
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/classification/classification.py` & `weaviate-client-3.9.0b0/weaviate/classification/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Classification class definition.
 """
-
 from weaviate.exceptions import UnexpectedStatusCodeException, RequestsConnectionError
 from weaviate.util import get_valid_uuid
 from weaviate.connect import Connection
 from .config_builder import ConfigBuilder
 
 class Classification:
     """
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/classification/config_builder.py` & `weaviate-client-3.9.0b0/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/client.py` & `weaviate-client-3.9.0b0/weaviate/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Client class definition.
 """
-from typing import Optional, Tuple, Union
+import warnings
 from numbers import Real
+from typing import Optional, Tuple, Union
+
 from .auth import AuthCredentials
-from .exceptions import UnexpectedStatusCodeException, RequestsConnectionError
-from .connect import Connection
+from .backup import Backup
+from .batch import Batch
 from .classification import Classification
-from .schema import Schema
+from .connect import Connection
 from .contextionary import Contextionary
-from .batch import Batch
-from .backup import Backup
 from .data import DataObject
+from .exceptions import UnexpectedStatusCodeException, RequestsConnectionError
 from .gql import Query
-from .util import deprecation
+from .cluster import Cluster
+from .schema import Schema
 from .version import __version__
+from .error_msgs import CLIENT_V14_W
 
 
 class Client:
     """
     A python native weaviate Client class that encapsulates Weaviate functionalities in one object.
     A Client instance creates all the needed objects to interact with Weaviate, and connects all of
     them to the same Weaviate instance. See below the Attributes of the Client instance. For the
@@ -39,35 +42,35 @@
     schema : weaviate.schema.Schema
         A Schema object instance connected to the same Weaviate instance as the Client.
     query : weaviate.gql.Query
         A Query object instance connected to the same Weaviate instance as the Client.
     """
 
     def __init__(self,
-            url: str,
-            auth_client_secret: Optional[AuthCredentials]=None,
-            timeout_config: Union[Tuple[Real, Real], Real]=(300, 240),
-            proxies: Union[dict, str, None]=None,
-            trust_env: bool=False,
-            additional_headers: Optional[dict]=None,
-        ):
+                 url: str,
+                 auth_client_secret: Optional[AuthCredentials] = None,
+                 timeout_config: Union[Tuple[Real, Real], Real] = (10, 60),
+                 proxies: Union[dict, str, None] = None,
+                 trust_env: bool = False,
+                 additional_headers: Optional[dict] = None,
+                 ):
         """
         Initialize a Client class instance.
 
         Parameters
         ----------
         url : str
             The URL to the weaviate instance.
         auth_client_secret : weaviate.AuthCredentials or None, optional
             Authentication client secret, by default None.
         timeout_config : tuple(Real, Real) or Real, optional
             Set the timeout configuration for all requests to the Weaviate server. It can be a
             real number or, a tuple of two real numbers: (connect timeout, read timeout).
             If only one real number is passed then both connect and read timeout will be set to
-            that value, by default (300, 240).
+            that value, by default (2, 20).
         proxies : dict, str or None, optional
             Proxies to be used for requests. Are used by both 'requests' and 'aiohttp'. Can be
             passed as a dict ('requests' format:
             https://docs.python-requests.org/en/stable/user/advanced/#proxies), str (HTTP/HTTPS
             protocols are going to use this proxy) or None.
             By default None.
         trust_env : bool, optional
@@ -122,23 +125,23 @@
         self.classification = Classification(self._connection)
         self.schema = Schema(self._connection)
         self.contextionary = Contextionary(self._connection)
         self.batch = Batch(self._connection)
         self.data_object = DataObject(self._connection)
         self.query = Query(self._connection)
         self.backup = Backup(self._connection)
+        self.cluster = Cluster(self._connection)
 
         self._set_server_version()
 
         if self._connection.server_version < '1.14':
-            deprecation(
-                f"You are using the Weaviate Python Client version {__version__} which introduces "
-                "the new changes/features of the Weaviate Server 1.14.x. If you want to make use "
-                "of the new changes/features of the Weaviate Server 1.14.x using this Python "
-                "Client version, upgrade the Weaviate Server version."
+            warnings.warn(
+                message=CLIENT_V14_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
 
     def is_ready(self) -> bool:
         """
         Ping Weaviate's ready state
 
         Returns
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/connect/connection.py` & `weaviate-client-3.9.0b0/weaviate/connect/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Connection class definition.
 """
+import datetime
 import os
 import time
-import datetime
-from typing import Tuple, Optional, Union
 from numbers import Real
+from typing import Tuple, Optional, Union
+
 import requests
 from requests import RequestException
-from weaviate.exceptions import AuthenticationFailedException
+
 from weaviate.auth import AuthCredentials
+from weaviate.exceptions import AuthenticationFailedException
 from weaviate.util import _get_valid_timeout_config
 
 
 class Connection:
     """
     Connection class used to communicate to a weaviate instance.
     """
@@ -60,15 +62,15 @@
             configured.
         """
 
         self._api_version_path = '/v1'
         self._server_version = None
         self._session = requests.Session()
         self.url = url  # e.g. http://localhost:80
-        self._timeout_config = timeout_config # this uses the setter
+        self.timeout_config = timeout_config  # this uses the setter
 
         self._auth_expires = 0  # unix time when auth expires
         self._auth_bearer = None
         self._auth_client_secret = auth_client_secret
 
         self._is_authentication_required = False
 
@@ -154,17 +156,18 @@
                 )
             except RequestException as error:
                 raise AuthenticationFailedException("Cannot connect to weaviate.") from error
             if request.status_code != 200:
                 raise AuthenticationFailedException("Cannot authenticate http status not ok.")
 
             # Set the client ID
-            client_id = request.json()['clientId']
+            response_json = request.json()
+            client_id = response_json['clientId']
 
-            self._set_bearer(client_id=client_id, href=request.json()['href'])
+            self._set_bearer(client_id=client_id, href=response_json['href'])
 
     def _set_bearer(self, client_id: str, href: str) -> None:
         """
         Set bearer for a refreshed authentication.
 
         Parameters
         ----------
@@ -194,27 +197,28 @@
             ) from error
         if request_third_part.status_code != 200:
             raise AuthenticationFailedException(
                 "Status not OK in connection to the third party authentication service."
             )
 
         # Validate third part auth info
-        if 'client_credentials' not in request_third_part.json()['grant_types_supported']:
+        json_third_party_response = request_third_part.json()
+        if 'client_credentials' not in json_third_party_response['grant_types_supported']:
             raise AuthenticationFailedException(
                 "The grant_types supported by the third-party authentication service are "
                 "insufficient. Please add 'client_credentials'."
             )
 
         request_body = self._auth_client_secret.get_credentials()
         request_body["client_id"] = client_id
 
         # try the request
         try:
             request = requests.post(
-                request_third_part.json()['token_endpoint'],
+                json_third_party_response['token_endpoint'],
                 request_body,
                 timeout=(30, 45),
                 proxies=self._proxies,
             )
         except RequestException:
             raise AuthenticationFailedException(
                 "Unable to get a OAuth token from server. Are the credentials "
@@ -224,17 +228,18 @@
         # sleep to process
         time.sleep(0.125)
 
         if request.status_code == 401:
             raise AuthenticationFailedException(
                 "Authentication access denied. Are the credentials correct?"
             )
-        self._auth_bearer = request.json()['access_token']
+        json_request = request.json()
+        self._auth_bearer = json_request['access_token']
         # -2 for some lag time
-        self._auth_expires = int(_get_epoch_time() + request.json()['expires_in'] - 2)
+        self._auth_expires = int(_get_epoch_time() + json_request['expires_in'] - 2)
 
     def _get_request_header(self) -> dict:
         """
         Returns the correct headers for a request.
 
         Returns
         -------
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/contextionary/crud_contextionary.py` & `weaviate-client-3.9.0b0/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/data/crud_data.py` & `weaviate-client-3.9.0b0/weaviate/data/crud_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 DataObject class definition.
 """
+import warnings
 import uuid as uuid_lib
 from typing import Union, Optional, List, Sequence
 from weaviate.connect import Connection
 from weaviate.exceptions import (
     ObjectAlreadyExistsException,
     RequestsConnectionError,
     UnexpectedStatusCodeException
 )
 from weaviate.util import (
     _get_dict_from_object,
     get_vector,
     get_valid_uuid,
     _capitalize_first_letter,
-    deprecation,
 )
 from weaviate.data.references import Reference
+from weaviate.error_msgs import (
+    DATA_DEPRECATION_NEW_V14_CLS_NS_W,
+    DATA_DEPRECATION_OLD_V14_CLS_NS_W
+)
 
 
 class DataObject:
     """
     DataObject class used to manipulate object to/from weaviate.
 
     Attributes
@@ -213,38 +217,15 @@
         ValueError
             If argument contains an invalid value.
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none successful status.
         """
-
-        if not isinstance(class_name, str):
-            raise TypeError("Class must be type str")
-
-        uuid = get_valid_uuid(uuid)
-
-        object_dict = _get_dict_from_object(data_object)
-
-        weaviate_obj = {
-            "id": uuid,
-            "properties": object_dict
-        }
-
-        if vector is not None:
-            weaviate_obj['vector'] = get_vector(vector)
-
-        is_server_version_14 = (self._connection.server_version >= '1.14')
-
-        if is_server_version_14:
-            path = f"/objects/{_capitalize_first_letter(class_name)}/{uuid}"
-        else:
-            weaviate_obj["class"] = _capitalize_first_letter(class_name)
-            path = f"/objects/{uuid}"
-
+        weaviate_obj, path = self._create_object_for_update(data_object, class_name, uuid, vector)
         try:
             response = self._connection.patch(
                 path=path,
                 weaviate_object=weaviate_obj
             )
         except RequestsConnectionError as conn_err:
             raise RequestsConnectionError('Object was not updated.') from conn_err
@@ -321,49 +302,56 @@
         ValueError
             If argument contains an invalid value.
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
         """
+        weaviate_obj, path = self._create_object_for_update(data_object, class_name, uuid, vector)
+        try:
+            response = self._connection.put(
+                path=path,
+                weaviate_object=weaviate_obj
+            )
+        except RequestsConnectionError as conn_err:
+            raise RequestsConnectionError('Object was not replaced.') from conn_err
+        if response.status_code == 200:
+            # Successful update
+            return
+        raise UnexpectedStatusCodeException("Replace object", response)
 
+    def _create_object_for_update(self,
+        data_object: Union[dict, str],
+        class_name: str,
+        uuid: Union[str, uuid_lib.UUID],
+        vector: Optional[Sequence]=None
+        ):
         if not isinstance(class_name, str):
             raise TypeError("Class must be type str")
 
         uuid = get_valid_uuid(uuid)
 
         object_dict = _get_dict_from_object(data_object)
 
         weaviate_obj = {
             "id": uuid,
-            "properties": object_dict
+            "properties": object_dict,
+            "class": _capitalize_first_letter(class_name)
         }
 
         if vector is not None:
             weaviate_obj['vector'] = get_vector(vector)
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if is_server_version_14:
             path = f"/objects/{_capitalize_first_letter(class_name)}/{uuid}"
         else:
-            weaviate_obj["class"] = _capitalize_first_letter(class_name)
             path = f"/objects/{uuid}"
-
-        try:
-            response = self._connection.put(
-                path=path,
-                weaviate_object=weaviate_obj
-            )
-        except RequestsConnectionError as conn_err:
-            raise RequestsConnectionError('Object was not replaced.') from conn_err
-        if response.status_code == 200:
-            # Successful update
-            return
-        raise UnexpectedStatusCodeException("Replace object", response)
+        return weaviate_obj, path
 
     def get_by_id(self,
             uuid: Union[str, uuid_lib.UUID],
             additional_properties: List[str]=None,
             with_vector: bool=False,
             class_name: Optional[str]=None,
         ) -> Optional[dict]:
@@ -473,28 +461,25 @@
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if class_name is None and is_server_version_14 and uuid is not None:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs, please specify the `class_name` argument for this. The non-class "
-                "namespaced APIs (None value for `class_name`) are going to be removed in the "
-                "future versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=DATA_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if class_name is not None and uuid is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. The "
-                    "non-class namespaced APIs calls are going to be made instead (None value for "
-                    "`class_name`). The non-class namespaced APIs are going to be removed in "
-                    "future versions of the Weaviate Server and Weaviate Python Client. "
-                    "Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=DATA_DEPRECATION_OLD_V14_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             if not isinstance(class_name, str):
                 raise TypeError(
                     f"'class_name' must be of type str. Given type: {type(class_name)}"
                 )
 
         params = _get_params(additional_properties, with_vector)
@@ -582,28 +567,25 @@
         """
 
         uuid = get_valid_uuid(uuid)
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if class_name is None and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs, please specify the `class_name` argument for this. The non-class "
-                "namespaced APIs (None value for `class_name`) are going to be removed in the "
-                "future versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=DATA_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. The "
-                    "non-class namespaced APIs calls are going to be made instead (None value for "
-                    "`class_name`). The non-class namespaced APIs are going to be removed in "
-                    "future versions of the Weaviate Server and Weaviate Python Client. "
-                    "Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=DATA_DEPRECATION_OLD_V14_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             if not isinstance(class_name, str):
                 raise TypeError(
                     f"'class_name' must be of type str. Given type: {type(class_name)}"
                 )
 
         if class_name and is_server_version_14:
@@ -673,28 +655,25 @@
         ValueError
             If uuid is not properly formed.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if class_name is None and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs, please specify the `class_name` argument for this. The non-class "
-                "namespaced APIs (None value for `class_name`) are going to be removed in the "
-                "future versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=DATA_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. The "
-                    "non-class namespaced APIs calls are going to be made instead (None value for "
-                    "`class_name`). The non-class namespaced APIs are going to be removed in "
-                    "future versions of the Weaviate Server and Weaviate Python Client. "
-                    "Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=DATA_DEPRECATION_OLD_V14_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             if not isinstance(class_name, str):
                 raise TypeError(
                     f"'class_name' must be of type str. Given type: {type(class_name)}"
                 )
 
         if class_name and is_server_version_14:
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/data/references/crud_references.py` & `weaviate-client-3.9.0b0/weaviate/data/references/crud_references.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """
 Reference class definition.
 """
+import warnings
 from typing import Union, Optional
 from weaviate.connect import Connection
 from weaviate.exceptions import RequestsConnectionError, UnexpectedStatusCodeException
 from weaviate.util import (
     get_valid_uuid,
-    deprecation,
     _capitalize_first_letter,
 )
+from weaviate.error_msgs import (
+    REF_DEPRECATION_NEW_V14_CLS_NS_W,
+    REF_DEPRECATION_OLD_V14_FROM_CLS_NS_W,
+    REF_DEPRECATION_OLD_V14_TO_CLS_NS_W
+)
 
 
 class Reference:
     """
     Reference class used to manipulate references within objects.
     """
 
@@ -141,42 +146,36 @@
         ValueError
             If uuid is not properly formed.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if (from_class_name is None or to_class_name is None) and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs and beacons, please set the `from_class_name` AND `to_class_name` arguments "
-                "for this. The non-class namespaced APIs and beacons (None value for "
-                "`from_class_name` AND `to_class_name`) are going to be removed in future "
-                "versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=REF_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if from_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. "
-                    "The non-class namespaced APIs calls are going to be made instead "
-                    "(None value for `from_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_FROM_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             _validate_string_arguments(
                 argument=from_class_name,
                 argument_name='from_class_name',
             )
         if to_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced beacons. "
-                    "The non-class namespaced beacons are going to be constructed instead "
-                    "(None value for `to_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_TO_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             _validate_string_arguments(
                 argument=to_class_name,
                 argument_name='to_class_name',
             )
 
         # Validate and create Beacon
@@ -338,42 +337,36 @@
         ValueError
             If the parameters are of the wrong value.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if (from_class_name is None or to_class_names is None) and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs and beacons, please set the `from_class_name` AND `to_class_name` arguments "
-                "for this. The non-class namespaced APIs and beacons (None value for "
-                "`from_class_name` AND `to_class_name`) are going to be removed in future "
-                "versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=REF_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if from_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. "
-                    "The non-class namespaced APIs calls are going to be made instead "
-                    "(None value for `from_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_FROM_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             _validate_string_arguments(
                 argument=from_class_name,
                 argument_name='from_class_name',
             )
         if to_class_names is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced beacons. "
-                    "The non-class namespaced beacons are going to be constructed instead "
-                    "(None value for `to_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_TO_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
 
             if not isinstance(to_class_names, list):
                 _validate_string_arguments(
                     argument=to_class_names,
                     argument_name='to_class_names',
                 )
@@ -535,42 +528,36 @@
         ValueError
             If the parameters are of the wrong value.
         """
 
         is_server_version_14 = (self._connection.server_version >= '1.14')
 
         if (from_class_name is None or to_class_name is None) and is_server_version_14:
-            deprecation(
-                "Weaviate Server version >= 1.14.x STRONGLY recommends using class namespaced "
-                "APIs and beacons, please set the `from_class_name` AND `to_class_name` arguments "
-                "for this. The non-class namespaced APIs and beacons (None value for "
-                "`from_class_name` AND `to_class_name`) are going to be removed in future "
-                "versions of the Weaviate Server and Weaviate Python Client."
+            warnings.warn(
+                message=REF_DEPRECATION_NEW_V14_CLS_NS_W,
+                category=DeprecationWarning,
+                stacklevel=1,
             )
         if from_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced APIs. "
-                    "The non-class namespaced APIs calls are going to be made instead "
-                    "(None value for `from_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_FROM_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             _validate_string_arguments(
                 argument=from_class_name,
                 argument_name='from_class_name',
             )
         if to_class_name is not None:
             if not is_server_version_14:
-                deprecation(
-                    "Weaviate Server version < 1.14.x does not support class namespaced beacons. "
-                    "The non-class namespaced beacons are going to be constructed instead "
-                    "(None value for `to_class_name`). The non-class namespaced APIs and "
-                    "beacons are going to be removed in future versions of the Weaviate Server "
-                    "and Weaviate Python Client. Please upgrade your Weaviate Server version."
+                warnings.warn(
+                    message=REF_DEPRECATION_OLD_V14_TO_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
             _validate_string_arguments(
                 argument=to_class_name,
                 argument_name='to_class_name',
             )
 
         # Validate and create Beacon
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/exceptions.py` & `weaviate-client-3.9.0b0/weaviate/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,7 +78,12 @@
     Schema Validation Exception.
     """
 
 class BackupFailedException(WeaviateBaseError):
     """
     Backup Failed Exception.
     """
+
+class EmptyResponseException(WeaviateBaseError):
+    """
+    Occurs when an HTTP request unexpectedly returns an empty response
+    """
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/gql/aggregate.py` & `weaviate-client-3.9.0b0/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/gql/filter.py` & `weaviate-client-3.9.0b0/weaviate/gql/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 GraphQL filters for `Get` and `Aggregate` commands.
 GraphQL abstract class for GraphQL commands to inherit from.
 """
+import warnings
 from json import dumps
 from copy import deepcopy
 from typing import Any, Union
 from abc import ABC, abstractmethod
 from weaviate.connect import Connection
 from weaviate.exceptions import UnexpectedStatusCodeException, RequestsConnectionError
-from weaviate.util import get_vector, deprecation
+from weaviate.util import get_vector
+from weaviate.error_msgs import FILTER_BEACON_V14_CLS_NS_W
 
 class GraphQL(ABC):
     """
     A base abstract class for GraphQL commands, such as Get, Aggregate.
     """
 
     def __init__(self, connection: Connection):
@@ -278,20 +280,18 @@
             raise ValueError("The 'content' argument should contain EITHER `id` OR `beacon`!")
 
         if 'id' in self._content:
             self.obj_id = 'id'
         else:
             self.obj_id = 'beacon'
             if is_server_version_14 and len(self._content['beacon'].strip('/').split('/')) == 4:
-                deprecation(
-                    "Based on the number of '/' in the beacon it seems that the beacon is not "
-                    "class namespaced. Weaviate version >= 1.14.0 STRONGLY recommends using class "
-                    "namespaced beacons. Non-class namespaced beacons will be removed in future "
-                    "versions. Class namespaced beacons look like this: "
-                    "'weaviate://localhost/{CLASS_NAME}/{UUID}'"
+                warnings.warn(
+                    message=FILTER_BEACON_V14_CLS_NS_W,
+                    category=DeprecationWarning,
+                    stacklevel=1,
                 )
 
         _check_type(
             var_name=self.obj_id,
             value=self._content[self.obj_id],
             dtype=str
         )
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/gql/get.py` & `weaviate-client-3.9.0b0/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/gql/query.py` & `weaviate-client-3.9.0b0/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/schema/crud_schema.py` & `weaviate-client-3.9.0b0/weaviate/schema/crud_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         weaviate.SchemaValidationException
             If the 'schema_class' could not be validated against the standard format.
         """
 
         loaded_schema_class = _get_dict_from_object(schema_class)
         # validate the class before loading
         check_class(loaded_schema_class)
-        self._create_class_with_premitives(loaded_schema_class)
+        self._create_class_with_primitives(loaded_schema_class)
         self._create_complex_properties_from_class(loaded_schema_class)
 
     def delete_class(self, class_name: str) -> None:
         """
         Delete a schema class from weaviate. This deletes all associated data.
 
         Parameters
@@ -598,15 +598,15 @@
         if shard_name is None:
             return to_return
         return to_return[0]
 
 
     def _create_complex_properties_from_class(self, schema_class: dict) -> None:
         """
-        Add crossreferences to already existing class.
+        Add cross-references to already existing class.
 
         Parameters
         ----------
         schema_class : dict
             Description of the class that should be added.
 
         Raises
@@ -647,33 +647,33 @@
                     'Property may not have been created properly.'
                 ) from conn_err
             if response.status_code != 200:
                 raise UnexpectedStatusCodeException("Add properties to classes", response)
 
     def _create_complex_properties_from_classes(self, schema_classes_list: list) -> None:
         """
-        Add crossreferences to already existing classes.
+        Add cross-references to already existing classes.
 
         Parameters
         ----------
         schema_classes_list : list
             A list of classes as they are found in a schema json description.
         """
 
         for schema_class in schema_classes_list:
             self._create_complex_properties_from_class(schema_class)
 
-    def _create_class_with_premitives(self, weaviate_class: dict) -> None:
+    def _create_class_with_primitives(self, weaviate_class: dict) -> None:
         """
         Create class with only primitives.
 
         Parameters
         ----------
         weaviate_class : dict
-            A single weaviate formated class
+            A single weaviate formatted class
 
         Raises
         ------
         requests.ConnectionError
             If the network connection to weaviate fails.
         weaviate.UnexpectedStatusCodeException
             If weaviate reports a none OK status.
@@ -716,15 +716,15 @@
         Parameters
         ----------
         schema_classes_list : list
             A list of classes as they are found in a schema json description.
         """
 
         for weaviate_class in schema_classes_list:
-            self._create_class_with_premitives(weaviate_class)
+            self._create_class_with_primitives(weaviate_class)
 
 
 def _property_is_primitive(data_type_list: list) -> bool:
     """
     Check if the property is primitive.
 
     Parameters
@@ -747,15 +747,15 @@
 def _get_primitive_properties(properties_list: list) -> list:
     """
     Filter the list of properties for only primitive properties.
 
     Parameters
     ----------
     properties_list : list
-        A list of properties to exctract the primitive properties.
+        A list of properties to extract the primitive properties.
 
     Returns
     -------
     list
         A list of properties containing only primitives.
     """
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/schema/properties/crud_properties.py` & `weaviate-client-3.9.0b0/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/schema/validate_schema.py` & `weaviate-client-3.9.0b0/weaviate/schema/validate_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate/util.py` & `weaviate-client-3.9.0b0/weaviate/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Helper functions!
 """
-import os
-import json
 import base64
-import warnings
+import json
+import os
 import uuid as uuid_lib
-from typing import Union, Sequence, Tuple, Any, Optional
-from numbers import Real
 from io import BufferedReader
-import validators
+from numbers import Real
+from typing import Union, Sequence, Tuple, Any, Optional
+
 import requests
+import validators
 
 from weaviate.exceptions import SchemaValidationException
 
 
 def image_encoder_b64(image_or_image_path: Union[str, BufferedReader]) -> str:
     """
     Encode a image in a Weaviate understandable format from a binary read file or by providing
@@ -455,19 +455,18 @@
     TypeError
         If arguments are of a wrong data type.
     ValueError
         If 'timeout_config' is not a tuple of 2.
     ValueError
         If 'timeout_config' is/contains negative number/s.
     """
-
     if isinstance(timeout_config, Real) and not isinstance(timeout_config, bool):
         if timeout_config <= 0.0:
             raise ValueError("'timeout_config' cannot be non-positive number/s!")
-        return (timeout_config, timeout_config)
+        return timeout_config, timeout_config
 
     if not isinstance(timeout_config, tuple):
         raise TypeError("'timeout_config' should be a (or tuple of) positive real number/s!")
     if len(timeout_config) != 2:
         raise ValueError("'timeout_config' must be of length 2!")
     if not (isinstance(timeout_config[0], Real) and isinstance(timeout_config[1], Real)) or \
             (isinstance(timeout_config[0], bool) and isinstance(timeout_config[1], bool)):
@@ -514,27 +513,14 @@
     """
 
     if len(string) == 1:
         return string.capitalize()
     return string[0].capitalize() + string[1:]
 
 
-def deprecation(message: str) -> None:
-    """
-    Show deprecation message.
-
-    Parameters
-    ----------
-    message : str
-        The deprecation message to show.
-    """
-
-    warnings.warn(message, DeprecationWarning, stacklevel=2)
-
-
 def check_batch_result(results: dict) -> None:
     """
     Check batch results for errors.
 
     Parameters
     ----------
     results : dict
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate/wcs/crud_wcs.py` & `weaviate-client-3.9.0b0/weaviate/wcs/crud_wcs.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-3.9.0.dev2/weaviate_client.egg-info/PKG-INFO` & `weaviate-client-3.9.0b0/weaviate_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 3.9.0.dev2
+Version: 3.9.0b0
 Summary: A python native weaviate client
 Author: SeMI Technologies
 Author-email: hello@semi.technology
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 
 Weaviate python client
 ======================
 .. image:: https://raw.githubusercontent.com/semi-technologies/weaviate/19de0956c69b66c5552447e84d016f4fe29d12c9/docs/assets/weaviate-logo.png
     :width: 180
```

### Comparing `weaviate-client-3.9.0.dev2/weaviate_client.egg-info/SOURCES.txt` & `weaviate-client-3.9.0b0/weaviate_client.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 test/test_client.py
 test/test_exceptions.py
 test/test_util.py
 test/test_version.py
 weaviate/__init__.py
 weaviate/auth.py
 weaviate/client.py
+weaviate/error_msgs.py
 weaviate/exceptions.py
 weaviate/util.py
 weaviate/version.py
 weaviate/backup/__init__.py
 weaviate/backup/backup.py
 weaviate/batch/__init__.py
 weaviate/batch/crud_batch.py
 weaviate/batch/requests.py
 weaviate/classification/__init__.py
 weaviate/classification/classification.py
 weaviate/classification/config_builder.py
+weaviate/cluster/__init__.py
+weaviate/cluster/cluster.py
 weaviate/connect/__init__.py
 weaviate/connect/connection.py
 weaviate/contextionary/__init__.py
 weaviate/contextionary/crud_contextionary.py
 weaviate/data/__init__.py
 weaviate/data/crud_data.py
 weaviate/data/references/__init__.py
@@ -36,13 +39,12 @@
 weaviate/schema/__init__.py
 weaviate/schema/crud_schema.py
 weaviate/schema/validate_schema.py
 weaviate/schema/properties/__init__.py
 weaviate/schema/properties/crud_properties.py
 weaviate/wcs/__init__.py
 weaviate/wcs/crud_wcs.py
-weaviate_client.egg-info/LICENSE.md
 weaviate_client.egg-info/PKG-INFO
 weaviate_client.egg-info/SOURCES.txt
 weaviate_client.egg-info/dependency_links.txt
 weaviate_client.egg-info/requires.txt
 weaviate_client.egg-info/top_level.txt
```

