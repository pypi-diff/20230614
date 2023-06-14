# Comparing `tmp/news-scraper-python-0.0.4.tar.gz` & `tmp/news-scraper-python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-scraper-python-0.0.4.tar", last modified: Wed Jun 14 04:02:24 2023, max compression
+gzip compressed data, was "news-scraper-python-0.0.5.tar", last modified: Wed Jun 14 06:17:32 2023, max compression
```

## Comparing `news-scraper-python-0.0.4.tar` & `news-scraper-python-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 04:02:24.545147 news-scraper-python-0.0.4/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 04:02:24.545041 news-scraper-python-0.0.4/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.4/README.md
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 04:02:24.544348 news-scraper-python-0.0.4/news_scraper_python/
--rw-r--r--   0 aayushrshah   (502) staff       (20)       22 2023-06-13 10:43:01.000000 news-scraper-python-0.0.4/news_scraper_python/__init__.py
--rw-r--r--   0 aayushrshah   (502) staff       (20)     3743 2023-06-14 03:59:13.000000 news-scraper-python-0.0.4/news_scraper_python/app.py
--rw-r--r--   0 aayushrshah   (502) staff       (20)     4425 2023-06-13 09:50:49.000000 news-scraper-python-0.0.4/news_scraper_python/utils.py
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 04:02:24.544885 news-scraper-python-0.0.4/news_scraper_python.egg-info/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 04:02:24.000000 news-scraper-python-0.0.4/news_scraper_python.egg-info/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)      320 2023-06-14 04:02:24.000000 news-scraper-python-0.0.4/news_scraper_python.egg-info/SOURCES.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-14 04:02:24.000000 news-scraper-python-0.0.4/news_scraper_python.egg-info/dependency_links.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-14 04:02:24.000000 news-scraper-python-0.0.4/news_scraper_python.egg-info/requires.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       20 2023-06-14 04:02:24.000000 news-scraper-python-0.0.4/news_scraper_python.egg-info/top_level.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-14 04:02:24.545183 news-scraper-python-0.0.4/setup.cfg
--rw-r--r--   0 aayushrshah   (502) staff       (20)      725 2023-06-14 04:01:48.000000 news-scraper-python-0.0.4/setup.py
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972970 news-scraper-python-0.0.5/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:17:32.972862 news-scraper-python-0.0.5/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.5/README.md
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972200 news-scraper-python-0.0.5/news_scraper_python/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       28 2023-06-14 06:17:12.000000 news-scraper-python-0.0.5/news_scraper_python/__init__.py
+-rw-r--r--   0 aayushrshah   (502) staff       (20)     3749 2023-06-14 06:15:06.000000 news-scraper-python-0.0.5/news_scraper_python/app.py
+-rw-r--r--   0 aayushrshah   (502) staff       (20)     4425 2023-06-14 04:26:19.000000 news-scraper-python-0.0.5/news_scraper_python/utils.py
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-14 06:17:32.972713 news-scraper-python-0.0.5/news_scraper_python.egg-info/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      320 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/SOURCES.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/dependency_links.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/requires.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       20 2023-06-14 06:17:32.000000 news-scraper-python-0.0.5/news_scraper_python.egg-info/top_level.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-14 06:17:32.973015 news-scraper-python-0.0.5/setup.cfg
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      725 2023-06-14 06:16:49.000000 news-scraper-python-0.0.5/setup.py
```

### Comparing `news-scraper-python-0.0.4/news_scraper_python/app.py` & `news-scraper-python-0.0.5/news_scraper_python/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
             #beautiful soup code for scraping google search
             for result in soup.select('.tF2Cxc'):
                 link = result.select_one('.yuRUbf a')['href']
                 data.append(link)
     return data
 
-def start(conn_string,keywords,websites):
+def scrape_news(conn_string,keywords,websites):
     links = get_links(keywords,websites)
     threaded(links,conn_string)
 
 
 '''
 optimization idea => make link fetching and article parsing parallel instead of sequential
 Don't fetch all links, then start parsing articles.
```

### Comparing `news-scraper-python-0.0.4/news_scraper_python/utils.py` & `news-scraper-python-0.0.5/news_scraper_python/utils.py`

 * *Files identical despite different names*

### Comparing `news-scraper-python-0.0.4/setup.py` & `news-scraper-python-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="news-scraper-python",
-    version="0.0.4",
+    version="0.0.5",
     author="Aayush Shah",
     author_email="aayushshah1142@gmail.com",
     description="A package to scrape news by keywords and source websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FarMart-Tech/news-scraper",
     project_urls={"Bug Tracker": "https://github.com/FarMart-Tech/news-scraper"},
```

