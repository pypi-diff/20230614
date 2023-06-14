# Comparing `tmp/revChatGPT-6.2.1.tar.gz` & `tmp/revChatGPT-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.2.1.tar", last modified: Wed Jun 14 10:01:51 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.2.tar", last modified: Wed Jun 14 10:33:29 2023, max compression
```

## Comparing `revChatGPT-6.2.1.tar` & `revChatGPT-6.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.943945 revChatGPT-6.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    54299 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 10:33:28.000000 revChatGPT-6.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.199158 revChatGPT-6.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    55337 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:33:29.000000 revChatGPT-6.2.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 10:33:29.000000 revChatGPT-6.2.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:33:29.000000 revChatGPT-6.2.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 10:33:29.000000 revChatGPT-6.2.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 10:33:29.000000 revChatGPT-6.2.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:33:29.203158 revChatGPT-6.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 10:32:59.000000 revChatGPT-6.2.2/tests/test_recipient.py
```

### Comparing `revChatGPT-6.2.1/LICENSE` & `revChatGPT-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/PKG-INFO` & `revChatGPT-6.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.1
+Version: 6.2.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.2.1/README.md` & `revChatGPT-6.2.2/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/setup.py` & `revChatGPT-6.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.2.1",
+    version="6.2.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.2.1/src/revChatGPT/V1.py` & `revChatGPT-6.2.2/src/revChatGPT/V1.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,50 @@
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
+import secrets
 
 import httpx
 import requests
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
 from .utils import get_input
 
+def generate_random_hex(length: int=17)-> str:
+    """Generate a random hex string
+
+    Args:
+        length (int, optional): Length of the hex string. Defaults to 17.
+
+    Returns:
+        str: Random hex string
+    """
+    return secrets.token_hex(length)
+
+def random_int(min:int,max:int) -> int:
+    """Generate a random integer
+
+    Args:
+        min (int): Minimum value
+        max (int): Maximum value
+
+    Returns:
+        int: Random integer
+    """
+    return secrets.randbelow(max - min) + min
+
 if __name__ == "__main__":
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(message)s",
     )
 
 log = logging.getLogger(__name__)
 
@@ -501,14 +525,16 @@
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model or self.config.get("model") or "text-davinci-002-render-sha",
             "history_and_training_disabled": self.disable_history,
         }
+        if model.startswith("gpt-4"):
+            data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
 
         yield from self.__send_request(
             data,
             timeout=timeout,
```

### Comparing `revChatGPT-6.2.1/src/revChatGPT/V3.py` & `revChatGPT-6.2.2/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT/__init__.py` & `revChatGPT-6.2.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT/__main__.py` & `revChatGPT-6.2.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT/typings.py` & `revChatGPT-6.2.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT/utils.py` & `revChatGPT-6.2.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.1
+Version: 6.2.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

