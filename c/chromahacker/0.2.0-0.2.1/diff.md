# Comparing `tmp/chromahacker-0.2.0.tar.gz` & `tmp/chromahacker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.2.0.tar", max compression
+gzip compressed data, was "chromahacker-0.2.1.tar", max compression
```

## Comparing `chromahacker-0.2.0.tar` & `chromahacker-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-14 21:10:33.358138 chromahacker-0.2.0/README.md
--rw-r--r--   0        0        0     6148 2023-06-14 21:10:33.358631 chromahacker-0.2.0/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-14 21:10:33.359019 chromahacker-0.2.0/chromahacker/__init__.py
--rw-r--r--   0        0        0      860 2023-06-14 21:10:33.361084 chromahacker-0.2.0/chromahacker/color_input.py
--rw-r--r--   0        0        0     1204 2023-06-14 21:10:33.362021 chromahacker-0.2.0/chromahacker/palettize/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      499 2023-06-14 21:13:01.421925 chromahacker-0.2.0/chromahacker/palettize.py
--rw-r--r--   0        0        0      357 2023-06-14 21:10:33.362270 chromahacker-0.2.0/chromahacker/process_image.py
--rw-r--r--   0        0        0      424 2023-06-14 21:10:33.362478 chromahacker-0.2.0/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-06-14 21:14:10.366581 chromahacker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 chromahacker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.092423 chromahacker-0.2.1/README.md
+-rw-r--r--   0        0        0     6148 2023-06-06 20:17:27.539807 chromahacker-0.2.1/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.434230 chromahacker-0.2.1/chromahacker/__init__.py
+-rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.371973 chromahacker-0.2.1/chromahacker/color_input.py
+-rw-r--r--   0        0        0      419 2023-06-14 21:19:09.134682 chromahacker-0.2.1/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.357804 chromahacker-0.2.1/chromahacker/process_image.py
+-rw-r--r--   0        0        0      424 2023-06-08 17:20:05.944611 chromahacker-0.2.1/chromahacker/spline.py
+-rw-r--r--   0        0        0      337 2023-06-14 21:19:50.220847 chromahacker-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.1/PKG-INFO
```

### Comparing `chromahacker-0.2.0/chromahacker/.DS_Store` & `chromahacker-0.2.1/chromahacker/.DS_Store`

 * *Files identical despite different names*

