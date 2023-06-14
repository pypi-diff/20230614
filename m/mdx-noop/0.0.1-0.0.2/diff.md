# Comparing `tmp/mdx_noop-0.0.1.tar.gz` & `tmp/mdx_noop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdx_noop-0.0.1.tar", last modified: Sat Jun  3 15:45:01 2023, max compression
+gzip compressed data, was "mdx_noop-0.0.2.tar", last modified: Wed Jun 14 12:57:53 2023, max compression
```

## Comparing `mdx_noop-0.0.1.tar` & `mdx_noop-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-06-03 15:45:01.777748 mdx_noop-0.0.1/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1074 2023-06-03 15:40:07.000000 mdx_noop-0.0.1/LICENSE.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1813 2023-06-03 15:45:01.777748 mdx_noop-0.0.1/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-06-02 12:59:32.000000 mdx_noop-0.0.1/README.md
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-06-03 15:45:01.777748 mdx_noop-0.0.1/mdx_noop.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1813 2023-06-03 15:45:01.000000 mdx_noop-0.0.1/mdx_noop.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      207 2023-06-03 15:45:01.000000 mdx_noop-0.0.1/mdx_noop.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-06-03 15:45:01.000000 mdx_noop-0.0.1/mdx_noop.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        9 2023-06-03 15:45:01.000000 mdx_noop-0.0.1/mdx_noop.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        9 2023-06-03 15:45:01.000000 mdx_noop-0.0.1/mdx_noop.egg-info/top_level.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      730 2023-06-03 15:32:23.000000 mdx_noop-0.0.1/mdx_noop.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      684 2023-06-03 15:44:14.000000 mdx_noop-0.0.1/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2023-06-03 15:45:01.777748 mdx_noop-0.0.1/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-06-14 12:57:53.944563 mdx_noop-0.0.2/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1074 2023-06-03 15:40:07.000000 mdx_noop-0.0.2/LICENSE.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1813 2023-06-14 12:57:53.944563 mdx_noop-0.0.2/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-06-02 12:59:32.000000 mdx_noop-0.0.2/README.md
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-06-14 12:57:53.944563 mdx_noop-0.0.2/mdx_noop.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1813 2023-06-14 12:57:53.000000 mdx_noop-0.0.2/mdx_noop.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      207 2023-06-14 12:57:53.000000 mdx_noop-0.0.2/mdx_noop.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-06-14 12:57:53.000000 mdx_noop-0.0.2/mdx_noop.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        9 2023-06-14 12:57:53.000000 mdx_noop-0.0.2/mdx_noop.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        9 2023-06-14 12:57:53.000000 mdx_noop-0.0.2/mdx_noop.egg-info/top_level.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      732 2023-06-14 12:45:31.000000 mdx_noop-0.0.2/mdx_noop.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      684 2023-06-14 12:54:48.000000 mdx_noop-0.0.2/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2023-06-14 12:57:53.944563 mdx_noop-0.0.2/setup.cfg
```

### Comparing `mdx_noop-0.0.1/LICENSE.txt` & `mdx_noop-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdx_noop-0.0.1/PKG-INFO` & `mdx_noop-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdx_noop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Markdown extension to add "noop" formatting directives
 Author-email: Fabian Geiselhart <me@f4814n.de>
 License: MIT License
         
         Copyright (c) 2023 Fabian Geiselhart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mdx_noop-0.0.1/mdx_noop.egg-info/PKG-INFO` & `mdx_noop-0.0.2/mdx_noop.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdx-noop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Markdown extension to add "noop" formatting directives
 Author-email: Fabian Geiselhart <me@f4814n.de>
 License: MIT License
         
         Copyright (c) 2023 Fabian Geiselhart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mdx_noop-0.0.1/mdx_noop.py` & `mdx_noop-0.0.2/mdx_noop.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
         return el, m.start(0), m.end(0)
 
 
 class IgnoreLatexExtension(Extension):
     def extendMarkdown(self, md):
         LATEX_PATTERN = r'(\$\$.+?\$\$|\$.+?\$)'  # like --del--
         md.inlinePatterns.register(
-            IgnoreLatexInlineProcessor(LATEX_PATTERN, md), 'latex', 175
+            IgnoreLatexInlineProcessor(LATEX_PATTERN, md), 'latex', 10000
         )
 
 
 def makeExtension(**kwargs):  # pragma: no cover
     return IgnoreLatexExtension(**kwargs)
```

### Comparing `mdx_noop-0.0.1/pyproject.toml` & `mdx_noop-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdx_noop"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
 	{ name="Fabian Geiselhart", email = "me@f4814n.de" },
 ]
 description = "Markdown extension to add \"noop\" formatting directives"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.7"
```

