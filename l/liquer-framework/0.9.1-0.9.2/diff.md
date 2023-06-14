# Comparing `tmp/liquer-framework-0.9.1.tar.gz` & `tmp/liquer-framework-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/liquer-framework-0.9.1.tar", last modified: Mon Jun 12 20:44:37 2023, max compression
+gzip compressed data, was "dist/liquer-framework-0.9.2.tar", last modified: Wed Jun 14 18:37:40 2023, max compression
```

## Comparing `liquer-framework-0.9.1.tar` & `liquer-framework-0.9.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/
--rw-r--r--   0 orest     (1000) orest     (1000)       77 2023-06-12 20:32:04.000000 liquer-framework-0.9.1/MANIFEST.in
--rw-rw-r--   0 orest     (1000) orest     (1000)     7755 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/PKG-INFO
--rw-rw-r--   0 orest     (1000) orest     (1000)     6536 2023-06-12 20:43:18.000000 liquer-framework-0.9.1/README.md
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.041494 liquer-framework-0.9.1/liquer/
--rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.9.1/liquer/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/blueprint.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    30437 2023-04-22 13:59:35.000000 liquer-framework-0.9.1/liquer/cache.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-02-04 11:03:51.000000 liquer-framework-0.9.1/liquer/commands.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/constants.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    41902 2023-05-18 22:09:05.000000 liquer-framework-0.9.1/liquer/context.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/dependencies.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/ext/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.1/liquer/ext/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/basic.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/ext/dataframe_batches.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_datafusion.py
--rw-r--r--   0 orest     (1000) orest     (1000)     4381 2023-05-10 20:11:49.000000 liquer-framework-0.9.1/liquer/ext/lq_hxl.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_keras.py
--rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.9.1/liquer/ext/lq_matplotlib.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_openpyxl.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    16337 2023-05-10 20:10:02.000000 liquer-framework-0.9.1/liquer/ext/lq_pandas.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_pil.py
--rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_plotly.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.9.1/liquer/ext/lq_polars.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.9.1/liquer/ext/lq_pptx.py
--rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_pygments.py
--rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_python.py
--rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.9.1/liquer/ext/lq_sklearn_regression.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.9.1/liquer/ext/lq_sweetviz.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     4222 2023-05-18 21:10:33.000000 liquer-framework-0.9.1/liquer/ext/lq_whoosh.html
--rw-rw-r--   0 orest     (1000) orest     (1000)     4300 2023-05-18 21:10:45.000000 liquer-framework-0.9.1/liquer/ext/lq_whoosh.py
--rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/ext/meta.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7326 2023-05-16 21:41:40.000000 liquer-framework-0.9.1/liquer/indexer.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/metadata.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    34618 2023-05-10 20:15:46.000000 liquer-framework-0.9.1/liquer/parser.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/pool.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.9.1/liquer/query.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    35996 2023-06-12 20:39:36.000000 liquer-framework-0.9.1/liquer/recipes.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/remote_store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.9.1/liquer/s3_store.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/server/
--rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.1/liquer/server/__init__.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/server/blueprint.py
--rw-r--r--   0 orest     (1000) orest     (1000)    19882 2023-05-18 22:06:45.000000 liquer-framework-0.9.1/liquer/server/handlers.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer/server/static/
--rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.9.1/liquer/server/static/index.html
--rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.9.1/liquer/server/static/liquer.js
--rw-r--r--   0 orest     (1000) orest     (1000)     7371 2023-05-18 21:51:28.000000 liquer-framework-0.9.1/liquer/server/tornado_handlers.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/state.py
--rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/state_types.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    44541 2023-06-12 20:38:12.000000 liquer-framework-0.9.1/liquer/store.py
--rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.9.1/liquer/template.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/tools.py
--rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.9.1/liquer/util.py
--rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.9.1/liquer/web.py
-drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/liquer_framework.egg-info/
--rw-r--r--   0 orest     (1000) orest     (1000)     7755 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/PKG-INFO
--rw-r--r--   0 orest     (1000) orest     (1000)     1339 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/SOURCES.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/dependency_links.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.9.1/liquer_framework.egg-info/not-zip-safe
--rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/requires.txt
--rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-06-12 20:44:36.000000 liquer-framework-0.9.1/liquer_framework.egg-info/top_level.txt
--rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-06-12 20:44:37.045493 liquer-framework-0.9.1/setup.cfg
--rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-06-12 20:32:12.000000 liquer-framework-0.9.1/setup.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.856578 liquer-framework-0.9.2/
+-rw-r--r--   0 orest     (1000) orest     (1000)       77 2023-06-12 20:32:04.000000 liquer-framework-0.9.2/MANIFEST.in
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7882 2023-06-14 18:37:40.856578 liquer-framework-0.9.2/PKG-INFO
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6655 2023-06-14 18:35:59.000000 liquer-framework-0.9.2/README.md
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.780577 liquer-framework-0.9.2/liquer/
+-rw-r--r--   0 orest     (1000) orest     (1000)      185 2023-01-22 17:32:54.000000 liquer-framework-0.9.2/liquer/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      259 2021-10-27 15:33:04.000000 liquer-framework-0.9.2/liquer/blueprint.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    30437 2023-04-22 13:59:35.000000 liquer-framework-0.9.2/liquer/cache.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    32155 2023-02-04 11:03:51.000000 liquer-framework-0.9.2/liquer/commands.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3631 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/constants.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    42578 2023-06-14 18:31:52.000000 liquer-framework-0.9.2/liquer/context.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3855 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/dependencies.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.784577 liquer-framework-0.9.2/liquer/ext/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.2/liquer/ext/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     9243 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/basic.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    13175 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/ext/dataframe_batches.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7937 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/lq_datafusion.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     4381 2023-05-10 20:11:49.000000 liquer-framework-0.9.2/liquer/ext/lq_hxl.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3933 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/lq_keras.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     3686 2022-07-07 19:34:25.000000 liquer-framework-0.9.2/liquer/ext/lq_matplotlib.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3447 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/lq_openpyxl.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    16337 2023-05-10 20:10:02.000000 liquer-framework-0.9.2/liquer/ext/lq_pandas.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     3432 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/lq_pil.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     2304 2021-10-27 15:33:04.000000 liquer-framework-0.9.2/liquer/ext/lq_plotly.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2853 2023-01-21 20:13:08.000000 liquer-framework-0.9.2/liquer/ext/lq_polars.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2244 2023-01-21 17:53:31.000000 liquer-framework-0.9.2/liquer/ext/lq_pptx.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      701 2021-10-27 15:33:04.000000 liquer-framework-0.9.2/liquer/ext/lq_pygments.py
+-rw-r--r--   0 orest     (1000) orest     (1000)      368 2021-10-27 15:33:04.000000 liquer-framework-0.9.2/liquer/ext/lq_python.py
+-rw-r--r--   0 orest     (1000) orest     (1000)     1805 2021-10-27 15:33:04.000000 liquer-framework-0.9.2/liquer/ext/lq_sklearn_regression.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      712 2023-01-21 22:45:23.000000 liquer-framework-0.9.2/liquer/ext/lq_sweetviz.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4222 2023-05-18 21:10:33.000000 liquer-framework-0.9.2/liquer/ext/lq_whoosh.html
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4300 2023-05-18 21:10:45.000000 liquer-framework-0.9.2/liquer/ext/lq_whoosh.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    16409 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/ext/meta.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7326 2023-05-16 21:41:40.000000 liquer-framework-0.9.2/liquer/indexer.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7020 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/metadata.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    34618 2023-05-10 20:15:46.000000 liquer-framework-0.9.2/liquer/parser.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     6273 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/pool.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     1199 2023-01-15 17:53:35.000000 liquer-framework-0.9.2/liquer/query.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    36002 2023-06-14 17:19:18.000000 liquer-framework-0.9.2/liquer/recipes.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     4122 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/remote_store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     5713 2023-01-08 21:15:57.000000 liquer-framework-0.9.2/liquer/s3_store.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.788577 liquer-framework-0.9.2/liquer/server/
+-rw-r--r--   0 orest     (1000) orest     (1000)        0 2019-06-09 11:48:28.000000 liquer-framework-0.9.2/liquer/server/__init__.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    14961 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/server/blueprint.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    19882 2023-05-18 22:06:45.000000 liquer-framework-0.9.2/liquer/server/handlers.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.788577 liquer-framework-0.9.2/liquer/server/static/
+-rw-rw-r--   0 orest     (1000) orest     (1000)    26489 2021-01-31 21:05:09.000000 liquer-framework-0.9.2/liquer/server/static/index.html
+-rw-rw-r--   0 orest     (1000) orest     (1000)    18057 2021-12-15 17:45:48.000000 liquer-framework-0.9.2/liquer/server/static/liquer.js
+-rw-r--r--   0 orest     (1000) orest     (1000)     7371 2023-05-18 21:51:28.000000 liquer-framework-0.9.2/liquer/server/tornado_handlers.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     7656 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/state.py
+-rw-r--r--   0 orest     (1000) orest     (1000)    17774 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/state_types.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    44509 2023-06-14 16:39:15.000000 liquer-framework-0.9.2/liquer/store.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)    11266 2022-07-30 08:12:25.000000 liquer-framework-0.9.2/liquer/template.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      621 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/tools.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)      521 2023-01-21 17:53:32.000000 liquer-framework-0.9.2/liquer/util.py
+-rw-rw-r--   0 orest     (1000) orest     (1000)     2721 2023-01-21 22:45:45.000000 liquer-framework-0.9.2/liquer/web.py
+drwxrwxr-x   0 orest     (1000) orest     (1000)        0 2023-06-14 18:37:40.856578 liquer-framework-0.9.2/liquer_framework.egg-info/
+-rw-r--r--   0 orest     (1000) orest     (1000)     7882 2023-06-14 18:37:39.000000 liquer-framework-0.9.2/liquer_framework.egg-info/PKG-INFO
+-rw-r--r--   0 orest     (1000) orest     (1000)     1339 2023-06-14 18:37:39.000000 liquer-framework-0.9.2/liquer_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2023-06-14 18:37:39.000000 liquer-framework-0.9.2/liquer_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        1 2019-12-07 17:16:04.000000 liquer-framework-0.9.2/liquer_framework.egg-info/not-zip-safe
+-rw-r--r--   0 orest     (1000) orest     (1000)        6 2023-06-14 18:37:39.000000 liquer-framework-0.9.2/liquer_framework.egg-info/requires.txt
+-rw-r--r--   0 orest     (1000) orest     (1000)        7 2023-06-14 18:37:39.000000 liquer-framework-0.9.2/liquer_framework.egg-info/top_level.txt
+-rw-rw-r--   0 orest     (1000) orest     (1000)       38 2023-06-14 18:37:40.856578 liquer-framework-0.9.2/setup.cfg
+-rw-r--r--   0 orest     (1000) orest     (1000)      702 2023-06-14 18:36:14.000000 liquer-framework-0.9.2/setup.py
```

### Comparing `liquer-framework-0.9.1/PKG-INFO` & `liquer-framework-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.1
+Version: 0.9.2
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -100,13 +100,14 @@
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
         - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
         - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
         - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
