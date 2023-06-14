# Comparing `tmp/shopee-api-wrapper-0.1.0.tar.gz` & `tmp/shopee-api-wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopee-api-wrapper-0.1.0.tar", last modified: Wed Jun 14 15:47:22 2023, max compression
+gzip compressed data, was "shopee-api-wrapper-0.1.1.tar", last modified: Wed Jun 14 18:36:57 2023, max compression
```

## Comparing `shopee-api-wrapper-0.1.0.tar` & `shopee-api-wrapper-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:47:22.889504 shopee-api-wrapper-0.1.0/
--rw-rw-rw-   0        0        0     1111 2023-06-14 15:47:22.888496 shopee-api-wrapper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      815 2023-06-14 15:44:49.000000 shopee-api-wrapper-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 15:47:22.890499 shopee-api-wrapper-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      584 2023-06-14 15:47:20.000000 shopee-api-wrapper-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:47:22.859502 shopee-api-wrapper-0.1.0/shopee_api/
--rw-rw-rw-   0        0        0     1480 2023-06-14 15:34:22.000000 shopee-api-wrapper-0.1.0/shopee_api/__init__.py
--rw-rw-rw-   0        0        0       44 2023-06-14 15:16:32.000000 shopee-api-wrapper-0.1.0/shopee_api/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:47:22.885499 shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0     1111 2023-06-14 15:47:22.000000 shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-14 15:47:22.000000 shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 15:47:22.000000 shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 15:47:22.000000 shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 18:36:57.356286 shopee-api-wrapper-0.1.1/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:36:57.353285 shopee-api-wrapper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-06-14 15:44:49.000000 shopee-api-wrapper-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 18:36:57.356286 shopee-api-wrapper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      599 2023-06-14 18:36:41.000000 shopee-api-wrapper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:36:57.250287 shopee-api-wrapper-0.1.1/shopee_api/
+-rw-rw-rw-   0        0        0     1480 2023-06-14 15:34:22.000000 shopee-api-wrapper-0.1.1/shopee_api/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-06-14 15:16:32.000000 shopee-api-wrapper-0.1.1/shopee_api/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:36:57.261290 shopee-api-wrapper-0.1.1/shopee_api/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:36:36.000000 shopee-api-wrapper-0.1.1/shopee_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      523 2023-06-14 15:27:05.000000 shopee-api-wrapper-0.1.1/shopee_api/utils/product_url.py
+-rw-rw-rw-   0        0        0      265 2023-06-14 15:04:35.000000 shopee-api-wrapper-0.1.1/shopee_api/utils/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-14 18:36:57.349286 shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:36:57.000000 shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-14 18:36:57.000000 shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 18:36:57.000000 shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-14 18:36:57.000000 shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/top_level.txt
```

### Comparing `shopee-api-wrapper-0.1.0/PKG-INFO` & `shopee-api-wrapper-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shopee-api-wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library that communicates with the Shopee website API.
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
-Keywords: amazon affiliate scraper
+Keywords: shopee api crawler scraper product shop
 Description-Content-Type: text/markdown
 
 # Shopee API Wrapper - Not official
 
 ## Install
 
 ```
```

### Comparing `shopee-api-wrapper-0.1.0/README.md` & `shopee-api-wrapper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shopee-api-wrapper-0.1.0/setup.py` & `shopee-api-wrapper-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="shopee-api-wrapper",
-    version="0.1.0",
+    version="0.1.1",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
-    keywords="amazon affiliate scraper",
+    keywords="shopee api crawler scraper product shop",
     description="A simple library that communicates with the Shopee website API.",
     packages=["shopee_api"] + [ "shopee_api/" + x for x in find_packages("shopee_api") ]
 )
```

### Comparing `shopee-api-wrapper-0.1.0/shopee_api/__init__.py` & `shopee-api-wrapper-0.1.1/shopee_api/__init__.py`

 * *Files identical despite different names*

### Comparing `shopee-api-wrapper-0.1.0/shopee_api_wrapper.egg-info/PKG-INFO` & `shopee-api-wrapper-0.1.1/shopee_api_wrapper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shopee-api-wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library that communicates with the Shopee website API.
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
-Keywords: amazon affiliate scraper
+Keywords: shopee api crawler scraper product shop
 Description-Content-Type: text/markdown
 
 # Shopee API Wrapper - Not official
 
 ## Install
 
 ```
```

