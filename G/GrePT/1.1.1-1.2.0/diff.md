# Comparing `tmp/GrePT-1.1.1.tar.gz` & `tmp/GrePT-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrePT-1.1.1.tar", last modified: Sun Apr 16 10:15:53 2023, max compression
+gzip compressed data, was "GrePT-1.2.0.tar", last modified: Tue Jun 13 20:03:10 2023, max compression
```

## Comparing `GrePT-1.1.1.tar` & `GrePT-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:15:53.543697 GrePT-1.1.1/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1067 2023-03-22 12:52:59.000000 GrePT-1.1.1/LICENSE.md
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       40 2023-03-22 13:38:22.000000 GrePT-1.1.1/MANIFEST.in
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-04-16 10:15:53.543697 GrePT-1.1.1/PKG-INFO
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      938 2023-04-06 12:22:25.000000 GrePT-1.1.1/README.md
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1007 2023-04-16 10:14:09.000000 GrePT-1.1.1/pyproject.toml
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       38 2023-04-16 10:15:53.543697 GrePT-1.1.1/setup.cfg
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:15:53.533697 GrePT-1.1.1/src/
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:15:53.543697 GrePT-1.1.1/src/GrePT.egg-info/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/PKG-INFO
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      359 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/SOURCES.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)        1 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/dependency_links.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       46 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/entry_points.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       48 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/requires.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)        6 2023-04-16 10:15:53.000000 GrePT-1.1.1/src/GrePT.egg-info/top_level.txt
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:15:53.543697 GrePT-1.1.1/src/grept/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       21 2023-04-16 10:14:09.000000 GrePT-1.1.1/src/grept/__init__.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     6174 2023-04-16 10:14:09.000000 GrePT-1.1.1/src/grept/__main__.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     3409 2023-04-07 14:24:03.000000 GrePT-1.1.1/src/grept/completions.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      121 2023-04-07 17:22:47.000000 GrePT-1.1.1/src/grept/config.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1058 2023-04-07 14:03:27.000000 GrePT-1.1.1/src/grept/tokenizer.py
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-06-13 20:03:10.835198 GrePT-1.2.0/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1067 2023-03-22 12:52:59.000000 GrePT-1.2.0/LICENSE.md
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)        9 2023-04-23 14:45:47.000000 GrePT-1.2.0/MANIFEST.in
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     2540 2023-06-13 20:03:10.835198 GrePT-1.2.0/PKG-INFO
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     2241 2023-05-28 21:16:06.000000 GrePT-1.2.0/README.md
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1004 2023-06-13 19:59:07.000000 GrePT-1.2.0/pyproject.toml
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       38 2023-06-13 20:03:10.835198 GrePT-1.2.0/setup.cfg
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-06-13 20:03:10.835198 GrePT-1.2.0/src/
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-06-13 20:03:10.835198 GrePT-1.2.0/src/GrePT.egg-info/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     2540 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/PKG-INFO
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      398 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/SOURCES.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)        1 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/dependency_links.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       77 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/entry_points.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       61 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/requires.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)        6 2023-06-13 20:03:10.000000 GrePT-1.2.0/src/GrePT.egg-info/top_level.txt
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-06-13 20:03:10.835198 GrePT-1.2.0/src/grept/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       21 2023-06-13 19:59:07.000000 GrePT-1.2.0/src/grept/__init__.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1791 2023-05-28 21:16:06.000000 GrePT-1.2.0/src/grept/__main__.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1634 2023-06-10 08:51:11.000000 GrePT-1.2.0/src/grept/completions.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      211 2023-06-13 19:45:24.000000 GrePT-1.2.0/src/grept/config.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1368 2023-06-10 08:51:18.000000 GrePT-1.2.0/src/grept/embed.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     2560 2023-06-10 08:51:28.000000 GrePT-1.2.0/src/grept/interactive.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     4178 2023-06-10 08:50:33.000000 GrePT-1.2.0/src/grept/util.py
```

### Comparing `GrePT-1.1.1/LICENSE.md` & `GrePT-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GrePT-1.1.1/pyproject.toml` & `GrePT-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [build-system]
 requires = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GrePT"
-version = "1.1.1"
+version = "1.2.0"
 description = "Talk to your code"
 readme = "README.md"
 authors = [{name = "Jack Barry", email = "jack.barry@live.com"}]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = ["GPT", "OpenAI", "GPT-3"]
 dependencies = [
     "openai >= 0.27.2",
     "termcolor >= 2.2.0",
     "tiktoken >= 0.3.3",
+    "rich >= 13.3.4",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/jackbarry24/GrePT"
 
 [project.scripts]
 grept = "grept.__main__:main"
+grept-embed = "grept.embed:main"
 
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
@@ -38,10 +40,8 @@
     'version = "{version}"',
 ]
 
 "src/grept/__init__.py" = [
     '__version__ = "{version}"',
 ]
 
-"src/grept/__main__.py" = [
-    'VERSION = "{version}"',
-]
+
```

