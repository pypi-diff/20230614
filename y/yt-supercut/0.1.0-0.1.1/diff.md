# Comparing `tmp/yt_supercut-0.1.0.tar.gz` & `tmp/yt_supercut-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_supercut-0.1.0.tar", max compression
+gzip compressed data, was "yt_supercut-0.1.1.tar", max compression
```

## Comparing `yt_supercut-0.1.0.tar` & `yt_supercut-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.0/README.md
--rw-r--r--   0        0        0      658 2023-06-02 22:13:39.612516 yt_supercut-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5959 2023-06-02 19:36:34.711692 yt_supercut-0.1.0/yt_supercut/db.py
--rw-r--r--   0        0        0     3542 2023-06-05 16:10:34.390386 yt_supercut-0.1.0/yt_supercut/main.py
--rw-r--r--   0        0        0     3460 2023-05-31 01:55:22.739587 yt_supercut-0.1.0/yt_supercut/utils.py
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 yt_supercut-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-29 21:15:44.453273 yt_supercut-0.1.1/README.md
+-rw-r--r--   0        0        0      683 2023-06-14 03:24:34.352461 yt_supercut-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5959 2023-06-02 19:36:34.711692 yt_supercut-0.1.1/yt_supercut/db.py
+-rw-r--r--   0        0        0     3542 2023-06-05 16:10:34.390386 yt_supercut-0.1.1/yt_supercut/main.py
+-rw-r--r--   0        0        0     3460 2023-05-31 01:55:22.739587 yt_supercut-0.1.1/yt_supercut/utils.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 yt_supercut-0.1.1/PKG-INFO
```

### Comparing `yt_supercut-0.1.0/pyproject.toml` & `yt_supercut-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yt-supercut"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["redraw <redraw@sdf.org>"]
 readme = "README.md"
 packages = [{include = "yt_supercut"}]
 
 [tool.poetry.scripts]
 yt-supercut = "yt_supercut.main:cli"
@@ -14,14 +14,15 @@
 typer = "^0.9.0"
 yt-dlp = "^2023.3.4"
 datasette = {version = "^0.64.3", extras = ["datasette"]}
 datasette-youtube-embed = {version = "^0.1", extras = ["datasette"]}
 tqdm = "^4.65.0"
 webvtt-py = "^0.4.6"
 tabulate = "^0.9.0"
+sqlite-utils = "^3.32.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.13.2"
 ipdb = "^0.13.13"
 
 
 [build-system]
```

### Comparing `yt_supercut-0.1.0/yt_supercut/db.py` & `yt_supercut-0.1.1/yt_supercut/db.py`

 * *Files identical despite different names*

### Comparing `yt_supercut-0.1.0/yt_supercut/main.py` & `yt_supercut-0.1.1/yt_supercut/main.py`

 * *Files identical despite different names*

### Comparing `yt_supercut-0.1.0/yt_supercut/utils.py` & `yt_supercut-0.1.1/yt_supercut/utils.py`

 * *Files identical despite different names*

### Comparing `yt_supercut-0.1.0/PKG-INFO` & `yt_supercut-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: yt-supercut
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: redraw
 Author-email: redraw@sdf.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasette-youtube-embed[datasette] (>=0.1,<0.2)
 Requires-Dist: datasette[datasette] (>=0.64.3,<0.65.0)
+Requires-Dist: sqlite-utils (>=3.32.1,<4.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: webvtt-py (>=0.4.6,<0.5.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
```

