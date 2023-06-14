# Comparing `tmp/test_jrubics_poetry_publish-0.2.1.tar.gz` & `tmp/test_jrubics_poetry_publish-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_jrubics_poetry_publish-0.2.1.tar", max compression
+gzip compressed data, was "test_jrubics_poetry_publish-0.2.2.tar", max compression
```

## Comparing `test_jrubics_poetry_publish-0.2.1.tar` & `test_jrubics_poetry_publish-0.2.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      320 2023-03-06 21:16:24.943687 test_jrubics_poetry_publish-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-03-06 21:16:24.943687 test_jrubics_poetry_publish-0.2.1/test_jrubics_poetry_publish/__init__.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 test_jrubics_poetry_publish-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      320 2023-05-22 07:48:36.461430 test_jrubics_poetry_publish-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-22 07:48:36.461430 test_jrubics_poetry_publish-0.2.2/test_jrubics_poetry_publish/__init__.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 test_jrubics_poetry_publish-0.2.2/PKG-INFO
```

