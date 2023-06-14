# Comparing `tmp/metaschema-0.0.1.tar.gz` & `tmp/metaschema-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaschema-0.0.1.tar", max compression
+gzip compressed data, was "metaschema-0.0.2.tar", max compression
```

## Comparing `metaschema-0.0.1.tar` & `metaschema-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-02-21 06:35:15.938858 metaschema-0.0.1/LICENSE
--rw-r--r--   0        0        0       64 2023-02-21 08:30:54.872896 metaschema-0.0.1/README.md
--rw-r--r--   0        0        0      501 2023-02-21 08:30:46.682881 metaschema-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-21 06:45:34.569626 metaschema-0.0.1/src/metaschema/__init__.py
--rw-r--r--   0        0        0     2452 2023-02-21 07:52:45.669390 metaschema-0.0.1/src/metaschema/indicators.py
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 metaschema-0.0.1/setup.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 metaschema-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-02-21 06:35:15.938858 metaschema-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1115 2023-05-27 20:50:26.950675 metaschema-0.0.2/README.md
+-rw-r--r--   0        0        0      639 2023-06-14 01:17:48.242391 metaschema-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-14 01:17:48.246786 metaschema-0.0.2/src/metaschema/__init__.py
+-rw-r--r--   0        0        0     9836 2023-05-27 21:25:33.959152 metaschema-0.0.2/src/metaschema/doc.py
+-rw-r--r--   0        0        0     2376 2023-02-21 09:06:26.479087 metaschema-0.0.2/src/metaschema/indicators.py
+-rw-r--r--   0        0        0    23342 2023-02-21 09:16:26.541485 metaschema-0.0.2/src/metaschema/indicators2.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 metaschema-0.0.2/PKG-INFO
```

### Comparing `metaschema-0.0.1/LICENSE` & `metaschema-0.0.2/LICENSE`

 * *Files identical despite different names*

