# Comparing `tmp/tpaw-0.0.1a0.tar.gz` & `tmp/tpaw-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpaw-0.0.1a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tpaw-0.0.1a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tpaw-0.0.1a0.tar` & `tpaw-0.0.1a2.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a0/LICENSE
--rw-r--r--   0        0        0      351 2023-06-14 01:51:34.980692 tpaw-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1894 2023-06-14 01:55:21.949566 tpaw-0.0.1a0/tpaw.py
--rw-r--r--   0        0        0      230 1970-01-01 00:00:00.000000 tpaw-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-06-14 03:45:27.697084 tpaw-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     1296 2023-06-14 01:52:01.890982 tpaw-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0      351 2023-06-14 01:51:34.980692 tpaw-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 03:27:30.402948 tpaw-0.0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0    17029 2023-06-14 04:07:11.683947 tpaw-0.0.1a2/tests/data/groups.html
+-rw-r--r--   0        0        0    35218 2023-06-14 06:34:57.679137 tpaw-0.0.1a2/tests/data/slash_new.html
+-rw-r--r--   0        0        0     1766 2023-06-14 06:50:37.218088 tpaw-0.0.1a2/tests/test_tpaw.py
+-rw-r--r--   0        0        0     6369 2023-06-14 07:10:58.211346 tpaw-0.0.1a2/tpaw.py
+-rw-r--r--   0        0        0      230 1970-01-01 00:00:00.000000 tpaw-0.0.1a2/PKG-INFO
```

### Comparing `tpaw-0.0.1a0/LICENSE` & `tpaw-0.0.1a2/LICENSE`

 * *Files identical despite different names*

