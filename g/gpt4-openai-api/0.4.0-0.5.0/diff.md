# Comparing `tmp/gpt4-openai-api-0.4.0.tar.gz` & `tmp/gpt4-openai-api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.4.0.tar", last modified: Fri Jun  2 17:58:02 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.5.0.tar", last modified: Sat Jun  3 12:04:11 2023, max compression
```

## Comparing `gpt4-openai-api-0.4.0.tar` & `gpt4-openai-api-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.082621 gpt4-openai-api-0.4.0/
--rw-rw-rw-   0        0        0     5005 2023-06-02 17:58:02.080621 gpt4-openai-api-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.022624 gpt4-openai-api-0.4.0/gpt4_openai/
--rw-rw-rw-   0        0        0     1366 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/gpt4_openai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.059627 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0     5005 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 17:58:01.000000 gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 17:58:02.082621 gpt4-openai-api-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-02 17:57:20.000000 gpt4-openai-api-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:58:02.077626 gpt4-openai-api-0.4.0/test/
--rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.4.0/test/test.py
--rw-rw-rw-   0        0        0      637 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_browsing.py
--rw-rw-rw-   0        0        0      987 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_langchain.py
--rw-rw-rw-   0        0        0      931 2023-06-02 17:56:38.000000 gpt4-openai-api-0.4.0/test/test_plugins.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:04:11.115461 gpt4-openai-api-0.5.0/
+-rw-rw-rw-   0        0        0     5279 2023-06-03 12:04:11.114465 gpt4-openai-api-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 12:04:11.038461 gpt4-openai-api-0.5.0/gpt4_openai/
+-rw-rw-rw-   0        0        0     1548 2023-06-03 11:59:10.000000 gpt4-openai-api-0.5.0/gpt4_openai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:04:11.079496 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0     5279 2023-06-03 12:04:10.000000 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-03 12:04:10.000000 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:04:10.000000 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-03 12:04:10.000000 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 12:04:10.000000 gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:04:11.115461 gpt4-openai-api-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-03 12:02:42.000000 gpt4-openai-api-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:04:11.112487 gpt4-openai-api-0.5.0/test/
+-rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.5.0/test/test.py
+-rw-rw-rw-   0        0        0      637 2023-06-02 17:56:38.000000 gpt4-openai-api-0.5.0/test/test_browsing.py
+-rw-rw-rw-   0        0        0      985 2023-06-03 12:02:44.000000 gpt4-openai-api-0.5.0/test/test_continue_generating.py
+-rw-rw-rw-   0        0        0      987 2023-06-02 17:56:38.000000 gpt4-openai-api-0.5.0/test/test_langchain.py
+-rw-rw-rw-   0        0        0      931 2023-06-02 17:56:38.000000 gpt4-openai-api-0.5.0/test/test_plugins.py
```

### Comparing `gpt4-openai-api-0.4.0/PKG-INFO` & `gpt4-openai-api-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # GPT4 OpenAI unofficial API
 
-## Unofficial GPT-4 API access via chat.openai.com using Selenium
+## Unofficial GPT-4 API access via chat.openai.com
 
 Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. If the account has `ChatGPT Plus`, you can use **GPT-4**.
 
 It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
 
 **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
 
@@ -98,14 +98,23 @@
 ```
 
 Output will be:
 ```
 AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
 ```
 
+## `Continue generating` support
+
+In case of a large prompt answer, ChatGPT allows you to click `Continue generating` button. This library supports that as well.
+
+```python
+llm = GPT4OpenAI(llm=my_token, model='gpt-4', auto_continue=True)
+very_long_response = llm(my_prompt)
+```
+
 ## How to get the access token
 
 1. Go to https://chat.openai.com/api/auth/session
 2. In the JSON, copy the whole `accessToken` field.
 
 ![image](https://github.com/Erol444/gpt4-openai-api/assets/18037362/c0bdfd9c-8ad1-48ca-8344-621a4513e04b)
```

