# Comparing `tmp/vcorelib-1.6.6.tar.gz` & `tmp/vcorelib-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.6.6.tar", last modified: Wed May 24 19:25:44 2023, max compression
+gzip compressed data, was "vcorelib-1.6.7.tar", last modified: Wed Jun 14 04:03:05 2023, max compression
```

## Comparing `vcorelib-1.6.6.tar` & `vcorelib-1.6.7.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 19:24:21.000000 vcorelib-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-24 19:25:44.275995 vcorelib-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-24 19:24:21.000000 vcorelib-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 19:24:21.000000 vcorelib-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:25:44.275995 vcorelib-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-24 19:24:21.000000 vcorelib-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-24 19:24:21.000000 vcorelib-1.6.6/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 19:24:21.000000 vcorelib-1.6.6/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-24 19:24:21.000000 vcorelib-1.6.6/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.271995 vcorelib-1.6.6/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.275995 vcorelib-1.6.6/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 19:24:21.000000 vcorelib-1.6.6/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:25:44.267995 vcorelib-1.6.6/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-24 19:25:44.000000 vcorelib-1.6.6/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-24 19:25:44.000000 vcorelib-1.6.6/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:25:44.000000 vcorelib-1.6.6/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 19:25:44.000000 vcorelib-1.6.6/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 19:25:44.000000 vcorelib-1.6.6/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.118990 vcorelib-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 04:01:44.000000 vcorelib-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 04:03:05.118990 vcorelib-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-14 04:01:44.000000 vcorelib-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 04:01:44.000000 vcorelib-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:03:05.118990 vcorelib-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-14 04:01:44.000000 vcorelib-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.098990 vcorelib-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:01:44.000000 vcorelib-1.6.7/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 04:01:44.000000 vcorelib-1.6.7/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 04:01:44.000000 vcorelib-1.6.7/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.098990 vcorelib-1.6.7/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.102990 vcorelib-1.6.7/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.102990 vcorelib-1.6.7/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.102990 vcorelib-1.6.7/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.106990 vcorelib-1.6.7/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.106990 vcorelib-1.6.7/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.106990 vcorelib-1.6.7/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.110990 vcorelib-1.6.7/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.114990 vcorelib-1.6.7/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 04:01:44.000000 vcorelib-1.6.7/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:03:05.102990 vcorelib-1.6.7/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 04:03:05.000000 vcorelib-1.6.7/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-14 04:03:05.000000 vcorelib-1.6.7/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:03:05.000000 vcorelib-1.6.7/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 04:03:05.000000 vcorelib-1.6.7/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 04:03:05.000000 vcorelib-1.6.7/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.6.6/LICENSE` & `vcorelib-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/PKG-INFO` & `vcorelib-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.6
+Version: 1.6.7
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=543d036eacba38e3777c937fea2219f4
+    hash=f4f4dcca83c4ad72ea03ca982f030b85
     =====================================
 -->
 
-# vcorelib ([1.6.6](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.7](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.6/README.md` & `vcorelib-1.6.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=543d036eacba38e3777c937fea2219f4
+    hash=f4f4dcca83c4ad72ea03ca982f030b85
     =====================================
 -->
 
-# vcorelib ([1.6.6](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.7](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.6/pyproject.toml` & `vcorelib-1.6.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.6.6"
+version = "1.6.7"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.6.6/setup.py` & `vcorelib-1.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/tests/test_logging.py` & `vcorelib-1.6.7/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/tests/test_names.py` & `vcorelib-1.6.7/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/tests/test_namespace.py` & `vcorelib-1.6.7/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/args/__init__.py` & `vcorelib-1.6.7/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/args/newline.py` & `vcorelib-1.6.7/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.7/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/asyncio/cli.py` & `vcorelib-1.6.7/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.7/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/dict/__init__.py` & `vcorelib-1.6.7/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/dict/cache.py` & `vcorelib-1.6.7/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/dict/codec.py` & `vcorelib-1.6.7/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/dict/config.py` & `vcorelib-1.6.7/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/dict/env.py` & `vcorelib-1.6.7/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/graph/__init__.py` & `vcorelib-1.6.7/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/graph/abc.py` & `vcorelib-1.6.7/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/graph/edge.py` & `vcorelib-1.6.7/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/graph/node.py` & `vcorelib-1.6.7/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/graph/port.py` & `vcorelib-1.6.7/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/__init__.py` & `vcorelib-1.6.7/vcorelib/io/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     JsonObject,
     JsonPrimitive,
     JsonValue,
     LoadResult,
     StreamProcessor,
 )
 
+DEFAULT_INCLUDES_KEY = "includes"
+
 __all__ = [
     "DataArbiter",
     "ARBITER",
     "JsonPrimitive",
     "JsonValue",
     "JsonArray",
     "JsonObject",
@@ -31,8 +33,9 @@
     "EncodeResult",
     "DataStream",
     "StreamProcessor",
     "DataDecoder",
     "DataEncoder",
     "Serializable",
     "FileEntity",
+    "DEFAULT_INCLUDES_KEY",
 ]
