# Comparing `tmp/Echoo-0.0.2.post2106021851-py3-none-any.whl.zip` & `tmp/Echoo-0.0.2.post2306141219-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4411 bytes, number of entries: 9
--rw-r--r--  2.0 unx       24 b- defN 21-Jun-02 10:17 Echoo/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 21-Jun-02 10:50 Echoo/echoo.py
--rwxr-xr-x  2.0 unx       77 b- defN 21-Jun-02 10:51 Echoo-0.0.2_2106021851.data/scripts/echoo
--rw-r--r--  2.0 unx     1067 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/LICENSE
--rw-r--r--  2.0 unx     1363 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      788 b- defN 21-Jun-02 10:51 Echoo-0.0.2.post2106021851.dist-info/RECORD
-9 files, 6560 bytes uncompressed, 3023 bytes compressed:  53.9%
+Zip file size: 4462 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-14 04:12 Echoo/__init__.py
+-rw-r--r--  2.0 unx     3360 b- defN 23-Jun-14 04:19 Echoo/echoo.py
+-rwxr-xr-x  2.0 unx       77 b- defN 23-Jun-14 04:19 Echoo-0.0.2_2306141219.data/scripts/echoo
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      788 b- defN 23-Jun-14 04:19 Echoo-0.0.2.post2306141219.dist-info/RECORD
+9 files, 6800 bytes uncompressed, 3074 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: Echoo/__init__.py
 Comment: 
 
 Filename: Echoo/echoo.py
 Comment: 
 
-Filename: Echoo-0.0.2_2106021851.data/scripts/echoo
+Filename: Echoo-0.0.2_2306141219.data/scripts/echoo
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/LICENSE
+Filename: Echoo-0.0.2.post2306141219.dist-info/LICENSE
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/METADATA
+Filename: Echoo-0.0.2.post2306141219.dist-info/METADATA
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/WHEEL
+Filename: Echoo-0.0.2.post2306141219.dist-info/WHEEL
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/top_level.txt
+Filename: Echoo-0.0.2.post2306141219.dist-info/top_level.txt
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/zip-safe
+Filename: Echoo-0.0.2.post2306141219.dist-info/zip-safe
 Comment: 
 
-Filename: Echoo-0.0.2.post2106021851.dist-info/RECORD
+Filename: Echoo-0.0.2.post2306141219.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Echoo/echoo.py

```diff
@@ -2,15 +2,16 @@
 # logging.basicConfig(format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
 #                     level=logging.INFO)
 
 import os
 import argparse
 import codecs
 import telegram
-from telegram.ext import Updater, CommandHandler, MessageHandler, Filters
+import asyncio
+# from telegram.ext import Updater, CommandHandler, MessageHandler, Filters
 
 def escape_fn(s):
     return s.replace("_", "\\_") \
             .replace("*", "\\*") \
             .replace("[", "\\[") \
             .replace("`", "\\`") \
             .replace("<", "\\<") \
@@ -32,32 +33,39 @@
                 self.chat_id = os.environ["TG_CHAT_ID"]
             except KeyError:
                 raise KeyError("Neither --chat_id nor TG_CHAT_ID is set.")
         self.bot = telegram.Bot(token=self.token)
         # self.parse_mode = "Markdown"
         self.parse_mode = parse_mode
     
-    def send_msg(self, msg, chat_id=None):
+    async def _send_msg(self, msg, chat_id=None):
         if chat_id is None:
             chat_id = self.chat_id
         print(f"===== Echo: {msg} =====")
-        self.bot.send_message(chat_id=chat_id, text=msg, parse_mode=self.parse_mode)    
+        await self.bot.send_message(chat_id=chat_id, text=msg, parse_mode=self.parse_mode)    
+    
+    def send_msg(self, msg, chat_id=None):
+        asyncio.run(
+            self._send_msg(chat_id=chat_id, text=msg, parse_mode=self.parse_mode)
+        )
     
     def __call__(self, function):
         print("Init from __call__")
         def wrapper( *args, **kwds):
             self.send_msg(escape_fn(f'''Start {str(function)}'''))
             res = function(*args, **kwds)
             self.send_msg(escape_fn(f'''Finish {str(function)}'''))
             return res
         return wrapper
 
 def main(token, chat_id, msg="Are u ok", parse_mode="MarkdownV2"):
     bot = telegram.Bot(token=token)
-    bot.send_message(chat_id=chat_id, text=escape_fn(msg), parse_mode=parse_mode)
+    asyncio.run(
+        bot.send_message(chat_id=chat_id, text=escape_fn(msg), parse_mode=parse_mode)
+    )
 
 def run():
     parser = argparse.ArgumentParser(description=r'''Echoo: A tool let's your program echo to Telegram.''')
 
     parser.add_argument("-t", "--token", default=None, type=str, help="Token for your bot.")
     parser.add_argument("-id", "--chat_id", default=None, type=str, help="Chat_id of your audience.")
     parser.add_argument("--parse-mode", default="Markdown", type=str, help='''Send Markdown or HTML, if you want Telegram apps to show bold,
```

