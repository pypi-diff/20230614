# Comparing `tmp/anycluster-2.3.2.tar.gz` & `tmp/anycluster-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.3.2.tar", last modified: Tue Jun 13 06:43:49 2023, max compression
+gzip compressed data, was "anycluster-2.3.3.tar", last modified: Wed Jun 14 09:36:24 2023, max compression
```

## Comparing `anycluster-2.3.2.tar` & `anycluster-2.3.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.2/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.2/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-13 06:43:49.706701 anycluster-2.3.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.2/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.2/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3536 2023-06-13 06:05:24.000000 anycluster-2.3.2/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    38198 2023-06-13 05:56:27.000000 anycluster-2.3.2/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.2/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.2/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.2/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.2/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     4685 2023-06-13 06:41:38.000000 anycluster-2.3.2/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.2/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     8087 2023-06-12 13:31:27.000000 anycluster-2.3.2/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.2/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5293 2023-06-13 06:41:37.000000 anycluster-2.3.2/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.2/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.3.2/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.2/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.2/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10055 2023-06-12 13:28:29.000000 anycluster-2.3.2/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.2/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.2/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.698701 anycluster-2.3.2/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.2/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.706701 anycluster-2.3.2/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.2/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.2/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    16331 2023-06-12 12:46:45.000000 anycluster-2.3.2/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.2/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.2/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.2/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.2/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    27459 2023-06-12 12:46:42.000000 anycluster-2.3.2/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.2/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-13 06:43:49.702701 anycluster-2.3.2/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-13 06:43:49.000000 anycluster-2.3.2/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-13 06:43:49.706701 anycluster-2.3.2/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-13 06:43:29.000000 anycluster-2.3.2/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.664059 anycluster-2.3.3/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.3/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.3/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-14 09:36:24.660060 anycluster-2.3.3/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.3/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.3/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3536 2023-06-13 06:05:24.000000 anycluster-2.3.3/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    38351 2023-06-13 06:57:30.000000 anycluster-2.3.3/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.3/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.3/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.3/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.3/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     4685 2023-06-13 06:41:38.000000 anycluster-2.3.3/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.3/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     8087 2023-06-12 13:31:27.000000 anycluster-2.3.3/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.3/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5293 2023-06-13 06:41:37.000000 anycluster-2.3.3/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.3.3/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.3/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.3/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10055 2023-06-12 13:28:29.000000 anycluster-2.3.3/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.3/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.3/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.3/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.3/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    16491 2023-06-13 07:05:25.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.3/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.3/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.3/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.3/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    28275 2023-06-13 07:05:23.000000 anycluster-2.3.3/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.3/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-14 09:36:24.664059 anycluster-2.3.3/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-14 09:36:13.000000 anycluster-2.3.3/setup.py
```

### Comparing `anycluster-2.3.2/LICENSE` & `anycluster-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/PKG-INFO` & `anycluster-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.2
+Version: 2.3.3
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.2/README.md` & `anycluster-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/ClusterCache.py` & `anycluster-2.3.3/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/FilterComposer.py` & `anycluster-2.3.3/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/MapClusterer.py` & `anycluster-2.3.3/anycluster/MapClusterer.py`

 * *Files 1% similar despite different names*

```diff
@@ -795,15 +795,19 @@
         geometries_for_counting = self.get_geometries_for_counting(geojson, geometry_type, zoom)
 
         unmodulated_count = self.query_map_content_count(geometries_for_counting, filters)
         result['count'] = unmodulated_count
 
         for modulation_name, modulation_filters in modulations.items():
 
-            combined_filters = filters + modulation_filters['filters']
+            if 'filters' in modulation_filters:
+                combined_filters = filters + modulation_filters['filters']
+            else:
+                combined_filters = filters + [modulation_filters]
+                
             modulated_count = self.query_map_content_count(geometries_for_counting, combined_filters)
             result['modulations'][modulation_name] = {
                 'count': modulated_count
             }
 
         return result
```

### Comparing `anycluster-2.3.2/anycluster/MapTools.py` & `anycluster-2.3.3/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/json_schemas.py` & `anycluster-2.3.3/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/serializers.py` & `anycluster-2.3.3/anycluster/api/serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.3.3/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/tests/test_serializers.py` & `anycluster-2.3.3/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/tests/test_views.py` & `anycluster-2.3.3/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/urls.py` & `anycluster-2.3.3/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/api/views.py` & `anycluster-2.3.3/anycluster/api/views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/clusters.py` & `anycluster-2.3.3/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/definitions.py` & `anycluster-2.3.3/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/globalmaptiles.py` & `anycluster-2.3.3/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/10.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/100.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/1000.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/10000.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/5.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/50.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.3.3/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.3.3/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 12 12:46:42 2023 UTC, .py size: 27459 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b213 8764 436b 0000  U..........dCk..
+00000000: 550d 0d0a 0000 0000 3315 8864 736e 0000  U.......3..dsn..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -55,967 +55,977 @@
 00000360: 641b 641c 8400 5a10 641d 641e 8400 5a11  d.d...Z.d.d...Z.
 00000370: 641f 6420 8400 5a12 6421 6422 8400 5a13  d.d ..Z.d!d"..Z.
 00000380: 6423 6424 8400 5a14 6425 6426 8400 5a15  d#d$..Z.d%d&..Z.
 00000390: 6427 6428 8400 5a16 6429 642a 8400 5a17  d'd(..Z.d)d*..Z.
 000003a0: 642b 642c 8400 5a18 642d 5300 292e da10  d+d,..Z.d-S.)...
 000003b0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
 000003c0: 6301 0000 0000 0000 0000 0000 0008 0000  c...............
-000003d0: 0009 0000 0043 0000 0073 a000 0000 7400  .....C...s....t.
-000003e0: 4400 5d96 7d01 7401 4400 5d8c 7d02 7c00  D.].}.t.D.].}.|.
-000003f0: a002 a100 7d03 7c03 4400 5d7a 7d04 7403  ....}.|.D.]z}.t.
+000003d0: 0009 0000 0043 0000 0073 8e00 0000 7400  .....C...s....t.
+000003e0: 4400 5d84 7d01 7401 4400 5d7a 7d02 7c00  D.].}.t.D.]z}.|.
+000003f0: a002 a100 7d03 7c03 4400 5d68 7d04 7403  ....}.|.D.]h}.t.
 00000400: 7d05 7c00 a004 7c02 7c05 7c01 7c04 a104  }.|...|.|.|.|...
 00000410: 7d06 7405 7c06 8301 7d07 7c00 a006 7c07  }.t.|...}.|...|.
 00000420: 6a07 7c06 a102 0100 7c00 a006 7c07 6a08  j.|.....|...|.j.
 00000430: 6401 a102 0100 7c00 a006 7c07 6a09 6402  d.....|...|.j.d.
 00000440: a102 0100 7c00 a006 7c07 6a0a 6403 a102  ....|...|.j.d...
 00000450: 0100 7c00 a006 7c07 6a0b 6a0c 740d a102  ..|...|.j.j.t...
