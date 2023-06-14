# Comparing `tmp/sdgym-0.7.0.tar.gz` & `tmp/sdgym-0.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgym-0.7.0.tar", last modified: Wed Jun 14 18:20:11 2023, max compression
+gzip compressed data, was "sdgym-0.7.0.dev0.tar", last modified: Tue Jun 13 19:19:41 2023, max compression
```

## Comparing `sdgym-0.7.0.tar` & `sdgym-0.7.0.dev0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.575837 sdgym-0.7.0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-02-21 05:08:00.000000 sdgym-0.7.0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11894 2023-06-14 18:20:08.000000 sdgym-0.7.0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4924 2023-02-21 05:08:00.000000 sdgym-0.7.0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      270 2023-02-21 05:08:00.000000 sdgym-0.7.0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18621 2023-06-14 18:20:11.576024 sdgym-0.7.0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5700 2023-06-14 18:20:08.000000 sdgym-0.7.0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.565901 sdgym-0.7.0/docs/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.568287 sdgym-0.7.0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   300580 2023-02-21 05:08:00.000000 sdgym-0.7.0/docs/images/SDGym_Results.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.570183 sdgym-0.7.0/sdgym/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1025 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19311 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/benchmark.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.572045 sdgym-0.7.0/sdgym/cli/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       18 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/cli/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12829 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/cli/__main__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1293 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/cli/collect.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10540 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/cli/summary.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3735 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/cli/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7791 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/datasets.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4069 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/metrics.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2173 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/progress.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4403 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/s3.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.573208 sdgym-0.7.0/sdgym/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1134 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5243 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9377 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/generate.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1285 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2082 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/independent.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4530 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/sdv.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1633 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/synthesizers/uniform.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4034 2023-06-14 18:20:08.000000 sdgym-0.7.0/sdgym/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.571219 sdgym-0.7.0/sdgym.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18621 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1253 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/entry_points.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2316 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-06-14 18:20:11.000000 sdgym-0.7.0/sdgym.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1192 2023-06-14 18:20:11.578658 sdgym-0.7.0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4093 2023-06-14 18:20:08.000000 sdgym-0.7.0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.573344 sdgym-0.7.0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       19 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.573628 sdgym-0.7.0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.574069 sdgym-0.7.0/tests/integration/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/integration/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1389 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/integration/synthesizers/test_independent.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2737 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/integration/synthesizers/test_uniform.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14371 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/integration/test_benchmark.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.575131 sdgym-0.7.0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-14 18:20:11.575662 sdgym-0.7.0/tests/unit/synthesizers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/synthesizers/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4239 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/synthesizers/test_generate.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      625 2023-02-21 05:08:00.000000 sdgym-0.7.0/tests/unit/synthesizers/test_independent.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2672 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/test_benchmark.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8493 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/test_datasets.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4987 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/test_s3.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5844 2023-06-14 18:20:08.000000 sdgym-0.7.0/tests/unit/test_summary.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      894 2023-02-21 05:08:00.000000 sdgym-0.7.0/tests/unit/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.931239 sdgym-0.7.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10403 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4924 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      270 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17135 2023-06-13 19:19:41.931367 sdgym-0.7.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5700 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.920623 sdgym-0.7.0.dev0/docs/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.922842 sdgym-0.7.0.dev0/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   300580 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/docs/images/SDGym_Results.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.924949 sdgym-0.7.0.dev0/sdgym/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1030 2023-06-13 19:14:33.000000 sdgym-0.7.0.dev0/sdgym/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19311 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/benchmark.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.927010 sdgym-0.7.0.dev0/sdgym/cli/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       18 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12829 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/__main__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1293 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/collect.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10540 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/summary.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3735 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7791 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/datasets.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/sdgym/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4069 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/metrics.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2173 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/progress.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4403 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/s3.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928209 sdgym-0.7.0.dev0/sdgym/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1134 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5243 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9377 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/generate.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1285 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2082 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4530 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/sdv.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1633 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/uniform.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4034 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.925969 sdgym-0.7.0.dev0/sdgym.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17135 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1253 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2316 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1197 2023-06-13 19:19:41.931881 sdgym-0.7.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4098 2023-06-13 19:14:33.000000 sdgym-0.7.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928366 sdgym-0.7.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       19 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928703 sdgym-0.7.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.929213 sdgym-0.7.0.dev0/tests/integration/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1389 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/test_independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2737 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/test_uniform.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14371 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/test_benchmark.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.930403 sdgym-0.7.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.931005 sdgym-0.7.0.dev0/tests/unit/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4239 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/test_generate.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      625 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/test_independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2672 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_benchmark.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8493 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_datasets.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4987 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_s3.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5844 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/tests/unit/test_summary.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      894 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/tests/unit/test_utils.py
```

### Comparing `sdgym-0.7.0/HISTORY.md` & `sdgym-0.7.0.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,9 @@
 # History
 
