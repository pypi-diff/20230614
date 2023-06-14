# Comparing `tmp/talkytrend-1.1.6.tar.gz` & `tmp/talkytrend-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.6.tar", max compression
+gzip compressed data, was "talkytrend-1.1.7.tar", max compression
```

## Comparing `talkytrend-1.1.6.tar` & `talkytrend-1.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-12 17:05:52.140946 talkytrend-1.1.6/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-12 17:05:52.140946 talkytrend-1.1.6/README.md
--rw-r--r--   0        0        0     1702 2023-06-12 17:06:11.493248 talkytrend-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-12 17:06:11.493248 talkytrend-1.1.6/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-12 17:05:52.140946 talkytrend-1.1.6/talkytrend/config.py
--rw-r--r--   0        0        0      779 2023-06-12 17:05:52.140946 talkytrend-1.1.6/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     4423 2023-06-12 17:05:52.140946 talkytrend-1.1.6/talkytrend/main.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 talkytrend-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-13 21:19:18.145304 talkytrend-1.1.7/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-13 21:19:18.145304 talkytrend-1.1.7/README.md
+-rw-r--r--   0        0        0     1702 2023-06-13 21:19:34.249194 talkytrend-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-13 21:19:34.249194 talkytrend-1.1.7/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/config.py
+-rw-r--r--   0        0        0      779 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     4570 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/main.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 talkytrend-1.1.7/PKG-INFO
```

### Comparing `talkytrend-1.1.6/LICENSE` & `talkytrend-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.6/README.md` & `talkytrend-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.6/pyproject.toml` & `talkytrend-1.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.6"
+version = "1.1.7"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.1.6/talkytrend/config.py` & `talkytrend-1.1.7/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.6/talkytrend/default_settings.toml` & `talkytrend-1.1.7/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.6/talkytrend/main.py` & `talkytrend-1.1.7/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,24 @@
                     for event in event_list:
                         impact = event.get('impact')
                         country = event.get('country')
                         title = event.get('title')
                         event_date = event.get('date')
                         if event_date and event_date.startswith(today):
                             if impact == 'High' and country in {'USD', 'ALL'}:
-                                return event
+                                return f"💬 {title}\n⏰ {event_date}T{event.get('time')}"
                             if "OPEC" in title or "FOMC" in title:
-                                return event
-
+                                return f"💬 {title}\n⏰ {event_date}T{event.get('time')}"
+    
     async def fetch_key_news(self):
         async with aiohttp.ClientSession() as session:
             async with session.get(self.news_url, timeout=10) as response:
                 data = await response.json()
-                articles = data['articles']
+                if not (articles := data.get('articles')):
+                    return None
                 key_news = []
                 for article in articles:
                     news_item = {
                         'title': article['title'],
                         'url': article['url']
                     }
                     key_news.append(news_item)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `talkytrend-1.1.6/PKG-INFO` & `talkytrend-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.6
+Version: 1.1.7
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