-00000460: 0100 7c00 a00e 740f 7c07 6a10 7411 8302  ..|...t.|.j.t...
-00000470: a101 0100 711c 710c 7104 6400 5300 2904  ....q.q.q.d.S.).
-00000480: 4eda 0670 7562 6c69 63e9 110f 0000 721a  N..public.....r.
-00000490: 0000 0029 1272 0b00 0000 720e 0000 00da  ...).r....r.....
-000004a0: 1067 6574 5f74 6573 745f 6669 6c74 6572  .get_test_filter
-000004b0: 73da 0f54 4553 545f 5a4f 4f4d 5f4c 4556  s..TEST_ZOOM_LEV
-000004c0: 454c da11 6765 745f 636c 7573 7465 725f  EL..get_cluster_
-000004d0: 6361 6368 6572 0900 0000 da0b 6173 7365  cacher......asse
-000004e0: 7274 4571 7561 6cda 0d63 6c75 7374 6572  rtEqual..cluster
-000004f0: 5f63 6163 6865 da0b 7363 6865 6d61 5f6e  _cache..schema_n
-00000500: 616d 65da 0764 625f 7372 6964 da09 6772  ame..db_srid..gr
-00000510: 6964 5f73 697a 655a 086d 6170 746f 6f6c  id_sizeZ.maptool
-00000520: 73da 095f 5f63 6c61 7373 5f5f 720a 0000  s..__class__r...
-00000530: 00da 0a61 7373 6572 7454 7275 65da 0a69  ...assertTrue..i
-00000540: 7369 6e73 7461 6e63 655a 0f76 616c 6964  sinstanceZ.valid
-00000550: 5f6f 7065 7261 746f 7273 da04 6c69 7374  _operators..list
-00000560: 2908 da04 7365 6c66 da0b 636c 7573 7465  )...self..cluste
-00000570: 7274 7970 65da 0d67 656f 6d65 7472 795f  rtype..geometry_
-00000580: 7479 7065 da0c 6669 6c74 6572 5f6c 6973  type..filter_lis
-00000590: 7473 da07 6669 6c74 6572 73da 047a 6f6f  ts..filters..zoo
-000005a0: 6d72 2200 0000 da0d 6d61 705f 636c 7573  mr".....map_clus
-000005b0: 7465 7265 72a9 0072 3100 0000 fa46 2f68  terer..r1....F/h
-000005c0: 6f6d 652f 746f 6d2f 616e 7963 6c75 7374  ome/tom/anyclust
-000005d0: 6572 2f64 656d 6f2f 646a 616e 676f 2f61  er/demo/django/a
-000005e0: 6e79 636c 7573 7465 722f 7465 7374 732f  nycluster/tests/
-000005f0: 7465 7374 5f4d 6170 436c 7573 7465 7265  test_MapClustere
-00000600: 722e 7079 da09 7465 7374 5f69 6e69 7417  r.py..test_init.
-00000610: 0000 0073 1a00 0000 0002 0802 0802 0801  ...s............
-00000620: 0802 0401 1002 0802 0e01 0e01 0e01 0e01  ................
-00000630: 1001 7a1a 5465 7374 4d61 7043 6c75 7374  ..z.TestMapClust
-00000640: 6572 6572 2e74 6573 745f 696e 6974 6301  erer.test_initc.
-00000650: 0000 0000 0000 0000 0000 0009 0000 0009  ................
-00000660: 0000 0043 0000 0073 5a00 0000 7400 4400  ...C...sZ...t.D.
-00000670: 5d50 7d01 7401 4400 5d46 7d02 7c00 a002  ]P}.t.D.]F}.|...
-00000680: a100 7d03 7c03 4400 5d34 7d04 6401 7d05  ..}.|.D.]4}.d.}.
-00000690: 7c00 a003 7c02 7c05 7c01 7c04 a104 7d06  |...|.|.|.|...}.
-000006a0: 7404 7c06 8301 7d07 7c07 a005 a100 7d08  t.|...}.|.....}.
-000006b0: 7c00 a006 7c08 6402 a102 0100 711c 710c  |...|.d.....q.q.
-000006c0: 7104 6400 5300 2903 4ee9 0100 0000 721d  q.d.S.).N.....r.
-000006d0: 0000 0029 0772 0b00 0000 720e 0000 0072  ...).r....r....r
-000006e0: 1e00 0000 7220 0000 0072 0900 0000 5a11  ....r ...r....Z.
-000006f0: 6765 745f 6461 7461 6261 7365 5f73 7269  get_database_sri
-00000700: 6472 2100 0000 2909 722a 0000 0072 2b00  dr!...).r*...r+.
-00000710: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00000720: 0072 2f00 0000 7222 0000 0072 3000 0000  .r/...r"...r0...
-00000730: 7224 0000 0072 3100 0000 7231 0000 0072  r$...r1...r1...r
-00000740: 3200 0000 da16 7465 7374 5f67 6574 5f64  2.....test_get_d
-00000750: 6174 6162 6173 655f 7372 6964 2d00 0000  atabase_srid-...
-00000760: 7312 0000 0000 0208 0208 0208 0108 0204  s...............
-00000770: 0110 0208 0208 017a 2754 6573 744d 6170  .......z'TestMap
-00000780: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
-00000790: 6574 5f64 6174 6162 6173 655f 7372 6964  et_database_srid
-000007a0: 6301 0000 0000 0000 0000 0000 000c 0000  c...............
-000007b0: 000a 0000 0043 0000 0073 d800 0000 7400  .....C...s....t.
-000007c0: 4400 5dce 7d01 7401 4400 5dc4 7d02 7c00  D.].}.t.D.].}.|.
-000007d0: a002 a100 7d03 7c03 4400 5db2 7d04 7403  ....}.|.D.].}.t.
-000007e0: 7d05 7c00 a004 7c02 7c05 7c01 7c04 a104  }.|...|.|.|.|...
-000007f0: 7d06 7405 7c06 8301 7d07 7406 7407 6602  }.t.|...}.t.t.f.
-00000800: 4400 5d46 7d08 7c07 a008 7c08 a101 7d09  D.]F}.|...|...}.
-00000810: 7c00 a009 740a 7c09 8301 6401 a102 0100  |...t.|...d.....
-00000820: 7c09 4400 5d22 7d0a 7c00 a00b 740c 7c0a  |.D.]"}.|...t.|.
-00000830: 740d 8302 a101 0100 7c00 a009 7c0a 6a0e  t.......|...|.j.
-00000840: 6402 a102 0100 7166 7144 7c07 a008 740f  d.....qfqD|...t.
-00000850: a101 7d0b 7c00 a009 740a 7c0b 8301 6403  ..}.|...t.|...d.
-00000860: a102 0100 7c0b 4400 5d22 7d0a 7c00 a00b  ....|.D.]"}.|...
-00000870: 740c 7c0a 740d 8302 a101 0100 7c00 a009  t.|.t.......|...
-00000880: 7c0a 6a0e 6402 a102 0100 71aa 711c 710c  |.j.d.....q.q.q.
-00000890: 7104 6400 5300 2904 4e72 3400 0000 721d  q.d.S.).Nr4...r.
-000008a0: 0000 00e9 0200 0000 2910 720b 0000 0072  ........).r....r
-000008b0: 0e00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-000008c0: 0000 0072 0900 0000 7211 0000 0072 1200  ...r....r....r..
-000008d0: 0000 5a1f 636f 6e76 6572 745f 6765 6f6a  ..Z.convert_geoj
-000008e0: 736f 6e5f 6665 6174 7572 655f 746f 5f67  son_feature_to_g
-000008f0: 656f 7372 2100 0000 da03 6c65 6e72 2700  eosr!.....lenr'.
-00000900: 0000 7228 0000 0072 0600 0000 da04 7372  ..r(...r......sr
-00000910: 6964 7213 0000 0029 0c72 2a00 0000 722b  idr....).r*...r+
-00000920: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00000930: 0000 722f 0000 0072 2200 0000 7230 0000  ..r/...r"...r0..
-00000940: 00da 0767 656f 6a73 6f6e da0f 6765 6f73  ...geojson..geos
-00000950: 5f67 656f 6d65 7472 6965 73da 0d67 656f  _geometries..geo
-00000960: 735f 6765 6f6d 6574 7279 5a12 6d70 5f67  s_geometryZ.mp_g
-00000970: 656f 735f 6765 6f6d 6574 7269 6573 7231  eos_geometriesr1
-00000980: 0000 0072 3100 0000 7232 0000 00da 2c74  ...r1...r2....,t
-00000990: 6573 745f 636f 6e76 6572 745f 6765 6f6a  est_convert_geoj
-000009a0: 736f 6e5f 6665 6174 7572 655f 746f 5f67  son_feature_to_g
-000009b0: 656f 735f 706f 6c79 676f 6e3f 0000 0073  eos_polygon?...s
-000009c0: 2c00 0000 0002 0801 0802 0801 0802 0401  ,...............
-000009d0: 1002 0802 0c02 0401 02ff 0403 1002 0801  ................
-000009e0: 1001 1202 0401 02ff 0403 1002 0801 1001  ................
-000009f0: 7a3d 5465 7374 4d61 7043 6c75 7374 6572  z=TestMapCluster
-00000a00: 6572 2e74 6573 745f 636f 6e76 6572 745f  er.test_convert_
-00000a10: 6765 6f6a 736f 6e5f 6665 6174 7572 655f  geojson_feature_
-00000a20: 746f 5f67 656f 735f 706f 6c79 676f 6e63  to_geos_polygonc
-00000a30: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
-00000a40: 0a00 0000 4300 0000 737a 0000 0074 0044  ....C...sz...t.D
-00000a50: 005d 707d 0174 0144 005d 667d 027c 00a0  .]p}.t.D.]f}.|..
-00000a60: 02a1 007d 037c 0344 005d 547d 0474 037d  ...}.|.D.]T}.t.}
-00000a70: 057c 00a0 047c 027c 057c 017c 04a1 047d  .|...|.|.|.|...}
-00000a80: 0674 057c 0683 017d 0774 0674 0774 0866  .t.|...}.t.t.t.f
-00000a90: 0344 005d 287d 087c 07a0 097c 08a1 017d  .D.](}.|...|...}
-00000aa0: 097c 0944 005d 147d 0a7c 00a0 0a74 0b7c  .|.D.].}.|...t.|
-00000ab0: 0a74 0c83 02a1 0101 0071 5871 4671 1c71  .t.......qXqFq.q
-00000ac0: 0c71 0464 0053 00a9 014e 290d 720b 0000  .q.d.S...N).r...
-00000ad0: 0072 0e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000ae0: 7220 0000 0072 0900 0000 7211 0000 0072  r ...r....r....r
-00000af0: 1200 0000 7213 0000 00da 1763 6f6e 7665  ....r......conve
-00000b00: 7274 5f67 656f 6a73 6f6e 5f74 6f5f 6765  rt_geojson_to_ge
-00000b10: 6f73 7227 0000 0072 2800 0000 7206 0000  osr'...r(...r...
-00000b20: 0029 0b72 2a00 0000 722b 0000 0072 2c00  .).r*...r+...r,.
-00000b30: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
-00000b40: 0072 2200 0000 7230 0000 0072 3900 0000  .r"...r0...r9...
-00000b50: 723a 0000 0072 3b00 0000 7231 0000 0072  r:...r;...r1...r
-00000b60: 3100 0000 7232 0000 00da 2474 6573 745f  1...r2....$test_
-00000b70: 636f 6e76 6572 745f 6765 6f6a 736f 6e5f  convert_geojson_
-00000b80: 746f 5f67 656f 735f 6665 6174 7572 6561  to_geos_featurea
-00000b90: 0000 0073 1a00 0000 0002 0801 0802 0801  ...s............
-00000ba0: 0802 0401 1002 0802 0e02 0401 02ff 0403  ................
-00000bb0: 0801 7a35 5465 7374 4d61 7043 6c75 7374  ..z5TestMapClust
-00000bc0: 6572 6572 2e74 6573 745f 636f 6e76 6572  erer.test_conver
-00000bd0: 745f 6765 6f6a 736f 6e5f 746f 5f67 656f  t_geojson_to_geo
-00000be0: 735f 6665 6174 7572 6563 0100 0000 0000  s_featurec......
-00000bf0: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
-00000c00: 0000 736a 0000 0074 0044 005d 607d 0174  ..sj...t.D.]`}.t
-00000c10: 0144 005d 567d 027c 00a0 02a1 007d 037c  .D.]V}.|.....}.|
-00000c20: 0344 005d 447d 0474 037d 057c 00a0 047c  .D.]D}.t.}.|...|
-00000c30: 027c 057c 017c 04a1 047d 0674 057c 0683  .|.|.|...}.t.|..
-00000c40: 017d 077c 07a0 0674 07a1 017d 087c 0844  .}.|...t...}.|.D
-00000c50: 005d 147d 097c 00a0 0874 097c 0974 0a83  .].}.|...t.|.t..
-00000c60: 02a1 0101 0071 4a71 1c71 0c71 0464 0053  .....qJq.q.q.d.S
-00000c70: 0072 3d00 0000 290b 720b 0000 0072 0e00  .r=...).r....r..
-00000c80: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000c90: 0072 0900 0000 723e 0000 0072 1400 0000  .r....r>...r....
-00000ca0: 7227 0000 0072 2800 0000 7206 0000 0029  r'...r(...r....)
-00000cb0: 0a72 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000cc0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00000cd0: 2200 0000 7230 0000 0072 3a00 0000 723b  "...r0...r:...r;
-00000ce0: 0000 0072 3100 0000 7231 0000 0072 3200  ...r1...r1...r2.
-00000cf0: 0000 da2e 7465 7374 5f63 6f6e 7665 7274  ....test_convert
-00000d00: 5f67 656f 6a73 6f6e 5f74 6f5f 6765 6f73  _geojson_to_geos
-00000d10: 5f66 6561 7475 7265 636f 6c6c 6563 7469  _featurecollecti
-00000d20: 6f6e 7700 0000 7318 0000 0000 0208 0108  onw...s.........
-00000d30: 0208 0108 0204 0110 0208 0104 0102 ff04  ................
-00000d40: 0308 017a 3f54 6573 744d 6170 436c 7573  ...z?TestMapClus
-00000d50: 7465 7265 722e 7465 7374 5f63 6f6e 7665  terer.test_conve
-00000d60: 7274 5f67 656f 6a73 6f6e 5f74 6f5f 6765  rt_geojson_to_ge
-00000d70: 6f73 5f66 6561 7475 7265 636f 6c6c 6563  os_featurecollec
-00000d80: 7469 6f6e 6301 0000 0000 0000 0000 0000  tionc...........
-00000d90: 000b 0000 000a 0000 0043 0000 0073 7e00  .........C...s~.
-00000da0: 0000 7400 4400 5d74 7d01 7401 4400 5d6a  ..t.D.]t}.t.D.]j
-00000db0: 7d02 7c00 a002 a100 7d03 7c03 4400 5d58  }.|.....}.|.D.]X
-00000dc0: 7d04 7403 7d05 7c00 a004 7c02 7c05 7c01  }.t.}.|...|.|.|.
-00000dd0: 7c04 a104 7d06 7405 7c06 8301 7d07 7406  |...}.t.|...}.t.
-00000de0: 7407 7408 6603 4400 5d2c 7d08 7c07 a009  t.t.f.D.],}.|...
-00000df0: 7c08 7c02 7c05 a103 7d09 7c09 4400 5d14  |.|.|...}.|.D.].
-00000e00: 7d0a 7c00 a00a 740b 7c0a 740c 8302 a101  }.|...t.|.t.....
-00000e10: 0100 715c 7146 711c 710c 7104 6400 5300  ..q\qFq.q.q.d.S.
-00000e20: 723d 0000 0029 0d72 0b00 0000 720e 0000  r=...).r....r...
-00000e30: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00000e40: 7209 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00000e50: 1300 0000 da16 6765 745f 636c 7573 7465  ......get_cluste
-00000e60: 725f 6765 6f6d 6574 7269 6573 7227 0000  r_geometriesr'..
-00000e70: 0072 2800 0000 7206 0000 0029 0b72 2a00  .r(...r....).r*.
-00000e80: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00000e90: 0072 2e00 0000 722f 0000 0072 2200 0000  .r....r/...r"...
-00000ea0: 7230 0000 0072 3900 0000 da12 636c 7573  r0...r9.....clus
-00000eb0: 7465 725f 6765 6f6d 6574 7269 6573 723b  ter_geometriesr;
-00000ec0: 0000 0072 3100 0000 7231 0000 0072 3200  ...r1...r1...r2.
-00000ed0: 0000 da24 7465 7374 5f67 6574 5f63 6c75  ...$test_get_clu
-00000ee0: 7374 6572 5f67 656f 6d65 7472 6965 735f  ster_geometries_
-00000ef0: 7669 6577 706f 7274 8a00 0000 731e 0000  viewport....s...
-00000f00: 0000 0208 0108 0308 0108 0204 0110 0208  ................
-00000f10: 020e 0204 0102 0002 0002 ff04 0308 017a  ...............z
-00000f20: 3554 6573 744d 6170 436c 7573 7465 7265  5TestMapClustere
-00000f30: 722e 7465 7374 5f67 6574 5f63 6c75 7374  r.test_get_clust
-00000f40: 6572 5f67 656f 6d65 7472 6965 735f 7669  er_geometries_vi
-00000f50: 6577 706f 7274 6301 0000 0000 0000 0000  ewportc.........
-00000f60: 0000 000d 0000 0009 0000 0043 0000 0073  ...........C...s
-00000f70: d600 0000 7400 4400 5dcc 7d01 7c00 a001  ....t.D.].}.|...
-00000f80: a100 7d02 7c02 4400 5dba 7d03 7402 7d04  ..}.|.D.].}.t.}.
-00000f90: 7c00 a003 7404 7c04 7c01 7c03 a104 7d05  |...t.|.|.|...}.
-00000fa0: 7405 7c05 8301 7d06 7406 7d07 7c06 a007  t.|...}.t.}.|...
-00000fb0: 7c07 7404 7c04 a103 7d08 7406 6401 1900  |.t.|...}.t.d...
-00000fc0: a008 a100 7d09 7409 740a a00b 7c09 a101  ....}.t.t...|...
-00000fd0: 6402 6403 8d02 7d0a 740c 740d 7c0a 6a0e  d.d...}.t.t.|.j.
-00000fe0: 8301 740d 6404 8301 8302 7d0b 7c0a a00f  ..t.d.....}.|...
-00000ff0: 7c0b a101 0100 7c00 a010 7c0a 6a11 7c08  |.....|...|.j.|.
-00001000: 6405 1900 6a11 a102 0100 7412 7406 7413  d...j.....t.t.t.
-00001010: 6603 4400 5d2c 7d07 7c06 a007 7c07 7404  f.D.],}.|...|.t.
-00001020: 7c04 a103 7d08 7c08 4400 5d14 7d0c 7c00  |...}.|.D.].}.|.
-00001030: a014 7415 7c0c 7409 8302 a101 0100 71b6  ..t.|.t.......q.
-00001040: 71a0 7114 7104 6400 5300 2906 4eda 0867  q.q.q.d.S.).N..g
-00001050: 656f 6d65 7472 79e9 e610 0000 2901 7238  eometry.....).r8
-00001060: 0000 0072 1d00 0000 7201 0000 0029 1672  ...r....r....).r
-00001070: 0b00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-00001080: 0000 0072 0d00 0000 7209 0000 0072 1200  ...r....r....r..
-00001090: 0000 7241 0000 00da 0463 6f70 7972 0600  ..rA.....copyr..
-000010a0: 0000 da04 6a73 6f6e da05 6475 6d70 7372  ....json..dumpsr
-000010b0: 0800 0000 7207 0000 0072 3800 0000 da09  ....r....r8.....
-000010c0: 7472 616e 7366 6f72 6d72 2100 0000 7239  transformr!...r9
-000010d0: 0000 0072 1100 0000 7213 0000 0072 2700  ...r....r....r'.
-000010e0: 0000 7228 0000 0029 0d72 2a00 0000 722b  ..r(...).r*...r+
-000010f0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-00001100: 0000 7222 0000 0072 3000 0000 7239 0000  ..r"...r0...r9..
-00001110: 0072 4200 0000 5a10 6d61 7463 6869 6e67  .rB...Z.matching
-00001120: 5f67 656f 6a73 6f6e 5a0c 696e 6974 6961  _geojsonZ.initia
-00001130: 6c5f 6765 6f73 da02 6374 723b 0000 0072  l_geos..ctr;...r
-00001140: 3100 0000 7231 0000 0072 3200 0000 da20  1...r1...r2.... 
-00001150: 7465 7374 5f67 6574 5f63 6c75 7374 6572  test_get_cluster
-00001160: 5f67 656f 6d65 7472 6965 735f 6172 6561  _geometries_area
-00001170: a100 0000 7344 0000 0000 0208 0308 0108  ....sD..........
-00001180: 0204 0110 0208 0204 0204 0102 0002 0002  ................
-00001190: ff04 030c 0102 0108 0002 ff06 0204 0104  ................
-000011a0: ff02 0106 ff04 020a 0208 0108 ff04 030e  ................
-000011b0: 0204 0102 0002 0002 ff04 0308 017a 3154  .............z1T
-000011c0: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
-000011d0: 7465 7374 5f67 6574 5f63 6c75 7374 6572  test_get_cluster
-000011e0: 5f67 656f 6d65 7472 6965 735f 6172 6561  _geometries_area
-000011f0: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
-00001200: 0009 0000 0043 0000 0073 7a00 0000 7400  .....C...sz...t.
-00001210: 7d01 7401 4400 5d6c 7d02 7402 7403 7404  }.t.D.]l}.t.t.t.
-00001220: 6603 4400 5d5c 7d03 7c00 a005 a100 7d04  f.D.]\}.|.....}.
-00001230: 7c04 4400 5d4a 7d05 7c00 a006 7c02 7c01  |.D.]J}.|...|.|.
-00001240: 7407 7c05 a104 7d06 7408 7c06 8301 7d07  t.|...}.t.|...}.
-00001250: 6700 7d05 7c07 a009 7c03 7c02 7c01 7c05  g.}.|...|.|.|.|.
-00001260: a104 7d08 7c02 740a 6b02 7226 7c00 a00b  ..}.|.t.k.r&|...
-00001270: 740c 7c08 8301 6401 6b04 a101 0100 7126  t.|...d.k.....q&
-00001280: 7116 7108 6400 5300 a902 4e72 0100 0000  q.q.d.S...Nr....
-00001290: 290d 721f 0000 0072 0e00 0000 7211 0000  ).r....r....r...
-000012a0: 0072 1200 0000 7213 0000 0072 1e00 0000  .r....r....r....
-000012b0: 7220 0000 0072 0f00 0000 7209 0000 00da  r ...r....r.....
-000012c0: 0e6b 6d65 616e 735f 636c 7573 7465 7272  .kmeans_clusterr
-000012d0: 0c00 0000 7227 0000 0072 3700 0000 2909  ....r'...r7...).
-000012e0: 722a 0000 0072 2f00 0000 722c 0000 0072  r*...r/...r,...r
-000012f0: 3900 0000 722d 0000 0072 2e00 0000 7222  9...r-...r....r"
-00001300: 0000 0072 3000 0000 da07 6d61 726b 6572  ...r0.....marker
-00001310: 7372 3100 0000 7231 0000 0072 3200 0000  sr1...r1...r2...
-00001320: da13 7465 7374 5f6b 6d65 616e 735f 636c  ..test_kmeans_cl
-00001330: 7573 7465 72c6 0000 0073 1600 0000 0002  uster....s......
-00001340: 0402 0801 0e03 0801 0802 1002 0802 0402  ................
-00001350: 1002 0801 7a24 5465 7374 4d61 7043 6c75  ....z$TestMapClu
-00001360: 7374 6572 6572 2e74 6573 745f 6b6d 6561  sterer.test_kmea
-00001370: 6e73 5f63 6c75 7374 6572 6301 0000 0000  ns_clusterc.....
-00001380: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
-00001390: 0000 0073 6a00 0000 7400 7d01 7401 4400  ...sj...t.}.t.D.
-000013a0: 5d5c 7d02 7402 4400 5d52 7d03 7c00 a003  ]\}.t.D.]R}.|...
-000013b0: a100 7d04 7c04 4400 5d40 7d05 7c00 a004  ..}.|.D.]@}.|...
-000013c0: 7c03 7c01 7c02 7c05 a104 7d06 7405 7c06  |.|.|.|...}.t.|.
-000013d0: 8301 7d07 7406 7407 6602 4400 5d1a 7d08  ..}.t.t.f.D.].}.
-000013e0: 7c07 a008 7c08 a101 7d09 7c00 a009 7c09  |...|...}.|...|.
-000013f0: 6401 a102 0100 7144 7120 7110 7108 6400  d.....qDq q.q.d.
-00001400: 5300 2902 4e72 4500 0000 290a 721f 0000  S.).NrE...).r...
-00001410: 0072 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
-00001420: 7220 0000 0072 0900 0000 7211 0000 0072  r ...r....r....r
-00001430: 1200 0000 5a1d 6765 745f 7372 6964 5f66  ....Z.get_srid_f
-00001440: 726f 6d5f 6765 6f6a 736f 6e5f 6665 6174  rom_geojson_feat
-00001450: 7572 6572 2100 0000 290a 722a 0000 0072  urer!...).r*...r
-00001460: 2f00 0000 722b 0000 0072 2c00 0000 722d  /...r+...r,...r-
-00001470: 0000 0072 2e00 0000 7222 0000 0072 3000  ...r....r"...r0.
-00001480: 0000 7239 0000 0072 3800 0000 7231 0000  ..r9...r8...r1..
-00001490: 0072 3100 0000 7232 0000 00da 2274 6573  .r1...r2...."tes
-000014a0: 745f 6765 745f 7372 6964 5f66 726f 6d5f  t_get_srid_from_
-000014b0: 6765 6f6a 736f 6e5f 6665 6174 7572 65dd  geojson_feature.
-000014c0: 0000 0073 1400 0000 0002 0402 0801 0802  ...s............
-000014d0: 0801 0802 1002 0802 0c02 0a02 7a33 5465  ............z3Te
-000014e0: 7374 4d61 7043 6c75 7374 6572 6572 2e74  stMapClusterer.t
-000014f0: 6573 745f 6765 745f 7372 6964 5f66 726f  est_get_srid_fro
-00001500: 6d5f 6765 6f6a 736f 6e5f 6665 6174 7572  m_geojson_featur
-00001510: 6563 0100 0000 0000 0000 0000 0000 0800  ec..............
-00001520: 0000 0700 0000 4300 0000 735a 0000 007c  ......C...sZ...|
-00001530: 00a0 00a1 007d 017c 0144 005d 487d 0274  .....}.|.D.]H}.t
-00001540: 017d 037c 00a0 0274 037c 0374 047c 02a1  .}.|...t.|.t.|..
-00001550: 047d 0474 057c 0483 017d 0567 007d 0274  .}.t.|...}.g.}.t
-00001560: 067d 067c 05a0 077c 067c 037c 02a1 037d  .}.|...|.|.|...}
-00001570: 077c 00a0 0874 097c 0783 0164 016b 04a1  .|...t.|...d.k..
-00001580: 0101 0071 0c64 0053 0072 4c00 0000 290a  ...q.d.S.rL...).
-00001590: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000015a0: 0c00 0000 7210 0000 0072 0900 0000 7212  ....r....r....r.
-000015b0: 0000 005a 0c67 7269 645f 636c 7573 7465  ...Z.grid_cluste
-000015c0: 7272 2700 0000 7237 0000 0029 0872 2a00  rr'...r7...).r*.
-000015d0: 0000 722d 0000 0072 2e00 0000 722f 0000  ..r-...r....r/..
-000015e0: 0072 2200 0000 7230 0000 0072 3900 0000  .r"...r0...r9...
-000015f0: da05 6365 6c6c 7372 3100 0000 7231 0000  ..cellsr1...r1..
-00001600: 0072 3200 0000 da11 7465 7374 5f67 7269  .r2.....test_gri
-00001610: 645f 636c 7573 7465 72f2 0000 0073 1200  d_cluster....s..
-00001620: 0000 0002 0801 0802 0401 1002 0802 0402  ................
-00001630: 0402 0e02 7a22 5465 7374 4d61 7043 6c75  ....z"TestMapClu
-00001640: 7374 6572 6572 2e74 6573 745f 6772 6964  sterer.test_grid
-00001650: 5f63 6c75 7374 6572 6301 0000 0000 0000  _clusterc.......
-00001660: 0000 0000 000a 0000 000a 0000 0043 0000  .............C..
-00001670: 0073 6c00 0000 7400 7d01 7401 4400 5d5e  .sl...t.}.t.D.]^
-00001680: 7d02 7402 4400 5d54 7d03 7c00 a003 a100  }.t.D.]T}.|.....
-00001690: 7d04 7c04 4400 5d42 7d05 7c00 a004 7c03  }.|.D.]B}.|...|.
-000016a0: 7c01 7c02 7c05 a104 7d06 7405 7c06 8301  |.|.|...}.t.|...
-000016b0: 7d07 7c07 a006 a100 7d08 6401 6402 6403  }.|.....}.d.d.d.
-000016c0: 6404 6405 6406 6407 6707 7d09 7c00 a007  d.d.d.d.g.}.|...
-000016d0: 7c08 7c09 a102 0100 7120 7110 7108 6400  |.|.....q q.q.d.
-000016e0: 5300 2908 4eda 0269 64da 046e 616d 65da  S.).N..id..name.
-000016f0: 0573 7479 6c65 da06 7261 7469 6e67 da0d  .style..rating..
-00001700: 6672 6565 5f65 6e74 7261 6e63 65da 0c6c  free_entrance..l
-00001710: 6173 745f 7265 6e65 7761 6cfa 1263 6f6f  ast_renewal..coo
-00001720: 7264 696e 6174 6573 3a3a 6279 7465 6129  rdinates::bytea)
-00001730: 0872 1f00 0000 720b 0000 0072 0e00 0000  .r....r....r....
-00001740: 721e 0000 0072 2000 0000 7209 0000 00da  r....r ...r.....
-00001750: 1367 6574 5f67 6973 5f66 6965 6c64 5f6e  .get_gis_field_n
-00001760: 616d 6573 7221 0000 0029 0a72 2a00 0000  amesr!...).r*...
-00001770: 722f 0000 0072 2b00 0000 722c 0000 0072  r/...r+...r,...r
-00001780: 2d00 0000 722e 0000 0072 2200 0000 7230  -...r....r"...r0
-00001790: 0000 00da 0b66 6965 6c64 5f6e 616d 6573  .....field_names
-000017a0: 5a14 6578 7065 6374 6564 5f66 6965 6c64  Z.expected_field
-000017b0: 5f6e 616d 6573 7231 0000 0072 3100 0000  _namesr1...r1...
-000017c0: 7232 0000 00da 1874 6573 745f 6765 745f  r2.....test_get_
-000017d0: 6769 735f 6669 656c 645f 6e61 6d65 7305  gis_field_names.
-000017e0: 0100 0073 1800 0000 0002 0402 0801 0802  ...s............
-000017f0: 0801 0802 1002 0802 0802 0c01 02ff 0403  ................
-00001800: 7a29 5465 7374 4d61 7043 6c75 7374 6572  z)TestMapCluster
-00001810: 6572 2e74 6573 745f 6765 745f 6769 735f  er.test_get_gis_
-00001820: 6669 656c 645f 6e61 6d65 7363 0100 0000  field_namesc....
-00001830: 0000 0000 0000 0000 0a00 0000 0900 0000  ................
-00001840: 4300 0000 735e 0000 0074 007d 0174 0144  C...s^...t.}.t.D
-00001850: 005d 507d 0274 0244 005d 467d 037c 00a0  .]P}.t.D.]F}.|..
-00001860: 03a1 007d 047c 0444 005d 347d 057c 00a0  ...}.|.D.]4}.|..
-00001870: 047c 037c 017c 027c 05a1 047d 0674 057c  .|.|.|.|...}.t.|
-00001880: 0683 017d 077c 07a0 06a1 007d 0864 017d  ...}.|.....}.d.}
-00001890: 097c 00a0 077c 087c 09a1 0201 0071 2071  .|...|.|.....q q
-000018a0: 1071 0864 0053 0029 024e 7a42 6964 2c6e  .q.d.S.).NzBid,n
-000018b0: 616d 652c 7374 796c 652c 7261 7469 6e67  ame,style,rating
-000018c0: 2c66 7265 655f 656e 7472 616e 6365 2c6c  ,free_entrance,l
-000018d0: 6173 745f 7265 6e65 7761 6c2c 636f 6f72  ast_renewal,coor
-000018e0: 6469 6e61 7465 733a 3a62 7974 6561 2908  dinates::bytea).
-000018f0: 721f 0000 0072 0b00 0000 720e 0000 0072  r....r....r....r
-00001900: 1e00 0000 7220 0000 0072 0900 0000 5a12  ....r ...r....Z.
-00001910: 6765 745f 6769 735f 6669 656c 6473 5f73  get_gis_fields_s
-00001920: 7472 7221 0000 0029 0a72 2a00 0000 722f  trr!...).r*...r/
-00001930: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
-00001940: 0000 722e 0000 0072 2200 0000 7230 0000  ..r....r"...r0..
-00001950: 005a 0a66 6965 6c64 735f 7374 725a 0c65  .Z.fields_strZ.e
-00001960: 7870 6563 7465 645f 7374 7272 3100 0000  xpected_strr1...
-00001970: 7231 0000 0072 3200 0000 da16 7465 7374  r1...r2.....test
-00001980: 5f67 6574 5f67 6973 5f66 6965 6c64 5f73  _get_gis_field_s
-00001990: 7472 1b01 0000 7314 0000 0000 0204 0208  tr....s.........
-000019a0: 0108 0308 0108 0210 0208 0208 0104 027a  ...............z
-000019b0: 2754 6573 744d 6170 436c 7573 7465 7265  'TestMapClustere
-000019c0: 722e 7465 7374 5f67 6574 5f67 6973 5f66  r.test_get_gis_f
-000019d0: 6965 6c64 5f73 7472 6301 0000 0000 0000  ield_strc.......
-000019e0: 0000 0000 000f 0000 000b 0000 0043 0000  .............C..
-000019f0: 0073 f200 0000 6401 7d01 7400 4400 5de4  .s....d.}.t.D.].
-00001a00: 7d02 7401 4400 5dda 7d03 7c00 a002 a100  }.t.D.].}.|.....
-00001a10: 7d04 7c04 4400 5dc8 7d05 7c00 a003 7c03  }.|.D.].}.|...|.
-00001a20: 7c01 7c02 7c05 a104 7d06 7404 7c06 8301  |.|.|...}.t.|...
-00001a30: 7d07 7405 7d08 6700 7d05 7c07 a006 7c08  }.t.}.g.}.|...|.
-00001a40: 7c03 7c01 7c05 a104 7d09 7c03 7407 6b02  |.|.|...}.|.t.k.
-00001a50: 7270 7c00 a008 7409 7c07 6a0a 6a0b 8301  rp|...t.|.j.j...
-00001a60: 6401 a102 0100 7c00 a00c 7409 7c09 8301  d.....|...t.|...
-00001a70: 6402 6b04 a101 0100 7c09 6402 1900 7d0a  d.k.....|.d...}.
-00001a80: 7c0a 6403 1900 7d0b 7c0a 6404 1900 6405  |.d...}.|.d...d.
-00001a90: 1900 7d0c 7c0a 6404 1900 6406 1900 7d0d  ..}.|.d...d...}.
-00001aa0: 7c07 a00d 7c03 7c0b 7c0c 7c0d 7c05 7c01  |...|.|.|.|.|.|.
-00001ab0: a106 7d0e 7c00 a00c 7c0a 6407 1900 6402  ..}.|...|.d...d.
-00001ac0: 6b04 a101 0100 7c00 a008 7409 740e 7c0e  k.....|...t.t.|.
-00001ad0: 8301 8301 7c0a 6407 1900 a102 0100 7120  ....|.d.......q 
-00001ae0: 7110 7108 6400 5300 2908 4e72 3400 0000  q.q.d.S.).Nr4...
-00001af0: 7201 0000 00da 0369 6473 da06 6365 6e74  r......ids..cent
-00001b00: 6572 da01 78da 0179 da05 636f 756e 7429  er..x..y..count)
-00001b10: 0f72 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
-00001b20: 7220 0000 0072 0900 0000 7212 0000 0072  r ...r....r....r
-00001b30: 4d00 0000 720d 0000 0072 2100 0000 7237  M...r....r!...r7
-00001b40: 0000 0072 2200 0000 da0a 6765 6f6d 6574  ...r".....geomet
-00001b50: 7269 6573 7227 0000 005a 1a67 6574 5f6b  riesr'...Z.get_k
-00001b60: 6d65 616e 735f 636c 7573 7465 725f 636f  means_cluster_co
-00001b70: 6e74 656e 7472 2900 0000 290f 722a 0000  ntentr)...).r*..
-00001b80: 0072 2f00 0000 722b 0000 0072 2c00 0000  .r/...r+...r,...
-00001b90: 722d 0000 0072 2e00 0000 7222 0000 0072  r-...r....r"...r
-00001ba0: 3000 0000 7239 0000 0072 4e00 0000 da06  0...r9...rN.....
-00001bb0: 6d61 726b 6572 725e 0000 0072 6000 0000  markerr^...r`...
-00001bc0: 7261 0000 005a 0f63 6c75 7374 6572 5f63  ra...Z.cluster_c
-00001bd0: 6f6e 7465 6e74 7231 0000 0072 3100 0000  ontentr1...r1...
-00001be0: 7232 0000 00da 1f74 6573 745f 6765 745f  r2.....test_get_
-00001bf0: 6b6d 6561 6e73 5f63 6c75 7374 6572 5f63  kmeans_cluster_c
-00001c00: 6f6e 7465 6e74 3001 0000 7328 0000 0000  ontent0...s(....
-00001c10: 0204 0208 0108 0308 0108 0210 0208 0204  ................
-00001c20: 0204 0210 0208 0114 0212 0208 0208 010c  ................
-00001c30: 010c 0214 0212 017a 3054 6573 744d 6170  .......z0TestMap
-00001c40: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
-00001c50: 6574 5f6b 6d65 616e 735f 636c 7573 7465  et_kmeans_cluste
-00001c60: 725f 636f 6e74 656e 7463 0100 0000 0000  r_contentc......
-00001c70: 0000 0000 0000 0a00 0000 0900 0000 4300  ..............C.
-00001c80: 0000 736e 0000 0064 017d 0174 0044 005d  ..sn...d.}.t.D.]
-00001c90: 607d 0274 0144 005d 567d 037c 00a0 02a1  `}.t.D.]V}.|....
-00001ca0: 007d 047c 0444 005d 447d 057c 00a0 037c  .}.|.D.]D}.|...|
-00001cb0: 037c 017c 027c 05a1 047d 0674 047c 0683  .|.|.|...}.t.|..
-00001cc0: 017d 0774 057d 0867 007d 057c 07a0 067c  .}.t.}.g.}.|...|
-00001cd0: 087c 05a1 027d 097c 00a0 0774 0874 097c  .|...}.|...t.t.|
-00001ce0: 0983 0183 0164 02a1 0201 0071 2071 1071  .....d.....q q.q
-00001cf0: 0864 0053 0029 034e 7234 0000 00e9 6400  .d.S.).Nr4....d.
-00001d00: 0000 290a 720b 0000 0072 0e00 0000 721e  ..).r....r....r.
-00001d10: 0000 0072 2000 0000 7209 0000 0072 1200  ...r ...r....r..
-00001d20: 0000 5a10 6765 745f 6172 6561 5f63 6f6e  ..Z.get_area_con
-00001d30: 7465 6e74 7221 0000 0072 3700 0000 7229  tentr!...r7...r)
-00001d40: 0000 0029 0a72 2a00 0000 722f 0000 0072  ...).r*...r/...r
-00001d50: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
-00001d60: 0000 0072 2200 0000 7230 0000 0072 3900  ...r"...r0...r9.
-00001d70: 0000 5a0c 6172 6561 5f63 6f6e 7465 6e74  ..Z.area_content
-00001d80: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
-00001d90: 1574 6573 745f 6765 745f 6172 6561 5f63  .test_get_area_c
-00001da0: 6f6e 7465 6e74 5601 0000 7316 0000 0000  ontentV...s.....
-00001db0: 0204 0208 0108 0308 0108 0210 0208 0204  ................
-00001dc0: 0104 020c 027a 2654 6573 744d 6170 436c  .....z&TestMapCl
-00001dd0: 7573 7465 7265 722e 7465 7374 5f67 6574  usterer.test_get
-00001de0: 5f61 7265 615f 636f 6e74 656e 7463 0100  _area_contentc..
-00001df0: 0000 0000 0000 0000 0000 0b00 0000 0900  ................
-00001e00: 0000 4300 0000 7364 0000 0064 017d 0174  ..C...sd...d.}.t
-00001e10: 0044 005d 567d 0274 0144 005d 4c7d 037c  .D.]V}.t.D.]L}.|
-00001e20: 00a0 02a1 007d 047c 0444 005d 3a7d 057c  .....}.|.D.]:}.|
-00001e30: 00a0 037c 037c 017c 027c 05a1 047d 0674  ...|.|.|.|...}.t
-00001e40: 047c 0683 017d 0774 057d 087c 07a0 067c  .|...}.t.}.|...|
-00001e50: 08a1 017d 0964 027d 0a7c 00a0 077c 097c  ...}.d.}.|...|.|
-00001e60: 0aa1 0201 0071 2071 1071 0864 0053 0029  .....q q.q.d.S.)
-00001e70: 034e 7234 0000 0061 0301 0000 2820 5354  .Nr4...a....( ST
-00001e80: 5f49 6e74 6572 7365 6374 7328 636f 6f72  _Intersects(coor
-00001e90: 6469 6e61 7465 732c 2053 545f 4765 6f6d  dinates, ST_Geom
-00001ea0: 6574 7279 4672 6f6d 5465 7874 2827 504f  etryFromText('PO
-00001eb0: 4c59 474f 4e20 2828 3939 3038 3532 2e35  LYGON ((990852.5
-00001ec0: 3438 3139 3339 3934 3120 3635 3339 3635  481939941 653965
-00001ed0: 302e 3638 3930 3732 3839 392c 2039 3930  0.689072899, 990
-00001ee0: 3835 322e 3534 3831 3933 3939 3431 2035  852.5481939941 5
-00001ef0: 3938 3032 3237 2e31 3032 3032 3834 3238  980227.102028428
-00001f00: 2c20 3135 3539 3837 362e 3232 3739 3935  , 1559876.227995
-00001f10: 3930 3238 2035 3938 3032 3237 2e31 3032  9028 5980227.102
-00001f20: 3032 3834 3238 2c20 3135 3539 3837 362e  028428, 1559876.
-00001f30: 3232 3739 3935 3930 3238 2036 3533 3936  2279959028 65396
-00001f40: 3530 2e36 3839 3037 3238 3939 2c20 3939  50.689072899, 99
-00001f50: 3038 3532 2e35 3438 3139 3339 3934 3120  0852.5481939941 
-00001f60: 3635 3339 3635 302e 3638 3930 3732 3839  6539650.68907289
-00001f70: 3929 2927 2c20 3338 3537 2920 2920 2929  9))', 3857) ) ))
-00001f80: 0872 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
-00001f90: 7220 0000 0072 0900 0000 7212 0000 005a  r ...r....r....Z
-00001fa0: 1567 6574 5f67 656f 6d5f 6669 6c74 6572  .get_geom_filter
-00001fb0: 7374 7269 6e67 7221 0000 0029 0b72 2a00  stringr!...).r*.
-00001fc0: 0000 722f 0000 0072 2b00 0000 722c 0000  ..r/...r+...r,..
-00001fd0: 0072 2d00 0000 722e 0000 0072 2200 0000  .r-...r....r"...
-00001fe0: 7230 0000 0072 3900 0000 5a11 6765 6f6d  r0...r9...Z.geom
-00001ff0: 5f66 696c 7465 7273 7472 696e 67da 0f65  _filterstring..e
-00002000: 7870 6563 7465 645f 7374 7269 6e67 7231  xpected_stringr1
-00002010: 0000 0072 3100 0000 7232 0000 00da 1a74  ...r1...r2.....t
-00002020: 6573 745f 6765 745f 6765 6f6d 5f66 696c  est_get_geom_fil
-00002030: 7465 7273 7472 696e 676d 0100 0073 1600  terstringm...s..
-00002040: 0000 0002 0402 0801 0803 0801 0802 1002  ................
-00002050: 0802 0402 0a02 0402 7a2b 5465 7374 4d61  ........z+TestMa
-00002060: 7043 6c75 7374 6572 6572 2e74 6573 745f  pClusterer.test_
-00002070: 6765 745f 6765 6f6d 5f66 696c 7465 7273  get_geom_filters
-00002080: 7472 696e 6763 0100 0000 0000 0000 0000  tringc..........
-00002090: 0000 0c00 0000 0900 0000 4300 0000 7388  ..........C...s.
-000020a0: 0000 0064 017d 0174 0044 005d 7a7d 0274  ...d.}.t.D.]z}.t
-000020b0: 0144 005d 707d 037c 00a0 02a1 007d 047c  .D.]p}.|.....}.|
-000020c0: 0444 005d 5e7d 057c 00a0 037c 037c 017c  .D.]^}.|...|.|.|
-000020d0: 027c 05a1 047d 0674 047c 0683 017d 0774  .|...}.t.|...}.t
-000020e0: 057d 087c 07a0 067c 0864 027c 01a1 037d  .}.|...|.d.|...}
-000020f0: 097c 00a0 0774 087c 0983 0164 03a1 0201  .|...t.|...d....
-00002100: 007c 0964 0419 007d 0a7c 07a0 097c 0a7c  .|.d...}.|...|.|
-00002110: 01a1 027d 0b7c 00a0 077c 0b64 05a1 0201  ...}.|...|.d....
-00002120: 0071 2071 1071 0864 0053 0029 064e e90a  .q q.q.d.S.).N..
-00002130: 0000 00da 0461 7265 6172 3400 0000 7201  .....arear4...r.
-00002140: 0000 00e9 1e00 0000 290a 720b 0000 0072  ........).r....r
-00002150: 0e00 0000 721e 0000 0072 2000 0000 7209  ....r....r ...r.
-00002160: 0000 0072 1100 0000 7241 0000 0072 2100  ...r....rA...r!.
-00002170: 0000 7237 0000 005a 0b63 616c 6375 6c61  ..r7...Z.calcula
-00002180: 7465 5f6b 290c 722a 0000 0072 2f00 0000  te_k).r*...r/...
-00002190: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
-000021a0: 2e00 0000 7222 0000 0072 3000 0000 7239  ....r"...r0...r9
-000021b0: 0000 0072 3a00 0000 da04 6765 6f73 da01  ...r:.....geos..
-000021c0: 6b72 3100 0000 7231 0000 0072 3200 0000  kr1...r1...r2...
-000021d0: da10 7465 7374 5f63 616c 6375 6c61 7465  ..test_calculate
-000021e0: 5f6b 8501 0000 731a 0000 0000 0204 0208  _k....s.........
-000021f0: 0108 0208 0108 0210 0208 0204 020e 0210  ................
-00002200: 0208 020c 027a 2154 6573 744d 6170 436c  .....z!TestMapCl
-00002210: 7573 7465 7265 722e 7465 7374 5f63 616c  usterer.test_cal
-00002220: 6375 6c61 7465 5f6b 6301 0000 0000 0000  culate_kc.......
-00002230: 0000 0000 000b 0000 0009 0000 0043 0000  .............C..
-00002240: 0073 c800 0000 7400 7d01 7401 4400 5dba  .s....t.}.t.D.].
-00002250: 7d02 7402 4400 5db0 7d03 7c00 a003 a100  }.t.D.].}.|.....
-00002260: 7d04 7c04 4400 5d9e 7d05 7c00 a004 7c02  }.|.D.].}.|...|.
-00002270: 7c01 7c03 7c05 a104 7d06 7405 7c06 8301  |.|.|...}.t.|...
-00002280: 7d07 7406 7d08 7c07 a007 7c08 7c02 7c01  }.t.}.|...|.|.|.
-00002290: a103 7d09 7c00 a008 7409 7c09 8301 6401  ..}.|...t.|...d.
-000022a0: 6b04 a101 0100 7c00 a00a 7c07 6a0b 6a0c  k.....|...|.j.j.
-000022b0: 7c01 a102 0100 7c00 a00a 7c07 6a0b 6a0d  |.....|...|.j.j.
-000022c0: 7c03 a102 0100 7c00 a00a 7c07 6a0b 6a0e  |.....|...|.j.j.
-000022d0: 7c02 a102 0100 7c00 a00a 7c07 6a0b 6a0f  |.....|...|.j.j.
-000022e0: 7c05 a102 0100 7c07 a007 7c08 7c02 7c01  |.....|...|.|.|.
-000022f0: a103 7d0a 7c00 a00a 7409 7c0a 8301 6401  ..}.|...t.|...d.
-00002300: a102 0100 7120 7110 7108 6400 5300 724c  ....q q.q.d.S.rL
-00002310: 0000 0029 1072 1f00 0000 720e 0000 0072  ...).r....r....r
-00002320: 0b00 0000 721e 0000 0072 2000 0000 7209  ....r....r ...r.
-00002330: 0000 0072 1200 0000 7241 0000 0072 2700  ...r....rA...r'.
-00002340: 0000 7237 0000 0072 2100 0000 7222 0000  ..r7...r!...r"..
-00002350: 0072 2f00 0000 722b 0000 0072 2c00 0000  .r/...r+...r,...
-00002360: 722e 0000 0029 0b72 2a00 0000 722f 0000  r....).r*...r/..
-00002370: 0072 2c00 0000 722b 0000 0072 2d00 0000  .r,...r+...r-...
-00002380: 722e 0000 0072 2200 0000 7230 0000 0072  r....r"...r0...r
-00002390: 3900 0000 7242 0000 005a 1863 6163 6865  9...rB...Z.cache
-000023a0: 5f63 6c75 7374 6572 5f67 656f 6d65 7472  _cluster_geometr
-000023b0: 6965 7372 3100 0000 7231 0000 0072 3200  iesr1...r1...r2.
-000023c0: 0000 da17 7465 7374 5f73 616d 655f 7265  ....test_same_re
-000023d0: 7175 6573 745f 7477 6963 65a0 0100 0073  quest_twice....s
-000023e0: 3000 0000 0002 0402 0801 0803 0801 0802  0...............
-000023f0: 1002 0802 0402 0401 0200 0200 02ff 0403  ................
-00002400: 1201 1001 1001 1001 1002 0401 0200 0200  ................
-00002410: 02ff 0403 7a28 5465 7374 4d61 7043 6c75  ....z(TestMapClu
-00002420: 7374 6572 6572 2e74 6573 745f 7361 6d65  sterer.test_same
-00002430: 5f72 6571 7565 7374 5f74 7769 6365 6301  _request_twicec.
-00002440: 0000 0000 0000 0000 0000 0008 0000 0008  ................
-00002450: 0000 0043 0000 0073 7a00 0000 7400 6a01  ...C...sz...t.j.
-00002460: a002 a100 a003 a100 7d01 7c00 a004 a100  ........}.|.....
-00002470: 7d02 7c02 4400 5d5a 7d03 7c00 a005 7406  }.|.D.]Z}.|...t.
-00002480: 7407 7408 7c03 a104 7d04 7409 7c04 8301  t.t.|...}.t.|...
-00002490: 7d05 7c05 a00a 7c01 6a0b a101 7d06 7c05  }.|...|.j...}.|.
-000024a0: a00c a100 4400 5d28 7d07 7c07 6401 6b02  ....D.](}.|.d.k.
-000024b0: 725a 6402 7d07 7c00 a00d 740e 7c01 7c07  rZd.}.|...t.|.|.
-000024c0: 8302 740e 7c06 7c07 8302 a102 0100 714a  ..t.|.|.......qJ
-000024d0: 711a 6400 5300 2903 4e72 5900 0000 da0b  q.d.S.).NrY.....
-000024e0: 636f 6f72 6469 6e61 7465 7329 0f72 1800  coordinates).r..
-000024f0: 0000 da07 6f62 6a65 6374 73da 0361 6c6c  ....objects..all
-00002500: da05 6669 7273 7472 1e00 0000 7220 0000  ..firstr....r ..
-00002510: 0072 0c00 0000 721f 0000 0072 1000 0000  .r....r....r....
-00002520: 7209 0000 005a 1367 6574 5f64 6174 6173  r....Z.get_datas
-00002530: 6574 5f63 6f6e 7465 6e74 7253 0000 0072  et_contentrS...r
-00002540: 5a00 0000 7221 0000 00da 0767 6574 6174  Z...r!.....getat
-00002550: 7472 2908 722a 0000 00da 0667 6172 6465  tr).r*.....garde
-00002560: 6e72 2d00 0000 722e 0000 0072 2200 0000  nr-...r....r"...
-00002570: 7230 0000 005a 0767 6172 6465 6e5f da0a  r0...Z.garden_..
-00002580: 6669 656c 645f 6e61 6d65 7231 0000 0072  field_namer1...r
-00002590: 3100 0000 7232 0000 00da 1874 6573 745f  1...r2.....test_
-000025a0: 6765 745f 6461 7461 7365 745f 636f 6e74  get_dataset_cont
-000025b0: 656e 74c0 0100 0073 1400 0000 0002 0e02  ent....s........
-000025c0: 0801 0802 1001 0802 0c02 0c02 0801 0402  ................
-000025d0: 7a29 5465 7374 4d61 7043 6c75 7374 6572  z)TestMapCluster
-000025e0: 6572 2e74 6573 745f 6765 745f 6461 7461  er.test_get_data
-000025f0: 7365 745f 636f 6e74 656e 7463 0100 0000  set_contentc....
-00002600: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00002610: 4300 0000 7304 0000 0064 0053 0072 3d00  C...s....d.S.r=.
-00002620: 0000 7231 0000 00a9 0172 2a00 0000 7231  ..r1.....r*...r1
-00002630: 0000 0072 3100 0000 7232 0000 00da 1374  ...r1...r2.....t
-00002640: 6573 745f 7061 6e6e 6564 5f72 6571 7565  est_panned_reque
-00002650: 7374 d301 0000 7302 0000 0000 017a 2454  st....s......z$T
-00002660: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
-00002670: 7465 7374 5f70 616e 6e65 645f 7265 7175  test_panned_requ
-00002680: 6573 7463 0100 0000 0000 0000 0000 0000  estc............
-00002690: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-000026a0: 0064 0053 0072 3d00 0000 7231 0000 0072  .d.S.r=...r1...r
-000026b0: 7900 0000 7231 0000 0072 3100 0000 7232  y...r1...r1...r2
-000026c0: 0000 00da 1774 6573 745f 7a6f 6f6d 5f6c  .....test_zoom_l
-000026d0: 6576 656c 5f63 6861 6e67 6564 d601 0000  evel_changed....
-000026e0: 7302 0000 0000 017a 2854 6573 744d 6170  s......z(TestMap
-000026f0: 436c 7573 7465 7265 722e 7465 7374 5f7a  Clusterer.test_z
-00002700: 6f6f 6d5f 6c65 7665 6c5f 6368 616e 6765  oom_level_change
-00002710: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-00002720: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-00002730: 0053 0072 3d00 0000 7231 0000 0072 7900  .S.r=...r1...ry.
-00002740: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
-00002750: 00da 1874 6573 745f 636c 7573 7465 7274  ...test_clustert
-00002760: 7970 655f 6368 616e 6765 64d9 0100 0073  ype_changed....s
-00002770: 0200 0000 0001 7a29 5465 7374 4d61 7043  ......z)TestMapC
-00002780: 6c75 7374 6572 6572 2e74 6573 745f 636c  lusterer.test_cl
-00002790: 7573 7465 7274 7970 655f 6368 616e 6765  ustertype_change
-000027a0: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-000027b0: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-000027c0: 0053 0072 3d00 0000 7231 0000 0072 7900  .S.r=...r1...ry.
-000027d0: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
-000027e0: 00da 1074 6573 745f 636c 6561 725f 6361  ...test_clear_ca
-000027f0: 6368 65dc 0100 0073 0200 0000 0001 7a21  che....s......z!
-00002800: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-00002810: 2e74 6573 745f 636c 6561 725f 6361 6368  .test_clear_cach
-00002820: 654e 2919 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
-00002830: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00002840: 616c 6e61 6d65 5f5f 7233 0000 0072 3500  alname__r3...r5.
-00002850: 0000 723c 0000 0072 3f00 0000 7240 0000  ..r<...r?...r@..
-00002860: 0072 4300 0000 724b 0000 0072 4f00 0000  .rC...rK...rO...
-00002870: 7250 0000 0072 5200 0000 725c 0000 0072  rP...rR...r\...r
-00002880: 5d00 0000 7265 0000 0072 6700 0000 7269  ]...re...rg...ri
-00002890: 0000 0072 6f00 0000 7270 0000 0072 7800  ...ro...rp...rx.
-000028a0: 0000 727a 0000 0072 7b00 0000 727c 0000  ..rz...r{...r|..
-000028b0: 0072 7d00 0000 7231 0000 0072 3100 0000  .r}...r1...r1...
-000028c0: 7231 0000 0072 3200 0000 721b 0000 0014  r1...r2...r.....
-000028d0: 0000 0073 2c00 0000 0803 0816 0812 0822  ...s,.........."
-000028e0: 0816 0813 0817 0825 0817 0815 0813 0816  .......%........
-000028f0: 0815 0826 0817 0818 081b 0820 0813 0803  ...&....... ....
-00002900: 0803 0803 721b 0000 0063 0000 0000 0000  ....r....c......
-00002910: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00002920: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
-00002930: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
-00002940: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
-00002950: 0964 0a84 005a 0764 0b53 0029 0cda 1d54  .d...Z.d.S.)...T
-00002960: 6573 744d 6170 436c 7573 7465 7265 7243  estMapClustererC
-00002970: 6f6e 7465 6e74 436f 756e 7473 6301 0000  ontentCountsc...
-00002980: 0000 0000 0000 0000 000d 0000 000a 0000  ................
-00002990: 0043 0000 0073 6e01 0000 6401 7d01 6402  .C...sn...d.}.d.
-000029a0: 6403 6404 6405 9c03 6701 7d02 6406 6407  d.d.d...g.}.d.d.
-000029b0: 6408 6404 6405 9c03 6701 6901 6406 6407  d.d.d...g.i.d.d.
-000029c0: 6408 6409 6405 9c03 6701 6901 640a 9c02  d.d.d...g.i.d...
-000029d0: 7d03 7400 4400 9001 5d2a 7d04 7401 4400  }.t.D...]*}.t.D.
-000029e0: 9001 5d1e 7d05 7402 7403 7404 7405 6604  ..].}.t.t.t.t.f.
-000029f0: 4400 9001 5d0a 7d06 7c04 7406 6b02 7270  D...].}.|.t.k.rp
-00002a00: 7c05 7407 6b03 7270 7158 7c05 7407 6b02  |.t.k.rpqX|.t.k.
-00002a10: 7282 7c06 7403 6b03 7282 7158 7c00 a008  r.|.t.k.r.qX|...
-00002a20: 7c05 7c01 7c04 7c02 a104 7d07 7409 7c07  |.|.|.|...}.t.|.
-00002a30: 740a 640b 8d02 7d08 7c08 a00b 7c06 7c05  t.d...}.|...|.|.
-00002a40: 7c02 7c01 7c03 a105 7d09 640c 640d 640c  |.|.|...}.d.d.d.
-00002a50: 6901 640d 640c 6901 640a 9c02 640e 9c02  i.d.d.i.d...d...
-00002a60: 7d0a 7c00 a00c 7c09 7c0a a102 0100 7c05  }.|...|.|.....|.
-00002a70: 7407 6b02 9001 722c 7c00 a00d 640f 6403  t.k...r,|...d.d.
-00002a80: a102 0100 7c00 a00d 6410 6411 a102 0100  ....|...d.d.....
-00002a90: 7c08 a00b 7c06 7c05 7c02 7c01 7c03 a105  |...|.|.|.|.|...
-00002aa0: 7d09 6412 640d 640c 6901 640d 6412 6901  }.d.d.d.i.d.d.i.
-00002ab0: 640a 9c02 640e 9c02 7d0a 7c00 a00c 7c09  d...d...}.|...|.
-00002ac0: 7c0a a102 0100 740e 6a0f a010 a100 7d0b  |.....t.j.....}.
-00002ad0: 7c0b 4400 5d0e 7d0c 7c0c a011 a100 0100  |.D.].}.|.......
-00002ae0: 9001 713a 740e 6a0f a010 a100 7d0b 7c00  ..q:t.j.....}.|.
-00002af0: a00c 7c0b a012 a100 640c a102 0100 7158  ..|.....d.....qX
-00002b00: 7146 713c 6400 5300 2913 4e72 6a00 0000  qFq<d.S.).Nrj...
-00002b10: 7255 0000 00da 0573 746f 6e65 fa01 3da9  rU.....stone..=.
-00002b20: 03da 0663 6f6c 756d 6eda 0576 616c 7565  ...column..value
-00002b30: da08 6f70 6572 6174 6f72 722e 0000 0072  ..operatorr....r
-00002b40: 5700 0000 547a 0221 3d29 02da 0466 7265  W...Tz.!=)...fre
-00002b50: 655a 0470 6169 64a9 0172 2500 0000 7201  eZ.paid..r%...r.
-00002b60: 0000 0072 6200 0000 2902 7262 0000 00da  ...rb...).rb....
-00002b70: 0b6d 6f64 756c 6174 696f 6e73 fa06 6e61  .modulations..na
-00002b80: 6d65 2031 fa06 6e61 6d65 2032 da06 666c  me 1..name 2..fl
-00002b90: 6f77 6572 7234 0000 0029 1372 0b00 0000  owerr4...).r....
-00002ba0: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00002bb0: 1300 0000 7214 0000 0072 1000 0000 720c  ....r....r....r.
-00002bc0: 0000 0072 2000 0000 7209 0000 00da 0e54  ...r ...r......T
-00002bd0: 4553 545f 4752 4944 5f53 495a 455a 1667  EST_GRID_SIZEZ.g
-00002be0: 6574 5f6d 6170 5f63 6f6e 7465 6e74 5f63  et_map_content_c
-00002bf0: 6f75 6e74 7372 2100 0000 da0c 6372 6561  ountsr!.....crea
-00002c00: 7465 5f70 6f69 6e74 7218 0000 0072 7200  te_pointr....rr.
-00002c10: 0000 7273 0000 00da 0664 656c 6574 6572  ..rs.....deleter
-00002c20: 6200 0000 290d 722a 0000 0072 2f00 0000  b...).r*...r/...
-00002c30: 722e 0000 0072 8a00 0000 722b 0000 0072  r....r....r+...r
-00002c40: 2c00 0000 7239 0000 0072 2200 0000 7230  ,...r9...r"...r0
-00002c50: 0000 00da 0672 6573 756c 74da 0f65 7870  .....result..exp
-00002c60: 6563 7465 645f 7265 7375 6c74 da07 6761  ected_result..ga
-00002c70: 7264 656e 7372 7600 0000 7231 0000 0072  rdensrv...r1...r
-00002c80: 3100 0000 7232 0000 00da 1a74 6573 745f  1...r2.....test_
-00002c90: 6765 745f 6d61 705f 636f 6e74 656e 745f  get_map_content_
-00002ca0: 636f 756e 74e2 0100 0073 7800 0000 0002  count....sx.....
-00002cb0: 0405 0201 0201 02fd 04ff 040b 0202 0201  ................
-00002cc0: 0201 02fd 04ff 02fe 020b 0202 0201 0201  ................
-00002cd0: 02fd 04ff 02ff 02f5 0617 0a01 0a02 1202  ................
-00002ce0: 1001 0202 1001 0202 1001 0c02 1203 0203  ................
-00002cf0: 0200 02ff 0204 0200 02ff 02fc 04fe 060b  ................
-00002d00: 0c02 0a02 0c01 0c02 1203 0203 0200 02ff  ................
-00002d10: 0204 0200 02ff 02fc 04fe 060e 0c02 0a01  ................
-00002d20: 0801 0c03 0a02 7a38 5465 7374 4d61 7043  ......z8TestMapC
-00002d30: 6c75 7374 6572 6572 436f 6e74 656e 7443  lustererContentC
-00002d40: 6f75 6e74 732e 7465 7374 5f67 6574 5f6d  ounts.test_get_m
-00002d50: 6170 5f63 6f6e 7465 6e74 5f63 6f75 6e74  ap_content_count
-00002d60: 6301 0000 0000 0000 0000 0000 000c 0000  c...............
-00002d70: 0006 0000 0043 0000 0073 3201 0000 6401  .....C...s2...d.
-00002d80: 7d01 7400 7d02 7401 7d03 6700 7d04 7c00  }.t.}.t.}.g.}.|.
-00002d90: a002 7c02 7c01 7c03 7c04 a104 7d05 7403  ..|.|.|.|...}.t.
-00002da0: 7c05 7404 6402 8d02 7d06 7405 7d07 7c06  |.t.d...}.t.}.|.
-00002db0: a006 7c07 7c02 7c01 a103 7d08 7c06 a007  ..|.|.|...}.|...
-00002dc0: 7c08 7c04 a102 7d09 7c00 a008 7c09 6403  |.|...}.|...|.d.
-00002dd0: a102 0100 7c00 a009 6404 6405 a102 0100  ....|...d.d.....
-00002de0: 7c06 a007 7c08 7c04 a102 7d09 7c00 a008  |...|.|...}.|...
-00002df0: 7c09 6406 a102 0100 7c00 a009 6407 6408  |.d.....|...d.d.
-00002e00: a102 0100 7c06 a007 7c08 7c04 a102 7d09  ....|...|.|...}.
-00002e10: 7c00 a008 7c09 6409 a102 0100 640a 6405  |...|.d.....d.d.
-00002e20: 640b 640c 9c03 6701 7d04 7c06 a007 7c08  d.d...g.}.|...|.
-00002e30: 7c04 a102 7d09 7c00 a008 7c09 6406 a102  |...}.|...|.d...
-00002e40: 0100 640a 6405 640b 640c 9c03 640a 6408  ..d.d.d.d...d.d.
-00002e50: 640b 640d 640e 9c04 6702 7d04 7c06 a007  d.d.d...g.}.|...
-00002e60: 7c08 7c04 a102 7d09 7c00 a008 7c09 6409  |.|...}.|...|.d.
-00002e70: a102 0100 740a 6a0b a00c a100 7d0a 7c0a  ....t.j.....}.|.
-00002e80: 4400 5d0e 7d0b 7c0b a00d a100 0100 9001  D.].}.|.........
-00002e90: 7104 740a 6a0b a00c a100 7d0a 7c00 a008  q.t.j.....}.|...
-00002ea0: 7c0a a00e a100 6403 a102 0100 6400 5300  |.....d.....d.S.
-00002eb0: 290f 4e72 6a00 0000 7289 0000 0072 0100  ).Nrj...r....r..
-00002ec0: 0000 728b 0000 0072 8200 0000 7234 0000  ..r....r....r4..
-00002ed0: 0072 8c00 0000 728d 0000 0072 3600 0000  .r....r....r6...
-00002ee0: 7255 0000 0072 8300 0000 7284 0000 00da  rU...r....r.....
-00002ef0: 024f 5229 0472 8500 0000 7286 0000 0072  .OR).r....r....r
-00002f00: 8700 0000 da0f 6c6f 6769 6361 6c4f 7065  ......logicalOpe
-00002f10: 7261 746f 7229 0f72 0c00 0000 720f 0000  rator).r....r...
-00002f20: 0072 2000 0000 7209 0000 0072 8e00 0000  .r ...r....r....
-00002f30: 7212 0000 00da 1b67 6574 5f67 656f 6d65  r......get_geome
-00002f40: 7472 6965 735f 666f 725f 636f 756e 7469  tries_for_counti
-00002f50: 6e67 5a17 7175 6572 795f 6d61 705f 636f  ngZ.query_map_co
-00002f60: 6e74 656e 745f 636f 756e 7472 2100 0000  ntent_countr!...
-00002f70: 728f 0000 0072 1800 0000 7272 0000 0072  r....r....rr...r
-00002f80: 7300 0000 7290 0000 0072 6200 0000 290c  s...r....rb...).
-00002f90: 722a 0000 0072 2f00 0000 722c 0000 0072  r*...r/...r,...r
-00002fa0: 2b00 0000 722e 0000 0072 2200 0000 7230  +...r....r"...r0
-00002fb0: 0000 0072 3900 0000 5a17 6765 6f6d 6574  ...r9...Z.geomet
-00002fc0: 7269 6573 5f66 6f72 5f63 6f75 6e74 696e  ries_for_countin
-00002fd0: 6772 6200 0000 7293 0000 0072 7600 0000  grb...r....rv...
-00002fe0: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
-00002ff0: 1c74 6573 745f 7175 6572 795f 6d61 705f  .test_query_map_
-00003000: 636f 6e74 656e 745f 636f 756e 7444 0200  content_countD..
-00003010: 0073 5000 0000 0002 0401 0401 0403 0402  .sP.............
-00003020: 1001 0c02 0402 0e02 0c01 0c02 0c02 0c01  ................
-00003030: 0c02 0c02 0c01 0c05 0201 0201 02fd 04ff  ................
-00003040: 0408 0c01 0c04 0201 0201 02fd 0406 0201  ................
-00003050: 0201 0201 02fc 04fa 040e 0c01 0c02 0a01  ................
-00003060: 0801 0c03 0a02 7a3a 5465 7374 4d61 7043  ......z:TestMapC
-00003070: 6c75 7374 6572 6572 436f 6e74 656e 7443  lustererContentC
-00003080: 6f75 6e74 732e 7465 7374 5f71 7565 7279  ounts.test_query
-00003090: 5f6d 6170 5f63 6f6e 7465 6e74 5f63 6f75  _map_content_cou
-000030a0: 6e74 6301 0000 0000 0000 0000 0000 000a  ntc.............
-000030b0: 0000 0009 0000 0043 0000 0073 aa00 0000  .......C...s....
-000030c0: 6401 7d01 7400 4400 5d9c 7d02 7401 4400  d.}.t.D.].}.t.D.
-000030d0: 5d92 7d03 7402 7403 7404 7405 6604 4400  ].}.t.t.t.t.f.D.
-000030e0: 5d80 7d04 7c02 7406 6b02 7236 7c03 7407  ].}.|.t.k.r6|.t.
-000030f0: 6b03 7236 7120 7c03 7407 6b02 7248 7c04  k.r6q |.t.k.rH|.
-00003100: 7403 6b03 7248 7120 6700 7d05 7c00 a008  t.k.rHq g.}.|...
-00003110: 7c03 7c01 7c02 7c05 a104 7d06 7409 7c06  |.|.|.|...}.t.|.
-00003120: 740a 6402 8d02 7d07 7c07 a00b 7c04 7c03  t.d...}.|...|.|.
-00003130: 7c01 a103 7d08 7c00 a00c 740d 7c08 740e  |...}.|...t.|.t.
-00003140: 8302 a101 0100 7c08 4400 5d14 7d09 7c00  ......|.D.].}.|.
-00003150: a00c 6403 7c09 6a0f 6b06 a101 0100 718a  ..d.|.j.k.....q.
-00003160: 7120 7110 7108 6400 5300 2904 4e72 6a00  q q.q.d.S.).Nrj.
-00003170: 0000 7289 0000 00da 0750 4f4c 5947 4f4e  ..r......POLYGON
-00003180: 2910 720b 0000 0072 0e00 0000 7211 0000  ).r....r....r...
-00003190: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-000031a0: 7210 0000 0072 0c00 0000 7220 0000 0072  r....r....r ...r
-000031b0: 0900 0000 728e 0000 0072 9700 0000 7227  ....r....r....r'
-000031c0: 0000 0072 2800 0000 7229 0000 00da 0377  ...r(...r).....w
-000031d0: 6b74 290a 722a 0000 0072 2f00 0000 722b  kt).r*...r/...r+
-000031e0: 0000 0072 2c00 0000 7239 0000 0072 2e00  ...r,...r9...r..
-000031f0: 0000 7222 0000 0072 3000 0000 723a 0000  ..r"...r0...r:..
-00003200: 0072 4400 0000 7231 0000 0072 3100 0000  .rD...r1...r1...
-00003210: 7232 0000 00da 2074 6573 745f 6765 745f  r2.... test_get_
-00003220: 6765 6f6d 6574 7269 6573 5f66 6f72 5f63  geometries_for_c
-00003230: 6f75 6e74 696e 6788 0200 0073 1e00 0000  ounting....s....
-00003240: 0002 0402 0801 0802 1002 1001 0202 1001  ................
-00003250: 0202 0402 1001 0c02 0e02 1002 0802 7a3e  ..............z>
-00003260: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-00003270: 436f 6e74 656e 7443 6f75 6e74 732e 7465  ContentCounts.te
-00003280: 7374 5f67 6574 5f67 656f 6d65 7472 6965  st_get_geometrie
-00003290: 735f 666f 725f 636f 756e 7469 6e67 6301  s_for_countingc.
-000032a0: 0000 0000 0000 0000 0000 000a 0000 0008  ................
-000032b0: 0000 0043 0000 0073 8e00 0000 6700 7d01  ...C...s....g.}.
-000032c0: 6401 7d02 7400 4400 5d7c 7d03 7401 4400  d.}.t.D.]|}.t.D.
-000032d0: 5d72 7d04 7c00 a002 7c04 7c02 7c03 7c01  ]r}.|...|.|.|.|.
-000032e0: a104 7d05 7403 7c05 7404 6402 8d02 7d06  ..}.t.|.t.d...}.
-000032f0: 7c06 a005 7406 a101 7d07 7c06 a007 7c07  |...t...}.|...|.
-00003300: 7c02 a102 7d08 7c00 a008 7409 7c08 8301  |...}.|...t.|...
-00003310: 6403 a102 0100 7c00 a008 7c08 6a0a 6404  d.....|...|.j.d.
-00003320: a102 0100 7c08 a00b 6405 a101 0100 6406  ....|...d.....d.
-00003330: 7d09 7c00 a008 7c09 7409 7c08 8301 a102  }.|...|.t.|.....
-00003340: 0100 7114 710c 6400 5300 2907 4e72 6a00  ..q.q.d.S.).Nrj.
-00003350: 0000 7289 0000 007a a753 5249 443d 3338  ..r....z.SRID=38
-00003360: 3537 3b50 4f4c 5947 4f4e 2028 2839 3738  57;POLYGON ((978
-00003370: 3339 332e 3936 3230 3520 3539 3438 3633  393.96205 594863
-00003380: 352e 3238 3930 3136 2c20 3135 3635 3433  5.289016, 156543
-00003390: 302e 3333 3932 3820 3539 3438 3633 352e  0.33928 5948635.
-000033a0: 3238 3930 3136 2c20 3135 3635 3433 302e  289016, 1565430.
-000033b0: 3333 3932 3820 3635 3734 3830 372e 3432  33928 6574807.42
-000033c0: 3437 3238 2c20 3937 3833 3933 2e39 3632  4728, 978393.962
-000033d0: 3035 2036 3537 3438 3037 2e34 3234 3732  05 6574807.42472
-000033e0: 382c 2039 3738 3339 332e 3936 3230 3520  8, 978393.96205 
-000033f0: 3539 3438 3633 352e 3238 3930 3136 2929  5948635.289016))
-00003400: 721d 0000 0072 4500 0000 7ac5 5352 4944  r....rE...z.SRID
-00003410: 3d34 3332 363b 504f 4c59 474f 4e20 2828  =4326;POLYGON ((
-00003420: 382e 3738 3930 3632 3439 3939 3937 3720  8.7890624999977 
-00003430: 3437 2e30 3430 3138 3231 3433 3237 3838  47.0401821432788
-00003440: 392c 2031 342e 3036 3234 3939 3939 3939  9, 14.0624999999
-00003450: 3936 3332 2034 372e 3034 3031 3832 3134  9632 47.04018214
-00003460: 3332 3738 3839 2c20 3134 2e30 3632 3439  327889, 14.06249
-00003470: 3939 3939 3939 3633 3220 3530 2e37 3336  999999632 50.736
-00003480: 3435 3531 3335 3539 3039 2c20 382e 3738  4551355909, 8.78
-00003490: 3930 3632 3439 3939 3937 3720 3530 2e37  90624999977 50.7
-000034a0: 3336 3435 3531 3335 3539 3039 2c20 382e  364551355909, 8.
+00000460: 0100 711c 710c 7104 6400 5300 2904 4eda  ..q.q.q.d.S.).N.
+00000470: 0670 7562 6c69 63e9 110f 0000 721a 0000  .public.....r...
+00000480: 0029 0e72 0b00 0000 720e 0000 00da 1067  .).r....r......g
+00000490: 6574 5f74 6573 745f 6669 6c74 6572 73da  et_test_filters.
+000004a0: 0f54 4553 545f 5a4f 4f4d 5f4c 4556 454c  .TEST_ZOOM_LEVEL
+000004b0: da11 6765 745f 636c 7573 7465 725f 6361  ..get_cluster_ca
+000004c0: 6368 6572 0900 0000 da0b 6173 7365 7274  cher......assert
+000004d0: 4571 7561 6cda 0d63 6c75 7374 6572 5f63  Equal..cluster_c
+000004e0: 6163 6865 da0b 7363 6865 6d61 5f6e 616d  ache..schema_nam
+000004f0: 65da 0764 625f 7372 6964 da09 6772 6964  e..db_srid..grid
+00000500: 5f73 697a 655a 086d 6170 746f 6f6c 73da  _sizeZ.maptools.
+00000510: 095f 5f63 6c61 7373 5f5f 720a 0000 0029  .__class__r....)
+00000520: 08da 0473 656c 66da 0b63 6c75 7374 6572  ...self..cluster
+00000530: 7479 7065 da0d 6765 6f6d 6574 7279 5f74  type..geometry_t
+00000540: 7970 65da 0c66 696c 7465 725f 6c69 7374  ype..filter_list
+00000550: 73da 0766 696c 7465 7273 da04 7a6f 6f6d  s..filters..zoom
+00000560: 7222 0000 00da 0d6d 6170 5f63 6c75 7374  r".....map_clust
+00000570: 6572 6572 a900 722e 0000 00fa 462f 686f  erer..r.....F/ho
+00000580: 6d65 2f74 6f6d 2f61 6e79 636c 7573 7465  me/tom/anycluste
+00000590: 722f 6465 6d6f 2f64 6a61 6e67 6f2f 616e  r/demo/django/an
+000005a0: 7963 6c75 7374 6572 2f74 6573 7473 2f74  ycluster/tests/t
+000005b0: 6573 745f 4d61 7043 6c75 7374 6572 6572  est_MapClusterer
+000005c0: 2e70 79da 0974 6573 745f 696e 6974 1700  .py..test_init..
+000005d0: 0000 7318 0000 0000 0208 0208 0208 0108  ..s.............
+000005e0: 0204 0110 0208 020e 010e 010e 010e 017a  ...............z
+000005f0: 1a54 6573 744d 6170 436c 7573 7465 7265  .TestMapClustere
+00000600: 722e 7465 7374 5f69 6e69 7463 0100 0000  r.test_initc....
+00000610: 0000 0000 0000 0000 0900 0000 0900 0000  ................
+00000620: 4300 0000 735a 0000 0074 0044 005d 507d  C...sZ...t.D.]P}
+00000630: 0174 0144 005d 467d 027c 00a0 02a1 007d  .t.D.]F}.|.....}
+00000640: 037c 0344 005d 347d 0464 017d 057c 00a0  .|.D.]4}.d.}.|..
+00000650: 037c 027c 057c 017c 04a1 047d 0674 047c  .|.|.|.|...}.t.|
+00000660: 0683 017d 077c 07a0 05a1 007d 087c 00a0  ...}.|.....}.|..
+00000670: 067c 0864 02a1 0201 0071 1c71 0c71 0464  .|.d.....q.q.q.d
+00000680: 0053 0029 034e e901 0000 0072 1d00 0000  .S.).N.....r....
+00000690: 2907 720b 0000 0072 0e00 0000 721e 0000  ).r....r....r...
+000006a0: 0072 2000 0000 7209 0000 005a 1167 6574  .r ...r....Z.get
+000006b0: 5f64 6174 6162 6173 655f 7372 6964 7221  _database_sridr!
+000006c0: 0000 0029 0972 2700 0000 7228 0000 0072  ...).r'...r(...r
+000006d0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
+000006e0: 0000 0072 2200 0000 722d 0000 0072 2400  ...r"...r-...r$.
+000006f0: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+00000700: 00da 1674 6573 745f 6765 745f 6461 7461  ...test_get_data
+00000710: 6261 7365 5f73 7269 642c 0000 0073 1200  base_srid,...s..
+00000720: 0000 0002 0802 0802 0801 0802 0401 1002  ................
+00000730: 0802 0801 7a27 5465 7374 4d61 7043 6c75  ....z'TestMapClu
+00000740: 7374 6572 6572 2e74 6573 745f 6765 745f  sterer.test_get_
+00000750: 6461 7461 6261 7365 5f73 7269 6463 0100  database_sridc..
+00000760: 0000 0000 0000 0000 0000 0c00 0000 0a00  ................
+00000770: 0000 4300 0000 73d8 0000 0074 0044 005d  ..C...s....t.D.]
+00000780: ce7d 0174 0144 005d c47d 027c 00a0 02a1  .}.t.D.].}.|....
+00000790: 007d 037c 0344 005d b27d 0474 037d 057c  .}.|.D.].}.t.}.|
+000007a0: 00a0 047c 027c 057c 017c 04a1 047d 0674  ...|.|.|.|...}.t
+000007b0: 057c 0683 017d 0774 0674 0766 0244 005d  .|...}.t.t.f.D.]
+000007c0: 467d 087c 07a0 087c 08a1 017d 097c 00a0  F}.|...|...}.|..
+000007d0: 0974 0a7c 0983 0164 01a1 0201 007c 0944  .t.|...d.....|.D
+000007e0: 005d 227d 0a7c 00a0 0b74 0c7c 0a74 0d83  .]"}.|...t.|.t..
+000007f0: 02a1 0101 007c 00a0 097c 0a6a 0e64 02a1  .....|...|.j.d..
+00000800: 0201 0071 6671 447c 07a0 0874 0fa1 017d  ...qfqD|...t...}
+00000810: 0b7c 00a0 0974 0a7c 0b83 0164 03a1 0201  .|...t.|...d....
+00000820: 007c 0b44 005d 227d 0a7c 00a0 0b74 0c7c  .|.D.]"}.|...t.|
+00000830: 0a74 0d83 02a1 0101 007c 00a0 097c 0a6a  .t.......|...|.j
+00000840: 0e64 02a1 0201 0071 aa71 1c71 0c71 0464  .d.....q.q.q.q.d
+00000850: 0053 0029 044e 7231 0000 0072 1d00 0000  .S.).Nr1...r....
+00000860: e902 0000 0029 1072 0b00 0000 720e 0000  .....).r....r...
+00000870: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000880: 7209 0000 0072 1100 0000 7212 0000 005a  r....r....r....Z
+00000890: 1f63 6f6e 7665 7274 5f67 656f 6a73 6f6e  .convert_geojson
+000008a0: 5f66 6561 7475 7265 5f74 6f5f 6765 6f73  _feature_to_geos
+000008b0: 7221 0000 00da 036c 656e da0a 6173 7365  r!.....len..asse
+000008c0: 7274 5472 7565 da0a 6973 696e 7374 616e  rtTrue..isinstan
+000008d0: 6365 7206 0000 00da 0473 7269 6472 1300  cer......sridr..
+000008e0: 0000 290c 7227 0000 0072 2800 0000 7229  ..).r'...r(...r)
+000008f0: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
+00000900: 0000 7222 0000 0072 2d00 0000 da07 6765  ..r"...r-.....ge
+00000910: 6f6a 736f 6eda 0f67 656f 735f 6765 6f6d  ojson..geos_geom
+00000920: 6574 7269 6573 da0d 6765 6f73 5f67 656f  etries..geos_geo
+00000930: 6d65 7472 795a 126d 705f 6765 6f73 5f67  metryZ.mp_geos_g
+00000940: 656f 6d65 7472 6965 7372 2e00 0000 722e  eometriesr....r.
+00000950: 0000 0072 2f00 0000 da2c 7465 7374 5f63  ...r/....,test_c
+00000960: 6f6e 7665 7274 5f67 656f 6a73 6f6e 5f66  onvert_geojson_f
+00000970: 6561 7475 7265 5f74 6f5f 6765 6f73 5f70  eature_to_geos_p
+00000980: 6f6c 7967 6f6e 3e00 0000 732c 0000 0000  olygon>...s,....
+00000990: 0208 0108 0208 0108 0204 0110 0208 020c  ................
+000009a0: 0204 0102 ff04 0310 0208 0110 0112 0204  ................
+000009b0: 0102 ff04 0310 0208 0110 017a 3d54 6573  ...........z=Tes
+000009c0: 744d 6170 436c 7573 7465 7265 722e 7465  tMapClusterer.te
+000009d0: 7374 5f63 6f6e 7665 7274 5f67 656f 6a73  st_convert_geojs
+000009e0: 6f6e 5f66 6561 7475 7265 5f74 6f5f 6765  on_feature_to_ge
+000009f0: 6f73 5f70 6f6c 7967 6f6e 6301 0000 0000  os_polygonc.....
+00000a00: 0000 0000 0000 000b 0000 000a 0000 0043  ...............C
+00000a10: 0000 0073 7a00 0000 7400 4400 5d70 7d01  ...sz...t.D.]p}.
+00000a20: 7401 4400 5d66 7d02 7c00 a002 a100 7d03  t.D.]f}.|.....}.
+00000a30: 7c03 4400 5d54 7d04 7403 7d05 7c00 a004  |.D.]T}.t.}.|...
+00000a40: 7c02 7c05 7c01 7c04 a104 7d06 7405 7c06  |.|.|.|...}.t.|.
+00000a50: 8301 7d07 7406 7407 7408 6603 4400 5d28  ..}.t.t.t.f.D.](
+00000a60: 7d08 7c07 a009 7c08 a101 7d09 7c09 4400  }.|...|...}.|.D.
+00000a70: 5d14 7d0a 7c00 a00a 740b 7c0a 740c 8302  ].}.|...t.|.t...
+00000a80: a101 0100 7158 7146 711c 710c 7104 6400  ....qXqFq.q.q.d.
+00000a90: 5300 a901 4e29 0d72 0b00 0000 720e 0000  S...N).r....r...
+00000aa0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000ab0: 7209 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000ac0: 1300 0000 da17 636f 6e76 6572 745f 6765  ......convert_ge
+00000ad0: 6f6a 736f 6e5f 746f 5f67 656f 7372 3500  ojson_to_geosr5.
+00000ae0: 0000 7236 0000 0072 0600 0000 290b 7227  ..r6...r....).r'
+00000af0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00000b00: 0000 722b 0000 0072 2c00 0000 7222 0000  ..r+...r,...r"..
+00000b10: 0072 2d00 0000 7238 0000 0072 3900 0000  .r-...r8...r9...
+00000b20: 723a 0000 0072 2e00 0000 722e 0000 0072  r:...r....r....r
+00000b30: 2f00 0000 da24 7465 7374 5f63 6f6e 7665  /....$test_conve
+00000b40: 7274 5f67 656f 6a73 6f6e 5f74 6f5f 6765  rt_geojson_to_ge
+00000b50: 6f73 5f66 6561 7475 7265 6000 0000 731a  os_feature`...s.
+00000b60: 0000 0000 0208 0108 0208 0108 0204 0110  ................
+00000b70: 0208 020e 0204 0102 ff04 0308 017a 3554  .............z5T
+00000b80: 6573 744d 6170 436c 7573 7465 7265 722e  estMapClusterer.
+00000b90: 7465 7374 5f63 6f6e 7665 7274 5f67 656f  test_convert_geo
+00000ba0: 6a73 6f6e 5f74 6f5f 6765 6f73 5f66 6561  json_to_geos_fea
+00000bb0: 7475 7265 6301 0000 0000 0000 0000 0000  turec...........
+00000bc0: 000a 0000 0009 0000 0043 0000 0073 6a00  .........C...sj.
+00000bd0: 0000 7400 4400 5d60 7d01 7401 4400 5d56  ..t.D.]`}.t.D.]V
+00000be0: 7d02 7c00 a002 a100 7d03 7c03 4400 5d44  }.|.....}.|.D.]D
+00000bf0: 7d04 7403 7d05 7c00 a004 7c02 7c05 7c01  }.t.}.|...|.|.|.
+00000c00: 7c04 a104 7d06 7405 7c06 8301 7d07 7c07  |...}.t.|...}.|.
+00000c10: a006 7407 a101 7d08 7c08 4400 5d14 7d09  ..t...}.|.D.].}.
+00000c20: 7c00 a008 7409 7c09 740a 8302 a101 0100  |...t.|.t.......
+00000c30: 714a 711c 710c 7104 6400 5300 723c 0000  qJq.q.q.d.S.r<..
+00000c40: 0029 0b72 0b00 0000 720e 0000 0072 1e00  .).r....r....r..
+00000c50: 0000 721f 0000 0072 2000 0000 7209 0000  ..r....r ...r...
+00000c60: 0072 3d00 0000 7214 0000 0072 3500 0000  .r=...r....r5...
+00000c70: 7236 0000 0072 0600 0000 290a 7227 0000  r6...r....).r'..
+00000c80: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00000c90: 722b 0000 0072 2c00 0000 7222 0000 0072  r+...r,...r"...r
+00000ca0: 2d00 0000 7239 0000 0072 3a00 0000 722e  -...r9...r:...r.
+00000cb0: 0000 0072 2e00 0000 722f 0000 00da 2e74  ...r....r/.....t
+00000cc0: 6573 745f 636f 6e76 6572 745f 6765 6f6a  est_convert_geoj
+00000cd0: 736f 6e5f 746f 5f67 656f 735f 6665 6174  son_to_geos_feat
+00000ce0: 7572 6563 6f6c 6c65 6374 696f 6e76 0000  urecollectionv..
+00000cf0: 0073 1800 0000 0002 0801 0802 0801 0802  .s..............
+00000d00: 0401 1002 0801 0401 02ff 0403 0801 7a3f  ..............z?
+00000d10: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+00000d20: 2e74 6573 745f 636f 6e76 6572 745f 6765  .test_convert_ge
+00000d30: 6f6a 736f 6e5f 746f 5f67 656f 735f 6665  ojson_to_geos_fe
+00000d40: 6174 7572 6563 6f6c 6c65 6374 696f 6e63  aturecollectionc
+00000d50: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
+00000d60: 0a00 0000 4300 0000 737e 0000 0074 0044  ....C...s~...t.D
+00000d70: 005d 747d 0174 0144 005d 6a7d 027c 00a0  .]t}.t.D.]j}.|..
+00000d80: 02a1 007d 037c 0344 005d 587d 0474 037d  ...}.|.D.]X}.t.}
+00000d90: 057c 00a0 047c 027c 057c 017c 04a1 047d  .|...|.|.|.|...}
+00000da0: 0674 057c 0683 017d 0774 0674 0774 0866  .t.|...}.t.t.t.f
+00000db0: 0344 005d 2c7d 087c 07a0 097c 087c 027c  .D.],}.|...|.|.|
+00000dc0: 05a1 037d 097c 0944 005d 147d 0a7c 00a0  ...}.|.D.].}.|..
+00000dd0: 0a74 0b7c 0a74 0c83 02a1 0101 0071 5c71  .t.|.t.......q\q
+00000de0: 4671 1c71 0c71 0464 0053 0072 3c00 0000  Fq.q.q.d.S.r<...
+00000df0: 290d 720b 0000 0072 0e00 0000 721e 0000  ).r....r....r...
+00000e00: 0072 1f00 0000 7220 0000 0072 0900 0000  .r....r ...r....
+00000e10: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000e20: 1667 6574 5f63 6c75 7374 6572 5f67 656f  .get_cluster_geo
+00000e30: 6d65 7472 6965 7372 3500 0000 7236 0000  metriesr5...r6..
+00000e40: 0072 0600 0000 290b 7227 0000 0072 2800  .r....).r'...r(.
+00000e50: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
+00000e60: 0072 2c00 0000 7222 0000 0072 2d00 0000  .r,...r"...r-...
+00000e70: 7238 0000 00da 1263 6c75 7374 6572 5f67  r8.....cluster_g
+00000e80: 656f 6d65 7472 6965 7372 3a00 0000 722e  eometriesr:...r.
+00000e90: 0000 0072 2e00 0000 722f 0000 00da 2474  ...r....r/....$t
+00000ea0: 6573 745f 6765 745f 636c 7573 7465 725f  est_get_cluster_
+00000eb0: 6765 6f6d 6574 7269 6573 5f76 6965 7770  geometries_viewp
+00000ec0: 6f72 7489 0000 0073 1e00 0000 0002 0801  ort....s........
+00000ed0: 0803 0801 0802 0401 1002 0802 0e02 0401  ................
+00000ee0: 0200 0200 02ff 0403 0801 7a35 5465 7374  ..........z5Test
+00000ef0: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
+00000f00: 745f 6765 745f 636c 7573 7465 725f 6765  t_get_cluster_ge
+00000f10: 6f6d 6574 7269 6573 5f76 6965 7770 6f72  ometries_viewpor
+00000f20: 7463 0100 0000 0000 0000 0000 0000 0d00  tc..............
+00000f30: 0000 0900 0000 4300 0000 73d6 0000 0074  ......C...s....t
+00000f40: 0044 005d cc7d 017c 00a0 01a1 007d 027c  .D.].}.|.....}.|
+00000f50: 0244 005d ba7d 0374 027d 047c 00a0 0374  .D.].}.t.}.|...t
+00000f60: 047c 047c 017c 03a1 047d 0574 057c 0583  .|.|.|...}.t.|..
+00000f70: 017d 0674 067d 077c 06a0 077c 0774 047c  .}.t.}.|...|.t.|
+00000f80: 04a1 037d 0874 0664 0119 00a0 08a1 007d  ...}.t.d.......}
+00000f90: 0974 0974 0aa0 0b7c 09a1 0164 0264 038d  .t.t...|...d.d..
+00000fa0: 027d 0a74 0c74 0d7c 0a6a 0e83 0174 0d64  .}.t.t.|.j...t.d
+00000fb0: 0483 0183 027d 0b7c 0aa0 0f7c 0ba1 0101  .....}.|...|....
+00000fc0: 007c 00a0 107c 0a6a 117c 0864 0519 006a  .|...|.j.|.d...j
+00000fd0: 11a1 0201 0074 1274 0674 1366 0344 005d  .....t.t.t.f.D.]
+00000fe0: 2c7d 077c 06a0 077c 0774 047c 04a1 037d  ,}.|...|.t.|...}
+00000ff0: 087c 0844 005d 147d 0c7c 00a0 1474 157c  .|.D.].}.|...t.|
+00001000: 0c74 0983 02a1 0101 0071 b671 a071 1471  .t.......q.q.q.q
+00001010: 0464 0053 0029 064e da08 6765 6f6d 6574  .d.S.).N..geomet
+00001020: 7279 e9e6 1000 0029 0172 3700 0000 721d  ry.....).r7...r.
+00001030: 0000 0072 0100 0000 2916 720b 0000 0072  ...r....).r....r
+00001040: 1e00 0000 721f 0000 0072 2000 0000 720d  ....r....r ...r.
+00001050: 0000 0072 0900 0000 7212 0000 0072 4000  ...r....r....r@.
+00001060: 0000 da04 636f 7079 7206 0000 00da 046a  ....copyr......j
+00001070: 736f 6eda 0564 756d 7073 7208 0000 0072  son..dumpsr....r
+00001080: 0700 0000 7237 0000 00da 0974 7261 6e73  ....r7.....trans
+00001090: 666f 726d 7221 0000 0072 3800 0000 7211  formr!...r8...r.
+000010a0: 0000 0072 1300 0000 7235 0000 0072 3600  ...r....r5...r6.
+000010b0: 0000 290d 7227 0000 0072 2800 0000 722a  ..).r'...r(...r*
+000010c0: 0000 0072 2b00 0000 722c 0000 0072 2200  ...r+...r,...r".
+000010d0: 0000 722d 0000 0072 3800 0000 7241 0000  ..r-...r8...rA..
+000010e0: 005a 106d 6174 6368 696e 675f 6765 6f6a  .Z.matching_geoj
+000010f0: 736f 6e5a 0c69 6e69 7469 616c 5f67 656f  sonZ.initial_geo
+00001100: 73da 0263 7472 3a00 0000 722e 0000 0072  s..ctr:...r....r
+00001110: 2e00 0000 722f 0000 00da 2074 6573 745f  ....r/.... test_
+00001120: 6765 745f 636c 7573 7465 725f 6765 6f6d  get_cluster_geom
+00001130: 6574 7269 6573 5f61 7265 61a0 0000 0073  etries_area....s
+00001140: 4400 0000 0002 0803 0801 0802 0401 1002  D...............
+00001150: 0802 0402 0401 0200 0200 02ff 0403 0c01  ................
+00001160: 0201 0800 02ff 0602 0401 04ff 0201 06ff  ................
+00001170: 0402 0a02 0801 08ff 0403 0e02 0401 0200  ................
+00001180: 0200 02ff 0403 0801 7a31 5465 7374 4d61  ........z1TestMa
+00001190: 7043 6c75 7374 6572 6572 2e74 6573 745f  pClusterer.test_
+000011a0: 6765 745f 636c 7573 7465 725f 6765 6f6d  get_cluster_geom
+000011b0: 6574 7269 6573 5f61 7265 6163 0100 0000  etries_areac....
+000011c0: 0000 0000 0000 0000 0900 0000 0900 0000  ................
+000011d0: 4300 0000 737a 0000 0074 007d 0174 0144  C...sz...t.}.t.D
+000011e0: 005d 6c7d 0274 0274 0374 0466 0344 005d  .]l}.t.t.t.f.D.]
+000011f0: 5c7d 037c 00a0 05a1 007d 047c 0444 005d  \}.|.....}.|.D.]
+00001200: 4a7d 057c 00a0 067c 027c 0174 077c 05a1  J}.|...|.|.t.|..
+00001210: 047d 0674 087c 0683 017d 0767 007d 057c  .}.t.|...}.g.}.|
+00001220: 07a0 097c 037c 027c 017c 05a1 047d 087c  ...|.|.|.|...}.|
+00001230: 0274 0a6b 0272 267c 00a0 0b74 0c7c 0883  .t.k.r&|...t.|..
+00001240: 0164 016b 04a1 0101 0071 2671 1671 0864  .d.k.....q&q.q.d
+00001250: 0053 00a9 024e 7201 0000 0029 0d72 1f00  .S...Nr....).r..
+00001260: 0000 720e 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00001270: 0072 1300 0000 721e 0000 0072 2000 0000  .r....r....r ...
+00001280: 720f 0000 0072 0900 0000 da0e 6b6d 6561  r....r......kmea
+00001290: 6e73 5f63 6c75 7374 6572 720c 0000 0072  ns_clusterr....r
+000012a0: 3500 0000 7234 0000 0029 0972 2700 0000  5...r4...).r'...
+000012b0: 722c 0000 0072 2900 0000 7238 0000 0072  r,...r)...r8...r
+000012c0: 2a00 0000 722b 0000 0072 2200 0000 722d  *...r+...r"...r-
+000012d0: 0000 00da 076d 6172 6b65 7273 722e 0000  .....markersr...
+000012e0: 0072 2e00 0000 722f 0000 00da 1374 6573  .r....r/.....tes
+000012f0: 745f 6b6d 6561 6e73 5f63 6c75 7374 6572  t_kmeans_cluster
+00001300: c500 0000 7316 0000 0000 0204 0208 010e  ....s...........
+00001310: 0308 0108 0210 0208 0204 0210 0208 017a  ...............z
+00001320: 2454 6573 744d 6170 436c 7573 7465 7265  $TestMapClustere
+00001330: 722e 7465 7374 5f6b 6d65 616e 735f 636c  r.test_kmeans_cl
+00001340: 7573 7465 7263 0100 0000 0000 0000 0000  usterc..........
+00001350: 0000 0a00 0000 0900 0000 4300 0000 736a  ..........C...sj
+00001360: 0000 0074 007d 0174 0144 005d 5c7d 0274  ...t.}.t.D.]\}.t
+00001370: 0244 005d 527d 037c 00a0 03a1 007d 047c  .D.]R}.|.....}.|
+00001380: 0444 005d 407d 057c 00a0 047c 037c 017c  .D.]@}.|...|.|.|
+00001390: 027c 05a1 047d 0674 057c 0683 017d 0774  .|...}.t.|...}.t
+000013a0: 0674 0766 0244 005d 1a7d 087c 07a0 087c  .t.f.D.].}.|...|
+000013b0: 08a1 017d 097c 00a0 097c 0964 01a1 0201  ...}.|...|.d....
+000013c0: 0071 4471 2071 1071 0864 0053 0029 024e  .qDq q.q.d.S.).N
+000013d0: 7244 0000 0029 0a72 1f00 0000 720b 0000  rD...).r....r...
+000013e0: 0072 0e00 0000 721e 0000 0072 2000 0000  .r....r....r ...
+000013f0: 7209 0000 0072 1100 0000 7212 0000 005a  r....r....r....Z
+00001400: 1d67 6574 5f73 7269 645f 6672 6f6d 5f67  .get_srid_from_g
+00001410: 656f 6a73 6f6e 5f66 6561 7475 7265 7221  eojson_featurer!
+00001420: 0000 0029 0a72 2700 0000 722c 0000 0072  ...).r'...r,...r
+00001430: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
+00001440: 0000 0072 2200 0000 722d 0000 0072 3800  ...r"...r-...r8.
+00001450: 0000 7237 0000 0072 2e00 0000 722e 0000  ..r7...r....r...
+00001460: 0072 2f00 0000 da22 7465 7374 5f67 6574  .r/...."test_get
+00001470: 5f73 7269 645f 6672 6f6d 5f67 656f 6a73  _srid_from_geojs
+00001480: 6f6e 5f66 6561 7475 7265 dc00 0000 7314  on_feature....s.
+00001490: 0000 0000 0204 0208 0108 0208 0108 0210  ................
+000014a0: 0208 020c 020a 027a 3354 6573 744d 6170  .......z3TestMap
+000014b0: 436c 7573 7465 7265 722e 7465 7374 5f67  Clusterer.test_g
+000014c0: 6574 5f73 7269 645f 6672 6f6d 5f67 656f  et_srid_from_geo
+000014d0: 6a73 6f6e 5f66 6561 7475 7265 6301 0000  json_featurec...
+000014e0: 0000 0000 0000 0000 0008 0000 0007 0000  ................
+000014f0: 0043 0000 0073 5a00 0000 7c00 a000 a100  .C...sZ...|.....
+00001500: 7d01 7c01 4400 5d48 7d02 7401 7d03 7c00  }.|.D.]H}.t.}.|.
+00001510: a002 7403 7c03 7404 7c02 a104 7d04 7405  ..t.|.t.|...}.t.
+00001520: 7c04 8301 7d05 6700 7d02 7406 7d06 7c05  |...}.g.}.t.}.|.
+00001530: a007 7c06 7c03 7c02 a103 7d07 7c00 a008  ..|.|.|...}.|...
+00001540: 7409 7c07 8301 6401 6b04 a101 0100 710c  t.|...d.k.....q.
+00001550: 6400 5300 724b 0000 0029 0a72 1e00 0000  d.S.rK...).r....
+00001560: 721f 0000 0072 2000 0000 720c 0000 0072  r....r ...r....r
+00001570: 1000 0000 7209 0000 0072 1200 0000 5a0c  ....r....r....Z.
+00001580: 6772 6964 5f63 6c75 7374 6572 7235 0000  grid_clusterr5..
+00001590: 0072 3400 0000 2908 7227 0000 0072 2a00  .r4...).r'...r*.
+000015a0: 0000 722b 0000 0072 2c00 0000 7222 0000  ..r+...r,...r"..
+000015b0: 0072 2d00 0000 7238 0000 00da 0563 656c  .r-...r8.....cel
+000015c0: 6c73 722e 0000 0072 2e00 0000 722f 0000  lsr....r....r/..
+000015d0: 00da 1174 6573 745f 6772 6964 5f63 6c75  ...test_grid_clu
+000015e0: 7374 6572 f100 0000 7312 0000 0000 0208  ster....s.......
+000015f0: 0108 0204 0110 0208 0204 0204 020e 027a  ...............z
+00001600: 2254 6573 744d 6170 436c 7573 7465 7265  "TestMapClustere
+00001610: 722e 7465 7374 5f67 7269 645f 636c 7573  r.test_grid_clus
+00001620: 7465 7263 0100 0000 0000 0000 0000 0000  terc............
+00001630: 0a00 0000 0a00 0000 4300 0000 736c 0000  ........C...sl..
+00001640: 0074 007d 0174 0144 005d 5e7d 0274 0244  .t.}.t.D.]^}.t.D
+00001650: 005d 547d 037c 00a0 03a1 007d 047c 0444  .]T}.|.....}.|.D
+00001660: 005d 427d 057c 00a0 047c 037c 017c 027c  .]B}.|...|.|.|.|
+00001670: 05a1 047d 0674 057c 0683 017d 077c 07a0  ...}.t.|...}.|..
+00001680: 06a1 007d 0864 0164 0264 0364 0464 0564  ...}.d.d.d.d.d.d
+00001690: 0664 0767 077d 097c 00a0 077c 087c 09a1  .d.g.}.|...|.|..
+000016a0: 0201 0071 2071 1071 0864 0053 0029 084e  ...q q.q.d.S.).N
+000016b0: da02 6964 da04 6e61 6d65 da05 7374 796c  ..id..name..styl
+000016c0: 65da 0672 6174 696e 67da 0d66 7265 655f  e..rating..free_
+000016d0: 656e 7472 616e 6365 da0c 6c61 7374 5f72  entrance..last_r
+000016e0: 656e 6577 616c fa12 636f 6f72 6469 6e61  enewal..coordina
+000016f0: 7465 733a 3a62 7974 6561 2908 721f 0000  tes::bytea).r...
+00001700: 0072 0b00 0000 720e 0000 0072 1e00 0000  .r....r....r....
+00001710: 7220 0000 0072 0900 0000 da13 6765 745f  r ...r......get_
+00001720: 6769 735f 6669 656c 645f 6e61 6d65 7372  gis_field_namesr
+00001730: 2100 0000 290a 7227 0000 0072 2c00 0000  !...).r'...r,...
+00001740: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+00001750: 2b00 0000 7222 0000 0072 2d00 0000 da0b  +...r"...r-.....
+00001760: 6669 656c 645f 6e61 6d65 735a 1465 7870  field_namesZ.exp
+00001770: 6563 7465 645f 6669 656c 645f 6e61 6d65  ected_field_name
+00001780: 7372 2e00 0000 722e 0000 0072 2f00 0000  sr....r....r/...
+00001790: da18 7465 7374 5f67 6574 5f67 6973 5f66  ..test_get_gis_f
+000017a0: 6965 6c64 5f6e 616d 6573 0401 0000 7318  ield_names....s.
+000017b0: 0000 0000 0204 0208 0108 0208 0108 0210  ................
+000017c0: 0208 0208 020c 0102 ff04 037a 2954 6573  ...........z)Tes
+000017d0: 744d 6170 436c 7573 7465 7265 722e 7465  tMapClusterer.te
+000017e0: 7374 5f67 6574 5f67 6973 5f66 6965 6c64  st_get_gis_field
+000017f0: 5f6e 616d 6573 6301 0000 0000 0000 0000  _namesc.........
+00001800: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
+00001810: 5e00 0000 7400 7d01 7401 4400 5d50 7d02  ^...t.}.t.D.]P}.
+00001820: 7402 4400 5d46 7d03 7c00 a003 a100 7d04  t.D.]F}.|.....}.
+00001830: 7c04 4400 5d34 7d05 7c00 a004 7c03 7c01  |.D.]4}.|...|.|.
+00001840: 7c02 7c05 a104 7d06 7405 7c06 8301 7d07  |.|...}.t.|...}.
+00001850: 7c07 a006 a100 7d08 6401 7d09 7c00 a007  |.....}.d.}.|...
+00001860: 7c08 7c09 a102 0100 7120 7110 7108 6400  |.|.....q q.q.d.
+00001870: 5300 2902 4e7a 4269 642c 6e61 6d65 2c73  S.).NzBid,name,s
+00001880: 7479 6c65 2c72 6174 696e 672c 6672 6565  tyle,rating,free
+00001890: 5f65 6e74 7261 6e63 652c 6c61 7374 5f72  _entrance,last_r
+000018a0: 656e 6577 616c 2c63 6f6f 7264 696e 6174  enewal,coordinat
+000018b0: 6573 3a3a 6279 7465 6129 0872 1f00 0000  es::bytea).r....
+000018c0: 720b 0000 0072 0e00 0000 721e 0000 0072  r....r....r....r
+000018d0: 2000 0000 7209 0000 005a 1267 6574 5f67   ...r....Z.get_g
+000018e0: 6973 5f66 6965 6c64 735f 7374 7272 2100  is_fields_strr!.
+000018f0: 0000 290a 7227 0000 0072 2c00 0000 7228  ..).r'...r,...r(
+00001900: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00001910: 0000 7222 0000 0072 2d00 0000 5a0a 6669  ..r"...r-...Z.fi
+00001920: 656c 6473 5f73 7472 5a0c 6578 7065 6374  elds_strZ.expect
+00001930: 6564 5f73 7472 722e 0000 0072 2e00 0000  ed_strr....r....
+00001940: 722f 0000 00da 1674 6573 745f 6765 745f  r/.....test_get_
+00001950: 6769 735f 6669 656c 645f 7374 721a 0100  gis_field_str...
+00001960: 0073 1400 0000 0002 0402 0801 0803 0801  .s..............
+00001970: 0802 1002 0802 0801 0402 7a27 5465 7374  ..........z'Test
+00001980: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
+00001990: 745f 6765 745f 6769 735f 6669 656c 645f  t_get_gis_field_
+000019a0: 7374 7263 0100 0000 0000 0000 0000 0000  strc............
+000019b0: 0f00 0000 0b00 0000 4300 0000 73f2 0000  ........C...s...
+000019c0: 0064 017d 0174 0044 005d e47d 0274 0144  .d.}.t.D.].}.t.D
+000019d0: 005d da7d 037c 00a0 02a1 007d 047c 0444  .].}.|.....}.|.D
+000019e0: 005d c87d 057c 00a0 037c 037c 017c 027c  .].}.|...|.|.|.|
+000019f0: 05a1 047d 0674 047c 0683 017d 0774 057d  ...}.t.|...}.t.}
+00001a00: 0867 007d 057c 07a0 067c 087c 037c 017c  .g.}.|...|.|.|.|
+00001a10: 05a1 047d 097c 0374 076b 0272 707c 00a0  ...}.|.t.k.rp|..
+00001a20: 0874 097c 076a 0a6a 0b83 0164 01a1 0201  .t.|.j.j...d....
+00001a30: 007c 00a0 0c74 097c 0983 0164 026b 04a1  .|...t.|...d.k..
+00001a40: 0101 007c 0964 0219 007d 0a7c 0a64 0319  ...|.d...}.|.d..
+00001a50: 007d 0b7c 0a64 0419 0064 0519 007d 0c7c  .}.|.d...d...}.|
+00001a60: 0a64 0419 0064 0619 007d 0d7c 07a0 0d7c  .d...d...}.|...|
+00001a70: 037c 0b7c 0c7c 0d7c 057c 01a1 067d 0e7c  .|.|.|.|.|...}.|
+00001a80: 00a0 0c7c 0a64 0719 0064 026b 04a1 0101  ...|.d...d.k....
+00001a90: 007c 00a0 0874 0974 0e7c 0e83 0183 017c  .|...t.t.|.....|
+00001aa0: 0a64 0719 00a1 0201 0071 2071 1071 0864  .d.......q q.q.d
+00001ab0: 0053 0029 084e 7231 0000 0072 0100 0000  .S.).Nr1...r....
+00001ac0: da03 6964 73da 0663 656e 7465 72da 0178  ..ids..center..x
+00001ad0: da01 79da 0563 6f75 6e74 290f 720b 0000  ..y..count).r...
+00001ae0: 0072 0e00 0000 721e 0000 0072 2000 0000  .r....r....r ...
+00001af0: 7209 0000 0072 1200 0000 724c 0000 0072  r....r....rL...r
+00001b00: 0d00 0000 7221 0000 0072 3400 0000 7222  ....r!...r4...r"
+00001b10: 0000 00da 0a67 656f 6d65 7472 6965 7372  .....geometriesr
+00001b20: 3500 0000 5a1a 6765 745f 6b6d 6561 6e73  5...Z.get_kmeans
+00001b30: 5f63 6c75 7374 6572 5f63 6f6e 7465 6e74  _cluster_content
+00001b40: da04 6c69 7374 290f 7227 0000 0072 2c00  ..list).r'...r,.
+00001b50: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00001b60: 0072 2b00 0000 7222 0000 0072 2d00 0000  .r+...r"...r-...
+00001b70: 7238 0000 0072 4d00 0000 da06 6d61 726b  r8...rM.....mark
+00001b80: 6572 725d 0000 0072 5f00 0000 7260 0000  err]...r_...r`..
+00001b90: 005a 0f63 6c75 7374 6572 5f63 6f6e 7465  .Z.cluster_conte
+00001ba0: 6e74 722e 0000 0072 2e00 0000 722f 0000  ntr....r....r/..
+00001bb0: 00da 1f74 6573 745f 6765 745f 6b6d 6561  ...test_get_kmea
+00001bc0: 6e73 5f63 6c75 7374 6572 5f63 6f6e 7465  ns_cluster_conte
+00001bd0: 6e74 2f01 0000 7328 0000 0000 0204 0208  nt/...s(........
+00001be0: 0108 0308 0108 0210 0208 0204 0204 0210  ................
+00001bf0: 0208 0114 0212 0208 0208 010c 010c 0214  ................
+00001c00: 0212 017a 3054 6573 744d 6170 436c 7573  ...z0TestMapClus
+00001c10: 7465 7265 722e 7465 7374 5f67 6574 5f6b  terer.test_get_k
+00001c20: 6d65 616e 735f 636c 7573 7465 725f 636f  means_cluster_co
+00001c30: 6e74 656e 7463 0100 0000 0000 0000 0000  ntentc..........
+00001c40: 0000 0a00 0000 0900 0000 4300 0000 736e  ..........C...sn
+00001c50: 0000 0064 017d 0174 0044 005d 607d 0274  ...d.}.t.D.]`}.t
+00001c60: 0144 005d 567d 037c 00a0 02a1 007d 047c  .D.]V}.|.....}.|
+00001c70: 0444 005d 447d 057c 00a0 037c 037c 017c  .D.]D}.|...|.|.|
+00001c80: 027c 05a1 047d 0674 047c 0683 017d 0774  .|...}.t.|...}.t
+00001c90: 057d 0867 007d 057c 07a0 067c 087c 05a1  .}.g.}.|...|.|..
+00001ca0: 027d 097c 00a0 0774 0874 097c 0983 0183  .}.|...t.t.|....
+00001cb0: 0164 02a1 0201 0071 2071 1071 0864 0053  .d.....q q.q.d.S
+00001cc0: 0029 034e 7231 0000 00e9 6400 0000 290a  .).Nr1....d...).
+00001cd0: 720b 0000 0072 0e00 0000 721e 0000 0072  r....r....r....r
+00001ce0: 2000 0000 7209 0000 0072 1200 0000 5a10   ...r....r....Z.
+00001cf0: 6765 745f 6172 6561 5f63 6f6e 7465 6e74  get_area_content
+00001d00: 7221 0000 0072 3400 0000 7263 0000 0029  r!...r4...rc...)
+00001d10: 0a72 2700 0000 722c 0000 0072 2800 0000  .r'...r,...r(...
+00001d20: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
+00001d30: 2200 0000 722d 0000 0072 3800 0000 5a0c  "...r-...r8...Z.
+00001d40: 6172 6561 5f63 6f6e 7465 6e74 722e 0000  area_contentr...
+00001d50: 0072 2e00 0000 722f 0000 00da 1574 6573  .r....r/.....tes
+00001d60: 745f 6765 745f 6172 6561 5f63 6f6e 7465  t_get_area_conte
+00001d70: 6e74 5501 0000 7316 0000 0000 0204 0208  ntU...s.........
+00001d80: 0108 0308 0108 0210 0208 0204 0104 020c  ................
+00001d90: 027a 2654 6573 744d 6170 436c 7573 7465  .z&TestMapCluste
+00001da0: 7265 722e 7465 7374 5f67 6574 5f61 7265  rer.test_get_are
+00001db0: 615f 636f 6e74 656e 7463 0100 0000 0000  a_contentc......
+00001dc0: 0000 0000 0000 0b00 0000 0900 0000 4300  ..............C.
+00001dd0: 0000 7364 0000 0064 017d 0174 0044 005d  ..sd...d.}.t.D.]
+00001de0: 567d 0274 0144 005d 4c7d 037c 00a0 02a1  V}.t.D.]L}.|....
+00001df0: 007d 047c 0444 005d 3a7d 057c 00a0 037c  .}.|.D.]:}.|...|
+00001e00: 037c 017c 027c 05a1 047d 0674 047c 0683  .|.|.|...}.t.|..
+00001e10: 017d 0774 057d 087c 07a0 067c 08a1 017d  .}.t.}.|...|...}
+00001e20: 0964 027d 0a7c 00a0 077c 097c 0aa1 0201  .d.}.|...|.|....
+00001e30: 0071 2071 1071 0864 0053 0029 034e 7231  .q q.q.d.S.).Nr1
+00001e40: 0000 0061 0301 0000 2820 5354 5f49 6e74  ...a....( ST_Int
+00001e50: 6572 7365 6374 7328 636f 6f72 6469 6e61  ersects(coordina
+00001e60: 7465 732c 2053 545f 4765 6f6d 6574 7279  tes, ST_Geometry
+00001e70: 4672 6f6d 5465 7874 2827 504f 4c59 474f  FromText('POLYGO
+00001e80: 4e20 2828 3939 3038 3532 2e35 3438 3139  N ((990852.54819
+00001e90: 3339 3934 3120 3635 3339 3635 302e 3638  39941 6539650.68
+00001ea0: 3930 3732 3839 392c 2039 3930 3835 322e  9072899, 990852.
+00001eb0: 3534 3831 3933 3939 3431 2035 3938 3032  5481939941 59802
+00001ec0: 3237 2e31 3032 3032 3834 3238 2c20 3135  27.102028428, 15
+00001ed0: 3539 3837 362e 3232 3739 3935 3930 3238  59876.2279959028
+00001ee0: 2035 3938 3032 3237 2e31 3032 3032 3834   5980227.1020284
+00001ef0: 3238 2c20 3135 3539 3837 362e 3232 3739  28, 1559876.2279
+00001f00: 3935 3930 3238 2036 3533 3936 3530 2e36  959028 6539650.6
+00001f10: 3839 3037 3238 3939 2c20 3939 3038 3532  89072899, 990852
+00001f20: 2e35 3438 3139 3339 3934 3120 3635 3339  .5481939941 6539
+00001f30: 3635 302e 3638 3930 3732 3839 3929 2927  650.689072899))'
+00001f40: 2c20 3338 3537 2920 2920 2929 0872 0b00  , 3857) ) )).r..
+00001f50: 0000 720e 0000 0072 1e00 0000 7220 0000  ..r....r....r ..
+00001f60: 0072 0900 0000 7212 0000 005a 1567 6574  .r....r....Z.get
+00001f70: 5f67 656f 6d5f 6669 6c74 6572 7374 7269  _geom_filterstri
+00001f80: 6e67 7221 0000 0029 0b72 2700 0000 722c  ngr!...).r'...r,
+00001f90: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00001fa0: 0000 722b 0000 0072 2200 0000 722d 0000  ..r+...r"...r-..
+00001fb0: 0072 3800 0000 5a11 6765 6f6d 5f66 696c  .r8...Z.geom_fil
+00001fc0: 7465 7273 7472 696e 67da 0f65 7870 6563  terstring..expec
+00001fd0: 7465 645f 7374 7269 6e67 722e 0000 0072  ted_stringr....r
+00001fe0: 2e00 0000 722f 0000 00da 1a74 6573 745f  ....r/.....test_
+00001ff0: 6765 745f 6765 6f6d 5f66 696c 7465 7273  get_geom_filters
+00002000: 7472 696e 676c 0100 0073 1600 0000 0002  tringl...s......
+00002010: 0402 0801 0803 0801 0802 1002 0802 0402  ................
+00002020: 0a02 0402 7a2b 5465 7374 4d61 7043 6c75  ....z+TestMapClu
+00002030: 7374 6572 6572 2e74 6573 745f 6765 745f  sterer.test_get_
+00002040: 6765 6f6d 5f66 696c 7465 7273 7472 696e  geom_filterstrin
+00002050: 6763 0100 0000 0000 0000 0000 0000 0c00  gc..............
+00002060: 0000 0900 0000 4300 0000 7388 0000 0064  ......C...s....d
+00002070: 017d 0174 0044 005d 7a7d 0274 0144 005d  .}.t.D.]z}.t.D.]
+00002080: 707d 037c 00a0 02a1 007d 047c 0444 005d  p}.|.....}.|.D.]
+00002090: 5e7d 057c 00a0 037c 037c 017c 027c 05a1  ^}.|...|.|.|.|..
+000020a0: 047d 0674 047c 0683 017d 0774 057d 087c  .}.t.|...}.t.}.|
+000020b0: 07a0 067c 0864 027c 01a1 037d 097c 00a0  ...|.d.|...}.|..
+000020c0: 0774 087c 0983 0164 03a1 0201 007c 0964  .t.|...d.....|.d
+000020d0: 0419 007d 0a7c 07a0 097c 0a7c 01a1 027d  ...}.|...|.|...}
+000020e0: 0b7c 00a0 077c 0b64 05a1 0201 0071 2071  .|...|.d.....q q
+000020f0: 1071 0864 0053 0029 064e e90a 0000 00da  .q.d.S.).N......
+00002100: 0461 7265 6172 3100 0000 7201 0000 00e9  .arear1...r.....
+00002110: 1e00 0000 290a 720b 0000 0072 0e00 0000  ....).r....r....
+00002120: 721e 0000 0072 2000 0000 7209 0000 0072  r....r ...r....r
+00002130: 1100 0000 7240 0000 0072 2100 0000 7234  ....r@...r!...r4
+00002140: 0000 005a 0b63 616c 6375 6c61 7465 5f6b  ...Z.calculate_k
+00002150: 290c 7227 0000 0072 2c00 0000 7228 0000  ).r'...r,...r(..
+00002160: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+00002170: 7222 0000 0072 2d00 0000 7238 0000 0072  r"...r-...r8...r
+00002180: 3900 0000 da04 6765 6f73 da01 6b72 2e00  9.....geos..kr..
+00002190: 0000 722e 0000 0072 2f00 0000 da10 7465  ..r....r/.....te
+000021a0: 7374 5f63 616c 6375 6c61 7465 5f6b 8401  st_calculate_k..
+000021b0: 0000 731a 0000 0000 0204 0208 0108 0208  ..s.............
+000021c0: 0108 0210 0208 0204 020e 0210 0208 020c  ................
+000021d0: 027a 2154 6573 744d 6170 436c 7573 7465  .z!TestMapCluste
+000021e0: 7265 722e 7465 7374 5f63 616c 6375 6c61  rer.test_calcula
+000021f0: 7465 5f6b 6301 0000 0000 0000 0000 0000  te_kc...........
+00002200: 000b 0000 0009 0000 0043 0000 0073 c800  .........C...s..
+00002210: 0000 7400 7d01 7401 4400 5dba 7d02 7402  ..t.}.t.D.].}.t.
+00002220: 4400 5db0 7d03 7c00 a003 a100 7d04 7c04  D.].}.|.....}.|.
+00002230: 4400 5d9e 7d05 7c00 a004 7c02 7c01 7c03  D.].}.|...|.|.|.
+00002240: 7c05 a104 7d06 7405 7c06 8301 7d07 7406  |...}.t.|...}.t.
+00002250: 7d08 7c07 a007 7c08 7c02 7c01 a103 7d09  }.|...|.|.|...}.
+00002260: 7c00 a008 7409 7c09 8301 6401 6b04 a101  |...t.|...d.k...
+00002270: 0100 7c00 a00a 7c07 6a0b 6a0c 7c01 a102  ..|...|.j.j.|...
+00002280: 0100 7c00 a00a 7c07 6a0b 6a0d 7c03 a102  ..|...|.j.j.|...
+00002290: 0100 7c00 a00a 7c07 6a0b 6a0e 7c02 a102  ..|...|.j.j.|...
+000022a0: 0100 7c00 a00a 7c07 6a0b 6a0f 7c05 a102  ..|...|.j.j.|...
+000022b0: 0100 7c07 a007 7c08 7c02 7c01 a103 7d0a  ..|...|.|.|...}.
+000022c0: 7c00 a00a 7409 7c0a 8301 6401 a102 0100  |...t.|...d.....
+000022d0: 7120 7110 7108 6400 5300 724b 0000 0029  q q.q.d.S.rK...)
+000022e0: 1072 1f00 0000 720e 0000 0072 0b00 0000  .r....r....r....
+000022f0: 721e 0000 0072 2000 0000 7209 0000 0072  r....r ...r....r
+00002300: 1200 0000 7240 0000 0072 3500 0000 7234  ....r@...r5...r4
+00002310: 0000 0072 2100 0000 7222 0000 0072 2c00  ...r!...r"...r,.
+00002320: 0000 7228 0000 0072 2900 0000 722b 0000  ..r(...r)...r+..
+00002330: 0029 0b72 2700 0000 722c 0000 0072 2900  .).r'...r,...r).
+00002340: 0000 7228 0000 0072 2a00 0000 722b 0000  ..r(...r*...r+..
+00002350: 0072 2200 0000 722d 0000 0072 3800 0000  .r"...r-...r8...
+00002360: 7241 0000 005a 1863 6163 6865 5f63 6c75  rA...Z.cache_clu
+00002370: 7374 6572 5f67 656f 6d65 7472 6965 7372  ster_geometriesr
+00002380: 2e00 0000 722e 0000 0072 2f00 0000 da17  ....r....r/.....
+00002390: 7465 7374 5f73 616d 655f 7265 7175 6573  test_same_reques
+000023a0: 745f 7477 6963 659f 0100 0073 3000 0000  t_twice....s0...
+000023b0: 0002 0402 0801 0803 0801 0802 1002 0802  ................
+000023c0: 0402 0401 0200 0200 02ff 0403 1201 1001  ................
+000023d0: 1001 1001 1002 0401 0200 0200 02ff 0403  ................
+000023e0: 7a28 5465 7374 4d61 7043 6c75 7374 6572  z(TestMapCluster
+000023f0: 6572 2e74 6573 745f 7361 6d65 5f72 6571  er.test_same_req
+00002400: 7565 7374 5f74 7769 6365 6301 0000 0000  uest_twicec.....
+00002410: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
+00002420: 0000 0073 7a00 0000 7400 6a01 a002 a100  ...sz...t.j.....
+00002430: a003 a100 7d01 7c00 a004 a100 7d02 7c02  ....}.|.....}.|.
+00002440: 4400 5d5a 7d03 7c00 a005 7406 7407 7408  D.]Z}.|...t.t.t.
+00002450: 7c03 a104 7d04 7409 7c04 8301 7d05 7c05  |...}.t.|...}.|.
+00002460: a00a 7c01 6a0b a101 7d06 7c05 a00c a100  ..|.j...}.|.....
+00002470: 4400 5d28 7d07 7c07 6401 6b02 725a 6402  D.](}.|.d.k.rZd.
+00002480: 7d07 7c00 a00d 740e 7c01 7c07 8302 740e  }.|...t.|.|...t.
+00002490: 7c06 7c07 8302 a102 0100 714a 711a 6400  |.|.......qJq.d.
+000024a0: 5300 2903 4e72 5800 0000 da0b 636f 6f72  S.).NrX.....coor
+000024b0: 6469 6e61 7465 7329 0f72 1800 0000 da07  dinates).r......
+000024c0: 6f62 6a65 6374 73da 0361 6c6c da05 6669  objects..all..fi
+000024d0: 7273 7472 1e00 0000 7220 0000 0072 0c00  rstr....r ...r..
+000024e0: 0000 721f 0000 0072 1000 0000 7209 0000  ..r....r....r...
+000024f0: 005a 1367 6574 5f64 6174 6173 6574 5f63  .Z.get_dataset_c
+00002500: 6f6e 7465 6e74 7252 0000 0072 5900 0000  ontentrR...rY...
+00002510: 7221 0000 00da 0767 6574 6174 7472 2908  r!.....getattr).
+00002520: 7227 0000 00da 0667 6172 6465 6e72 2a00  r'.....gardenr*.
+00002530: 0000 722b 0000 0072 2200 0000 722d 0000  ..r+...r"...r-..
+00002540: 005a 0767 6172 6465 6e5f da0a 6669 656c  .Z.garden_..fiel
+00002550: 645f 6e61 6d65 722e 0000 0072 2e00 0000  d_namer....r....
+00002560: 722f 0000 00da 1874 6573 745f 6765 745f  r/.....test_get_
+00002570: 6461 7461 7365 745f 636f 6e74 656e 74bf  dataset_content.
+00002580: 0100 0073 1400 0000 0002 0e02 0801 0802  ...s............
+00002590: 1001 0802 0c02 0c02 0801 0402 7a29 5465  ............z)Te
+000025a0: 7374 4d61 7043 6c75 7374 6572 6572 2e74  stMapClusterer.t
+000025b0: 6573 745f 6765 745f 6461 7461 7365 745f  est_get_dataset_
+000025c0: 636f 6e74 656e 7463 0100 0000 0000 0000  contentc........
+000025d0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+000025e0: 7304 0000 0064 0053 0072 3c00 0000 722e  s....d.S.r<...r.
+000025f0: 0000 00a9 0172 2700 0000 722e 0000 0072  .....r'...r....r
+00002600: 2e00 0000 722f 0000 00da 1374 6573 745f  ....r/.....test_
+00002610: 7061 6e6e 6564 5f72 6571 7565 7374 d201  panned_request..
+00002620: 0000 7302 0000 0000 017a 2454 6573 744d  ..s......z$TestM
+00002630: 6170 436c 7573 7465 7265 722e 7465 7374  apClusterer.test
+00002640: 5f70 616e 6e65 645f 7265 7175 6573 7463  _panned_requestc
+00002650: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002660: 0100 0000 4300 0000 7304 0000 0064 0053  ....C...s....d.S
+00002670: 0072 3c00 0000 722e 0000 0072 7900 0000  .r<...r....ry...
+00002680: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
+00002690: 1774 6573 745f 7a6f 6f6d 5f6c 6576 656c  .test_zoom_level
+000026a0: 5f63 6861 6e67 6564 d501 0000 7302 0000  _changed....s...
+000026b0: 0000 017a 2854 6573 744d 6170 436c 7573  ...z(TestMapClus
+000026c0: 7465 7265 722e 7465 7374 5f7a 6f6f 6d5f  terer.test_zoom_
+000026d0: 6c65 7665 6c5f 6368 616e 6765 6463 0100  level_changedc..
+000026e0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000026f0: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
+00002700: 3c00 0000 722e 0000 0072 7900 0000 722e  <...r....ry...r.
+00002710: 0000 0072 2e00 0000 722f 0000 00da 1874  ...r....r/.....t
+00002720: 6573 745f 636c 7573 7465 7274 7970 655f  est_clustertype_
+00002730: 6368 616e 6765 64d8 0100 0073 0200 0000  changed....s....
+00002740: 0001 7a29 5465 7374 4d61 7043 6c75 7374  ..z)TestMapClust
+00002750: 6572 6572 2e74 6573 745f 636c 7573 7465  erer.test_cluste
+00002760: 7274 7970 655f 6368 616e 6765 6463 0100  rtype_changedc..
+00002770: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00002780: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
+00002790: 3c00 0000 722e 0000 0072 7900 0000 722e  <...r....ry...r.
+000027a0: 0000 0072 2e00 0000 722f 0000 00da 1074  ...r....r/.....t
+000027b0: 6573 745f 636c 6561 725f 6361 6368 65db  est_clear_cache.
+000027c0: 0100 0073 0200 0000 0001 7a21 5465 7374  ...s......z!Test
+000027d0: 4d61 7043 6c75 7374 6572 6572 2e74 6573  MapClusterer.tes
+000027e0: 745f 636c 6561 725f 6361 6368 654e 2919  t_clear_cacheN).
+000027f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00002800: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00002810: 6d65 5f5f 7230 0000 0072 3200 0000 723b  me__r0...r2...r;
+00002820: 0000 0072 3e00 0000 723f 0000 0072 4200  ...r>...r?...rB.
+00002830: 0000 724a 0000 0072 4e00 0000 724f 0000  ..rJ...rN...rO..
+00002840: 0072 5100 0000 725b 0000 0072 5c00 0000  .rQ...r[...r\...
+00002850: 7265 0000 0072 6700 0000 7269 0000 0072  re...rg...ri...r
+00002860: 6f00 0000 7270 0000 0072 7800 0000 727a  o...rp...rx...rz
+00002870: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
+00002880: 0000 722e 0000 0072 2e00 0000 722e 0000  ..r....r....r...
+00002890: 0072 2f00 0000 721b 0000 0014 0000 0073  .r/...r........s
+000028a0: 2c00 0000 0803 0815 0812 0822 0816 0813  ,.........."....
+000028b0: 0817 0825 0817 0815 0813 0816 0815 0826  ...%...........&
+000028c0: 0817 0818 081b 0820 0813 0803 0803 0803  ....... ........
+000028d0: 721b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000028e0: 0000 0000 0000 0200 0000 4000 0000 7334  ..........@...s4
+000028f0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00002900: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+00002910: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
+00002920: 005a 0764 0b53 0029 0cda 1d54 6573 744d  .Z.d.S.)...TestM
+00002930: 6170 436c 7573 7465 7265 7243 6f6e 7465  apClustererConte
+00002940: 6e74 436f 756e 7473 6301 0000 0000 0000  ntCountsc.......
+00002950: 0000 0000 000f 0000 000a 0000 0043 0000  .............C..
+00002960: 0073 cc01 0000 6401 7d01 6402 6403 6404  .s....d.}.d.d.d.
+00002970: 6405 9c03 6701 7d02 6406 6407 6408 6404  d...g.}.d.d.d.d.
+00002980: 6405 9c03 6701 6901 6406 6407 6408 6409  d...g.i.d.d.d.d.
+00002990: 6405 9c03 6701 6901 640a 9c02 7d03 6407  d...g.i.d...}.d.
+000029a0: 6408 6404 6405 9c03 6407 6408 6409 6405  d.d.d...d.d.d.d.
+000029b0: 9c03 640a 9c02 7d04 7400 4400 9001 5d6e  ..d...}.t.D...]n
+000029c0: 7d05 7401 4400 9001 5d62 7d06 7402 7403  }.t.D...]b}.t.t.
+000029d0: 7404 7405 6604 4400 9001 5d4e 7d07 7c05  t.t.f.D...]N}.|.
+000029e0: 7406 6b02 728a 7c06 7407 6b03 728a 7172  t.k.r.|.t.k.r.qr
+000029f0: 7c06 7407 6b02 729c 7c07 7403 6b03 729c  |.t.k.r.|.t.k.r.
+00002a00: 7172 7c00 a008 7c06 7c01 7c05 7c02 a104  qr|...|.|.|.|...
+00002a10: 7d08 7409 7c08 740a 640b 8d02 7d09 7c09  }.t.|.t.d...}.|.
+00002a20: a00b 7c07 7c06 7c02 7c01 7c03 a105 7d0a  ..|.|.|.|.|...}.
+00002a30: 7c09 a00b 7c07 7c06 7c02 7c01 7c04 a105  |...|.|.|.|.|...
+00002a40: 0400 7d0b 7d0a 640c 640d 640c 6901 640d  ..}.}.d.d.d.i.d.
+00002a50: 640c 6901 640a 9c02 640e 9c02 7d0c 7c00  d.i.d...d...}.|.
+00002a60: a00c 7c0a 7c0c a102 0100 7c00 a00c 7c0b  ..|.|.....|...|.
+00002a70: 7c0c a102 0100 7c06 7407 6b02 9001 728a  |.....|.t.k...r.
+00002a80: 7c00 a00d 640f 6403 a102 0100 7c00 a00d  |...d.d.....|...
+00002a90: 6410 6411 a102 0100 7c09 a00b 7c07 7c06  d.d.....|...|.|.
+00002aa0: 7c02 7c01 7c03 a105 7d0a 7c09 a00b 7c07  |.|.|...}.|...|.
+00002ab0: 7c06 7c02 7c01 7c04 a105 0400 7d0b 7d0a  |.|.|.|.....}.}.
+00002ac0: 6412 640d 640c 6901 640d 6412 6901 640a  d.d.d.i.d.d.i.d.
+00002ad0: 9c02 640e 9c02 7d0c 7c00 a00c 7c0a 7c0c  ..d...}.|...|.|.
+00002ae0: a102 0100 7c00 a00c 7c0b 7c0c a102 0100  ....|...|.|.....
+00002af0: 740e 6a0f a010 a100 7d0d 7c0d 4400 5d0e  t.j.....}.|.D.].
+00002b00: 7d0e 7c0e a011 a100 0100 9001 7198 740e  }.|.........q.t.
+00002b10: 6a0f a010 a100 7d0d 7c00 a00c 7c0d a012  j.....}.|...|...
+00002b20: a100 640c a102 0100 7172 7160 7156 6400  ..d.....qrq`qVd.
+00002b30: 5300 2913 4e72 6a00 0000 7254 0000 00da  S.).Nrj...rT....
+00002b40: 0573 746f 6e65 fa01 3da9 03da 0663 6f6c  .stone..=....col
+00002b50: 756d 6eda 0576 616c 7565 da08 6f70 6572  umn..value..oper
+00002b60: 6174 6f72 722b 0000 0072 5600 0000 547a  atorr+...rV...Tz
+00002b70: 0221 3d29 02da 0466 7265 655a 0470 6169  .!=)...freeZ.pai
+00002b80: 64a9 0172 2500 0000 7201 0000 0072 6100  d..r%...r....ra.
+00002b90: 0000 2902 7261 0000 00da 0b6d 6f64 756c  ..).ra.....modul
+00002ba0: 6174 696f 6e73 fa06 6e61 6d65 2031 fa06  ations..name 1..
+00002bb0: 6e61 6d65 2032 da06 666c 6f77 6572 7231  name 2..flowerr1
+00002bc0: 0000 0029 1372 0b00 0000 720e 0000 0072  ...).r....r....r
+00002bd0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00002be0: 0000 0072 1000 0000 720c 0000 0072 2000  ...r....r....r .
+00002bf0: 0000 7209 0000 00da 0e54 4553 545f 4752  ..r......TEST_GR
+00002c00: 4944 5f53 495a 455a 1667 6574 5f6d 6170  ID_SIZEZ.get_map
+00002c10: 5f63 6f6e 7465 6e74 5f63 6f75 6e74 7372  _content_countsr
+00002c20: 2100 0000 da0c 6372 6561 7465 5f70 6f69  !.....create_poi
+00002c30: 6e74 7218 0000 0072 7200 0000 7273 0000  ntr....rr...rs..
+00002c40: 00da 0664 656c 6574 6572 6100 0000 290f  ...deletera...).
+00002c50: 7227 0000 0072 2c00 0000 722b 0000 0072  r'...r,...r+...r
+00002c60: 8a00 0000 5a12 7369 6d70 6c65 5f6d 6f64  ....Z.simple_mod
+00002c70: 756c 6174 696f 6e73 7228 0000 0072 2900  ulationsr(...r).
+00002c80: 0000 7238 0000 0072 2200 0000 722d 0000  ..r8...r"...r-..
+00002c90: 00da 0672 6573 756c 745a 1e72 6573 756c  ...resultZ.resul
+00002ca0: 745f 6672 6f6d 5f73 696d 706c 655f 6d6f  t_from_simple_mo
+00002cb0: 6475 6c61 7469 6f6e 73da 0f65 7870 6563  dulations..expec
+00002cc0: 7465 645f 7265 7375 6c74 da07 6761 7264  ted_result..gard
+00002cd0: 656e 7372 7600 0000 722e 0000 0072 2e00  ensrv...r....r..
+00002ce0: 0000 722f 0000 00da 1b74 6573 745f 6765  ..r/.....test_ge
+00002cf0: 745f 6d61 705f 636f 6e74 656e 745f 636f  t_map_content_co
+00002d00: 756e 7473 e201 0000 73a6 0000 0000 0204  unts....s.......
+00002d10: 0502 0102 0102 fd04 ff04 0b02 0202 0102  ................
+00002d20: 0102 fd04 ff02 fe02 0b02 0202 0102 0102  ................
+00002d30: fd04 ff02 ff02 f506 1802 0102 0102 fd04  ................
+00002d40: 0602 0102 0102 fd04 fa06 0e0a 010a 0212  ................
+00002d50: 0210 0102 0210 0102 0210 010c 0212 0206  ................
+00002d60: 0102 0002 0002 0002 ff08 0402 0302 0002  ................
+00002d70: ff02 0402 0002 ff02 fc04 fe06 0b0c 010c  ................
+00002d80: 020a 020c 010c 0212 0106 0102 0002 0002  ................
+00002d90: 0002 ff08 0402 0302 0002 ff02 0402 0002  ................
+00002da0: ff02 fc04 fe06 0e0c 010c 020a 0108 010c  ................
+00002db0: 030a 027a 3954 6573 744d 6170 436c 7573  ...z9TestMapClus
+00002dc0: 7465 7265 7243 6f6e 7465 6e74 436f 756e  tererContentCoun
+00002dd0: 7473 2e74 6573 745f 6765 745f 6d61 705f  ts.test_get_map_
+00002de0: 636f 6e74 656e 745f 636f 756e 7473 6301  content_countsc.
+00002df0: 0000 0000 0000 0000 0000 000c 0000 0006  ................
+00002e00: 0000 0043 0000 0073 3201 0000 6401 7d01  ...C...s2...d.}.
+00002e10: 7400 7d02 7401 7d03 6700 7d04 7c00 a002  t.}.t.}.g.}.|...
+00002e20: 7c02 7c01 7c03 7c04 a104 7d05 7403 7c05  |.|.|.|...}.t.|.
+00002e30: 7404 6402 8d02 7d06 7405 7d07 7c06 a006  t.d...}.t.}.|...
+00002e40: 7c07 7c02 7c01 a103 7d08 7c06 a007 7c08  |.|.|...}.|...|.
+00002e50: 7c04 a102 7d09 7c00 a008 7c09 6403 a102  |...}.|...|.d...
+00002e60: 0100 7c00 a009 6404 6405 a102 0100 7c06  ..|...d.d.....|.
+00002e70: a007 7c08 7c04 a102 7d09 7c00 a008 7c09  ..|.|...}.|...|.
+00002e80: 6406 a102 0100 7c00 a009 6407 6408 a102  d.....|...d.d...
+00002e90: 0100 7c06 a007 7c08 7c04 a102 7d09 7c00  ..|...|.|...}.|.
+00002ea0: a008 7c09 6409 a102 0100 640a 6405 640b  ..|.d.....d.d.d.
+00002eb0: 640c 9c03 6701 7d04 7c06 a007 7c08 7c04  d...g.}.|...|.|.
+00002ec0: a102 7d09 7c00 a008 7c09 6406 a102 0100  ..}.|...|.d.....
+00002ed0: 640a 6405 640b 640c 9c03 640a 6408 640b  d.d.d.d...d.d.d.
+00002ee0: 640d 640e 9c04 6702 7d04 7c06 a007 7c08  d.d...g.}.|...|.
+00002ef0: 7c04 a102 7d09 7c00 a008 7c09 6409 a102  |...}.|...|.d...
+00002f00: 0100 740a 6a0b a00c a100 7d0a 7c0a 4400  ..t.j.....}.|.D.
+00002f10: 5d0e 7d0b 7c0b a00d a100 0100 9001 7104  ].}.|.........q.
+00002f20: 740a 6a0b a00c a100 7d0a 7c00 a008 7c0a  t.j.....}.|...|.
+00002f30: a00e a100 6403 a102 0100 6400 5300 290f  ....d.....d.S.).
+00002f40: 4e72 6a00 0000 7289 0000 0072 0100 0000  Nrj...r....r....
+00002f50: 728b 0000 0072 8200 0000 7231 0000 0072  r....r....r1...r
+00002f60: 8c00 0000 728d 0000 0072 3300 0000 7254  ....r....r3...rT
+00002f70: 0000 0072 8300 0000 7284 0000 00da 024f  ...r....r......O
+00002f80: 5229 0472 8500 0000 7286 0000 0072 8700  R).r....r....r..
+00002f90: 0000 da0f 6c6f 6769 6361 6c4f 7065 7261  ....logicalOpera
+00002fa0: 746f 7229 0f72 0c00 0000 720f 0000 0072  tor).r....r....r
+00002fb0: 2000 0000 7209 0000 0072 8e00 0000 7212   ...r....r....r.
+00002fc0: 0000 00da 1b67 6574 5f67 656f 6d65 7472  .....get_geometr
+00002fd0: 6965 735f 666f 725f 636f 756e 7469 6e67  ies_for_counting
+00002fe0: 5a17 7175 6572 795f 6d61 705f 636f 6e74  Z.query_map_cont
+00002ff0: 656e 745f 636f 756e 7472 2100 0000 728f  ent_countr!...r.
+00003000: 0000 0072 1800 0000 7272 0000 0072 7300  ...r....rr...rs.
+00003010: 0000 7290 0000 0072 6100 0000 290c 7227  ..r....ra...).r'
+00003020: 0000 0072 2c00 0000 7229 0000 0072 2800  ...r,...r)...r(.
+00003030: 0000 722b 0000 0072 2200 0000 722d 0000  ..r+...r"...r-..
+00003040: 0072 3800 0000 5a17 6765 6f6d 6574 7269  .r8...Z.geometri
+00003050: 6573 5f66 6f72 5f63 6f75 6e74 696e 6772  es_for_countingr
+00003060: 6100 0000 7293 0000 0072 7600 0000 722e  a...r....rv...r.
+00003070: 0000 0072 2e00 0000 722f 0000 00da 1c74  ...r....r/.....t
+00003080: 6573 745f 7175 6572 795f 6d61 705f 636f  est_query_map_co
+00003090: 6e74 656e 745f 636f 756e 7458 0200 0073  ntent_countX...s
+000030a0: 5000 0000 0002 0401 0401 0403 0402 1001  P...............
+000030b0: 0c02 0402 0e02 0c01 0c02 0c02 0c01 0c02  ................
+000030c0: 0c02 0c01 0c05 0201 0201 02fd 04ff 0408  ................
+000030d0: 0c01 0c04 0201 0201 02fd 0406 0201 0201  ................
+000030e0: 0201 02fc 04fa 040e 0c01 0c02 0a01 0801  ................
+000030f0: 0c03 0a02 7a3a 5465 7374 4d61 7043 6c75  ....z:TestMapClu
+00003100: 7374 6572 6572 436f 6e74 656e 7443 6f75  stererContentCou
+00003110: 6e74 732e 7465 7374 5f71 7565 7279 5f6d  nts.test_query_m
+00003120: 6170 5f63 6f6e 7465 6e74 5f63 6f75 6e74  ap_content_count
+00003130: 6301 0000 0000 0000 0000 0000 000a 0000  c...............
+00003140: 0009 0000 0043 0000 0073 aa00 0000 6401  .....C...s....d.
+00003150: 7d01 7400 4400 5d9c 7d02 7401 4400 5d92  }.t.D.].}.t.D.].
+00003160: 7d03 7402 7403 7404 7405 6604 4400 5d80  }.t.t.t.t.f.D.].
+00003170: 7d04 7c02 7406 6b02 7236 7c03 7407 6b03  }.|.t.k.r6|.t.k.
+00003180: 7236 7120 7c03 7407 6b02 7248 7c04 7403  r6q |.t.k.rH|.t.
+00003190: 6b03 7248 7120 6700 7d05 7c00 a008 7c03  k.rHq g.}.|...|.
+000031a0: 7c01 7c02 7c05 a104 7d06 7409 7c06 740a  |.|.|...}.t.|.t.
+000031b0: 6402 8d02 7d07 7c07 a00b 7c04 7c03 7c01  d...}.|...|.|.|.
+000031c0: a103 7d08 7c00 a00c 740d 7c08 740e 8302  ..}.|...t.|.t...
+000031d0: a101 0100 7c08 4400 5d14 7d09 7c00 a00c  ....|.D.].}.|...
+000031e0: 6403 7c09 6a0f 6b06 a101 0100 718a 7120  d.|.j.k.....q.q 
+000031f0: 7110 7108 6400 5300 2904 4e72 6a00 0000  q.q.d.S.).Nrj...
+00003200: 7289 0000 00da 0750 4f4c 5947 4f4e 2910  r......POLYGON).
+00003210: 720b 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
+00003220: 1200 0000 7213 0000 0072 1400 0000 7210  ....r....r....r.
+00003230: 0000 0072 0c00 0000 7220 0000 0072 0900  ...r....r ...r..
+00003240: 0000 728e 0000 0072 9700 0000 7235 0000  ..r....r....r5..
+00003250: 0072 3600 0000 7263 0000 00da 0377 6b74  .r6...rc.....wkt
+00003260: 290a 7227 0000 0072 2c00 0000 7228 0000  ).r'...r,...r(..
+00003270: 0072 2900 0000 7238 0000 0072 2b00 0000  .r)...r8...r+...
+00003280: 7222 0000 0072 2d00 0000 7239 0000 0072  r"...r-...r9...r
+00003290: 4300 0000 722e 0000 0072 2e00 0000 722f  C...r....r....r/
+000032a0: 0000 00da 2074 6573 745f 6765 745f 6765  .... test_get_ge
+000032b0: 6f6d 6574 7269 6573 5f66 6f72 5f63 6f75  ometries_for_cou
+000032c0: 6e74 696e 679c 0200 0073 1e00 0000 0002  nting....s......
+000032d0: 0402 0801 0802 1002 1001 0202 1001 0202  ................
+000032e0: 0402 1001 0c02 0e02 1002 0802 7a3e 5465  ............z>Te
+000032f0: 7374 4d61 7043 6c75 7374 6572 6572 436f  stMapClustererCo
+00003300: 6e74 656e 7443 6f75 6e74 732e 7465 7374  ntentCounts.test
+00003310: 5f67 6574 5f67 656f 6d65 7472 6965 735f  _get_geometries_
+00003320: 666f 725f 636f 756e 7469 6e67 6301 0000  for_countingc...
+00003330: 0000 0000 0000 0000 000a 0000 0008 0000  ................
+00003340: 0043 0000 0073 8e00 0000 6700 7d01 6401  .C...s....g.}.d.
+00003350: 7d02 7400 4400 5d7c 7d03 7401 4400 5d72  }.t.D.]|}.t.D.]r
+00003360: 7d04 7c00 a002 7c04 7c02 7c03 7c01 a104  }.|...|.|.|.|...
+00003370: 7d05 7403 7c05 7404 6402 8d02 7d06 7c06  }.t.|.t.d...}.|.
+00003380: a005 7406 a101 7d07 7c06 a007 7c07 7c02  ..t...}.|...|.|.
+00003390: a102 7d08 7c00 a008 7409 7c08 8301 6403  ..}.|...t.|...d.
+000033a0: a102 0100 7c00 a008 7c08 6a0a 6404 a102  ....|...|.j.d...
+000033b0: 0100 7c08 a00b 6405 a101 0100 6406 7d09  ..|...d.....d.}.
+000033c0: 7c00 a008 7c09 7409 7c08 8301 a102 0100  |...|.t.|.......
+000033d0: 7114 710c 6400 5300 2907 4e72 6a00 0000  q.q.d.S.).Nrj...
+000033e0: 7289 0000 007a a753 5249 443d 3338 3537  r....z.SRID=3857
+000033f0: 3b50 4f4c 5947 4f4e 2028 2839 3738 3339  ;POLYGON ((97839
+00003400: 332e 3936 3230 3520 3539 3438 3633 352e  3.96205 5948635.
+00003410: 3238 3930 3136 2c20 3135 3635 3433 302e  289016, 1565430.
+00003420: 3333 3932 3820 3539 3438 3633 352e 3238  33928 5948635.28
+00003430: 3930 3136 2c20 3135 3635 3433 302e 3333  9016, 1565430.33
+00003440: 3932 3820 3635 3734 3830 372e 3432 3437  928 6574807.4247
+00003450: 3238 2c20 3937 3833 3933 2e39 3632 3035  28, 978393.96205
+00003460: 2036 3537 3438 3037 2e34 3234 3732 382c   6574807.424728,
+00003470: 2039 3738 3339 332e 3936 3230 3520 3539   978393.96205 59
+00003480: 3438 3633 352e 3238 3930 3136 2929 721d  48635.289016))r.
+00003490: 0000 0072 4400 0000 7ac5 5352 4944 3d34  ...rD...z.SRID=4
+000034a0: 3332 363b 504f 4c59 474f 4e20 2828 382e  326;POLYGON ((8.
 000034b0: 3738 3930 3632 3439 3939 3937 3720 3437  7890624999977 47
-000034c0: 2e30 3430 3138 3231 3433 3237 3838 3929  .04018214327889)
-000034d0: 2929 0c72 0b00 0000 720e 0000 0072 2000  )).r....r....r .
-000034e0: 0000 7209 0000 0072 8e00 0000 723e 0000  ..r....r....r>..
-000034f0: 0072 1200 0000 5a15 736e 6170 5f76 6965  .r....Z.snap_vie
-00003500: 7770 6f72 745f 746f 5f67 7269 6472 2100  wport_to_gridr!.
-00003510: 0000 da03 7374 7272 3800 0000 7249 0000  ....strr8...rI..
-00003520: 0029 0a72 2a00 0000 722e 0000 0072 2f00  .).r*...r....r/.
-00003530: 0000 722b 0000 0072 2c00 0000 7222 0000  ..r+...r,...r"..
-00003540: 0072 3000 0000 723a 0000 005a 0e67 7269  .r0...r:...Z.gri
-00003550: 645f 7265 6374 616e 676c 655a 0c70 6f6c  d_rectangleZ.pol
-00003560: 7967 6f6e 5f34 3332 3672 3100 0000 7231  ygon_4326r1...r1
-00003570: 0000 0072 3200 0000 da1a 7465 7374 5f73  ...r2.....test_s
-00003580: 6e61 705f 7669 6577 706f 7274 5f74 6f5f  nap_viewport_to_
-00003590: 6772 6964 a502 0000 731a 0000 0000 0204  grid....s.......
-000035a0: 0104 0208 0108 0210 020c 030a 020c 0210  ................
-000035b0: 010e 020a 0204 027a 3854 6573 744d 6170  .......z8TestMap
-000035c0: 436c 7573 7465 7265 7243 6f6e 7465 6e74  ClustererContent
-000035d0: 436f 756e 7473 2e74 6573 745f 736e 6170  Counts.test_snap
-000035e0: 5f76 6965 7770 6f72 745f 746f 5f67 7269  _viewport_to_gri
-000035f0: 6463 0100 0000 0000 0000 0000 0000 0c00  dc..............
-00003600: 0000 0a00 0000 4300 0000 73bc 0000 0064  ......C...s....d
-00003610: 017d 0167 007d 027c 00a0 0064 0264 03a1  .}.g.}.|...d.d..
-00003620: 0201 007c 00a0 0064 0464 05a1 0201 0074  ...|...d.d.....t
-00003630: 0144 005d 927d 0374 0244 005d 887d 0474  .D.].}.t.D.].}.t
-00003640: 0374 0474 0574 0666 0444 005d 767d 057c  .t.t.t.f.D.]v}.|
-00003650: 00a0 077c 047c 017c 037c 02a1 047d 0674  ...|.|.|.|...}.t
-00003660: 087c 0674 0964 068d 027d 0764 077d 087c  .|.t.d...}.d.}.|
-00003670: 07a0 0a7c 057c 047c 017c 027c 08a1 057d  ...|.|.|.|.|...}
-00003680: 097c 0474 0b6b 0272 9864 0864 0969 0164  .|.t.k.r.d.d.i.d
-00003690: 0864 0969 0164 0a9c 027d 0a7c 00a0 0c7c  .d.i.d...}.|...|
-000036a0: 097c 0aa1 0201 0074 0d6a 0ea0 0fa1 007d  .|.....t.j.....}
-000036b0: 0b7c 00a0 0c7c 0ba0 10a1 0064 0ba1 0201  .|...|.....d....
-000036c0: 0071 3c71 2c71 2464 0053 0029 0c4e 726a  .q<q,q$d.S.).Nrj
-000036d0: 0000 0072 8b00 0000 7282 0000 0072 8c00  ...r....r....r..
-000036e0: 0000 728d 0000 0072 8900 0000 7255 0000  ..r....r....rU..
-000036f0: 0072 6200 0000 7234 0000 0029 0272 8200  .rb...r4...).r..
-00003700: 0000 728d 0000 0072 3600 0000 2911 728f  ..r....r6...).r.
-00003710: 0000 0072 0b00 0000 720e 0000 0072 1100  ...r....r....r..
-00003720: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00003730: 0072 2000 0000 7209 0000 0072 8e00 0000  .r ...r....r....
-00003740: da18 6765 745f 6772 6f75 7065 645f 6d61  ..get_grouped_ma
-00003750: 705f 636f 6e74 656e 7473 720c 0000 0072  p_contentsr....r
-00003760: 2100 0000 7218 0000 0072 7200 0000 7273  !...r....rr...rs
-00003770: 0000 0072 6200 0000 290c 722a 0000 0072  ...rb...).r*...r
-00003780: 2f00 0000 722e 0000 0072 2b00 0000 722c  /...r....r+...r,
-00003790: 0000 0072 3900 0000 7222 0000 0072 3000  ...r9...r"...r0.
-000037a0: 0000 da08 6772 6f75 705f 6279 7291 0000  ....group_byr...
-000037b0: 0072 9200 0000 7293 0000 0072 3100 0000  .r....r....r1...
-000037c0: 7231 0000 0072 3200 0000 da1d 7465 7374  r1...r2.....test
-000037d0: 5f67 6574 5f67 726f 7570 6564 5f6d 6170  _get_grouped_map
-000037e0: 5f63 6f6e 7465 6e74 73bf 0200 0073 2c00  _contents....s,.
-000037f0: 0000 0002 0401 0402 0c01 0c02 0801 0802  ................
-00003800: 1002 1002 0c02 0402 1202 0804 0200 02ff  ................
-00003810: 0204 0200 02ff 02fc 0609 0c02 0a01 7a3b  ..............z;
-00003820: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
-00003830: 436f 6e74 656e 7443 6f75 6e74 732e 7465  ContentCounts.te
-00003840: 7374 5f67 6574 5f67 726f 7570 6564 5f6d  st_get_grouped_m
-00003850: 6170 5f63 6f6e 7465 6e74 734e 2908 727e  ap_contentsN).r~
-00003860: 0000 0072 7f00 0000 7280 0000 0072 9400  ...r....r....r..
-00003870: 0000 7298 0000 0072 9b00 0000 729d 0000  ..r....r....r...
-00003880: 0072 a000 0000 7231 0000 0072 3100 0000  .r....r1...r1...
-00003890: 7231 0000 0072 3200 0000 7281 0000 00e1  r1...r2...r.....
-000038a0: 0100 0073 0a00 0000 0801 0862 0844 081d  ...s.......b.D..
-000038b0: 081a 7281 0000 0072 5600 0000 7258 0000  ..r....rV...rX..
-000038c0: 0029 01da 2641 4e59 434c 5553 5445 525f  .)..&ANYCLUSTER_
-000038d0: 4144 4449 5449 4f4e 414c 5f47 524f 5550  ADDITIONAL_GROUP
-000038e0: 5f42 595f 434f 4c55 4d4e 5363 0000 0000  _BY_COLUMNSc....
-000038f0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00003900: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00003910: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00003920: 0464 0553 0029 06da 2354 6573 744d 6170  .d.S.)..#TestMap
-00003930: 436c 7573 7465 7265 7241 6c74 6572 6e61  ClustererAlterna
-00003940: 7469 7665 5365 7474 696e 6773 6301 0000  tiveSettingsc...
-00003950: 0000 0000 0000 0000 000a 0000 0009 0000  ................
-00003960: 0043 0000 0073 6600 0000 6401 7d01 6700  .C...sf...d.}.g.
-00003970: 7d02 7400 4400 5d54 7d03 7401 4400 5d4a  }.t.D.]T}.t.D.]J
-00003980: 7d04 7402 7403 7404 7405 6604 4400 5d38  }.t.t.t.t.f.D.]8
-00003990: 7d05 7c00 a006 7c04 7c01 7c03 7c02 a104  }.|...|.|.|.|...
-000039a0: 7d06 7407 7c06 7408 6402 8d02 7d07 7c07  }.t.|.t.d...}.|.
-000039b0: a009 a100 7d08 6403 7d09 7c00 a00a 7c08  ....}.d.}.|...|.
-000039c0: 7c09 a102 0100 7124 7114 710c 6400 5300  |.....q$q.q.d.S.
-000039d0: 2904 4e72 6a00 0000 7289 0000 007a 3a2c  ).Nrj...r....z:,
-000039e0: 204d 494e 2872 6174 696e 6729 2041 5320   MIN(rating) AS 
-000039f0: 7261 7469 6e67 2c20 4d49 4e28 6c61 7374  rating, MIN(last
-00003a00: 5f72 656e 6577 616c 2920 4153 206c 6173  _renewal) AS las
-00003a10: 745f 7265 6e65 7761 6c29 0b72 0b00 0000  t_renewal).r....
-00003a20: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00003a30: 1300 0000 7214 0000 0072 2000 0000 7209  ....r....r ...r.
-00003a40: 0000 0072 8e00 0000 5a26 6765 745f 6164  ...r....Z&get_ad
-00003a50: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
-00003a60: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
-00003a70: 7221 0000 0029 0a72 2a00 0000 722f 0000  r!...).r*...r/..
-00003a80: 0072 2e00 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
-00003a90: 7239 0000 0072 2200 0000 7230 0000 005a  r9...r"...r0...Z
-00003aa0: 0e63 6f6c 756d 6e73 5f73 7472 696e 6772  .columns_stringr
-00003ab0: 6800 0000 7231 0000 0072 3100 0000 7232  h...r1...r1...r2
-00003ac0: 0000 00da 2b74 6573 745f 6765 745f 6164  ....+test_get_ad
-00003ad0: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
-00003ae0: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
-00003af0: e902 0000 7314 0000 0000 0204 0104 0208  ....s...........
-00003b00: 0108 0210 0210 020c 0208 0204 017a 4f54  .............zOT
-00003b10: 6573 744d 6170 436c 7573 7465 7265 7241  estMapClustererA
-00003b20: 6c74 6572 6e61 7469 7665 5365 7474 696e  lternativeSettin
-00003b30: 6773 2e74 6573 745f 6765 745f 6164 6469  gs.test_get_addi
-00003b40: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
-00003b50: 636f 6c75 6d6e 735f 7374 7269 6e67 6301  columns_stringc.
-00003b60: 0000 0000 0000 0000 0000 000c 0000 000a  ................
-00003b70: 0000 0043 0000 0073 be00 0000 6401 7d01  ...C...s....d.}.
-00003b80: 6700 7d02 7c00 a000 6402 6403 a102 0100  g.}.|...d.d.....
-00003b90: 7c00 a000 6404 6405 a102 0100 7c00 a001  |...d.d.....|...
-00003ba0: 7402 7403 6406 8302 a101 0100 7404 4400  t.t.d.......t.D.
-00003bb0: 5d84 7d03 7405 4400 5d7a 7d04 7406 7407  ].}.t.D.]z}.t.t.
-00003bc0: 7408 7409 6604 4400 5d68 7d05 7c00 a00a  t.t.f.D.]h}.|...
-00003bd0: 7c04 7c01 7c03 7c02 a104 7d06 740b 7c06  |.|.|.|...}.t.|.
-00003be0: 740c 6407 8d02 7d07 6408 7d08 7c07 a00d  t.d...}.d.}.|...
-00003bf0: 7c05 7c04 7c01 7c02 7c08 a105 7d09 7c04  |.|.|.|.|...}.|.
-00003c00: 740e 6b02 724c 7c09 a00f a100 4400 5d20  t.k.rL|.....D.] 
-00003c10: 5c02 7d0a 7d0b 7c00 a010 6409 7c0b a102  \.}.}.|...d.|...
-00003c20: 0100 7c00 a010 640a 7c0b a102 0100 7192  ..|...d.|.....q.
-00003c30: 714c 713c 7134 6400 5300 290b 4e72 6a00  qLq<q4d.S.).Nrj.
-00003c40: 0000 728b 0000 0072 8200 0000 728c 0000  ..r....r....r...
-00003c50: 0072 8d00 0000 72a1 0000 0072 8900 0000  .r....r....r....
-00003c60: 7255 0000 0072 5600 0000 7258 0000 0029  rU...rV...rX...)
-00003c70: 1172 8f00 0000 7227 0000 00da 0768 6173  .r....r'.....has
-00003c80: 6174 7472 7205 0000 0072 0b00 0000 720e  attrr....r....r.
-00003c90: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00003ca0: 0000 7214 0000 0072 2000 0000 7209 0000  ..r....r ...r...
-00003cb0: 0072 8e00 0000 729e 0000 0072 0c00 0000  .r....r....r....
-00003cc0: da05 6974 656d 73da 0861 7373 6572 7449  ..items..assertI
-00003cd0: 6e29 0c72 2a00 0000 722f 0000 0072 2e00  n).r*...r/...r..
-00003ce0: 0000 722b 0000 0072 2c00 0000 7239 0000  ..r+...r,...r9..
-00003cf0: 0072 2200 0000 7230 0000 0072 9f00 0000  .r"...r0...r....
-00003d00: 7291 0000 00da 0961 6767 7265 6761 7465  r......aggregate
-00003d10: da04 6461 7461 7231 0000 0072 3100 0000  ..datar1...r1...
-00003d20: 7232 0000 00da 3074 6573 745f 6765 745f  r2....0test_get_
-00003d30: 6772 6f75 7065 645f 6d61 705f 636f 6e74  grouped_map_cont
-00003d40: 656e 7473 5f61 6464 6974 696f 6e61 6c5f  ents_additional_
-00003d50: 636f 6c75 6d6e 73fd 0200 0073 2000 0000  columns....s ...
-00003d60: 0002 0401 0402 0c01 0c02 1002 0801 0802  ................
-00003d70: 1002 1002 0c02 0402 1202 0802 1002 0c01  ................
-00003d80: 7a54 5465 7374 4d61 7043 6c75 7374 6572  zTTestMapCluster
-00003d90: 6572 416c 7465 726e 6174 6976 6553 6574  erAlternativeSet
-00003da0: 7469 6e67 732e 7465 7374 5f67 6574 5f67  tings.test_get_g
-00003db0: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
-00003dc0: 6e74 735f 6164 6469 7469 6f6e 616c 5f63  nts_additional_c
-00003dd0: 6f6c 756d 6e73 4e29 0572 7e00 0000 727f  olumnsN).r~...r.
-00003de0: 0000 0072 8000 0000 72a3 0000 0072 a900  ...r....r....r..
-00003df0: 0000 7231 0000 0072 3100 0000 7231 0000  ..r1...r1...r1..
-00003e00: 0072 3200 0000 72a2 0000 00e5 0200 0073  .r2...r........s
-00003e10: 0400 0000 0804 0814 72a2 0000 0029 27da  ........r....)'.
-00003e20: 0b64 6a61 6e67 6f2e 7465 7374 7202 0000  .django.testr...
-00003e30: 0072 0300 0000 7204 0000 00da 0b64 6a61  .r....r......dja
-00003e40: 6e67 6f2e 636f 6e66 7205 0000 00da 1764  ngo.confr......d
-00003e50: 6a61 6e67 6f2e 636f 6e74 7269 622e 6769  jango.contrib.gi
-00003e60: 732e 6765 6f73 7206 0000 00da 1764 6a61  s.geosr......dja
-00003e70: 6e67 6f2e 636f 6e74 7269 622e 6769 732e  ngo.contrib.gis.
-00003e80: 6764 616c 7207 0000 0072 0800 0000 5a17  gdalr....r....Z.
-00003e90: 616e 7963 6c75 7374 6572 2e4d 6170 436c  anycluster.MapCl
-00003ea0: 7573 7465 7265 7272 0900 0000 da0a 616e  ustererr......an
-00003eb0: 7963 6c75 7374 6572 720a 0000 00da 1661  yclusterr......a
-00003ec0: 6e79 636c 7573 7465 722e 6465 6669 6e69  nycluster.defini
-00003ed0: 7469 6f6e 7372 0b00 0000 720c 0000 0072  tionsr....r....r
-00003ee0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00003ef0: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
-00003f00: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
-00003f10: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00003f20: 5a17 616e 7963 6c75 7374 6572 2e74 6573  Z.anycluster.tes
-00003f30: 7473 2e6d 6978 696e 7372 1500 0000 7216  ts.mixinsr....r.
-00003f40: 0000 0072 1700 0000 5a0d 616e 796d 6170  ...r....Z.anymap
-00003f50: 2e6d 6f64 656c 7372 1800 0000 7247 0000  .modelsr....rG..
-00003f60: 0072 1f00 0000 728e 0000 0072 1b00 0000  .r....r....r....
-00003f70: 7281 0000 0072 a200 0000 7231 0000 0072  r....r....r1...r
-00003f80: 3100 0000 7231 0000 0072 3200 0000 da08  1...r1...r2.....
-00003f90: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
-00003fa0: 0014 010c 010c 0110 010c 010c 0220 0218  ............. ..
-00003fb0: 0114 020c 0208 0204 0104 0214 7f00 7f00  ................
-00003fc0: 7f00 5014 7f00 7f00 060c 01              ..P........
+000034c0: 2e30 3430 3138 3231 3433 3237 3838 392c  .04018214327889,
+000034d0: 2031 342e 3036 3234 3939 3939 3939 3936   14.062499999996
+000034e0: 3332 2034 372e 3034 3031 3832 3134 3332  32 47.0401821432
+000034f0: 3738 3839 2c20 3134 2e30 3632 3439 3939  7889, 14.0624999
+00003500: 3939 3939 3633 3220 3530 2e37 3336 3435  9999632 50.73645
+00003510: 3531 3335 3539 3039 2c20 382e 3738 3930  51355909, 8.7890
+00003520: 3632 3439 3939 3937 3720 3530 2e37 3336  624999977 50.736
+00003530: 3435 3531 3335 3539 3039 2c20 382e 3738  4551355909, 8.78
+00003540: 3930 3632 3439 3939 3937 3720 3437 2e30  90624999977 47.0
+00003550: 3430 3138 3231 3433 3237 3838 3929 2929  4018214327889)))
+00003560: 0c72 0b00 0000 720e 0000 0072 2000 0000  .r....r....r ...
+00003570: 7209 0000 0072 8e00 0000 723d 0000 0072  r....r....r=...r
+00003580: 1200 0000 5a15 736e 6170 5f76 6965 7770  ....Z.snap_viewp
+00003590: 6f72 745f 746f 5f67 7269 6472 2100 0000  ort_to_gridr!...
+000035a0: da03 7374 7272 3700 0000 7248 0000 0029  ..strr7...rH...)
+000035b0: 0a72 2700 0000 722b 0000 0072 2c00 0000  .r'...r+...r,...
+000035c0: 7228 0000 0072 2900 0000 7222 0000 0072  r(...r)...r"...r
+000035d0: 2d00 0000 7239 0000 005a 0e67 7269 645f  -...r9...Z.grid_
+000035e0: 7265 6374 616e 676c 655a 0c70 6f6c 7967  rectangleZ.polyg
+000035f0: 6f6e 5f34 3332 3672 2e00 0000 722e 0000  on_4326r....r...
+00003600: 0072 2f00 0000 da1a 7465 7374 5f73 6e61  .r/.....test_sna
+00003610: 705f 7669 6577 706f 7274 5f74 6f5f 6772  p_viewport_to_gr
+00003620: 6964 b902 0000 731a 0000 0000 0204 0104  id....s.........
+00003630: 0208 0108 0210 020c 030a 020c 0210 010e  ................
+00003640: 020a 0204 027a 3854 6573 744d 6170 436c  .....z8TestMapCl
+00003650: 7573 7465 7265 7243 6f6e 7465 6e74 436f  ustererContentCo
+00003660: 756e 7473 2e74 6573 745f 736e 6170 5f76  unts.test_snap_v
+00003670: 6965 7770 6f72 745f 746f 5f67 7269 6463  iewport_to_gridc
+00003680: 0100 0000 0000 0000 0000 0000 0c00 0000  ................
+00003690: 0a00 0000 4300 0000 73bc 0000 0064 017d  ....C...s....d.}
+000036a0: 0167 007d 027c 00a0 0064 0264 03a1 0201  .g.}.|...d.d....
+000036b0: 007c 00a0 0064 0464 05a1 0201 0074 0144  .|...d.d.....t.D
+000036c0: 005d 927d 0374 0244 005d 887d 0474 0374  .].}.t.D.].}.t.t
+000036d0: 0474 0574 0666 0444 005d 767d 057c 00a0  .t.t.f.D.]v}.|..
+000036e0: 077c 047c 017c 037c 02a1 047d 0674 087c  .|.|.|.|...}.t.|
+000036f0: 0674 0964 068d 027d 0764 077d 087c 07a0  .t.d...}.d.}.|..
+00003700: 0a7c 057c 047c 017c 027c 08a1 057d 097c  .|.|.|.|.|...}.|
+00003710: 0474 0b6b 0272 9864 0864 0969 0164 0864  .t.k.r.d.d.i.d.d
+00003720: 0969 0164 0a9c 027d 0a7c 00a0 0c7c 097c  .i.d...}.|...|.|
+00003730: 0aa1 0201 0074 0d6a 0ea0 0fa1 007d 0b7c  .....t.j.....}.|
+00003740: 00a0 0c7c 0ba0 10a1 0064 0ba1 0201 0071  ...|.....d.....q
+00003750: 3c71 2c71 2464 0053 0029 0c4e 726a 0000  <q,q$d.S.).Nrj..
+00003760: 0072 8b00 0000 7282 0000 0072 8c00 0000  .r....r....r....
+00003770: 728d 0000 0072 8900 0000 7254 0000 0072  r....r....rT...r
+00003780: 6100 0000 7231 0000 0029 0272 8200 0000  a...r1...).r....
+00003790: 728d 0000 0072 3300 0000 2911 728f 0000  r....r3...).r...
+000037a0: 0072 0b00 0000 720e 0000 0072 1100 0000  .r....r....r....
+000037b0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000037c0: 2000 0000 7209 0000 0072 8e00 0000 da18   ...r....r......
+000037d0: 6765 745f 6772 6f75 7065 645f 6d61 705f  get_grouped_map_
+000037e0: 636f 6e74 656e 7473 720c 0000 0072 2100  contentsr....r!.
+000037f0: 0000 7218 0000 0072 7200 0000 7273 0000  ..r....rr...rs..
+00003800: 0072 6100 0000 290c 7227 0000 0072 2c00  .ra...).r'...r,.
+00003810: 0000 722b 0000 0072 2800 0000 7229 0000  ..r+...r(...r)..
+00003820: 0072 3800 0000 7222 0000 0072 2d00 0000  .r8...r"...r-...
+00003830: da08 6772 6f75 705f 6279 7291 0000 0072  ..group_byr....r
+00003840: 9200 0000 7293 0000 0072 2e00 0000 722e  ....r....r....r.
+00003850: 0000 0072 2f00 0000 da1d 7465 7374 5f67  ...r/.....test_g
+00003860: 6574 5f67 726f 7570 6564 5f6d 6170 5f63  et_grouped_map_c
+00003870: 6f6e 7465 6e74 73d3 0200 0073 2c00 0000  ontents....s,...
+00003880: 0002 0401 0402 0c01 0c02 0801 0802 1002  ................
+00003890: 1002 0c02 0402 1202 0804 0200 02ff 0204  ................
+000038a0: 0200 02ff 02fc 0609 0c02 0a01 7a3b 5465  ............z;Te
+000038b0: 7374 4d61 7043 6c75 7374 6572 6572 436f  stMapClustererCo
+000038c0: 6e74 656e 7443 6f75 6e74 732e 7465 7374  ntentCounts.test
+000038d0: 5f67 6574 5f67 726f 7570 6564 5f6d 6170  _get_grouped_map
+000038e0: 5f63 6f6e 7465 6e74 734e 2908 727e 0000  _contentsN).r~..
+000038f0: 0072 7f00 0000 7280 0000 0072 9400 0000  .r....r....r....
+00003900: 7298 0000 0072 9b00 0000 729d 0000 0072  r....r....r....r
+00003910: a000 0000 722e 0000 0072 2e00 0000 722e  ....r....r....r.
+00003920: 0000 0072 2f00 0000 7281 0000 00e0 0100  ...r/...r.......
+00003930: 0073 0a00 0000 0802 0876 0844 081d 081a  .s.......v.D....
+00003940: 7281 0000 0072 5500 0000 7257 0000 0029  r....rU...rW...)
+00003950: 01da 2641 4e59 434c 5553 5445 525f 4144  ..&ANYCLUSTER_AD
+00003960: 4449 5449 4f4e 414c 5f47 524f 5550 5f42  DITIONAL_GROUP_B
+00003970: 595f 434f 4c55 4d4e 5363 0000 0000 0000  Y_COLUMNSc......
+00003980: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00003990: 0000 731c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000039a0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+000039b0: 0553 0029 06da 2354 6573 744d 6170 436c  .S.)..#TestMapCl
+000039c0: 7573 7465 7265 7241 6c74 6572 6e61 7469  ustererAlternati
+000039d0: 7665 5365 7474 696e 6773 6301 0000 0000  veSettingsc.....
+000039e0: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
+000039f0: 0000 0073 6600 0000 6401 7d01 6700 7d02  ...sf...d.}.g.}.
+00003a00: 7400 4400 5d54 7d03 7401 4400 5d4a 7d04  t.D.]T}.t.D.]J}.
+00003a10: 7402 7403 7404 7405 6604 4400 5d38 7d05  t.t.t.t.f.D.]8}.
+00003a20: 7c00 a006 7c04 7c01 7c03 7c02 a104 7d06  |...|.|.|.|...}.
+00003a30: 7407 7c06 7408 6402 8d02 7d07 7c07 a009  t.|.t.d...}.|...
+00003a40: a100 7d08 6403 7d09 7c00 a00a 7c08 7c09  ..}.d.}.|...|.|.
+00003a50: a102 0100 7124 7114 710c 6400 5300 2904  ....q$q.q.d.S.).
+00003a60: 4e72 6a00 0000 7289 0000 007a 4c2c 204d  Nrj...r....zL, M
+00003a70: 494e 2872 6174 696e 673a 3a56 4152 4348  IN(rating::VARCH
+00003a80: 4152 2920 4153 2072 6174 696e 672c 204d  AR) AS rating, M
+00003a90: 494e 286c 6173 745f 7265 6e65 7761 6c3a  IN(last_renewal:
+00003aa0: 3a56 4152 4348 4152 2920 4153 206c 6173  :VARCHAR) AS las
+00003ab0: 745f 7265 6e65 7761 6c29 0b72 0b00 0000  t_renewal).r....
+00003ac0: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00003ad0: 1300 0000 7214 0000 0072 2000 0000 7209  ....r....r ...r.
+00003ae0: 0000 0072 8e00 0000 5a26 6765 745f 6164  ...r....Z&get_ad
+00003af0: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
+00003b00: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
+00003b10: 7221 0000 0029 0a72 2700 0000 722c 0000  r!...).r'...r,..
+00003b20: 0072 2b00 0000 7228 0000 0072 2900 0000  .r+...r(...r)...
+00003b30: 7238 0000 0072 2200 0000 722d 0000 005a  r8...r"...r-...Z
+00003b40: 0e63 6f6c 756d 6e73 5f73 7472 696e 6772  .columns_stringr
+00003b50: 6800 0000 722e 0000 0072 2e00 0000 722f  h...r....r....r/
+00003b60: 0000 00da 2b74 6573 745f 6765 745f 6164  ....+test_get_ad
+00003b70: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
+00003b80: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
+00003b90: fd02 0000 7314 0000 0000 0204 0104 0208  ....s...........
+00003ba0: 0108 0210 0210 020c 0208 0204 017a 4f54  .............zOT
+00003bb0: 6573 744d 6170 436c 7573 7465 7265 7241  estMapClustererA
+00003bc0: 6c74 6572 6e61 7469 7665 5365 7474 696e  lternativeSettin
+00003bd0: 6773 2e74 6573 745f 6765 745f 6164 6469  gs.test_get_addi
+00003be0: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
+00003bf0: 636f 6c75 6d6e 735f 7374 7269 6e67 6301  columns_stringc.
+00003c00: 0000 0000 0000 0000 0000 000c 0000 000a  ................
+00003c10: 0000 0043 0000 0073 be00 0000 6401 7d01  ...C...s....d.}.
+00003c20: 6700 7d02 7c00 a000 6402 6403 a102 0100  g.}.|...d.d.....
+00003c30: 7c00 a000 6404 6405 a102 0100 7c00 a001  |...d.d.....|...
+00003c40: 7402 7403 6406 8302 a101 0100 7404 4400  t.t.d.......t.D.
+00003c50: 5d84 7d03 7405 4400 5d7a 7d04 7406 7407  ].}.t.D.]z}.t.t.
+00003c60: 7408 7409 6604 4400 5d68 7d05 7c00 a00a  t.t.f.D.]h}.|...
+00003c70: 7c04 7c01 7c03 7c02 a104 7d06 740b 7c06  |.|.|.|...}.t.|.
+00003c80: 740c 6407 8d02 7d07 6408 7d08 7c07 a00d  t.d...}.d.}.|...
+00003c90: 7c05 7c04 7c01 7c02 7c08 a105 7d09 7c04  |.|.|.|.|...}.|.
+00003ca0: 740e 6b02 724c 7c09 a00f a100 4400 5d20  t.k.rL|.....D.] 
+00003cb0: 5c02 7d0a 7d0b 7c00 a010 6409 7c0b a102  \.}.}.|...d.|...
+00003cc0: 0100 7c00 a010 640a 7c0b a102 0100 7192  ..|...d.|.....q.
+00003cd0: 714c 713c 7134 6400 5300 290b 4e72 6a00  qLq<q4d.S.).Nrj.
+00003ce0: 0000 728b 0000 0072 8200 0000 728c 0000  ..r....r....r...
+00003cf0: 0072 8d00 0000 72a1 0000 0072 8900 0000  .r....r....r....
+00003d00: 7254 0000 0072 5500 0000 7257 0000 0029  rT...rU...rW...)
+00003d10: 1172 8f00 0000 7235 0000 00da 0768 6173  .r....r5.....has
+00003d20: 6174 7472 7205 0000 0072 0b00 0000 720e  attrr....r....r.
+00003d30: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00003d40: 0000 7214 0000 0072 2000 0000 7209 0000  ..r....r ...r...
+00003d50: 0072 8e00 0000 729e 0000 0072 0c00 0000  .r....r....r....
+00003d60: da05 6974 656d 73da 0861 7373 6572 7449  ..items..assertI
+00003d70: 6e29 0c72 2700 0000 722c 0000 0072 2b00  n).r'...r,...r+.
+00003d80: 0000 7228 0000 0072 2900 0000 7238 0000  ..r(...r)...r8..
+00003d90: 0072 2200 0000 722d 0000 0072 9f00 0000  .r"...r-...r....
+00003da0: 7291 0000 00da 0961 6767 7265 6761 7465  r......aggregate
+00003db0: da04 6461 7461 722e 0000 0072 2e00 0000  ..datar....r....
+00003dc0: 722f 0000 00da 3074 6573 745f 6765 745f  r/....0test_get_
+00003dd0: 6772 6f75 7065 645f 6d61 705f 636f 6e74  grouped_map_cont
+00003de0: 656e 7473 5f61 6464 6974 696f 6e61 6c5f  ents_additional_
+00003df0: 636f 6c75 6d6e 7311 0300 0073 2000 0000  columns....s ...
+00003e00: 0002 0401 0402 0c01 0c02 1002 0801 0802  ................
+00003e10: 1002 1002 0c02 0402 1202 0802 1002 0c01  ................
+00003e20: 7a54 5465 7374 4d61 7043 6c75 7374 6572  zTTestMapCluster
+00003e30: 6572 416c 7465 726e 6174 6976 6553 6574  erAlternativeSet
+00003e40: 7469 6e67 732e 7465 7374 5f67 6574 5f67  tings.test_get_g
+00003e50: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
+00003e60: 6e74 735f 6164 6469 7469 6f6e 616c 5f63  nts_additional_c
+00003e70: 6f6c 756d 6e73 4e29 0572 7e00 0000 727f  olumnsN).r~...r.
+00003e80: 0000 0072 8000 0000 72a3 0000 0072 a900  ...r....r....r..
+00003e90: 0000 722e 0000 0072 2e00 0000 722e 0000  ..r....r....r...
+00003ea0: 0072 2f00 0000 72a2 0000 00f9 0200 0073  .r/...r........s
+00003eb0: 0400 0000 0804 0814 72a2 0000 0029 27da  ........r....)'.
+00003ec0: 0b64 6a61 6e67 6f2e 7465 7374 7202 0000  .django.testr...
+00003ed0: 0072 0300 0000 7204 0000 00da 0b64 6a61  .r....r......dja
+00003ee0: 6e67 6f2e 636f 6e66 7205 0000 00da 1764  ngo.confr......d
+00003ef0: 6a61 6e67 6f2e 636f 6e74 7269 622e 6769  jango.contrib.gi
+00003f00: 732e 6765 6f73 7206 0000 00da 1764 6a61  s.geosr......dja
+00003f10: 6e67 6f2e 636f 6e74 7269 622e 6769 732e  ngo.contrib.gis.
+00003f20: 6764 616c 7207 0000 0072 0800 0000 5a17  gdalr....r....Z.
+00003f30: 616e 7963 6c75 7374 6572 2e4d 6170 436c  anycluster.MapCl
+00003f40: 7573 7465 7265 7272 0900 0000 da0a 616e  ustererr......an
+00003f50: 7963 6c75 7374 6572 720a 0000 00da 1661  yclusterr......a
+00003f60: 6e79 636c 7573 7465 722e 6465 6669 6e69  nycluster.defini
+00003f70: 7469 6f6e 7372 0b00 0000 720c 0000 0072  tionsr....r....r
+00003f80: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
+00003f90: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
+00003fa0: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
+00003fb0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00003fc0: 5a17 616e 7963 6c75 7374 6572 2e74 6573  Z.anycluster.tes
+00003fd0: 7473 2e6d 6978 696e 7372 1500 0000 7216  ts.mixinsr....r.
+00003fe0: 0000 0072 1700 0000 5a0d 616e 796d 6170  ...r....Z.anymap
+00003ff0: 2e6d 6f64 656c 7372 1800 0000 7246 0000  .modelsr....rF..
+00004000: 0072 1f00 0000 728e 0000 0072 1b00 0000  .r....r....r....
+00004010: 7281 0000 0072 a200 0000 722e 0000 0072  r....r....r....r
+00004020: 2e00 0000 722e 0000 0072 2f00 0000 da08  ....r....r/.....
+00004030: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
+00004040: 0014 010c 010c 0110 010c 010c 0220 0218  ............. ..
+00004050: 0114 020c 0208 0204 0104 0214 7f00 7f00  ................
+00004060: 7f00 4f14 7f00 7f00 1b0c 01              ..O........
```

### Comparing `anycluster-2.3.2/anycluster/tests/common.py` & `anycluster-2.3.3/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/mixins.py` & `anycluster-2.3.3/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/test_ClusterCache.py` & `anycluster-2.3.3/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/test_FilterComposer.py` & `anycluster-2.3.3/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/anycluster/tests/test_MapClusterer.py` & `anycluster-2.3.3/anycluster/tests/test_MapClusterer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                     map_clusterer = MapClusterer(cluster_cache)
 
                     self.assertEqual(map_clusterer.cluster_cache, cluster_cache)
                     self.assertEqual(map_clusterer.schema_name, 'public')
                     self.assertEqual(map_clusterer.db_srid, 3857)
                     self.assertEqual(map_clusterer.grid_size, 256)
                     self.assertEqual(map_clusterer.maptools.__class__, MapTools)
