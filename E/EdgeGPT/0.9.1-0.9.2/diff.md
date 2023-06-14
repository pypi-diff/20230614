# Comparing `tmp/EdgeGPT-0.9.1.tar.gz` & `tmp/EdgeGPT-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.9.1.tar", last modified: Mon Jun  5 14:25:11 2023, max compression
+gzip compressed data, was "EdgeGPT-0.9.2.tar", last modified: Tue Jun  6 02:54:19 2023, max compression
```

## Comparing `EdgeGPT-0.9.1.tar` & `EdgeGPT-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-05 14:25:11.000000 EdgeGPT-0.9.1/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/ImageGen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:25:11.448655 EdgeGPT-0.9.1/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-05 14:24:43.000000 EdgeGPT-0.9.1/src/helpers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 02:54:19.000000 EdgeGPT-0.9.2/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:19.771070 EdgeGPT-0.9.2/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-06 02:53:51.000000 EdgeGPT-0.9.2/src/helpers/utilities.py
```

### Comparing `EdgeGPT-0.9.1/LICENSE` & `EdgeGPT-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.1/PKG-INFO` & `EdgeGPT-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.9.1
+Version: 0.9.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -78,24 +78,24 @@
 
 It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
 `Exception: Authentication failed. You have not been accepted into the beta.`
 
 <details>
 
 <summary>
-  
+
 ### Collecting cookies
 
 </summary>
 
 1. Get a browser that looks like Microsoft Edge.
-  
+
  * a) (Easy) Install the latest version of Microsoft Edge
  * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-  
+
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
 8. Paste your cookies into a file `cookies.json`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.9.1/README.md` & `EdgeGPT-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,24 +59,24 @@
 
 It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
 `Exception: Authentication failed. You have not been accepted into the beta.`
 
 <details>
 
 <summary>
-  
+
 ### Collecting cookies
 
 </summary>
 
 1. Get a browser that looks like Microsoft Edge.
-  
+
  * a) (Easy) Install the latest version of Microsoft Edge
  * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-  
+
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
 8. Paste your cookies into a file `cookies.json`
```

### Comparing `EdgeGPT-0.9.1/setup.py` & `EdgeGPT-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,23 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.9.1",
+    version="0.9.2",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
     project_urls={"Bug Report": "https://github.com/acheong08/EdgeGPT/issues/new"},
-    entry_points={
-        "console_scripts": [
-            "edge-gpt = EdgeGPT:main",
-            "edge-gpt-image = ImageGen:main",
-        ],
-    },
     install_requires=[
         "httpx[socks]>=0.24.0",
         "aiohttp",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
```

### Comparing `EdgeGPT-0.9.1/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.9.2/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.9.1
+Version: 0.9.2
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -78,24 +78,24 @@
 
 It was also found that it might depend on your IP address. For example, if you try to access the chat features from an IP that is known to belong to a datacenter range (vServers, root servers, VPN, common proxies, ...), you might be required to log in while being able to access the features just fine from your home IP address. If you receive the following error, you can try providing a cookie and see if it works then:
 `Exception: Authentication failed. You have not been accepted into the beta.`
 
 <details>
 
 <summary>
-  
+
 ### Collecting cookies
 
 </summary>
 
 1. Get a browser that looks like Microsoft Edge.
-  
+
  * a) (Easy) Install the latest version of Microsoft Edge
  * b) (Advanced) Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-  
