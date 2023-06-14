# Comparing `tmp/gauge_llm-0.0.11.tar.gz` & `tmp/gauge_llm-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauge_llm-0.0.11.tar", max compression
+gzip compressed data, was "gauge_llm-0.0.12.tar", max compression
```

## Comparing `gauge_llm-0.0.11.tar` & `gauge_llm-0.0.12.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-06-14 02:01:28.739715 gauge_llm-0.0.11/LICENSE
--rw-r--r--   0        0        0       50 2023-06-14 02:01:28.739715 gauge_llm-0.0.11/README.md
--rw-r--r--   0        0        0       24 2023-06-14 03:30:38.987167 gauge_llm-0.0.11/gauge/__init__.py
--rw-r--r--   0        0        0     5077 2023-06-14 03:36:47.806712 gauge_llm-0.0.11/gauge/gauge.py
--rw-r--r--   0        0        0      422 2023-06-14 03:39:08.749237 gauge_llm-0.0.11/pyproject.toml
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 gauge_llm-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-14 02:01:28.739715 gauge_llm-0.0.12/LICENSE
+-rw-r--r--   0        0        0       50 2023-06-14 02:01:28.739715 gauge_llm-0.0.12/README.md
+-rw-r--r--   0        0        0       67 2023-06-14 03:47:13.978184 gauge_llm-0.0.12/gauge/__init__.py
+-rw-r--r--   0        0        0     5077 2023-06-14 03:36:47.806712 gauge_llm-0.0.12/gauge/gauge.py
+-rw-r--r--   0        0        0      420 2023-06-14 03:48:33.419934 gauge_llm-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 gauge_llm-0.0.12/PKG-INFO
```

### Comparing `gauge_llm-0.0.11/LICENSE` & `gauge_llm-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `gauge_llm-0.0.11/gauge/gauge.py` & `gauge_llm-0.0.12/gauge/gauge.py`

 * *Files identical despite different names*

