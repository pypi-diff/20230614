# Comparing `tmp/code2gist-0.0.2.tar.gz` & `tmp/code2gist-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code2gist-0.0.2.tar", last modified: Tue Jun 13 18:37:04 2023, max compression
+gzip compressed data, was "code2gist-1.0.0.tar", last modified: Wed Jun 14 03:05:06 2023, max compression
```

## Comparing `code2gist-0.0.2.tar` & `code2gist-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.241269 code2gist-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1367 2023-06-13 18:37:04.240270 code2gist-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-06-13 16:04:03.000000 code2gist-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.193270 code2gist-0.0.2/code2gist/
--rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-0.0.2/code2gist/__init__.py
--rw-rw-rw-   0        0        0     2053 2023-06-13 18:34:48.000000 code2gist-0.0.2/code2gist/main.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.237269 code2gist-0.0.2/code2gist.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-13 18:37:04.000000 code2gist-0.0.2/code2gist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-06-13 18:35:23.000000 code2gist-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 18:37:04.241269 code2gist-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.987349 code2gist-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4021 2023-06-14 03:05:06.987349 code2gist-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3650 2023-06-14 02:59:51.000000 code2gist-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.924815 code2gist-1.0.0/code2gist/
+-rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-1.0.0/code2gist/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-06-14 02:33:47.000000 code2gist-1.0.0/code2gist/main.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.987349 code2gist-1.0.0/code2gist.egg-info/
+-rw-rw-rw-   0        0        0     4021 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      628 2023-06-14 03:03:42.000000 code2gist-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:05:06.987349 code2gist-1.0.0/setup.cfg
```

### Comparing `code2gist-0.0.2/LICENSE` & `code2gist-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code2gist-0.0.2/pyproject.toml` & `code2gist-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code2gist"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
     {name = "Cameron Spears", email = "crspears@outlook.com"},
 ]
 description = "Upload Python files in a directory to a GitHub Gist."
 readme = "README.md"
 requires-python = ">=3.11.4"
 keywords = ["python", "github", "gist", "upload"]
 license = {text = "GPL-3.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "requests>=2.28.2",
+    "pathspec>=0.11.1",
 ]
 
 [project.scripts]
 code2gist = "code2gist.main:main"
```

