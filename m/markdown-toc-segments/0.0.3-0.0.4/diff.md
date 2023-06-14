# Comparing `tmp/markdown_toc_segments-0.0.3.tar.gz` & `tmp/markdown_toc_segments-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_toc_segments-0.0.3.tar", max compression
+gzip compressed data, was "markdown_toc_segments-0.0.4.tar", max compression
```

## Comparing `markdown_toc_segments-0.0.3.tar` & `markdown_toc_segments-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     6131 2023-05-26 13:53:52.389529 markdown_toc_segments-0.0.3/README.md
--rw-r--r--   0        0        0      138 2023-05-26 12:30:58.695157 markdown_toc_segments-0.0.3/markdown_toc_segments/__init__.py
--rw-r--r--   0        0        0      358 2023-05-26 10:26:27.753009 markdown_toc_segments-0.0.3/markdown_toc_segments/footnote.py
--rw-r--r--   0        0        0     3505 2023-05-26 13:57:59.627945 markdown_toc_segments-0.0.3/markdown_toc_segments/main.py
--rw-r--r--   0        0        0     3235 2023-05-26 12:24:28.869101 markdown_toc_segments-0.0.3/markdown_toc_segments/segment.py
--rw-r--r--   0        0        0      333 2023-05-26 11:19:36.097115 markdown_toc_segments-0.0.3/markdown_toc_segments/utils.py
--rw-r--r--   0        0        0     1100 2023-05-26 13:58:34.582505 markdown_toc_segments-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6831 1970-01-01 00:00:00.000000 markdown_toc_segments-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6131 2023-06-14 09:31:42.319619 markdown_toc_segments-0.0.4/README.md
+-rw-r--r--   0        0        0      138 2023-06-14 09:31:42.319935 markdown_toc_segments-0.0.4/markdown_toc_segments/__init__.py
+-rw-r--r--   0        0        0     1063 2023-06-14 09:31:42.320056 markdown_toc_segments-0.0.4/markdown_toc_segments/clean.py
+-rw-r--r--   0        0        0      358 2023-06-14 09:31:42.320167 markdown_toc_segments-0.0.4/markdown_toc_segments/footnote.py
+-rw-r--r--   0        0        0     3505 2023-06-14 09:31:42.320268 markdown_toc_segments-0.0.4/markdown_toc_segments/main.py
+-rw-r--r--   0        0        0     3235 2023-06-14 09:31:42.320415 markdown_toc_segments-0.0.4/markdown_toc_segments/segment.py
+-rw-r--r--   0        0        0      333 2023-06-14 09:31:42.320534 markdown_toc_segments-0.0.4/markdown_toc_segments/utils.py
+-rw-r--r--   0        0        0     1225 2023-06-14 09:33:45.750094 markdown_toc_segments-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6827 1970-01-01 00:00:00.000000 markdown_toc_segments-0.0.4/PKG-INFO
```

### Comparing `markdown_toc_segments-0.0.3/README.md` & `markdown_toc_segments-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `markdown_toc_segments-0.0.3/markdown_toc_segments/main.py` & `markdown_toc_segments-0.0.4/markdown_toc_segments/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         >>> from pathlib import Path
         >>> from markdown_toc_segments import Outline
         >>> f = Path().cwd() / "temp.md"
         >>> obj = Outline(raw=f.read_text())
         >>> len(obj.segments)
         13
         >>> len(obj.footnotes)
-        5
+        7
         >>> len(obj.tree)
         1
         >>> len(obj.tree[0])
         5
         >>> len(obj.items) # same number of segments
         13
```

### Comparing `markdown_toc_segments-0.0.3/markdown_toc_segments/segment.py` & `markdown_toc_segments-0.0.4/markdown_toc_segments/segment.py`

 * *Files identical despite different names*

### Comparing `markdown_toc_segments-0.0.3/pyproject.toml` & `markdown_toc_segments-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 [tool.poetry]
 name = "markdown-toc-segments"
 description = "Create markdown segments based on a table of contents"
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/markdown-toc-segments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-markdown = "^3.4.3"
+markdown = "^3.2"
 beautifulsoup4 = "^4.12.2"
 markdownify = "^0.11.6"
 
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-cov = "^2.12"
 pre-commit = "^2.21"
+ipykernel = "^6.23.1"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.15"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
```

### Comparing `markdown_toc_segments-0.0.3/PKG-INFO` & `markdown_toc_segments-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: markdown-toc-segments
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create markdown segments based on a table of contents
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: markdown (>=3.2,<4.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Project-URL: Repository, https://github.com/justmars/markdown-toc-segments
 Description-Content-Type: text/markdown
 
 # markdown-toc-segments
 
 ![Github CI](https://github.com/justmars/markdown-toc-segments/actions/workflows/main.yml/badge.svg)
```

