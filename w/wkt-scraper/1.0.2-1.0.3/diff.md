# Comparing `tmp/wkt_scraper-1.0.2.tar.gz` & `tmp/wkt_scraper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkt_scraper-1.0.2.tar", last modified: Mon Jun 12 19:38:32 2023, max compression
+gzip compressed data, was "wkt_scraper-1.0.3.tar", last modified: Wed Jun 14 17:49:05 2023, max compression
```

## Comparing `wkt_scraper-1.0.2.tar` & `wkt_scraper-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1068 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/LICENSE
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       18 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/MANIFEST.in
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1097 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/PKG-INFO
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      567 2023-06-11 11:51:47.000000 wkt_scraper-1.0.2/README.md
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.855754 wkt_scraper-1.0.2/scraper/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       29 2023-05-27 22:07:08.000000 wkt_scraper-1.0.2/scraper/__init__.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1418 2023-06-11 11:48:55.000000 wkt_scraper-1.0.2/scraper/language.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)    15572 2023-06-12 19:27:13.000000 wkt_scraper-1.0.2/scraper/scraper.py
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       38 2023-06-12 19:38:32.859754 wkt_scraper-1.0.2/setup.cfg
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      820 2023-06-12 19:35:53.000000 wkt_scraper-1.0.2/setup.py
-drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-12 19:38:32.855754 wkt_scraper-1.0.2/wkt_scraper.egg-info/
--rw-rw-r--   0 fatih     (1000) fatih     (1000)     1097 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 fatih     (1000) fatih     (1000)      271 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)        1 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)       24 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/requires.txt
--rw-rw-r--   0 fatih     (1000) fatih     (1000)        8 2023-06-12 19:38:32.000000 wkt_scraper-1.0.2/wkt_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-14 17:49:05.175447 wkt_scraper-1.0.3/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1068 2023-05-27 22:07:08.000000 wkt_scraper-1.0.3/LICENSE
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       18 2023-05-27 22:07:08.000000 wkt_scraper-1.0.3/MANIFEST.in
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1088 2023-06-14 17:49:05.175447 wkt_scraper-1.0.3/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      558 2023-06-14 17:13:21.000000 wkt_scraper-1.0.3/README.md
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-14 17:49:05.175447 wkt_scraper-1.0.3/scraper/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       37 2023-06-14 17:14:04.000000 wkt_scraper-1.0.3/scraper/__init__.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1418 2023-06-11 11:48:55.000000 wkt_scraper-1.0.3/scraper/language.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)    15713 2023-06-14 17:12:38.000000 wkt_scraper-1.0.3/scraper/scraper.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       38 2023-06-14 17:49:05.175447 wkt_scraper-1.0.3/setup.cfg
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      820 2023-06-14 17:30:41.000000 wkt_scraper-1.0.3/setup.py
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-06-14 17:49:05.175447 wkt_scraper-1.0.3/wkt_scraper.egg-info/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1088 2023-06-14 17:49:05.000000 wkt_scraper-1.0.3/wkt_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      271 2023-06-14 17:49:05.000000 wkt_scraper-1.0.3/wkt_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        1 2023-06-14 17:49:05.000000 wkt_scraper-1.0.3/wkt_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       24 2023-06-14 17:49:05.000000 wkt_scraper-1.0.3/wkt_scraper.egg-info/requires.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        8 2023-06-14 17:49:05.000000 wkt_scraper-1.0.3/wkt_scraper.egg-info/top_level.txt
```

### Comparing `wkt_scraper-1.0.2/LICENSE` & `wkt_scraper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wkt_scraper-1.0.2/PKG-INFO` & `wkt_scraper-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkt_scraper
-Version: 1.0.2
+Version: 1.0.3
 Summary: Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
 Keywords: wiktionary scraper parser
 Classifier: License :: OSI Approved :: MIT License
@@ -19,12 +19,12 @@
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
 In python code, to look up the word "street" from English to Spanish:
 
-    from scraper import Scraper
-    response = Scraper('en', 'es').scrape('street')
+    from scraper import scrape
+    response = scrape('en', 'es', 'street')
 
 Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

### Comparing `wkt_scraper-1.0.2/README.md` & `wkt_scraper-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
 In python code, to look up the word "street" from English to Spanish:
 
-    from scraper import Scraper
-    response = Scraper('en', 'es').scrape('street')
+    from scraper import scrape
+    response = scrape('en', 'es', 'street')
 
 Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

### Comparing `wkt_scraper-1.0.2/scraper/language.py` & `wkt_scraper-1.0.3/scraper/language.py`

 * *Files identical despite different names*

### Comparing `wkt_scraper-1.0.2/scraper/scraper.py` & `wkt_scraper-1.0.3/scraper/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import re
 from typing import Dict, Any, List
 import requests
 from bs4 import BeautifulSoup, PageElement, ResultSet, Tag, NavigableString
 from scraper.language import get_language, language_names
 
 
+def scrape(from_language: str, to_language: str, word: str) -> Dict[str, Any]:
+    return Scraper(from_language, to_language).scrape(word)
+
+
 def get_html(url: str) -> str:
     response = requests.get(url)
     code = response.status_code
     if code != 200:
         raise FileNotFoundError(f'URL not found with status code {code}: {url}')
     return response.content.decode('utf-8')
```

### Comparing `wkt_scraper-1.0.2/setup.py` & `wkt_scraper-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='wkt_scraper',
-    version='1.0.2',
+    version='1.0.3',
     description='Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='wiktionary scraper parser',
     author='Fatih Akgul',
     author_email='akguls@gmail.com',
     license='MIT',
```

### Comparing `wkt_scraper-1.0.2/wkt_scraper.egg-info/PKG-INFO` & `wkt_scraper-1.0.3/wkt_scraper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkt-scraper
-Version: 1.0.2
+Version: 1.0.3
 Summary: Parse word information from Wiktionary. Currently only English, Spanish and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
 Keywords: wiktionary scraper parser
 Classifier: License :: OSI Approved :: MIT License
@@ -19,12 +19,12 @@
 ## Installation
 You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
     
     pip install wkt_scraper
 
 In python code, to look up the word "street" from English to Spanish:
 
-    from scraper import Scraper
-    response = Scraper('en', 'es').scrape('street')
+    from scraper import scrape
+    response = scrape('en', 'es', 'street')
 
 Currently only English, Spanish and Turkish are supported. 
 Supporting more languages will require additional work and testing.
```