```

### Comparing `vcorelib-1.6.6/vcorelib/io/abc.py` & `vcorelib-1.6.7/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/arbiter/base.py` & `vcorelib-1.6.7/vcorelib/io/arbiter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A module exposing data-file encoders and decoders.
 """
 
 # built-in
 import logging
-from typing import Any as _Any
 from typing import Optional as _Optional
 
 # internal
 from vcorelib import DEFAULT_ENCODING as _DEFAULT_ENCODING
 from vcorelib.dict import MergeStrategy, consume
 from vcorelib.io.mapping import DataMapping
 from vcorelib.io.types import DataDecoder as _DataDecoder
@@ -67,15 +66,15 @@
         return result
 
     def decode(
         self,
         pathlike: _Pathlike,
         logger: LoggerType = None,
         require_success: bool = False,
-        includes_key: _Any = None,
+        includes_key: str = None,
         preprocessor: _StreamProcessor = None,
         maxsplit: int = 1,
         expect_overwrite: bool = False,
         strategy: MergeStrategy = MergeStrategy.RECURSIVE,
         **kwargs,
     ) -> LoadResult:
         """Attempt to load data from a file."""
```

### Comparing `vcorelib-1.6.6/vcorelib/io/arbiter/context.py` & `vcorelib-1.6.7/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/arbiter/directory.py` & `vcorelib-1.6.7/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.7/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/cache.py` & `vcorelib-1.6.7/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/decode.py` & `vcorelib-1.6.7/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/encode.py` & `vcorelib-1.6.7/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/mapping.py` & `vcorelib-1.6.7/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/io/types.py` & `vcorelib-1.6.7/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/logging.py` & `vcorelib-1.6.7/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/math/__init__.py` & `vcorelib-1.6.7/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/math/analysis/average.py` & `vcorelib-1.6.7/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.7/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.7/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/math/time.py` & `vcorelib-1.6.7/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/names.py` & `vcorelib-1.6.7/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/namespace.py` & `vcorelib-1.6.7/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/paths/__init__.py` & `vcorelib-1.6.7/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/paths/context.py` & `vcorelib-1.6.7/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/paths/info.py` & `vcorelib-1.6.7/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/paths/info_cache.py` & `vcorelib-1.6.7/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/platform/__init__.py` & `vcorelib-1.6.7/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/schemas/__init__.py` & `vcorelib-1.6.7/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/schemas/base.py` & `vcorelib-1.6.7/vcorelib/schemas/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,24 @@
         self.data = data
 
     @_abc.abstractmethod
     def __call__(self, data: _Any) -> _Any:
         """Validate input data and return the result."""
 
     @classmethod
-    def from_path(cls: _Type[T], path: _Pathlike, **kwargs) -> T:
+    def from_path(
+        cls: _Type[T], path: _Pathlike, includes_key: str = None, **kwargs
+    ) -> T:
         """Load a schema from a data file on disk."""
-        return cls(_ARBITER.decode(path, require_success=True).data, **kwargs)
+        return cls(
+            _ARBITER.decode(
+                path, includes_key=includes_key, require_success=True
+            ).data,
+            **kwargs,
+        )
 
 
 V = _TypeVar("V", bound="SchemaMap")
 
 
 class SchemaMap(
     UserDict,  # type: ignore
```

### Comparing `vcorelib-1.6.6/vcorelib/schemas/json.py` & `vcorelib-1.6.7/vcorelib/schemas/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # third-party
 from fastjsonschema import JsonSchemaException as _JsonSchemaException
 from fastjsonschema import compile as _compile
 
 # internal
 from vcorelib.io import ARBITER as _ARBITER
+from vcorelib.io import DEFAULT_INCLUDES_KEY as _DEFAULT_INCLUDES_KEY
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import find_file
 from vcorelib.schemas.base import Schema as _Schema
 from vcorelib.schemas.base import SchemaMap as _SchemaMap
 from vcorelib.schemas.base import SchemaValidationError
 
 LOG = _getLogger(__name__)
@@ -27,15 +28,17 @@
     """Load data from a package."""
 
     parsed = _urlparse(uri)
     assert parsed.scheme == "package"
 
     path = find_file(parsed.path[1:], package=parsed.hostname, logger=LOG)
     assert path is not None, path
-    return _ARBITER.decode(path, require_success=True).data
+    return _ARBITER.decode(
+        path, includes_key=_DEFAULT_INCLUDES_KEY, require_success=True
+    ).data
 
 
 class JsonSchema(_Schema):
     """
     An object wrapper for: https://horejsek.github.io/python-fastjsonschema/.
 
     See also: https://json-schema.org/.
```

### Comparing `vcorelib-1.6.6/vcorelib/schemas/mixins.py` & `vcorelib-1.6.7/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/script/__init__.py` & `vcorelib-1.6.7/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/target/__init__.py` & `vcorelib-1.6.7/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/target/evaluation.py` & `vcorelib-1.6.7/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/target/expression.py` & `vcorelib-1.6.7/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/target/resolver.py` & `vcorelib-1.6.7/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/task/__init__.py` & `vcorelib-1.6.7/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/task/dict/melder.py` & `vcorelib-1.6.7/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/task/manager.py` & `vcorelib-1.6.7/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.7/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib/task/time/sleep.py` & `vcorelib-1.6.7/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.6/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.7/vcorelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.6
+Version: 1.6.7
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=543d036eacba38e3777c937fea2219f4
+    hash=f4f4dcca83c4ad72ea03ca982f030b85
     =====================================
 -->
 
-# vcorelib ([1.6.6](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.7](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.6/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.7/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