### Comparing `gpt4-openai-api-0.4.0/gpt4_openai/__init__.py` & `gpt4-openai-api-0.5.0/gpt4_openai/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,34 @@
     chatbot : Optional[Chatbot] = None
     call : int = 0
     conversation : Optional[str] = ""
     headless : bool = True
     __file__ = __file__
     model: str = "gpt-4"
     plugin_ids: List[str] = []
+    auto_continue: bool = False
 
     @property
     def _llm_type(self) -> str:
         return "custom"
 
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
         if self.chatbot is None:
             if self.token is None:
                 raise ValueError("You need to specify the token, please check https://github.com/Erol444/gpt4-openai-api#how-to-get-the-access-token")
 
-            self.chatbot = Chatbot({'access_token': self.token, 'model': self.model, 'plugin_ids': self.plugin_ids})
+            self.chatbot = Chatbot({
+                'access_token': self.token,
+                'model': self.model,
+                'plugin_ids': self.plugin_ids
+                })
 
         response = ""
-        for data in self.chatbot.ask(prompt):
+        for data in self.chatbot.ask(prompt=prompt,
+                                     auto_continue=self.auto_continue):
             response = data["message"]
 
         # Add to history
         self.history_data.append({"prompt":prompt,"response":response})
 
         return response
```

### Comparing `gpt4-openai-api-0.4.0/gpt4_openai_api.egg-info/PKG-INFO` & `gpt4-openai-api-0.5.0/gpt4_openai_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # GPT4 OpenAI unofficial API
 
-## Unofficial GPT-4 API access via chat.openai.com using Selenium
+## Unofficial GPT-4 API access via chat.openai.com
 
 Have you **applied to GPT-4 API access** but **OpenAI is too busy to reply**? Me too, that's why I created this package. If the account has `ChatGPT Plus`, you can use **GPT-4**.
 
 It supports both **GPT4 browser and plugins** by selecting model via `GPT4OpenAI(token=token, model='gpt-4-browsing')`, or `model='gpt-4-plugins'`.
 
 **Note:** This unofficial API library is not endorsed by OpenAI and violates their Terms of Service. Use it at your own risk; the creator assumes no liability for any consequences. Please adhere to platform's ToS and exercise caution with unofficial resources.
 
@@ -98,14 +98,23 @@
 ```
 
 Output will be:
 ```
 AI: Ahoy, me name be John an' I be likin' ta feast on some pizza, arr!
 ```
 
+## `Continue generating` support
+
+In case of a large prompt answer, ChatGPT allows you to click `Continue generating` button. This library supports that as well.
+
+```python
+llm = GPT4OpenAI(llm=my_token, model='gpt-4', auto_continue=True)
+very_long_response = llm(my_prompt)
+```
+
 ## How to get the access token
 
 1. Go to https://chat.openai.com/api/auth/session
 2. In the JSON, copy the whole `accessToken` field.
 
 ![image](https://github.com/Erol444/gpt4-openai-api/assets/18037362/c0bdfd9c-8ad1-48ca-8344-621a4513e04b)
```

### Comparing `gpt4-openai-api-0.4.0/setup.py` & `gpt4-openai-api-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 root = Path(__file__).parent.resolve()
 readme_file = root / 'readme.md'
 long_description = readme_file.read_text(encoding='utf-8')
 
 setup(
     name="gpt4-openai-api",
-    version="0.4.0",
+    version="0.5.0",
     description="Python package for unofficial GPT-4 API access via chat.openai.com",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Erol444",
     author_email="erol123444@gmail.com",
     url="https://github.com/Erol444/gpt4-openai-api",
     packages=["gpt4_openai"],
```

### Comparing `gpt4-openai-api-0.4.0/test/test_browsing.py` & `gpt4-openai-api-0.5.0/test/test_browsing.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.4.0/test/test_langchain.py` & `gpt4-openai-api-0.5.0/test/test_langchain.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.4.0/test/test_plugins.py` & `gpt4-openai-api-0.5.0/test/test_plugins.py`

 * *Files identical despite different names*

