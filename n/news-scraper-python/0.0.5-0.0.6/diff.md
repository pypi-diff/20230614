# Comparing `tmp/news-scraper-python-0.0.5.tar.gz` & `tmp/news-scraper-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-scraper-python-0.0.5.tar", last modified: Wed Jun 14 06:17:32 2023, max compression
+gzip compressed data, was "news-scraper-python-0.0.6.tar", last modified: Wed Jun 14 06:45:01 2023, max compression
```

## Comparing `news-scraper-python-0.0.5.tar` & `news-scraper-python-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972970 news-scraper-python-0.0.5/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:17:32.972862 news-scraper-python-0.0.5/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.5/README.md
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972200 news-scraper-python-0.0.5/news_scraper_python/
--rw-r--r--   0 aayushrshah   (502) staff       (20)       28 2023-06-14 06:17:12.000000 news-scraper-python-0.0.5/news_scraper_python/__init__.py
--rw-r--r--   0 aayushrshah   (502) staff       (20)     3749 2023-06-14 06:15:06.000000 news-scraper-python-0.0.5/news_scraper_python/app.py
--rw-r--r--   0 aayushrshah   (502) staff       (20)     4425 2023-06-14 04:26:19.000000 news-scraper-python-0.0.5/news_scraper_python/utils.py
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972713 news-scraper-python-0.0.5/news_scraper_python.egg-info/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)      320 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/SOURCES.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/dependency_links.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/requires.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       20 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/top_level.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-14 06:17:32.973015 news-scraper-python-0.0.5/setup.cfg
--rw-r--r--   0 aayushrshah   (502) staff       (20)      725 2023-06-14 06:16:49.000000 news-scraper-python-0.0.5/setup.py
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:45:01.807710 news-scraper-python-0.0.6/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:45:01.807584 news-scraper-python-0.0.6/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.6/README.md
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:45:01.806669 news-scraper-python-0.0.6/news_scraper_python/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       28 2023-06-14 06:17:12.000000 news-scraper-python-0.0.6/news_scraper_python/__init__.py
+-rw-r--r--   0 aayushrshah   (502) staff       (20)     3729 2023-06-14 06:43:46.000000 news-scraper-python-0.0.6/news_scraper_python/app.py
+-rw-r--r--   0 aayushrshah   (502) staff       (20)     4425 2023-06-14 04:26:19.000000 news-scraper-python-0.0.6/news_scraper_python/utils.py
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:45:01.807400 news-scraper-python-0.0.6/news_scraper_python.egg-info/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:45:01.000000 news-scraper-python-0.0.6/news_scraper_python.egg-info/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      320 2023-06-14 06:45:01.000000 news-scraper-python-0.0.6/news_scraper_python.egg-info/SOURCES.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-14 06:45:01.000000 news-scraper-python-0.0.6/news_scraper_python.egg-info/dependency_links.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-14 06:45:01.000000 news-scraper-python-0.0.6/news_scraper_python.egg-info/requires.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       20 2023-06-14 06:45:01.000000 news-scraper-python-0.0.6/news_scraper_python.egg-info/top_level.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-14 06:45:01.807749 news-scraper-python-0.0.6/setup.cfg
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      725 2023-06-14 06:44:01.000000 news-scraper-python-0.0.6/setup.py
```

### Comparing `news-scraper-python-0.0.5/news_scraper_python/app.py` & `news-scraper-python-0.0.6/news_scraper_python/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,31 +46,31 @@
     obj = {
         "title":article.title,
         "date":article.publish_date,
         "content":article.text,
         "image":article.top_image,
         "url":article.url,
     }
-    collection.insert_one(obj)
+    try:
+        collection.insert_one(obj)
+    except Exception as error:
+        print("error pushing to db",error)
 
 def threaded(links,conn_string):
     futures = []
     executor = ThreadPoolExecutor(max_workers=40)
     for link in links:
         future = executor.submit(handleArticle, link)
         futures.append(future)
         
     for _, future in enumerate(as_completed(futures)):
         article = future.result()
-        try:
-            if article.text == "":
-                continue
-            insert_to_db(article,conn_string)
-        except Exception as error:
-            print("error pushing to db",error)
+        if article.text == "":
+            continue
+        insert_to_db(article,conn_string)
 
 def get_links(keywords,websites):
     data = []
     for keyword in keywords:
         for website in websites:
 
             #sleep for a random interval so requests aren't sent in regular time periods
```

### Comparing `news-scraper-python-0.0.5/news_scraper_python/utils.py` & `news-scraper-python-0.0.6/news_scraper_python/utils.py`

 * *Files identical despite different names*

### Comparing `news-scraper-python-0.0.5/setup.py` & `news-scraper-python-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="news-scraper-python",
-    version="0.0.5",
+    version="0.0.6",
     author="Aayush Shah",
     author_email="aayushshah1142@gmail.com",
     description="A package to scrape news by keywords and source websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FarMart-Tech/news-scraper",
     project_urls={"Bug Tracker": "https://github.com/FarMart-Tech/news-scraper"},
```

