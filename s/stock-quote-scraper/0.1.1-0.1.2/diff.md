# Comparing `tmp/stock-quote-scraper-0.1.1.tar.gz` & `tmp/stock-quote-scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock-quote-scraper-0.1.1.tar", last modified: Tue Jun 13 22:51:23 2023, max compression
+gzip compressed data, was "stock-quote-scraper-0.1.2.tar", last modified: Tue Jun 13 23:02:05 2023, max compression
```

## Comparing `stock-quote-scraper-0.1.1.tar` & `stock-quote-scraper-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 stock-quote-scraper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2330 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-13 17:12:03.000000 stock-quote-scraper-0.1.1/README.md
--rw-rw-rw-   0        0        0     1345 2023-06-13 22:50:18.000000 stock-quote-scraper-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.209374 stock-quote-scraper-0.1.1/sqs/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 stock-quote-scraper-0.1.1/sqs/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 stock-quote-scraper-0.1.1/sqs/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:51:23.225015 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/
--rw-rw-rw-   0        0        0     2330 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 22:51:23.000000 stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 23:02:05.936285 stock-quote-scraper-0.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 stock-quote-scraper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2330 2023-06-13 23:02:05.936285 stock-quote-scraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-13 17:12:03.000000 stock-quote-scraper-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1375 2023-06-13 23:01:11.000000 stock-quote-scraper-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 23:02:05.936285 stock-quote-scraper-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 23:02:05.898502 stock-quote-scraper-0.1.2/sqs/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:55:42.000000 stock-quote-scraper-0.1.2/sqs/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:16:53.000000 stock-quote-scraper-0.1.2/sqs/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:02:05.914136 stock-quote-scraper-0.1.2/sqs/cnbc/
+-rw-rw-rw-   0        0        0       49 2023-06-13 21:33:37.000000 stock-quote-scraper-0.1.2/sqs/cnbc/__init__.py
+-rw-rw-rw-   0        0        0     7647 2023-06-13 22:18:31.000000 stock-quote-scraper-0.1.2/sqs/cnbc/quote_strip.py
+-rw-rw-rw-   0        0        0      835 2023-06-13 22:18:02.000000 stock-quote-scraper-0.1.2/sqs/cnbc/stock_quote.py
+drwxrwxrwx   0        0        0        0 2023-06-13 23:02:05.936285 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/
+-rw-rw-rw-   0        0        0     2330 2023-06-13 23:02:05.000000 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-06-13 23:02:05.000000 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 23:02:05.000000 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-13 23:02:05.000000 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-13 23:02:05.000000 stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/top_level.txt
```

### Comparing `stock-quote-scraper-0.1.1/LICENSE` & `stock-quote-scraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stock-quote-scraper-0.1.1/PKG-INFO` & `stock-quote-scraper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-quote-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Web scraper for various stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stock-quote-scraper-0.1.1/pyproject.toml` & `stock-quote-scraper-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stock-quote-scraper"
-version = "0.1.1"
+version = "0.1.2"
 description = "Web scraper for various stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Financial and Insurance Industry",
@@ -34,9 +34,14 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/stock-quote-scraper"
 
 [tool.setuptools.packages.find]
 where = ["."]
-include = ["sqs"]
-exclude = ["sqs.tests*"]
+include = [
+    "sqs",
+    "sqs.*"
+]
+exclude = [
+    "sqs.tests*"
+]
```

### Comparing `stock-quote-scraper-0.1.1/stock_quote_scraper.egg-info/PKG-INFO` & `stock-quote-scraper-0.1.2/stock_quote_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-quote-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Web scraper for various stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