+        - 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.9.1/README.md` & `liquer-framework-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -92,7 +92,8 @@
 - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
 - 2022-01-07 - v0.7.4  - more bugfixes
 - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
 - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
 - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
 - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
 - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
+- 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
```

### Comparing `liquer-framework-0.9.1/liquer/cache.py` & `liquer-framework-0.9.2/liquer/cache.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/commands.py` & `liquer-framework-0.9.2/liquer/commands.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/constants.py` & `liquer-framework-0.9.2/liquer/constants.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/context.py` & `liquer-framework-0.9.2/liquer/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 from liquer.store import (
     get_store,
     Store,
     KeyNotFoundStoreException,
     StoreException,
     key_extension,
+    parent_key,
 )
 
 
 def find_queries_in_template(template: str, prefix: str, sufix: str):
     try:
         start = template.index(prefix)
         end = template.index(sufix, start + len(prefix))
@@ -280,14 +281,16 @@
 
         self.vars = Vars(vars_clone())
         self.html_preview = ""
         self.store_key = None
         self.store_to = None
 
         self._metadata = Metadata()
+        self.cwd_key=None
+        self.evaluated_key=None
 
     def new_empty(self):
         return Context(debug=self.debug_messages)
 
     def store_data(self, key, data):
         """Convenience method to store data in the store including metadata.
         Note that the metadata are taken from the context.metadata() and slightly updated.
@@ -487,15 +490,19 @@
         self.child_log = self.child_log[:5]
         self.store_metadata()
         if self.parent_context is not None:
             self.parent_context.log_child_dict(d)
         return self
 
     def child_context(self):
-        return self.__class__(parent_context=self)
+        """Create a new context that is a child of this context.
+        This is used to create a new context for a subquery.
+        """
+        c = self.__class__(parent_context=self)
+        return c
 
     def root_context(self):
         return (
             self if self.parent_context is None else self.parent_context.root_context()
         )
 
     def log_subquery(self, query: str, description=None):
@@ -905,14 +912,17 @@
         """
         self.enable_store_metadata = False  # Prevents overwriting cache with metadata
         self.status = Status.EVALUATION
         self.debug(f"EVALUATE {query} ")
 
         self.vars = Vars(vars_clone())
 
