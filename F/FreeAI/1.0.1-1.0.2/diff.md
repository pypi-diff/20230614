# Comparing `tmp/FreeAI-1.0.1.tar.gz` & `tmp/FreeAI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeAI-1.0.1.tar", last modified: Tue Jun 13 17:35:44 2023, max compression
+gzip compressed data, was "FreeAI-1.0.2.tar", last modified: Wed Jun 14 15:21:49 2023, max compression
```

## Comparing `FreeAI-1.0.1.tar` & `FreeAI-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:35:44.917489 FreeAI-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:35:44.917489 FreeAI-1.0.1/FreeAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-13 17:35:44.000000 FreeAI-1.0.1/FreeAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-13 17:35:44.000000 FreeAI-1.0.1/FreeAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:35:44.000000 FreeAI-1.0.1/FreeAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 17:35:44.000000 FreeAI-1.0.1/FreeAI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:35:44.000000 FreeAI-1.0.1/FreeAI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-13 17:35:44.917489 FreeAI-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2883 2023-06-13 21:45:44.000000 FreeAI-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      811 2023-06-13 22:29:18.000000 FreeAI-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 17:35:44.917489 FreeAI-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-13 21:36:46.000000 FreeAI-1.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 15:21:49.960925 FreeAI-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)      538 2023-06-14 15:21:49.960925 FreeAI-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2868 2023-06-14 15:19:41.000000 FreeAI-1.0.2/README.md
+-rw-rw----   0 root         (0) everybody  (9997)      811 2023-06-14 15:18:48.000000 FreeAI-1.0.2/pyproject.toml
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-14 15:21:49.964925 FreeAI-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      654 2023-06-14 10:02:13.000000 FreeAI-1.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 15:21:49.932925 FreeAI-1.0.2/src/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 15:21:49.944925 FreeAI-1.0.2/src/FreeAI/
+-rw-rw----   0 root         (0) everybody  (9997)       69 2023-06-14 10:08:00.000000 FreeAI-1.0.2/src/FreeAI/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     1849 2023-06-14 15:17:45.000000 FreeAI-1.0.2/src/FreeAI/generator.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-14 15:21:49.956925 FreeAI-1.0.2/src/FreeAI.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      538 2023-06-14 15:21:49.000000 FreeAI-1.0.2/src/FreeAI.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      249 2023-06-14 15:21:49.000000 FreeAI-1.0.2/src/FreeAI.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-14 15:21:49.000000 FreeAI-1.0.2/src/FreeAI.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-06-14 15:21:49.000000 FreeAI-1.0.2/src/FreeAI.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-14 15:21:49.000000 FreeAI-1.0.2/src/FreeAI.egg-info/top_level.txt
```

### Comparing `FreeAI-1.0.1/README.md` & `FreeAI-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # FreeAI: An Advanced GPT-based Text Generation Package
 
-<!-- ![FreeAI Logo](https://example.com/freeai_logo.png)-->
+<!-- ![FreeAI Logo](/img/freeai_logo.png)-->
 
 FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT-3/4 (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 
 ## Features
 
 - **Advanced GPT Text Generation**: FreeAI leverages state-of-the-art GPT models to generate high-quality and contextually relevant text.
 - **Flexible Prompt Customization**: Users can easily provide their own prompts to guide the text generation process.
```

### Comparing `FreeAI-1.0.1/pyproject.toml` & `FreeAI-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FreeAI"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Ashiq Hussain", email="imseldrith@gmail.com" }
 ]
 description = "FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