## Comparing `Echoo-0.0.2.post2106021851.dist-info/LICENSE` & `Echoo-0.0.2.post2306141219.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Echoo-0.0.2.post2106021851.dist-info/METADATA` & `Echoo-0.0.2.post2306141219.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: Echoo
-Version: 0.0.2-2106021851
+Version: 0.0.2-2306141219
 Summary: Let your program echo to you~
 Home-page: https://github.com/Lyken17/Echoo/
 Author: Ligeng Zhu
 Author-email: lykensyu+github@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: python-telegram-bot
 
 # Echoo
 
 Let your program echo to you~
 
 ## Installation
```

## Comparing `Echoo-0.0.2.post2106021851.dist-info/RECORD` & `Echoo-0.0.2.post2306141219.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Echoo/__init__.py,sha256=brP4byVZwlMnNfX5fJv_BVbUd0aJRVrISti4-NA2nBQ,24
-Echoo/echoo.py,sha256=oKzi7RC3JAO6VjZy1v7tPT7BPS7KqjoOfJCCJC-f-fE,3142
-Echoo-0.0.2_2106021851.data/scripts/echoo,sha256=JGNpFj2uGAye3Z0IvoE_UkJ4xzuDvpO3SG9CIhWcPMw,77
-Echoo-0.0.2.post2106021851.dist-info/LICENSE,sha256=NvV3rSiPG-roGItuwJgI6u0njAi4KEusxpS7Vv-_Pfw,1067
-Echoo-0.0.2.post2106021851.dist-info/METADATA,sha256=OLil7C2TU9-BikzCbui0fyyItFbWhrcDXuu3weChB3o,1363
-Echoo-0.0.2.post2106021851.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-Echoo-0.0.2.post2106021851.dist-info/top_level.txt,sha256=0Nw7QC7eZkxPz2KKJSlO1D5uXG6VjoSpzmxoKP2ZByE,6
-Echoo-0.0.2.post2106021851.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-Echoo-0.0.2.post2106021851.dist-info/RECORD,,
+Echoo/echoo.py,sha256=t-G8wc3X4khRhKRxmU6PH3s9ezKutTU30GespeGvHho,3360
+Echoo-0.0.2_2306141219.data/scripts/echoo,sha256=JGNpFj2uGAye3Z0IvoE_UkJ4xzuDvpO3SG9CIhWcPMw,77
+Echoo-0.0.2.post2306141219.dist-info/LICENSE,sha256=NvV3rSiPG-roGItuwJgI6u0njAi4KEusxpS7Vv-_Pfw,1067
+Echoo-0.0.2.post2306141219.dist-info/METADATA,sha256=eSRtusuBHTt-mBu3wwlHP93I_gFMDPp_sQIabtR7vUg,1385
+Echoo-0.0.2.post2306141219.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Echoo-0.0.2.post2306141219.dist-info/top_level.txt,sha256=0Nw7QC7eZkxPz2KKJSlO1D5uXG6VjoSpzmxoKP2ZByE,6
+Echoo-0.0.2.post2306141219.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+Echoo-0.0.2.post2306141219.dist-info/RECORD,,
```