+        self.evaluated_key = self.evaluated_key if store_key is None else store_key
+        self.cwd_key = self.cwd_key if store_key is None else parent_key(store_key)
+
         if self.query is not None:
             self.enable_store_metadata = True
             print(f"Subquery {query} called from {self.query.encode()}")
             state = self.child_context().evaluate(
                 query, store_key=store_key, store_to=store_to
             )
             if not isinstance(query, str):
@@ -974,15 +984,18 @@
                 state = self.create_initial_state()
                 state.metadata["created"] = self.now()
                 self.debug(f"INITIAL STATE")
             else:
                 self.parent_query = p.encode()
                 self.status = Status.EVALUATING_PARENT
                 self.store_metadata(force=True)
-                state = self.child_context().evaluate(p, cache=cache)
+                c=self.child_context()
+                c.evaluated_key = self.evaluated_key
+                c.cwd_key = self.cwd_key
+                state = c.evaluate(p, cache=cache)
             if state.is_error:
                 self.status = Status.ERROR
                 self.store_metadata()
                 state = state.next_state()
                 state.query = query.encode()
                 state.metadata["created"] = self.now()
                 self.debug(f"ERROR in '{state.query}'")
@@ -1112,24 +1125,26 @@
             if store is None:
                 store = self.store()
 
             store.store(key, b, state.metadata)
 
         return state
 