-## v0.7.0 - 2023-06-13
-
-This release adds support for SDV 1.0 and PyTorch 2.0!
-
-### New Features
-
-* Add functions to top level import - Issue [#229](https://github.com/sdv-dev/SDGym/issues/229) by @fealho
-* Cleanup SDGym to the new SDV 1.0 metadata and synthesizers - Issue [#212](https://github.com/sdv-dev/SDGym/issues/212) by @fealho
-
-### Bugs Fixed
-
-* limit_dataset_size causes sdgym to crash - Issue [#231](https://github.com/sdv-dev/SDGym/issues/231) by @fealho
-* benchmark_single_table crashes with metadata dict - Issue [#232](https://github.com/sdv-dev/SDGym/issues/232) by @fealho
-* Passing None as synthesizers runs all of them - Issue [#233](https://github.com/sdv-dev/SDGym/issues/233) by @fealho
-* timeout parameter causes sdgym to crash - Issue [#234](https://github.com/sdv-dev/SDGym/issues/234) by @pvk-developer
-* SDGym is not working with latest torch - Issue [#210](https://github.com/sdv-dev/SDGym/issues/210) by @amontanez24
-* Fix sdgym --help - Issue [#206](https://github.com/sdv-dev/SDGym/issues/206) by @katxiao
-
-### Internal
-
-* Increase code style lint - Issue [#123](https://github.com/sdv-dev/SDGym/issues/123) by @fealho
-* Remove code support for synthesizers that are not strings/classes - PR [#236](https://github.com/sdv-dev/SDGym/pull/236) by @fealho
-* Code Refactoring - Issue [#215](https://github.com/sdv-dev/SDGym/issues/215) by @fealho
-
-### Maintenance
-
-* Remove pomegranate - Issue [#230](https://github.com/sdv-dev/SDGym/issues/230) by @amontanez24
-
 ## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
```

### Comparing `sdgym-0.7.0/LICENSE` & `sdgym-0.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/PKG-INFO` & `sdgym-0.7.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgym
-Version: 0.7.0
+Version: 0.7.0.dev0
 Summary: Benchmark tabular synthetic data generators using a variety of datasets
 Home-page: https://github.com/sdv-dev/SDGym
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: machine learning synthetic data generation benchmark generative models
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -184,42 +184,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.7.0 - 2023-06-13
-
-This release adds support for SDV 1.0 and PyTorch 2.0!
-
-### New Features
-
-* Add functions to top level import - Issue [#229](https://github.com/sdv-dev/SDGym/issues/229) by @fealho
-* Cleanup SDGym to the new SDV 1.0 metadata and synthesizers - Issue [#212](https://github.com/sdv-dev/SDGym/issues/212) by @fealho
-
-### Bugs Fixed
-
-* limit_dataset_size causes sdgym to crash - Issue [#231](https://github.com/sdv-dev/SDGym/issues/231) by @fealho
-* benchmark_single_table crashes with metadata dict - Issue [#232](https://github.com/sdv-dev/SDGym/issues/232) by @fealho
-* Passing None as synthesizers runs all of them - Issue [#233](https://github.com/sdv-dev/SDGym/issues/233) by @fealho
-* timeout parameter causes sdgym to crash - Issue [#234](https://github.com/sdv-dev/SDGym/issues/234) by @pvk-developer
-* SDGym is not working with latest torch - Issue [#210](https://github.com/sdv-dev/SDGym/issues/210) by @amontanez24
-* Fix sdgym --help - Issue [#206](https://github.com/sdv-dev/SDGym/issues/206) by @katxiao
-
-### Internal
-
-* Increase code style lint - Issue [#123](https://github.com/sdv-dev/SDGym/issues/123) by @fealho
-* Remove code support for synthesizers that are not strings/classes - PR [#236](https://github.com/sdv-dev/SDGym/pull/236) by @fealho
-* Code Refactoring - Issue [#215](https://github.com/sdv-dev/SDGym/issues/215) by @fealho
-
-### Maintenance
-
-* Remove pomegranate - Issue [#230](https://github.com/sdv-dev/SDGym/issues/230) by @amontanez24
-
 ## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
```

### Comparing `sdgym-0.7.0/README.md` & `sdgym-0.7.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/docs/images/SDGym_Results.png` & `sdgym-0.7.0.dev0/docs/images/SDGym_Results.png`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/__init__.py` & `sdgym-0.7.0.dev0/sdgym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 tabular data.
 """
 
 __author__ = 'DataCebo, Inc.'
 __copyright__ = 'Copyright (c) 2022 DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
 __license__ = 'BSL-1.1'
-__version__ = '0.7.0'
+__version__ = '0.7.0.dev0'
 
 import logging
 
 from sdgym.benchmark import benchmark_single_table
 from sdgym.cli.collect import collect_results
 from sdgym.cli.summary import make_summary_spreadsheet
 from sdgym.datasets import get_available_datasets, load_dataset
```

### Comparing `sdgym-0.7.0/sdgym/benchmark.py` & `sdgym-0.7.0.dev0/sdgym/benchmark.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/cli/__main__.py` & `sdgym-0.7.0.dev0/sdgym/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/cli/collect.py` & `sdgym-0.7.0.dev0/sdgym/cli/collect.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/cli/summary.py` & `sdgym-0.7.0.dev0/sdgym/cli/summary.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/cli/utils.py` & `sdgym-0.7.0.dev0/sdgym/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/datasets.py` & `sdgym-0.7.0.dev0/sdgym/datasets.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/metrics.py` & `sdgym-0.7.0.dev0/sdgym/metrics.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/progress.py` & `sdgym-0.7.0.dev0/sdgym/progress.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/s3.py` & `sdgym-0.7.0.dev0/sdgym/s3.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/__init__.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/base.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/generate.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/generate.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/identity.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/identity.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/independent.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/independent.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/sdv.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/sdv.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/synthesizers/uniform.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/uniform.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym/utils.py` & `sdgym-0.7.0.dev0/sdgym/utils.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym.egg-info/PKG-INFO` & `sdgym-0.7.0.dev0/sdgym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgym
-Version: 0.7.0
+Version: 0.7.0.dev0
 Summary: Benchmark tabular synthetic data generators using a variety of datasets
 Home-page: https://github.com/sdv-dev/SDGym
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: machine learning synthetic data generation benchmark generative models
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -184,42 +184,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.7.0 - 2023-06-13
-
-This release adds support for SDV 1.0 and PyTorch 2.0!
-
-### New Features
-
-* Add functions to top level import - Issue [#229](https://github.com/sdv-dev/SDGym/issues/229) by @fealho
-* Cleanup SDGym to the new SDV 1.0 metadata and synthesizers - Issue [#212](https://github.com/sdv-dev/SDGym/issues/212) by @fealho
-
-### Bugs Fixed
-
-* limit_dataset_size causes sdgym to crash - Issue [#231](https://github.com/sdv-dev/SDGym/issues/231) by @fealho
-* benchmark_single_table crashes with metadata dict - Issue [#232](https://github.com/sdv-dev/SDGym/issues/232) by @fealho
-* Passing None as synthesizers runs all of them - Issue [#233](https://github.com/sdv-dev/SDGym/issues/233) by @fealho
-* timeout parameter causes sdgym to crash - Issue [#234](https://github.com/sdv-dev/SDGym/issues/234) by @pvk-developer
-* SDGym is not working with latest torch - Issue [#210](https://github.com/sdv-dev/SDGym/issues/210) by @amontanez24
-* Fix sdgym --help - Issue [#206](https://github.com/sdv-dev/SDGym/issues/206) by @katxiao
-
-### Internal
-
-* Increase code style lint - Issue [#123](https://github.com/sdv-dev/SDGym/issues/123) by @fealho
-* Remove code support for synthesizers that are not strings/classes - PR [#236](https://github.com/sdv-dev/SDGym/pull/236) by @fealho
-* Code Refactoring - Issue [#215](https://github.com/sdv-dev/SDGym/issues/215) by @fealho
-
-### Maintenance
-
-* Remove pomegranate - Issue [#230](https://github.com/sdv-dev/SDGym/issues/230) by @amontanez24
-
 ## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
```

### Comparing `sdgym-0.7.0/sdgym.egg-info/SOURCES.txt` & `sdgym-0.7.0.dev0/sdgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/sdgym.egg-info/requires.txt` & `sdgym-0.7.0.dev0/sdgym.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/setup.cfg` & `sdgym-0.7.0.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.0
+current_version = 0.7.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdgym-0.7.0/setup.py` & `sdgym-0.7.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,10 +138,10 @@
     name='sdgym',
     packages=find_packages(include=['sdgym', 'sdgym.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDGym',
-    version='0.7.0',
+    version='0.7.0.dev0',
     zip_safe=False,
 )
```

### Comparing `sdgym-0.7.0/tests/integration/synthesizers/test_independent.py` & `sdgym-0.7.0.dev0/tests/integration/synthesizers/test_independent.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/integration/synthesizers/test_uniform.py` & `sdgym-0.7.0.dev0/tests/integration/synthesizers/test_uniform.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/integration/test_benchmark.py` & `sdgym-0.7.0.dev0/tests/integration/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/synthesizers/test_generate.py` & `sdgym-0.7.0.dev0/tests/unit/synthesizers/test_generate.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/synthesizers/test_independent.py` & `sdgym-0.7.0.dev0/tests/unit/synthesizers/test_independent.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/test_benchmark.py` & `sdgym-0.7.0.dev0/tests/unit/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/test_datasets.py` & `sdgym-0.7.0.dev0/tests/unit/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/test_s3.py` & `sdgym-0.7.0.dev0/tests/unit/test_s3.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/test_summary.py` & `sdgym-0.7.0.dev0/tests/unit/test_summary.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.7.0/tests/unit/test_utils.py` & `sdgym-0.7.0.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

