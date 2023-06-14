# Comparing `tmp/revChatGPT-6.2.3.tar.gz` & `tmp/revChatGPT-6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.2.3.tar", last modified: Wed Jun 14 14:14:08 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.4.tar", last modified: Wed Jun 14 14:17:24 2023, max compression
```

## Comparing `revChatGPT-6.2.3.tar` & `revChatGPT-6.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 14:14:07.000000 revChatGPT-6.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.091578 revChatGPT-6.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    56888 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:14:08.000000 revChatGPT-6.2.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 14:14:08.000000 revChatGPT-6.2.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:14:08.000000 revChatGPT-6.2.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 14:14:08.000000 revChatGPT-6.2.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 14:14:08.000000 revChatGPT-6.2.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:14:08.095578 revChatGPT-6.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 14:13:40.000000 revChatGPT-6.2.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.345338 revChatGPT-6.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.349338 revChatGPT-6.2.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    57094 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.349338 revChatGPT-6.2.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 14:17:24.000000 revChatGPT-6.2.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:17:24.353338 revChatGPT-6.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 14:16:56.000000 revChatGPT-6.2.4/tests/test_recipient.py
```

### Comparing `revChatGPT-6.2.3/LICENSE` & `revChatGPT-6.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/PKG-INFO` & `revChatGPT-6.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.3
+Version: 6.2.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.2.3/README.md` & `revChatGPT-6.2.4/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/setup.py` & `revChatGPT-6.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.2.3",
+    version="6.2.4",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.2.3/src/revChatGPT/V1.py` & `revChatGPT-6.2.4/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,21 +516,21 @@
                 parent_id = self.conversation_mapping[conversation_id]
             else:
                 print(
                     "Warning: Invalid conversation_id provided, treat as a new conversation",
                 )
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
-
+        model = model or self.config.get("model") or "text-davinci-002-render-sha"
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": model or self.config.get("model") or "text-davinci-002-render-sha",
+            "model": model,
             "history_and_training_disabled": self.disable_history,
         }
         if model.startswith("gpt-4"):
             data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
@@ -652,15 +652,15 @@
                     )
                     self.__map_conversations()
             if conversation_id in self.conversation_mapping:
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
-
+        model = model or self.config.get("model") or "text-davinci-002-render-sha"
         data = {
             "action": "continue",
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
             or self.config.get("model")
             or (
@@ -1066,21 +1066,21 @@
                 parent_id = self.conversation_mapping[conversation_id]
             else:
                 print(
                     "Warning: Invalid conversation_id provided, treat as a new conversation",
                 )
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
-
+        model = model or self.config.get("model") or "text-davinci-002-render-sha"
         data = {
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
-            "model": model or self.config.get("model") or "text-davinci-002-render-sha",
+            "model": model,
             "history_and_training_disabled": self.disable_history,
         }
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
         if model.startswith("gpt-4"):
             data["arkose_token"] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
@@ -1191,15 +1191,15 @@
             if conversation_id not in self.conversation_mapping:
                 await self.__map_conversations()
             if conversation_id in self.conversation_mapping:
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
-
+        model = model or self.config.get("model") or "text-davinci-002-render-sha"
         data = {
             "action": "continue",
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model
             or self.config.get("model")
             or (
```

### Comparing `revChatGPT-6.2.3/src/revChatGPT/V3.py` & `revChatGPT-6.2.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT/__init__.py` & `revChatGPT-6.2.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT/__main__.py` & `revChatGPT-6.2.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT/typings.py` & `revChatGPT-6.2.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT/utils.py` & `revChatGPT-6.2.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.3
+Version: 6.2.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