-    def evaluate_template(self, template: str, prefix="$", sufix="$", cache=None):
+    def evaluate_template(self, template: str, prefix="$", sufix="$", path=None, resource_segment_name=""):
         """Evaluate a string template; replace all queries by their values
         Queries in the template are delimited by prefix and sufix.
         Queries should evaluate to strings and should not cause errors.
         """
         local_cache = {}
         result = ""
         for text, q in find_queries_in_template(template, prefix, sufix):
             result += text
             if q is not None:
+                if path is not None:
+                    q = parse(q).to_absolute(path, resource_segment_name=resource_segment_name).encode()
                 if q in local_cache:
                     result += local_cache[q]
                 else:
                     state = self.evaluate(q, description=f"template expansion of {q}")
                     if state.is_error:
                         self.error(f"Template failed to expand {q}")
                         qr = f"ERROR({q})"
```

### Comparing `liquer-framework-0.9.1/liquer/dependencies.py` & `liquer-framework-0.9.2/liquer/dependencies.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/basic.py` & `liquer-framework-0.9.2/liquer/ext/basic.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/dataframe_batches.py` & `liquer-framework-0.9.2/liquer/ext/dataframe_batches.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_datafusion.py` & `liquer-framework-0.9.2/liquer/ext/lq_datafusion.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_hxl.py` & `liquer-framework-0.9.2/liquer/ext/lq_hxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_keras.py` & `liquer-framework-0.9.2/liquer/ext/lq_keras.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_matplotlib.py` & `liquer-framework-0.9.2/liquer/ext/lq_matplotlib.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_openpyxl.py` & `liquer-framework-0.9.2/liquer/ext/lq_openpyxl.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_pandas.py` & `liquer-framework-0.9.2/liquer/ext/lq_pandas.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_pil.py` & `liquer-framework-0.9.2/liquer/ext/lq_pil.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_plotly.py` & `liquer-framework-0.9.2/liquer/ext/lq_plotly.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_polars.py` & `liquer-framework-0.9.2/liquer/ext/lq_polars.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_pptx.py` & `liquer-framework-0.9.2/liquer/ext/lq_pptx.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_pygments.py` & `liquer-framework-0.9.2/liquer/ext/lq_pygments.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_sklearn_regression.py` & `liquer-framework-0.9.2/liquer/ext/lq_sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_sweetviz.py` & `liquer-framework-0.9.2/liquer/ext/lq_sweetviz.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_whoosh.html` & `liquer-framework-0.9.2/liquer/ext/lq_whoosh.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/lq_whoosh.py` & `liquer-framework-0.9.2/liquer/ext/lq_whoosh.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/ext/meta.py` & `liquer-framework-0.9.2/liquer/ext/meta.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/indexer.py` & `liquer-framework-0.9.2/liquer/indexer.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/metadata.py` & `liquer-framework-0.9.2/liquer/metadata.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/parser.py` & `liquer-framework-0.9.2/liquer/parser.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/pool.py` & `liquer-framework-0.9.2/liquer/pool.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/query.py` & `liquer-framework-0.9.2/liquer/query.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/recipes.py` & `liquer-framework-0.9.2/liquer/recipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 
     def metadata(self, key):
         metadata = Metadata(super().metadata(key))
         metadata.query = self.data["query"]
         return metadata.as_dict()
 
     def make(self, key, store=None, context=None):
