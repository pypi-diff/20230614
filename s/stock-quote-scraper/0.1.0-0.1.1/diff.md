# Comparing `tmp/stock-quote-scraper-0.1.0.tar.gz` & `tmp/stock-quote-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock-quote-scraper-0.1.0.tar", last modified: Tue Jun 13 22:40:13 2023, max compression
+gzip compressed data, was "stock-quote-scraper-0.1.1.tar", last modified: Tue Jun 13 22:51:23 2023, max compression
```

## Comparing `stock-quote-scraper-0.1.0.tar` & `stock-quote-scraper-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:40:13.019066 stock-quote-scraper-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 stock-quote-scraper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2330 2023-06-13 22:40:13.018059 stock-quote-scraper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-13 17:12:03.000000 stock-quote-scraper-0.1.0/README.md
--rw-rw-rw-   0        0        0     1202 2023-06-13 22:39:11.000000 stock-quote-scraper-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 22:40:13.019066 stock-quote-scraper-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 22:40:12.988079 stock-quote-scraper-0.1.0/sqs/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 stock-quote-scraper-0.1.0/sqs/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 stock-quote-scraper-0.1.0/sqs/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:40:13.017047 stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/
--rw-rw-rw-   0        0        0     2330 2023-06-13 22:40:12.000000 stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-13 22:40:12.000000 stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:40:12.000000 stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 22:40:12.000000 stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 stock-quote-scraper-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2330 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-13 17:12:03.000000 stock-quote-scraper-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1345 2023-06-13 22:50:18.000000 stock-quote-scraper-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.209374 stock-quote-scraper-0.1.1/sqs/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 stock-quote-scraper-0.1.1/sqs/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 stock-quote-scraper-0.1.1/sqs/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/
+-rw-rw-rw-   0        0        0     2330 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/top_level.txt
```

### Comparing `stock-quote-scraper-0.1.0/LICENSE` & `stock-quote-scraper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stock-quote-scraper-0.1.0/PKG-INFO` & `stock-quote-scraper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-quote-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web scraper for various stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stock-quote-scraper-0.1.0/pyproject.toml` & `stock-quote-scraper-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stock-quote-scraper"
-version = "0.1.0"
+version = "0.1.1"
 description = "Web scraper for various stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Financial and Insurance Industry",
@@ -22,14 +22,20 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development"
 ]
 requires-python = ">=3.6"
+dependencies = [
+    "beautifulsoup4==4.12.2",
+    "lxml==4.9.2",
+    "numpy==1.24.3",
+    "soupsieve==2.4.1; python_version >= '3.7'"
+]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/stock-quote-scraper"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["sqs"]
```

### Comparing `stock-quote-scraper-0.1.0/stock_quote_scraper.egg-info/PKG-INFO` & `stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-quote-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web scraper for various stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

