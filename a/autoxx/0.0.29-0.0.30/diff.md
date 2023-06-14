# Comparing `tmp/autoxx-0.0.29.tar.gz` & `tmp/autoxx-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.29.tar", max compression
+gzip compressed data, was "autoxx-0.0.30.tar", max compression
```

## Comparing `autoxx-0.0.29.tar` & `autoxx-0.0.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.29/README.md
--rw-r--r--   0        0        0     7348 2023-06-08 08:33:03.275169 autoxx-0.0.29/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.29/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.29/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6052 2023-05-27 08:29:33.321541 autoxx-0.0.29/autoxx/config/config.py
--rw-r--r--   0        0        0      230 2023-05-27 08:43:09.345534 autoxx-0.0.29/autoxx/setup.py
--rw-r--r--   0        0        0     7252 2023-06-13 02:10:49.096956 autoxx-0.0.29/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-05-26 07:39:48.123009 autoxx-0.0.29/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.29/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13304 2023-06-12 05:37:24.331952 autoxx-0.0.29/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.29/autoxx/utils/base.py
--rw-r--r--   0        0        0     3198 2023-05-27 10:33:03.387959 autoxx-0.0.29/autoxx/utils/llm.py
--rw-r--r--   0        0        0     1905 2023-05-26 07:22:28.056438 autoxx-0.0.29/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.29/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5550 2023-05-27 10:33:16.566378 autoxx-0.0.29/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-05-27 01:02:06.078829 autoxx-0.0.29/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      659 2023-06-12 07:57:51.854344 autoxx-0.0.29/pyproject.toml
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 autoxx-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.30/README.md
+-rw-r--r--   0        0        0     7686 2023-06-13 13:41:17.104277 autoxx-0.0.30/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3617 2023-06-13 13:39:08.524255 autoxx-0.0.30/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.30/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.30/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.30/autoxx/setup.py
+-rw-r--r--   0        0        0     7659 2023-06-14 01:42:51.264483 autoxx-0.0.30/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.30/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.30/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13243 2023-06-14 02:32:00.475100 autoxx-0.0.30/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.30/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3198 2023-06-14 02:49:33.778554 autoxx-0.0.30/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.30/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.30/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.30/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2676 2023-06-14 03:38:54.107786 autoxx-0.0.30/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      660 2023-06-14 04:24:59.228393 autoxx-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 autoxx-0.0.30/PKG-INFO
```

### Comparing `autoxx-0.0.29/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.30/autoxx/agent/babyagi/agi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import json, time
+import threading
 from typing import Dict, List, Dict, Optional
 import logging
 
 from autoxx.tools.llm.base import get_chat_completion
 
 from autoxx.tools.web_search.search import web_search
 from autoxx.tools.llm.base import llm_uils
 from autoxx.utils.llm import create_message
 
 
 class AGIExecutor:
-    def __init__(self, objective:str, max_tasks_count: Optional[int] = 5):
+    def __init__(self, objective:str, max_tasks_count: Optional[int] = 5, cancel_event: Optional[threading.Event] = None):
         if objective is None or len(objective) <= 1:  
             raise ValueError("Must provide an objective")  
 
         self.objective = objective
         self.max_tasks_count = max_tasks_count
 
         self.task_list = self.init_task_list(objective)
-        self.status = "initizing"
+        self.status = "pending"
         self.error_message = None
         self.final_answer = None
+        self.cancel_event = cancel_event
 
     def get_task_by_id(self, task_id: int):
         for task in self.task_list:
             if task["id"] == task_id:
                 return task
         return None
 
@@ -106,14 +108,18 @@
         task["result"] = result
         return task
     
     def execute(self):
         self.status = "running"
         # Main loop
         while any(task["status"] == "incomplete" for task in self.task_list):
+            if self.cancel_event is not None and self.cancel_event.is_set():
+                logging.info(f"\033[91m\033[1m CANCELLED({self.objective}) \033[0m\033[0m")
+                self.status = "cancelled"
+                return
               # Filter out incomplete tasks
             incomplete_tasks = [task for task in self.task_list if task["status"] == "incomplete"]
             logging.info(f"\033[95m\033[1m INCOMPLETE TASK LIST({self.objective}) \033[0m\033[0m {[str(t['id'])+': '+t['task'] + '[' + t['tool'] + ']' for t in incomplete_tasks]}")
             if incomplete_tasks:
                 # Sort tasks by ID
                 incomplete_tasks.sort(key=lambda x: x["id"])
```

### Comparing `autoxx-0.0.29/autoxx/agent/react/agent.py` & `autoxx-0.0.30/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.29/autoxx/config/config.py` & `autoxx-0.0.30/autoxx/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     def __init__(self) -> None:
         """Initialize the Config class"""
         self.debug_mode = False
 
         self.openai_api_key = os.getenv("OPENAI_API_KEY")
