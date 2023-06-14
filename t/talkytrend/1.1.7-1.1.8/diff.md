# Comparing `tmp/talkytrend-1.1.7.tar.gz` & `tmp/talkytrend-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.7.tar", max compression
+gzip compressed data, was "talkytrend-1.1.8.tar", max compression
```

## Comparing `talkytrend-1.1.7.tar` & `talkytrend-1.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-13 21:19:18.145304 talkytrend-1.1.7/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-13 21:19:18.145304 talkytrend-1.1.7/README.md
--rw-r--r--   0        0        0     1702 2023-06-13 21:19:34.249194 talkytrend-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-13 21:19:34.249194 talkytrend-1.1.7/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/config.py
--rw-r--r--   0        0        0      779 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     4570 2023-06-13 21:19:18.149304 talkytrend-1.1.7/talkytrend/main.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 talkytrend-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 09:27:52.576081 talkytrend-1.1.8/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-14 09:27:52.576081 talkytrend-1.1.8/README.md
+-rw-r--r--   0        0        0     1702 2023-06-14 09:28:15.136003 talkytrend-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-14 09:28:15.136003 talkytrend-1.1.8/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-14 09:27:52.576081 talkytrend-1.1.8/talkytrend/config.py
+-rw-r--r--   0        0        0      779 2023-06-14 09:27:52.576081 talkytrend-1.1.8/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     5304 2023-06-14 09:27:52.576081 talkytrend-1.1.8/talkytrend/main.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 talkytrend-1.1.8/PKG-INFO
```

### Comparing `talkytrend-1.1.7/LICENSE` & `talkytrend-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.7/README.md` & `talkytrend-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.7/pyproject.toml` & `talkytrend-1.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.7"
+version = "1.1.8"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.1.7/talkytrend/config.py` & `talkytrend-1.1.8/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.7/talkytrend/default_settings.toml` & `talkytrend-1.1.8/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.7/talkytrend/main.py` & `talkytrend-1.1.8/talkytrend/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,14 @@
                     messages.append(message)
                 elif not self.asset_signals.get(asset["id"]):
                     self.asset_signals[asset["id"]] = {asset["interval"]: current_signal}
                 else:
                     self.asset_signals[asset["id"]][asset["interval"]] = current_signal
             return messages
 
-
     def get_asset_signals(self):
         return self.asset_signals
 
     async def fetch_key_events(self):
         async with aiohttp.ClientSession() as session:
             async with session.get(self.economic_calendar, timeout=10) as response:
                 if response.status == 200:
@@ -91,30 +90,45 @@
                     news_item = {
                         'title': article['title'],
                         'url': article['url']
                     }
                     key_news.append(news_item)
                 return key_news
 
+#    async def scanner(self):
+#        while True:
+#            try:
+#                tasks = [self.fetch_key_events(), self.fetch_key_news()]
+#                results = await asyncio.gather(*tasks)
+
+#                if results[0] is not None:
+#                    print("Key event:", results[0])
+#                    return results[0]
+                
+#                if results[1] is not None:
+#                    if results[1]:
+#                        print("Key news:", results[1][0])
+#                        return results[1]
 
-
+#            except Exception as e:
+#                print(f"Error in scanner loop: {e}")
+            
+#            await asyncio.sleep(settings.scanner_frequency)
     async def scanner(self):
         while True:
             try:
                 tasks = [self.fetch_key_events(), self.fetch_key_news()]
                 results = await asyncio.gather(*tasks)
 
                 if results[0] is not None:
                     print("Key event:", results[0])
-                    return results[0]
-                
+                    yield results[0]  # Use 'yield' to return the result as an asynchronous iterator
+
                 if results[1] is not None:
                     if results[1]:
                         print("Key news:", results[1][0])
-                        return results[1]
+                        yield results[1]  # Use 'yield' to return the result as an asynchronous iterator
 
             except Exception as e:
                 print(f"Error in scanner loop: {e}")
-            
-            await asyncio.sleep(settings.scanner_frequency)
```

### Comparing `talkytrend-1.1.7/PKG-INFO` & `talkytrend-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.7
+Version: 1.1.8
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

