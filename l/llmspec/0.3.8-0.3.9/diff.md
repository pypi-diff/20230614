# Comparing `tmp/llmspec-0.3.8.tar.gz` & `tmp/llmspec-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.8.tar", last modified: Fri Jun  2 03:35:36 2023, max compression
+gzip compressed data, was "llmspec-0.3.9.tar", last modified: Mon Jun  5 07:30:38 2023, max compression
```

## Comparing `llmspec-0.3.8.tar` & `llmspec-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11098 2023-06-02 03:35:25.098366 llmspec-0.3.8/LICENSE
--rw-r--r--   0        0        0       33 2023-06-02 03:35:25.098366 llmspec-0.3.8/README.md
--rw-r--r--   0        0        0      659 2023-06-02 03:35:25.098366 llmspec-0.3.8/llmspec/__init__.py
--rw-r--r--   0        0        0     9928 2023-06-02 03:35:25.102367 llmspec-0.3.8/llmspec/llmspec.py
--rw-r--r--   0        0        0      215 2023-06-02 03:35:25.102367 llmspec-0.3.8/llmspec/mixins.py
--rw-r--r--   0        0        0     1130 2023-06-02 03:35:36.530713 llmspec-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-02 03:35:25.102367 llmspec-0.3.8/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-06-05 07:30:24.820378 llmspec-0.3.9/LICENSE
+-rw-r--r--   0        0        0       33 2023-06-05 07:30:24.820378 llmspec-0.3.9/README.md
+-rw-r--r--   0        0        0      659 2023-06-05 07:30:24.820378 llmspec-0.3.9/llmspec/__init__.py
+-rw-r--r--   0        0        0     9905 2023-06-05 07:30:24.820378 llmspec-0.3.9/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-06-05 07:30:24.820378 llmspec-0.3.9/llmspec/mixins.py
+-rw-r--r--   0        0        0     1130 2023-06-05 07:30:38.516965 llmspec-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-05 07:30:24.820378 llmspec-0.3.9/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.9/PKG-INFO
```

### Comparing `llmspec-0.3.8/LICENSE` & `llmspec-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.8/llmspec/__init__.py` & `llmspec-0.3.9/llmspec/__init__.py`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.8/llmspec/llmspec.py` & `llmspec-0.3.9/llmspec/llmspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     sep_token: str = ""
     append_assistant_token: bool = False
 
     # model class name in `transformers`
     transformer_model_cls: str = "AutoModelForCausalLM"
     tokenizer_cls: str = "AutoTokenizer"
 
-    # model structure
-    is_encoder_decoder: bool = True
+    low_cpu_mem_usage: bool = True
 
     def get_conversation_prompt(self, messages: List[ChatMessage]) -> str:
         """Get the prompt for a conversation using the specific tokens of the model."""
         formatted_messages = []
         for message in messages:
             if message.role == Role.USER:
                 message_prefix = self.user_token
@@ -68,14 +67,15 @@
 
 ChatGLM = LanguageModelInfo(
     user_token="问：",
     assistant_token="答：",
     system_token="",
     sep_token="\n",
     transformer_model_cls="AutoModel",
+    low_cpu_mem_usage=False,
 )
 MOSS = LanguageModelInfo(
     user_token="<|USER|>",
     assistant_token="<|ASSISTANT|>",
     system_token="<|SYSTEM|>",
     sep_token="\n",
     transformer_model_cls="AutoModelForCausalLM",
@@ -104,15 +104,14 @@
 )
 BloomZ = LanguageModelInfo(
     user_token="USER: ",
     assistant_token="ASSISTANT: ",
     system_token="",
     sep_token="\n",
     append_assistant_token=True,
-    is_encoder_decoder=False,
 )
 FastChatT5 = LanguageModelInfo(
     user_token="USER: ",
     assistant_token="ASSISTANT: ",
     system_token="",
     sep_token="\n### ",
     append_assistant_token=True,
@@ -326,14 +325,15 @@
 
 class EmbeddingRequest(msgspec.Struct, JSONSerializableMixin):
     model: str = ""
     input: Union[str, List[str]] = None
     user: str = ""
     encoding_format: str = "json"
 
+
 class EmbeddingData(msgspec.Struct):
     embedding: Union[List[float], str]
     index: int
     object: str = "embedding"
 
 
 class EmbeddingResponse(msgspec.Struct, JSONSerializableMixin):
```

### Comparing `llmspec-0.3.8/pyproject.toml` & `llmspec-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.8"
+version = "0.3.9"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
```