-        self.llm_models =   os.getenv("LLM_MODELS", "gpt-3.5-turbo,gpt-4").split(",")
+        self.llm_models =   os.getenv("LLM_MODELS", "gpt-3.5-turbo,gpt-4,gpt-3.5-turbo-16k").split(",")
         self.embedding_models = os.getenv("EMBEDDING_MODELS", "text-embedding-ada-002").split(",")
         self.model_config = {}
         for model in self.llm_models:
             self.set_llm_model_config(model)
         for model in self.embedding_models:
             self.set_embedding_model_config(model)
```

### Comparing `autoxx-0.0.29/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.30/autoxx/tools/knowledge_base/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pinecone,re
-import os
+import os, time
 from typing import Optional,List
 from langchain.chat_models import ChatOpenAI
 from autoxx.config.config import GlobalConfig
 from llama_index.embeddings.openai import OpenAIEmbedding
+import logging
 
 from llama_index import (LLMPredictor,
                         ServiceContext,
                         StorageContext,
                         VectorStoreIndex)
 from llama_index.indices.loading import load_index_from_storage
 from llama_index.storage.docstore import MongoDocumentStore
@@ -15,14 +16,15 @@
 from llama_index.vector_stores import PineconeVectorStore
 from llama_index.readers.schema.base import Document
 from llama_index.node_parser import SimpleNodeParser
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.callbacks.base import CallbackManager
 from llama_index.indices.query.query_transform import HyDEQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
+from llama_index.indices.response import ResponseMode
 
 class knowleage_bot:
 
     def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo", embedding_model: str="text-embedding-ada-002"):
         if not is_valid_corpus_name(corpus):
             raise ValueError(f"Invalid corpus name: {corpus}. coprus name must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character")
 
@@ -101,33 +103,40 @@
                     storage_context=storage_context,
                     service_context=service_context,
                 )
             else:
                raise e
 
     def query(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
+        start_time = time.time()
         query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k)
+
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
             query_engine = TransformQueryEngine(query_engine, hyde)
 
         try:
-            return query_engine.query(query)
+            response = query_engine.query(query)
+            logging.info(f"query: {query}, response: {response}, cost: {time.time() - start_time}")
+            return response
         except Exception as e:
             print("Error:", e)
             raise Exception(f"failed to finish query: {str(e)}")
 
     def similarity_search(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
+        start_time = time.time()
         query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k)
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
             query_engine = TransformQueryEngine(query_engine, hyde)
 
         try:
-            return query_engine.retrieve(query)
+            response =  query_engine.retrieve(query)
+            logging.info(f"query: {query}, response: {response}, cost: {time.time() - start_time}")
+            return response
         except Exception as e:
             print("Error:", e)
             raise Exception(f"failed to retrieve nodes: {str(e)}")
 
     def upsert_document(self, documents: List[Document]) -> None:
         self.index.docstore.add_documents(documents, allow_update=True)
         for document in documents:
```

### Comparing `autoxx-0.0.29/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.30/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.29/autoxx/tools/web_search/search.py` & `autoxx-0.0.30/autoxx/tools/web_search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from autoxx.utils.llm import get_chat_completion
 from autoxx.utils.processing_text import split_text
 from autoxx.utils.token_counter import count_message_tokens
 from autoxx.utils.processing_html import extract_hyperlinks, format_hyperlinks
 from autoxx.utils.base import Message
 
 BrowserOptions = ChromeOptions | EdgeOptions | FirefoxOptions | SafariOptions
-MaxChunkTokenSize = 3072
 MaxSummaryTokenSize = 2048
 
 FILE_DIR = Path(__file__).parent
 
 def create_summary_message(chunk: str, question: str) -> Message:
     """Create a message for the chat completion
 
@@ -200,15 +199,15 @@
         str: The summary of the chunks
     """
     model = "gpt-3.5-turbo"
     logging.debug(f"Memorizing text:\n{'-'*32}\n{text}\n{'-'*32}\n")
     chunks = [
         chunk
         for chunk, _ in (
-            split_text(text, for_model=model, max_chunk_length=MaxChunkTokenSize)
+            split_text(text, for_model=model)
         )
     ]
 
     summaries = []
     scroll_ratio = 1 / len(chunks)
     for i, chunk in enumerate(chunks):
         if driver:
```

### Comparing `autoxx-0.0.29/autoxx/utils/base.py` & `autoxx-0.0.30/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.29/autoxx/utils/llm.py` & `autoxx-0.0.30/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.29/autoxx/utils/openai_models.py` & `autoxx-0.0.30/autoxx/utils/openai_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,39 +6,51 @@
         ChatModelInfo(
             name="gpt-3.5-turbo",
             prompt_token_cost=0.002,
             completion_token_cost=0.002,
             max_tokens=4096,
         ),
         ChatModelInfo(
-            name="gpt-3.5-turbo-0301",
-            prompt_token_cost=0.002,
+            name="gpt-3.5-turbo-16k",
+            prompt_token_cost=0.003,
+            completion_token_cost=0.004,
+            max_tokens=16384,
+        ),
+        ChatModelInfo(
+            name="gpt-3.5-turbo-0613",
+            prompt_token_cost=0.0015,
             completion_token_cost=0.002,
             max_tokens=4096,
         ),
         ChatModelInfo(
+            name="gpt-3.5-turbo-16k-0613",
+            prompt_token_cost=0.003,
+            completion_token_cost=0.004,
+            max_tokens=16384,
+        ),
+        ChatModelInfo(
             name="gpt-4",
             prompt_token_cost=0.03,
             completion_token_cost=0.06,
             max_tokens=8192,
         ),
         ChatModelInfo(
-            name="gpt-4-0314",
+            name="gpt-4-0613",
             prompt_token_cost=0.03,
             completion_token_cost=0.06,
             max_tokens=8192,
         ),
         ChatModelInfo(
             name="gpt-4-32k",
             prompt_token_cost=0.06,
             completion_token_cost=0.12,
             max_tokens=32768,
         ),
         ChatModelInfo(
-            name="gpt-4-32k-0314",
+            name="gpt-4-32k-0613",
             prompt_token_cost=0.06,
             completion_token_cost=0.12,
             max_tokens=32768,
         ),
     ]
 }
 
@@ -55,15 +67,15 @@
 }
 
 OPEN_AI_EMBEDDING_MODELS = {
     info.name: info
     for info in [
         EmbeddingModelInfo(
             name="text-embedding-ada-002",
-            prompt_token_cost=0.0004,
+            prompt_token_cost=0.0001,
             completion_token_cost=0.0,
             max_tokens=8191,
             embedding_dimensions=1536,
         ),
     ]
 }
```

### Comparing `autoxx-0.0.29/autoxx/utils/processing_html.py` & `autoxx-0.0.30/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.29/autoxx/utils/processing_text.py` & `autoxx-0.0.30/autoxx/utils/processing_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # batched('ABCDEFG', 3) --> ABC DEF G
     if max_batch_length < 1:
         raise ValueError("n must be at least one")
     for i in range(0, len(iterable), max_batch_length - overlap):
         yield iterable[i : i + max_batch_length]
 
 def _max_chunk_length(model: str, max: Optional[int] = None) -> int:
-    model_max_input_tokens = OPEN_AI_MODELS[model].max_tokens - 1
+    model_max_input_tokens = OPEN_AI_MODELS[model].max_tokens - 1024
     if max is not None and max > 0:
         return min(max, model_max_input_tokens)
     return model_max_input_tokens
 
 
 def must_chunk_content(
     text: str, for_model: str, max_chunk_length: Optional[int] = None
```

### Comparing `autoxx-0.0.29/autoxx/utils/token_counter.py` & `autoxx-0.0.30/autoxx/utils/token_counter.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,27 @@
         int: The number of tokens used by the list of messages.
     """
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         logging.warn("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model == "gpt-3.5-turbo":
+    if model in ("gpt-3.5-turbo-0301", "gpt-3.5-turbo-16k", "gpt-3.5-turbo-0613"):
         # !Note: gpt-3.5-turbo may change over time.
         # Returning num tokens assuming gpt-3.5-turbo-0301.")
         return count_message_tokens(messages, model="gpt-3.5-turbo-0301")
-    elif model == "gpt-4":
+    elif model == "gpt-4-0314":
         # !Note: gpt-4 may change over time. Returning num tokens assuming gpt-4-0314.")
         return count_message_tokens(messages, model="gpt-4-0314")
-    elif model == "gpt-3.5-turbo-0301":
+    elif model == "gpt-3.5-turbo":
         tokens_per_message = (
             4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         )
         tokens_per_name = -1  # if there's a name, the role is omitted
-    elif model == "gpt-4-0314":
+    elif model == "gpt-4":
         tokens_per_message = 3
         tokens_per_name = 1
     else:
         raise NotImplementedError(
             f"num_tokens_from_messages() is not implemented for model {model}.\n"
             " See https://github.com/openai/openai-python/blob/main/chatml.md for"
             " information on how messages are converted to tokens."
```

### Comparing `autoxx-0.0.29/pyproject.toml` & `autoxx-0.0.30/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.29"
+version = "0.0.30"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pinecone-client = "2.2.1"
 selenium = "4.9.0"
 openai = "0.27.6"
-colorama = "0.4.6"
+colorama = "^0.4.6"
 python-dotenv = "1.0.0"
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
```

### Comparing `autoxx-0.0.29/PKG-INFO` & `autoxx-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.29
+Version: 0.0.30
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
-Requires-Dist: colorama (==0.4.6)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
 Requires-Dist: llama-index (>=0.6.23,<0.7.0)
 Requires-Dist: openai (==0.27.6)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
```

