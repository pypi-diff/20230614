# Comparing `tmp/revChatGPT-6.2.4.tar.gz` & `tmp/revChatGPT-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.2.4.tar", last modified: Wed Jun 14 14:17:24 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.5.tar", last modified: Wed Jun 14 15:37:44 2023, max compression
```

## Comparing `revChatGPT-6.2.4.tar` & `revChatGPT-6.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.345338 revChatGPT-6.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.349338 revChatGPT-6.2.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    57094 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.349338 revChatGPT-6.2.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 15:37:44.820719 revChatGPT-6.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 15:37:44.820719 revChatGPT-6.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.812719 revChatGPT-6.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 15:37:44.000000 revChatGPT-6.2.5/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:37:44.816719 revChatGPT-6.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-14 15:37:08.000000 revChatGPT-6.2.5/tests/test_recipient.py
```

### Comparing `revChatGPT-6.2.4/LICENSE` & `revChatGPT-6.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.4/PKG-INFO` & `revChatGPT-6.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.4
+Version: 6.2.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.2.4/README.md` & `revChatGPT-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.4/setup.py` & `revChatGPT-6.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.2.4",
+    version="6.2.5",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.2.4/src/revChatGPT/V1.py` & `revChatGPT-6.2.5/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,59 +4,62 @@
 from __future__ import annotations
 
 import base64
 import binascii
 import contextlib
 import json
 import logging
+import secrets
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
-import secrets
 
 import httpx
 import requests
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
-def generate_random_hex(length: int=17)-> str:
+
+def generate_random_hex(length: int = 17) -> str:
     """Generate a random hex string
 
     Args:
         length (int, optional): Length of the hex string. Defaults to 17.
 
     Returns:
         str: Random hex string
     """
     return secrets.token_hex(length)
 
-def random_int(min:int,max:int) -> int:
+
+def random_int(min: int, max: int) -> int:
     """Generate a random integer
 
     Args:
         min (int): Minimum value
         max (int): Maximum value
 
     Returns:
         int: Random integer
     """
     return secrets.randbelow(max - min) + min
 
+
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(message)s",
     )
 
 log = logging.getLogger(__name__)
 
@@ -526,15 +529,17 @@
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model,
             "history_and_training_disabled": self.disable_history,
         }
         if model.startswith("gpt-4"):
-            data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
+            data[
+                "arkose_token"
+            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
 
         yield from self.__send_request(
             data,
             timeout=timeout,
@@ -665,18 +670,19 @@
             or self.config.get("model")
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
             "history_and_training_disabled": self.disable_history,
-
         }
         if model.startswith("gpt-4"):
-            data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
+            data[
+                "arkose_token"
+            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
 
         yield from self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         )
 
@@ -1079,15 +1085,17 @@
             "model": model,
             "history_and_training_disabled": self.disable_history,
         }
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
         if model.startswith("gpt-4"):
-            data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
+            data[
+                "arkose_token"
+            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         async for msg in self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         ):
             yield msg
 
@@ -1206,15 +1214,17 @@
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
             "history_and_training_disabled": self.disable_history,
         }
         if model.startswith("gpt-4"):
-            data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
+            data[
+                "arkose_token"
+            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
 
         async for msg in self.__send_request(
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
             yield msg
```

### Comparing `revChatGPT-6.2.4/src/revChatGPT/V3.py` & `revChatGPT-6.2.5/src/revChatGPT/V3.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,25 @@
 from . import typings as t
 from .utils import create_completer
 from .utils import create_keybindings
 from .utils import create_session
 from .utils import get_filtered_keys_from_object
 from .utils import get_input
 
+ENGINES = [
+    "gpt-3.5-turbo",
+    "gpt-3.5-turbo-16k",
+    "gpt-3.5-turbo-0301",
+    "gpt-3.5-turbo-0613" "gpt-4",
+    "gpt-4-0314",
+    "gpt-4-32k",
+    "gpt-4-32k-0314",
+    "gpt-4-0613",
+]
+
 
 class Chatbot:
     """
     Official ChatGPT API
     """
 
     def __init__(
@@ -46,18 +57,30 @@
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine: str = engine
         self.api_key: str = api_key
         self.system_prompt: str = system_prompt
         self.max_tokens: int = max_tokens or (
-            31000 if "gpt-4-32k" in engine else 7000 if "gpt-4" in engine else 15000 if "gpt-3.5-turbo-16k" in engine else 4000
+            31000
+            if "gpt-4-32k" in engine
+            else 7000
+            if "gpt-4" in engine
+            else 15000
+            if "gpt-3.5-turbo-16k" in engine
+            else 4000
         )
         self.truncate_limit: int = truncate_limit or (
-            30500 if "gpt-4-32k" in engine else 6500 if "gpt-4" in engine else 14500 if "gpt-3.5-turbo-16k" in engine else 3500
+            30500
+            if "gpt-4-32k" in engine
+            else 6500
+            if "gpt-4" in engine
+            else 14500
+            if "gpt-3.5-turbo-16k" in engine
+            else 3500
         )
         self.temperature: float = temperature
         self.top_p: float = top_p
         self.presence_penalty: float = presence_penalty
         self.frequency_penalty: float = frequency_penalty
         self.reply_count: int = reply_count
         self.timeout: float = timeout
@@ -123,23 +146,15 @@
                 break
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        if self.engine not in [
-            "gpt-3.5-turbo",
-            "gpt-3.5-turbo-16k",
-            "gpt-3.5-turbo-0301",
-            "gpt-4",
-            "gpt-4-0314",
-            "gpt-4-32k",
-            "gpt-4-32k-0314",
-        ]:
+        if self.engine not in ENGINES:
             raise NotImplementedError(f"Unsupported engine {self.engine}")
 
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
@@ -583,15 +598,15 @@
         default=None,
         help="Custom submit key for chatbot. For more information on keys, see README",
     )
     parser.add_argument(
         "--model",
         type=str,
         default="gpt-3.5-turbo",
-        choices=["gpt-3.5-turbo", "gpt-4", "gpt-4-32k"],
+        choices=ENGINES,
     )
 
     parser.add_argument(
         "--truncate_limit",
         type=int,
         default=None,
     )
```

### Comparing `revChatGPT-6.2.4/src/revChatGPT/__init__.py` & `revChatGPT-6.2.5/src/revChatGPT/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The __init__ file does not a main file
 
 You can import the following module to use:
 revChatGPT.V1
 revChatGPT.V3
 """
-__version__ = "5.0.0"
+__version__ = "6.2"
 __all__ = ()
 
 
 def verify() -> None:
     # Available Python Version Verify
     from . import typings as t
```

### Comparing `revChatGPT-6.2.4/src/revChatGPT/__main__.py` & `revChatGPT-6.2.5/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.5/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.4/src/revChatGPT/typings.py` & `revChatGPT-6.2.5/src/revChatGPT/typings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module that contains all the types used in this project
 """
 import os
+import platform
 from enum import Enum
 from typing import Union
-import platform
 
 
 python_version = [each for each in platform.python_version_tuple()]
 SUPPORT_ADD_NOTES = int(python_version[0]) >= 3 and int(python_version[1]) >= 11
 
 
 class ChatbotError(Exception):
```

### Comparing `revChatGPT-6.2.4/src/revChatGPT/utils.py` & `revChatGPT-6.2.5/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.5/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.4
+Version: 6.2.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

