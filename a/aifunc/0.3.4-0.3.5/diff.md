# Comparing `tmp/aifunc-0.3.4.tar.gz` & `tmp/aifunc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.3.4.tar", max compression
+gzip compressed data, was "aifunc-0.3.5.tar", max compression
```

## Comparing `aifunc-0.3.4.tar` & `aifunc-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       94 2023-06-13 21:34:20.685507 aifunc-0.3.4/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.3.4/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      372 2023-06-13 21:47:21.569396 aifunc-0.3.4/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0     3180 2023-06-13 21:46:26.251737 aifunc-0.3.4/aifunc/evaluate_answer.yaml
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.3.4/aifunc/follow_up.py
--rw-r--r--   0        0        0     1812 2023-06-13 22:07:51.183195 aifunc-0.3.4/aifunc/follow_up.yaml
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.4/aifunc/generate_question.py
--rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.4/aifunc/generate_question.yaml
--rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.4/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-13 22:09:11.919455 aifunc-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      126 2023-06-13 22:25:34.728002 aifunc-0.3.5/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.3.5/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      372 2023-06-13 21:47:21.569396 aifunc-0.3.5/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0     3180 2023-06-13 21:46:26.251737 aifunc-0.3.5/aifunc/evaluate_answer.yaml
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.3.5/aifunc/follow_up.py
+-rw-r--r--   0        0        0     1812 2023-06-13 22:07:51.183195 aifunc-0.3.5/aifunc/follow_up.yaml
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.5/aifunc/generate_question.py
+-rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.5/aifunc/generate_question.yaml
+-rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.5/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-13 22:25:37.392275 aifunc-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.5/PKG-INFO
```

### Comparing `aifunc-0.3.4/aifunc/add_ai_function.py` & `aifunc-0.3.5/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.3.4/aifunc/evaluate_answer.yaml` & `aifunc-0.3.5/aifunc/evaluate_answer.yaml`

 * *Files identical despite different names*

### Comparing `aifunc-0.3.4/aifunc/follow_up.yaml` & `aifunc-0.3.5/aifunc/follow_up.yaml`

 * *Files identical despite different names*

### Comparing `aifunc-0.3.4/aifunc/utility.py` & `aifunc-0.3.5/aifunc/utility.py`

 * *Files identical despite different names*