+        print(f"Making query recipe {key}")
         context = get_context(context)
         if store is None:
             store = context.store()
         context.evaluate(
             self.data["query"],
             store_key=key,
             store_to=store,
@@ -844,16 +845,15 @@
                     for directory, items in spec.items():
                         for i, r in enumerate(items):
                             cwd = (
                                 parent
                                 if directory == self.LOCAL_RECIPES
                                 else join_key(parent, directory)
                             )
-                            cwd = self.to_root_key(cwd)
-                            d = resolve_recipe_definition(r, cwd, metadata)
+                            d = resolve_recipe_definition(r, self.to_root_key(cwd), metadata)
                             if d is None:
                                 metadata.warning(
                                     f"Failed parsing the definition of recipe {i+1} in {directory}"
                                 )
                             d["recipe_name"] = (
                                 self.to_root_key(recipes_key)
                                 + f"/-Ryaml/{directory}/{i}#"
```

### Comparing `liquer-framework-0.9.1/liquer/remote_store.py` & `liquer-framework-0.9.2/liquer/remote_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/s3_store.py` & `liquer-framework-0.9.2/liquer/s3_store.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/server/blueprint.py` & `liquer-framework-0.9.2/liquer/server/blueprint.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/server/handlers.py` & `liquer-framework-0.9.2/liquer/server/handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/server/static/index.html` & `liquer-framework-0.9.2/liquer/server/static/index.html`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/server/static/liquer.js` & `liquer-framework-0.9.2/liquer/server/static/liquer.js`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/server/tornado_handlers.py` & `liquer-framework-0.9.2/liquer/server/tornado_handlers.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/state.py` & `liquer-framework-0.9.2/liquer/state.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/state_types.py` & `liquer-framework-0.9.2/liquer/state_types.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/store.py` & `liquer-framework-0.9.2/liquer/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1091,15 +1091,14 @@
         self.default_store = default_store
         if default_store is not None:
             self.default_store.parent_store = self
         self.routing_table = [] if routing_table is None else routing_table
 
     def sync(self):
         for key, store in self.routing_table:
-            print("SYNC ", key)
             store.sync()
         if self.default_store is not None:
             self.default_store.sync()
 
     def umount(self, umount_key):
         for key, store in self.routing_table:
             if key == umount_key:
```

### Comparing `liquer-framework-0.9.1/liquer/template.py` & `liquer-framework-0.9.2/liquer/template.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/tools.py` & `liquer-framework-0.9.2/liquer/tools.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/util.py` & `liquer-framework-0.9.2/liquer/util.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer/web.py` & `liquer-framework-0.9.2/liquer/web.py`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/liquer_framework.egg-info/PKG-INFO` & `liquer-framework-0.9.2/liquer_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquer-framework
-Version: 0.9.1
+Version: 0.9.2
 Summary: LiQuer - Query in (URL) link
 Home-page: https://github.com/orest-d/liquer
 Author: Orest Dubay
 Author-email: orest3.dubay@gmail.com
 License: UNKNOWN
 Description: # LiQuer (Link Query) 
         
@@ -100,13 +100,14 @@
         - 2022-01-06 - v0.7.3  - two bugfixes, recipe version
         - 2022-01-07 - v0.7.4  - more bugfixes
         - 2022-01-12 - v0.7.5  - more bugfixes, pandas_concat recipe
         - 2022-01-25 - v0.7.6  - bugfixes in recipe metadata, development of extra parameters to evaluate
         - 2023-01-22 - v0.8.0  - tools, indexers, S3 store, remote liquer as a store, 
         - 2023-06-11 - v0.9.0  - relative path in recipes, experimental search engine support (whoosh) 
         - 2023-06-12 - v0.9.1  - fixing bugs in relative path and search engine support
+        - 2023-06-14 - v0.9.2  - another bugfix, context.cwd_key and context.evaluated_key; relative path in evaluate_template
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `liquer-framework-0.9.1/liquer_framework.egg-info/SOURCES.txt` & `liquer-framework-0.9.2/liquer_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liquer-framework-0.9.1/setup.py` & `liquer-framework-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="liquer-framework",
-    version="0.9.1",
+    version="0.9.2",
     author="Orest Dubay",
     author_email="orest3.dubay@gmail.com",
     description="LiQuer - Query in (URL) link",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/orest-d/liquer",
     packages=setuptools.find_packages(),
```

