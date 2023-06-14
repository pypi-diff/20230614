# Comparing `tmp/pelican_email_cloak-0.1.0.tar.gz` & `tmp/pelican_email_cloak-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_email_cloak-0.1.0.tar", max compression
+gzip compressed data, was "pelican_email_cloak-0.1.2.tar", max compression
```

## Comparing `pelican_email_cloak-0.1.0.tar` & `pelican_email_cloak-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.1.0/LICENSE
--rw-r--r--   0        0        0      826 2023-06-08 13:14:16.143047 pelican_email_cloak-0.1.0/README.md
--rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/__init__.py
--rw-r--r--   0        0        0     2075 2023-06-09 12:53:31.768695 pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/email_cloak.py
--rw-r--r--   0        0        0     2472 2023-06-09 12:55:34.703029 pelican_email_cloak-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 pelican_email_cloak-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.1.2/LICENSE
+-rw-r--r--   0        0        0      826 2023-06-08 13:14:16.143047 pelican_email_cloak-0.1.2/README.md
+-rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.1.2/pelican/plugins/email_cloak/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-09 12:53:31.768695 pelican_email_cloak-0.1.2/pelican/plugins/email_cloak/email_cloak.py
+-rw-r--r--   0        0        0     2472 2023-06-14 06:39:35.896395 pelican_email_cloak-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2200 1970-01-01 00:00:00.000000 pelican_email_cloak-0.1.2/PKG-INFO
```

### Comparing `pelican_email_cloak-0.1.0/LICENSE` & `pelican_email_cloak-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.1.0/README.md` & `pelican_email_cloak-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.1.0/pelican/plugins/email_cloak/email_cloak.py` & `pelican_email_cloak-0.1.2/pelican/plugins/email_cloak/email_cloak.py`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.1.0/pyproject.toml` & `pelican_email_cloak-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-email-cloak"
-version = "0.1.0"
+version = "0.1.2"
 description = "E-mail cloaking plugin for Pelican"
 authors = ["Demetrio Battaglia <deme3.iot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pelican", "plugin"]
 repository = "https://github.com/deme3/pelican-email-cloak"
 documentation = "https://docs.getpelican.com"
@@ -26,15 +26,15 @@
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/deme3/pelican-email-cloak/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pelican = ">=4.5"
-mailscrambler = ">=0.0.1"
+mailscrambler = ">=0.1.2"
 markdown = {version = ">=3.2", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23"
 invoke = "^2.0"
 markdown = "^3.4"
 ruff = ">=0.0.272"
```

### Comparing `pelican_email_cloak-0.1.0/PKG-INFO` & `pelican_email_cloak-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-email-cloak
-Version: 0.1.0
+Version: 0.1.2
 Summary: E-mail cloaking plugin for Pelican
 Home-page: https://github.com/deme3/pelican-email-cloak
 License: MIT
 Keywords: pelican,plugin
 Author: Demetrio Battaglia
 Author-email: deme3.iot@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: markdown
-Requires-Dist: mailscrambler (>=0.0.1)
+Requires-Dist: mailscrambler (>=0.1.2)
 Requires-Dist: markdown (>=3.2) ; extra == "markdown"
 Requires-Dist: pelican (>=4.5)
 Project-URL: Documentation, https://docs.getpelican.com
 Project-URL: Funding, https://donate.getpelican.com/
 Project-URL: Issue Tracker, https://github.com/deme3/pelican-email-cloak/issues
 Project-URL: Repository, https://github.com/deme3/pelican-email-cloak
 Description-Content-Type: text/markdown
```

