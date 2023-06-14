# Comparing `tmp/idoctorai-0.3.3.tar.gz` & `tmp/idoctorai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.3.3.tar", max compression
+gzip compressed data, was "idoctorai-0.3.4.tar", max compression
```

## Comparing `idoctorai-0.3.3.tar` & `idoctorai-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.3/LICENSE
--rw-r--r--   0        0        0    19255 2023-06-12 10:47:39.546717 idoctorai-0.3.3/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.3/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.3/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.3/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.3/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.3/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.3/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.3/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.3/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.3/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2909 2023-06-12 10:52:31.217546 idoctorai-0.3.3/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.3/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.3/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.3.3/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.3/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.3/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.3/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3240 2023-06-10 07:56:37.939765 idoctorai-0.3.3/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.3/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.3/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.3/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.3/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.3/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.3/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1474 2023-06-12 10:59:18.425545 idoctorai-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.3/README.md
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 idoctorai-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.3.4/LICENSE
+-rw-r--r--   0        0        0    19255 2023-06-12 12:05:15.993358 idoctorai-0.3.4/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.3.4/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.3.4/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.3.4/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.3.4/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.3.4/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.3.4/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.3.4/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.3.4/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.3.4/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2982 2023-06-14 13:10:20.872222 idoctorai-0.3.4/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.3.4/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.3.4/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.3.4/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.3.4/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.3.4/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.3.4/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.3.4/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.3.4/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1845 2023-05-31 07:10:59.369581 idoctorai-0.3.4/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.3.4/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1646 2023-05-31 07:10:59.370561 idoctorai-0.3.4/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.3.4/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1511 2023-06-08 05:58:42.812889 idoctorai-0.3.4/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1474 2023-06-14 13:12:56.242390 idoctorai-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.3.4/README.md
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 idoctorai-0.3.4/PKG-INFO
```

### Comparing `idoctorai-0.3.3/LICENSE` & `idoctorai-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/__init__.py` & `idoctorai-0.3.4/pandasai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     """
 
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = False
     _enforce_privacy: bool = False
-    _max_retries: int = 3
+    _max_retries: int = 1
     _is_notebook: bool = False
     _original_instructions: dict = {
         "question": None,
         "df_head": None,
         "num_rows": None,
         "num_columns": None,
         "rows_to_display": None,
```

### Comparing `idoctorai-0.3.3/pandasai/constants.py` & `idoctorai-0.3.4/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/exceptions.py` & `idoctorai-0.3.4/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/_optional.py` & `idoctorai-0.3.4/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/anonymizer.py` & `idoctorai-0.3.4/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/cache.py` & `idoctorai-0.3.4/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/from_excel.py` & `idoctorai-0.3.4/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/notebook.py` & `idoctorai-0.3.4/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/helpers/save_chart.py` & `idoctorai-0.3.4/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/langchain/__init__.py` & `idoctorai-0.3.4/pandasai/langchain/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 Assistant is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
 
 Overall, Assistant is a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether you need help with a specific question or just want to have a conversation about a particular topic, Assistant is here to assist.
 
 {history}
 Human: {human_input}
 Assistant:"""
+    
+    template= """
+{history}
+Human: {human_input}
+Assistant:"""
 
     def __init__(self, api_token: Optional[str] = None, **kwargs,):
         self.api_token = api_token or None
         self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0, max_tokens=512)
         prompt = PromptTemplate(
             input_variables=["history","human_input"], 
             template=self.template
```

### Comparing `idoctorai-0.3.3/pandasai/llm/azure_openai.py` & `idoctorai-0.3.4/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/llm/base.py` & `idoctorai-0.3.4/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/llm/fake.py` & `idoctorai-0.3.4/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/llm/google_palm.py` & `idoctorai-0.3.4/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/llm/open_assistant.py` & `idoctorai-0.3.4/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/llm/openai.py` & `idoctorai-0.3.4/pandasai/llm/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
             # response = self.chat_completion(str(instruction) + str(value) + suffix)
             response = self.langchain_input(str(instruction) + str(value) + suffix, history)
+            print(response)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `idoctorai-0.3.3/pandasai/llm/starcoder.py` & `idoctorai-0.3.4/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/base.py` & `idoctorai-0.3.4/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.3.4/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.3.4/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/generate_python_code.py` & `idoctorai-0.3.4/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/generate_response.py` & `idoctorai-0.3.4/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.3.4/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.3.3/pyproject.toml` & `idoctorai-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.3.3"
+version = "0.3.4"
 description = "this is idoctorai, Generate code with natural speech"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
```

### Comparing `idoctorai-0.3.3/PKG-INFO` & `idoctorai-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.3.3
+Version: 0.3.4
 Summary: this is idoctorai, Generate code with natural speech
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