-                    self.assertTrue(isinstance(map_clusterer.valid_operators, list))
 
 
     def test_get_database_srid(self):
 
         for clustertype in CLUSTER_TYPES:
 
             for geometry_type in GEOMETRY_TYPES:
@@ -475,15 +474,16 @@
 
     def test_clear_cache(self):
         pass
 
 
 
 class TestMapClustererContentCounts(WithFilters, WithGardens, TestCase):
-    def test_get_map_content_count(self):
+
+    def test_get_map_content_counts(self):
 
         zoom = 10
 
         # test modulations
         filters = [
             {
                 'column': 'style',
@@ -510,14 +510,27 @@
                         'value': True,
                         'operator': '!=',
                     }
                 ]
             }
         }
 
+        simple_modulations = {
+            'free' : {
+                'column': 'free_entrance',
+                'value': True,
+                'operator': '=',
+            },
+            'paid' : {
+                'column': 'free_entrance',
+                'value': True,
+                'operator': '!=',
+            }
+        }
+
         
         for clustertype in CLUSTER_TYPES:
             for geometry_type in GEOMETRY_TYPES:
 
                 for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
 
                     if clustertype == CLUSTER_TYPE_GRID and geometry_type != GEOMETRY_TYPE_VIEWPORT:
@@ -527,33 +540,39 @@
                         continue
 
                     cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
                     map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
 
                     result = map_clusterer.get_map_content_counts(geojson, geometry_type, filters, zoom, modulations)
 