+
 2. Open [bing.com/chat](https://bing.com/chat)
 3. If you see a chat feature, you are good to continue...
 4. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 5. Go to [bing.com](https://bing.com)
 6. Open the extension
 7. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
 8. Paste your cookies into a file `cookies.json`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.1 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.9.2 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.9.1/src/EdgeGPT.py` & `EdgeGPT-0.9.2/src/EdgeGPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 """
 Main.py
 """
 from __future__ import annotations
 
-import argparse
-import asyncio
 import json
 
-import re
-import sys
-from pathlib import Path
-from typing import Generator, Union
-
-from prompt_toolkit import PromptSession
-from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
-from prompt_toolkit.completion import WordCompleter
-from prompt_toolkit.history import InMemoryHistory
-from prompt_toolkit.key_binding import KeyBindings
-from rich.live import Live
-from rich.markdown import Markdown
+from typing import Generator
 
-from src.helpers.chathub.chathub import ChatHub
-from src.helpers.chathub.request import ChatHubRequest
-from src.helpers.conversation import Conversation
-from src.helpers.utilities import guess_locale, get_ran_hex
-from src.helpers.conversation_style import CONVERSATION_STYLE_TYPE
+try:
+    from helpers.chathub.chathub import ChatHub
+    from helpers.chathub.request import ChatHubRequest
+    from helpers.conversation import Conversation
+    from helpers.conversation_style import CONVERSATION_STYLE_TYPE
+    from helpers.utilities import guess_locale
+except ImportError:
+    from src.helpers.chathub.chathub import ChatHub
+    from src.helpers.chathub.request import ChatHubRequest
+    from src.helpers.conversation import Conversation
+    from src.helpers.conversation_style import CONVERSATION_STYLE_TYPE
+    from src.helpers.utilities import guess_locale
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
@@ -69,22 +63,22 @@
             invocation_id = self.chat_hub.request.invocation_id
             f.write(
                 {
                     "conversation_id": conversation_id,
                     "conversation_signature": conversation_signature,
                     "client_id": client_id,
                     "invocation_id": invocation_id,
-                }
+                },
             )
 
     async def load_conversation(self, filename: str) -> None:
         """
         Load the conversation from a file
         """
-        with open(filename, "r") as f:
+        with open(filename) as f:
             conversation = json.load(f)
             self.chat_hub.request = ChatHubRequest(
                 conversation_signature=conversation["conversation_signature"],
                 client_id=conversation["client_id"],
                 conversation_id=conversation["conversation_id"],
                 invocation_id=conversation["invocation_id"],
             )
@@ -125,15 +119,15 @@
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         webpage_context: str | None = None,
         search_result: bool = False,
         locale: str = guess_locale(),
-    ) -> Generator[bool, Union[dict, str], None]:
+    ) -> Generator[bool, dict | str, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
@@ -158,29 +152,29 @@
         self.chat_hub = ChatHub(
             await Conversation.create(self.proxy, cookies=self.chat_hub.cookies),
             proxy=self.proxy,
             cookies=self.chat_hub.cookies,
         )
 
 
-async def _get_input_async(
-    session: PromptSession = None,
-    completer: WordCompleter = None,
-) -> str:
-    """
-    Multiline input function.
-    """
-    return await session.prompt_async(
-        completer=completer,
-        multiline=True,
-        auto_suggest=AutoSuggestFromHistory(),
-    )
+import argparse, asyncio, json
+from rich.live import Live
+from rich.markdown import Markdown
+from pathlib import Path
+import re
+import sys
+from prompt_toolkit import PromptSession
+from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
+from prompt_toolkit.completion import WordCompleter
+from prompt_toolkit.history import InMemoryHistory
+from prompt_toolkit.key_binding import KeyBindings
+from EdgeGPT import Chatbot
 
 
-def _create_session() -> PromptSession:
+def create_session() -> PromptSession:
     kb = KeyBindings()
 
     @kb.add("enter")
     def _(event) -> None:
         buffer_text = event.current_buffer.text
         if buffer_text.startswith("!"):
             event.current_buffer.validate_and_handle()
@@ -192,41 +186,55 @@
         if event.current_buffer.complete_state:
             # event.current_buffer.cancel_completion()
             event.current_buffer.text = ""
 
     return PromptSession(key_bindings=kb, history=InMemoryHistory())
 
 
-def _create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
+def create_completer(commands: list, pattern_str: str = "$") -> WordCompleter:
     return WordCompleter(words=commands, pattern=re.compile(pattern_str))
 
 
 def _create_history_logger(f):
     def logger(*args, **kwargs) -> None:
         tmp = sys.stdout
         sys.stdout = f
         print(*args, **kwargs, flush=True)
         sys.stdout = tmp
 
     return logger
 
 
+async def get_input_async(
+    session: PromptSession = None,
+    completer: WordCompleter = None,
+) -> str:
+    """
+    Multiline input function.
+    """
+    return await session.prompt_async(
+        completer=completer,
+        multiline=True,
+        auto_suggest=AutoSuggestFromHistory(),
+    )
+
+
 async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
     # Read and parse cookies
     cookies = None
     if args.cookie_file:
         cookies = json.loads(Path.open(args.cookie_file, encoding="utf-8").read())
     bot = await Chatbot.create(proxy=args.proxy, cookies=cookies)
-    session = _create_session()
-    completer = _create_completer(["!help", "!exit", "!reset"])
+    session = create_session()
+    completer = create_completer(["!help", "!exit", "!reset"])
     initial_prompt = args.prompt
 
     # Log chat history
     def p_hist(*args, **kwargs) -> None:
         pass
 
     if args.history_file:
@@ -240,15 +248,15 @@
             question = initial_prompt
             print(question)
             initial_prompt = None
         else:
             question = (
                 input()
                 if args.enter_once
-                else await _get_input_async(session=session, completer=completer)
+                else await get_input_async(session=session, completer=completer)
             )
         print()
         p_hist(question + "\n")
         if question == "!exit":
             break
         if question == "!help":
             print(
```

### Comparing `EdgeGPT-0.9.1/src/EdgeUtils.py` & `EdgeGPT-0.9.2/src/EdgeUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import json
 import re
 import time
 from pathlib import Path
 
-from EdgeGPT import Chatbot, ConversationStyle
+from EdgeGPT import Chatbot
+from EdgeGPT import ConversationStyle
 from ImageGen import ImageGen
 
+
 class Cookie:
     """
     Convenience class for Bing Cookie files, data, and configuration. This Class
     is updated dynamically by the Query class to allow cycling through >1
     cookie/credentials file e.g. when daily request limits (current 200 per
     account per day) are exceeded.
     """
```

### Comparing `EdgeGPT-0.9.1/src/helpers/constants.py` & `EdgeGPT-0.9.2/src/helpers/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import base64
 import random
-import secrets, base64
+import secrets
 
 sec_websocket_key = secrets.token_urlsafe(16)
 sec_websocket_key = base64.b64encode(sec_websocket_key.encode()).decode()
 
 DELIMITER = "\x1e"
```

### Comparing `EdgeGPT-0.9.1/src/helpers/conversation.py` & `EdgeGPT-0.9.2/src/helpers/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import os, httpx, json
+import json
+import os
+
+import httpx
+
 from .constants import HEADERS_INIT_CONVER
 from .exceptions import NotAllowedToAccess
 
 
 class Conversation:
     def __init__(
         self,
```

### Comparing `EdgeGPT-0.9.1/src/helpers/conversation_style.py` & `EdgeGPT-0.9.2/src/helpers/conversation_style.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.1/src/helpers/locale.py` & `EdgeGPT-0.9.2/src/helpers/locale.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.9.1/src/helpers/utilities.py` & `EdgeGPT-0.9.2/src/helpers/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import json, random, locale
+import json
+import locale
+import random
+
 from .constants import DELIMITER
 from .locale import LocationHint
 
 
 def append_identifier(msg: dict) -> str:
     # Convert dict to json string
     return json.dumps(msg, ensure_ascii=False) + DELIMITER
```

