# Comparing `tmp/revChatGPT-6.2.0.tar.gz` & `tmp/revChatGPT-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.2.0.tar", last modified: Mon Jun 12 10:29:06 2023, max compression
+gzip compressed data, was "revChatGPT-6.2.1.tar", last modified: Wed Jun 14 10:01:51 2023, max compression
```

## Comparing `revChatGPT-6.2.0.tar` & `revChatGPT-6.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 10:29:06.361603 revChatGPT-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    54299 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 10:29:06.000000 revChatGPT-6.2.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:06.357603 revChatGPT-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-12 10:28:38.000000 revChatGPT-6.2.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.943945 revChatGPT-6.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    54299 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 10:01:51.000000 revChatGPT-6.2.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:01:51.947944 revChatGPT-6.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-14 10:01:20.000000 revChatGPT-6.2.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.2.0/LICENSE` & `revChatGPT-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/PKG-INFO` & `revChatGPT-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.0
+Version: 6.2.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.2.0/README.md` & `revChatGPT-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/setup.py` & `revChatGPT-6.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.2.0",
+    version="6.2.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.2.0/src/revChatGPT/V1.py` & `revChatGPT-6.2.1/src/revChatGPT/V1.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT/V3.py` & `revChatGPT-6.2.1/src/revChatGPT/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine: str = engine
         self.api_key: str = api_key
         self.system_prompt: str = system_prompt
         self.max_tokens: int = max_tokens or (
-            31000 if engine == "gpt-4-32k" else 7000 if engine == "gpt-4" else 4000
+            31000 if "gpt-4-32k" in engine else 7000 if "gpt-4" in engine else 15000 if "gpt-3.5-turbo-16k" in engine else 4000
         )
         self.truncate_limit: int = truncate_limit or (
-            30500 if engine == "gpt-4-32k" else 6500 if engine == "gpt-4" else 3500
+            30500 if "gpt-4-32k" in engine else 6500 if "gpt-4" in engine else 14500 if "gpt-3.5-turbo-16k" in engine else 3500
         )
         self.temperature: float = temperature
         self.top_p: float = top_p
         self.presence_penalty: float = presence_penalty
         self.frequency_penalty: float = frequency_penalty
         self.reply_count: int = reply_count
         self.timeout: float = timeout
@@ -125,14 +125,15 @@
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
         if self.engine not in [
             "gpt-3.5-turbo",
+            "gpt-3.5-turbo-16k",
             "gpt-3.5-turbo-0301",
             "gpt-4",
             "gpt-4-0314",
             "gpt-4-32k",
             "gpt-4-32k-0314",
         ]:
             raise NotImplementedError(f"Unsupported engine {self.engine}")
```

### Comparing `revChatGPT-6.2.0/src/revChatGPT/__init__.py` & `revChatGPT-6.2.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT/__main__.py` & `revChatGPT-6.2.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.2.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT/typings.py` & `revChatGPT-6.2.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT/utils.py` & `revChatGPT-6.2.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.2.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.2.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.2.0
+Version: 6.2.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