+                    result_from_simple_modulations = result = map_clusterer.get_map_content_counts(geojson,
+                        geometry_type, filters, zoom, simple_modulations)
+
                     expected_result = {
                         'count': 0,
                         'modulations':  {
                             'free' : {
                                 'count': 0,
                             },
                             'paid' : {
                                 'count': 0,
                             }
                         },
                     }
                     self.assertEqual(result, expected_result)
+                    self.assertEqual(result_from_simple_modulations, expected_result)
 
                     if geometry_type == GEOMETRY_TYPE_VIEWPORT:
 
                         self.create_point('name 1', 'stone')
                         self.create_point('name 2', 'flower')
 
                         result = map_clusterer.get_map_content_counts(geojson, geometry_type, filters, zoom, modulations)
+                        result_from_simple_modulations = result = map_clusterer.get_map_content_counts(geojson,
+                            geometry_type, filters, zoom, simple_modulations)
 
                         expected_result = {
                             'count': 1,
                             'modulations': {
                                 'free': {
                                     'count': 0
                                     },
@@ -562,14 +581,15 @@
                                 }
                             }
                         }
 
                         # print(result)
 
                         self.assertEqual(result, expected_result)
+                        self.assertEqual(result_from_simple_modulations, expected_result)
                     
                     gardens = Gardens.objects.all()
                     for garden in gardens:
                         garden.delete()
 
 
                     gardens = Gardens.objects.all()
@@ -754,15 +774,15 @@
 
                     cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
 
                     map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
 
                     columns_string = map_clusterer.get_additional_group_by_columns_string()
 
-                    expected_string = ', MIN(rating) AS rating, MIN(last_renewal) AS last_renewal'
+                    expected_string = ', MIN(rating::VARCHAR) AS rating, MIN(last_renewal::VARCHAR) AS last_renewal'
                     self.assertEqual(columns_string, expected_string)
 
 
     def test_get_grouped_map_contents_additional_columns(self):
 
         zoom = 10
         filters = []
```

### Comparing `anycluster-2.3.2/anycluster.egg-info/PKG-INFO` & `anycluster-2.3.3/anycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.2
+Version: 2.3.3
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.2/anycluster.egg-info/SOURCES.txt` & `anycluster-2.3.3/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.2/setup.py` & `anycluster-2.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.3.2',
+    version='2.3.3',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

