# Comparing `tmp/cs-telegram-bot-api-0.0.7.tar.gz` & `tmp/cs-telegram-bot-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.7.tar", last modified: Mon Jun 12 17:50:20 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.8.tar", last modified: Wed Jun 14 06:16:57 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.7.tar` & `cs-telegram-bot-api-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:50:20.686257 cs-telegram-bot-api-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 17:50:20.686257 cs-telegram-bot-api-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-12 17:50:00.000000 cs-telegram-bot-api-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:50:20.682257 cs-telegram-bot-api-0.0.7/cs_telegram_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 17:50:00.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-12 17:50:00.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:50:20.686257 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 17:50:20.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-12 17:50:20.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:50:20.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 17:50:20.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 17:50:20.000000 cs-telegram-bot-api-0.0.7/cs_telegram_bot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:50:20.686257 cs-telegram-bot-api-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-12 17:50:00.000000 cs-telegram-bot-api-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/cs_telegram_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot/get_chat_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 06:16:57.000000 cs-telegram-bot-api-0.0.8/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 06:16:57.647955 cs-telegram-bot-api-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-14 06:16:40.000000 cs-telegram-bot-api-0.0.8/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.7/README.md` & `cs-telegram-bot-api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.7/cs_telegram_bot/api.py` & `cs-telegram-bot-api-0.0.8/cs_telegram_bot/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 A Python module for interacting with the Telegram Bot API.
 """
 import requests
 import os
 import logging
 from secrets_loader import load_secret
-
+import psycopg2
+from urllib.parse import urlparse
 
 class TelegramClient:
     """
     A client for the Telegram Bot API.
     """
 
     def __init__(self, bot_token=None):
         """
         Create a new TelegramClient.
         """
         self.bot_token = bot_token or load_secret("TELEGRAM_TOKEN")
         self.offset = 0
+        self.chat_ids = self._get_chat_ids(load_secret("CONFIG_DB_URL"))
 
     def get_new_messages(self):
         """
         Get new messages from the API.
         """
         try:
             response = requests.get(
@@ -53,21 +55,54 @@
         Send a message to a chat.
         """
         try:
             response = requests.post(
                 "https://api.telegram.org/bot{}/sendMessage".format(
                     self.bot_token),
                 json={
-                    "chat_id": chat_id,
+                    "chat_id": self.chat_ids[chat_id],
                     "text": message
                 }
             )
             response.raise_for_status()
         except requests.exceptions.RequestException as e:
             raise SystemExit(e)
 
         # If the API call was successful, the response will contain
         # the sent message in the "result" field
         result = response.json()["result"]
         logging.info(message.encode())
         return result
 
+    @staticmethod
+    def _get_chat_ids(db_url):
+        # Parse the database URL
+        result = urlparse(db_url)
+        username = result.username
+        password = result.password
+        database = result.path[1:]
+        hostname = result.hostname
+        port = result.port
+
+        # Connect to the database
+        conn = psycopg2.connect(
+            dbname=database,
+            user=username,
+            password=password,
+            host=hostname,
+            port=port
+        )
+
+        # Execute the SQL query
+        cursor = conn.cursor()
+        cursor.execute("SELECT * FROM telegram_chat_ids")
+        
+        # Fetch all results
+        results = cursor.fetchall()
+
+        # Close the connection
+        conn.close()
+
+        # Unpack chat IDs from results (which are tuples)
+        chat_ids = {chat[0]:chat[1] for chat in results}
+        
+        return chat_ids
```

### Comparing `cs-telegram-bot-api-0.0.7/setup.py` & `cs-telegram-bot-api-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Telegram Bot API Wrapper'
 LONG_DESCRIPTION = 'A Python module for interacting with the Telegram Bot API.'
 
 # Setting up
 setup(
     name="cs-telegram-bot-api",
     version=VERSION,
     author="Richard",
     author_email="<rich_swainson@hotmail.co.uk>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['requests'],
+    install_requires=['requests', 'psycopg2'],
     keywords=['telegram', 'bot', 'api', 'wrapper'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ]
```

