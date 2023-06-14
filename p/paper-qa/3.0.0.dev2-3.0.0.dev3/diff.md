# Comparing `tmp/paper-qa-3.0.0.dev2.tar.gz` & `tmp/paper-qa-3.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.0.0.dev2.tar", last modified: Tue Jun 13 16:48:09 2023, max compression
+gzip compressed data, was "paper-qa-3.0.0.dev3.tar", last modified: Wed Jun 14 05:53:43 2023, max compression
```

## Comparing `paper-qa-3.0.0.dev2.tar` & `paper-qa-3.0.0.dev3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20465 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18141 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 05:53:43.000000 paper-qa-3.0.0.dev3/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:53:43.152098 paper-qa-3.0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-06-14 05:53:04.000000 paper-qa-3.0.0.dev3/tests/test_paperqa.py
```

### Comparing `paper-qa-3.0.0.dev2/LICENSE` & `paper-qa-3.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev2/PKG-INFO` & `paper-qa-3.0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev2
+Version: 3.0.0.dev3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -140,14 +140,15 @@
 ```py
 import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
 from langchain.embeddings import LlamaCppEmbeddings
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
     model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
@@ -196,19 +197,20 @@
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
 
 
 ### New Features
 
 The following new features are in v3:
 
-1. `add_url` and `add_file` are now supported for adding from URLs and file objects
-2. Prompts can be customized, and now can be executed pre and post query
-3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
-4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
-5. Various simplifications, bug fixes, and performance improvements
+1. Memory is now possible in `query` by setting `Docs(memory=True)` - this means follow-up questions will have a record of the previous question and answer.
+2. `add_url` and `add_file` are now supported for adding from URLs and file objects
+3. Prompts can be customized, and now can be executed pre and post query
+4. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+5. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+6. Various simplifications, bug fixes, and performance improvements
 
 ### Naming
 
 The following table shows the old names and the new names:
 
 | Old Name | New Name | Explanation |
 | :--- | :---: | ---: |
@@ -345,14 +347,15 @@
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
 from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
 ## LLM/Embedding Caching
```

### Comparing `paper-qa-3.0.0.dev2/README.md` & `paper-qa-3.0.0.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 ```py
 import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
 from langchain.embeddings import LlamaCppEmbeddings
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
     model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
@@ -182,19 +183,20 @@
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
 
 
 ### New Features
 
 The following new features are in v3:
 
-1. `add_url` and `add_file` are now supported for adding from URLs and file objects
-2. Prompts can be customized, and now can be executed pre and post query
-3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
-4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
-5. Various simplifications, bug fixes, and performance improvements
+1. Memory is now possible in `query` by setting `Docs(memory=True)` - this means follow-up questions will have a record of the previous question and answer.
+2. `add_url` and `add_file` are now supported for adding from URLs and file objects
+3. Prompts can be customized, and now can be executed pre and post query
+4. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+5. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+6. Various simplifications, bug fixes, and performance improvements
 
 ### Naming
 
 The following table shows the old names and the new names:
 
 | Old Name | New Name | Explanation |
 | :--- | :---: | ---: |
@@ -331,14 +333,15 @@
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
 from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
 ## LLM/Embedding Caching
```

### Comparing `paper-qa-3.0.0.dev2/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.0.0.dev3/paper_qa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev2
+Version: 3.0.0.dev3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -140,14 +140,15 @@
 ```py
 import paperscraper
 from paperqa import Docs
 from langchain.llms import LlamaCpp
 from langchain import PromptTemplate, LLMChain
 from langchain.callbacks.manager import CallbackManager
 from langchain.embeddings import LlamaCppEmbeddings
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 # Make sure the model path is correct for your system!
 llm = LlamaCpp(
     model_path="./ggml-model-q4_0.bin", callbacks=[StreamingStdOutCallbackHandler()]
 )
 embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
 
@@ -196,19 +197,20 @@
 Version 3 includes many changes to type the code, make it more focused/modular, and enable performance to very large numbers of documents. The major breaking changes are documented below:
 
 
 ### New Features
 
 The following new features are in v3:
 
-1. `add_url` and `add_file` are now supported for adding from URLs and file objects
-2. Prompts can be customized, and now can be executed pre and post query
-3. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
-4. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
-5. Various simplifications, bug fixes, and performance improvements
+1. Memory is now possible in `query` by setting `Docs(memory=True)` - this means follow-up questions will have a record of the previous question and answer.
+2. `add_url` and `add_file` are now supported for adding from URLs and file objects
+3. Prompts can be customized, and now can be executed pre and post query
+4. Consistent use of `dockey` and `docname` for unique and natural language names enable better tracking with external databases
+5. Texts and embeddings are no longer required to be part of `Docs` object, so you can use external databases or other strategies to manage them
+6. Various simplifications, bug fixes, and performance improvements
 
 ### Naming
 
 The following table shows the old names and the new names:
 
 | Old Name | New Name | Explanation |
 | :--- | :---: | ---: |
@@ -345,14 +347,15 @@
 
 To stream the completions as they occur (giving that ChatGPT typewriter look), you can simply instantiate models with those properties:
 
 ```python
 from paperqa import Docs
 from langchain.callbacks.manager import CallbackManager
 from langchain.chat_models import ChatOpenAI
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 my_llm = ChatOpenAI(callbacks=[StreamingStdOutCallbackHandler()], streaming=True)
 docs = Docs(llm=my_llm)
 ```
 
 ## LLM/Embedding Caching
```

### Comparing `paper-qa-3.0.0.dev2/paperqa/contrib/zotero.py` & `paper-qa-3.0.0.dev3/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev2/paperqa/docs.py` & `paper-qa-3.0.0.dev3/paperqa/docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from pathlib import Path
 from typing import BinaryIO, Dict, List, Optional, Set, Union, cast
 
 from langchain.base_language import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings.base import Embeddings
 from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain.memory import ConversationTokenBufferMemory
+from langchain.memory.chat_memory import BaseChatMemory
 from langchain.vectorstores import FAISS, VectorStore
 from pydantic import BaseModel, validator
 
 from .chains import get_score, make_chain
 from .paths import PAPERQA_DIR
 from .readers import read_doc
 from .types import Answer, CallbackFactory, Context, Doc, DocKey, PromptCollection, Text
@@ -44,27 +46,47 @@
     summary_llm: Optional[Union[str, BaseLanguageModel]] = None
     name: str = "default"
     index_path: Optional[Path] = PAPERQA_DIR / name
     embeddings: Embeddings = OpenAIEmbeddings(client=None)
     max_concurrent: int = 5
     deleted_dockeys: Set[DocKey] = set()
     prompts: PromptCollection = PromptCollection()
+    memory: bool = False
+    memory_model: Optional[BaseChatMemory] = None
 
     # TODO: Not sure how to get this to work
     # while also passing mypy checks
     @validator("llm", "summary_llm")
     def check_llm(cls, v: Union[BaseLanguageModel, str]) -> BaseLanguageModel:
         if type(v) is str:
             return ChatOpenAI(temperature=0.1, model=v, client=None)
-        return v
+        return cast(BaseLanguageModel, v)
 
     @validator("summary_llm", always=True)
     def copy_llm_if_not_set(cls, v, values):
         return v or values["llm"]
 
+    @validator("memory_model", always=True)
+    def check_memory_model(cls, v, values):
+        if values["memory"]:
+            if v is None:
+                return ConversationTokenBufferMemory(
+                    llm=values["summary_llm"],
+                    max_token_limit=512,
+                    memory_key="memory",
+                    human_prefix="Question",
+                    ai_prefix="Answer",
+                    input_key="Question",
+                    output_key="Answer",
+                )
+            if v.memory_variables()[0] != "memory":
+                raise ValueError("Memory model must have memory_variables=['memory']")
+            return values["memory_model"]
+        return None
+
     def update_llm(
         self,
         llm: Union[BaseLanguageModel, str],
         summary_llm: Optional[Union[BaseLanguageModel, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
         if type(llm) is str:
@@ -72,15 +94,15 @@
         if type(summary_llm) is str:
             summary_llm = ChatOpenAI(temperature=0.1, model=summary_llm, client=None)
         self.llm = cast(BaseLanguageModel, llm)
         if summary_llm is None:
             summary_llm = llm
         self.summary_llm = cast(BaseLanguageModel, summary_llm)
 
-    def get_unique_name(self, docname: str) -> str:
+    def _get_unique_name(self, docname: str) -> str:
         """Create a unique name given proposed name"""
         suffix = ""
         while docname + suffix in self.docnames:
             # move suffix to next letter
             if suffix == "":
                 suffix = "a"
             else:
@@ -178,20 +200,22 @@
                     "(path, citation, key='mykey')"
                 )
             year = ""
             match = re.search(r"(\d{4})", citation)
             if match is not None:
                 year = match.group(1)  # type: ignore
             docname = f"{author}{year}"
-        docname = self.get_unique_name(docname)
+        docname = self._get_unique_name(docname)
         doc = Doc(docname=docname, citation=citation, dockey=dockey)
         texts = read_doc(path, doc, chunk_chars=chunk_chars, overlap=100)
         # loose check to see if document was loaded
-        if len(texts[0].text) < 10 or (
-            not disable_check and not maybe_is_text(texts[0].text)
+        if (
+            len(texts) == 0
+            or len(texts[0].text) < 10
+            or (not disable_check and not maybe_is_text(texts[0].text))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
             )
         self.add_texts(texts, doc)
         return docname
 
@@ -202,15 +226,15 @@
     ):
         """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself."""
         if doc.dockey in self.docs:
             raise ValueError(f"Document {doc.dockey} already in collection.")
         if len(texts) == 0:
             raise ValueError("No texts to add.")
         if doc.docname in self.docnames:
-            new_docname = self.get_unique_name(doc.docname)
+            new_docname = self._get_unique_name(doc.docname)
             for t in texts:
                 t.name = t.name.replace(doc.docname, new_docname)
             doc.docname = new_docname
         if texts[0].embeddings is None:
             text_embeddings = self.embeddings.embed_documents([t.text for t in texts])
             for i, t in enumerate(texts):
                 t.embeddings = text_embeddings[i]
@@ -257,15 +281,17 @@
             self.doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         matches = self.doc_index.max_marginal_relevance_search(
             query, k=k + len(self.deleted_dockeys)
         )
         matched_docs = [self.docs[m.metadata["dockey"]] for m in matches]
-        chain = make_chain(self.prompts.select, cast(BaseLanguageModel, self.llm))
+        chain = make_chain(
+            self.prompts.select, cast(BaseLanguageModel, self.llm), skip_system=True
+        )
         papers = [f"{d.docname}: {d.citation}" for d in matched_docs]
         result = await chain.arun(  # type: ignore
             question=query, papers="\n".join(papers), callbacks=get_callbacks("filter")
         )
         return set([d.dockey for d in matched_docs if d.docname in result])
 
     def __getstate__(self):
@@ -294,14 +320,19 @@
             self.texts_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(raw_texts, text_embeddings)),
                 embedding=self.embeddings,
                 metadatas=metadatas,
             )
 
+    def clear_memory(self):
+        """Clear the memory of the model."""
+        if self.memory_model is not None:
+            self.memory_model.clear()
+
     def get_evidence(
         self,
         answer: Answer,
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
@@ -371,15 +402,17 @@
         matches = [m for m in matches if m.metadata["name"] not in cur_names]
 
         # now finally cut down
         matches = matches[:k]
 
         async def process(match):
             callbacks = get_callbacks("evidence:" + match.metadata["name"])
-            summary_chain = make_chain(self.prompts.summary, self.summary_llm)
+            summary_chain = make_chain(
+                self.prompts.summary, self.summary_llm, memory=self.memory_model
+            )
             # This is dangerous because it
             # could mask errors that are important- like auth errors
             # I also cannot know what the exception
             # type is because any model could be used
             # my best idea is see if there is a 4XX
             # http code in the exception
             try:
@@ -387,15 +420,15 @@
                     question=answer.question,
                     citation=match.metadata["doc"]["citation"],
                     summary_length=answer.summary_length,
                     text=match.page_content,
                     callbacks=callbacks,
                 )
             except Exception as e:
-                if guess_is_4xx(e):
+                if guess_is_4xx(str(e)):
                     return None
                 raise e
             if "not applicable" in context.lower():
                 return None
             c = Context(
                 context=context,
                 text=Text(
@@ -472,43 +505,51 @@
         get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         if k < max_sources:
             raise ValueError("k should be greater than max_sources")
         if answer is None:
             answer = Answer(question=query, answer_length=length_prompt)
         if len(answer.contexts) == 0:
-            # this is heuristic - max_sources and len(docs) are not
+            # this is heuristic - k and len(docs) are not
             # comparable - one is chunks and one is docs
-            if key_filter or (key_filter is None and len(self.docs) > max_sources):
+            if key_filter or (key_filter is None and len(self.docs) > k):
                 keys = await self.adoc_match(
                     answer.question, get_callbacks=get_callbacks
                 )
                 if len(keys) > 0:
                     answer.dockey_filter = keys
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 get_callbacks=get_callbacks,
             )
         if self.prompts.pre is not None:
-            chain = make_chain(self.prompts.pre, self.llm)
+            chain = make_chain(
+                self.prompts.pre,
+                cast(BaseLanguageModel, self.llm),
+                memory=self.memory_model,
+            )
             pre = await chain.arun(
                 question=answer.question, callbacks=get_callbacks("pre")
             )
             answer.context = pre + "\n\n" + answer.context
         bib = dict()
-        if len(answer.context) < 10:
+        if len(answer.context) < 10 and not self.memory:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
             callbacks = get_callbacks("answer")
-            qa_chain = make_chain(self.prompts.qa, self.llm)
+            qa_chain = make_chain(
+                self.prompts.qa,
+                cast(BaseLanguageModel, self.llm),
+                memory=self.memory_model,
+            )
             answer_text = await qa_chain.arun(
                 context=answer.context,
                 answer_length=answer.answer_length,
                 question=answer.question,
                 callbacks=callbacks,
             )
         # it still happens
@@ -527,15 +568,24 @@
         if len(bib) > 0:
             formatted_answer += f"\nReferences\n\n{bib_str}\n"
         answer.answer = answer_text
         answer.formatted_answer = formatted_answer
         answer.references = bib_str
 
         if self.prompts.post is not None:
-            chain = make_chain(self.prompts.post, self.llm)
+            chain = make_chain(
+                self.prompts.post,
+                cast(BaseLanguageModel, self.llm),
+                memory=self.memory_model,
+            )
             post = await chain.arun(**answer.dict(), callbacks=get_callbacks("post"))
             answer.answer = post
             answer.formatted_answer = f"Question: {query}\n\n{post}\n"
             if len(bib) > 0:
                 answer.formatted_answer += f"\nReferences\n\n{bib_str}\n"
+        if self.memory_model is not None:
+            answer.memory = self.memory_model.load_memory_variables(inputs={})["memory"]
+            self.memory_model.save_context(
+                {"Question": answer.question}, {"Answer": answer.answer}
+            )
 
         return answer
```

### Comparing `paper-qa-3.0.0.dev2/paperqa/prompts.py` & `paper-qa-3.0.0.dev3/paperqa/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from langchain.prompts import PromptTemplate
 
 summary_prompt = PromptTemplate(
     input_variables=["text", "citation", "question", "summary_length"],
     template="Summarize the text below to help answer a question. "
     "Do not directly answer the question, instead summarize "
-    "to give evidence to help answer the question. Include direct quotes. "
+    "to give evidence to help answer the question. "
     'Reply "Not applicable" if text is irrelevant. '
     "Use {summary_length}. At the end of your response, provide a score from 1-10 on a newline "
     "indicating relevance to question. Do not explain your score. "
     "\n\n"
-    "{text}\n"
-    "Extracted from {citation}\n"
+    "{text}\n\n"
+    "Excerpt from {citation}\n"
     "Question: {question}\n"
     "Relevant Information Summary:",
 )
 
 qa_prompt = PromptTemplate(
     input_variables=["context", "answer_length", "question"],
     template="Write an answer ({answer_length}) "
```

### Comparing `paper-qa-3.0.0.dev2/paperqa/readers.py` & `paper-qa-3.0.0.dev3/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev2/paperqa/types.py` & `paper-qa-3.0.0.dev3/paperqa/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     context: str = ""
     contexts: List[Context] = []
     references: str = ""
     formatted_answer: str = ""
     dockey_filter: Optional[Set[DocKey]] = None
     summary_length: str = "about 100 words"
     answer_length: str = "about 100 words"
+    memory: Optional[str] = None
     # these two below are for convenience
     # and are not set. But you can set them
     # if you want to use them.
     cost: Optional[float] = None
     token_counts: Optional[Dict[str, List[int]]] = None
 
     def __str__(self) -> str:
```

### Comparing `paper-qa-3.0.0.dev2/paperqa/utils.py` & `paper-qa-3.0.0.dev3/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev2/setup.py` & `paper-qa-3.0.0.dev3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
     license="MIT",
     packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
-        "langchain>=0.0.195",
+        "langchain>=0.0.198",
         "openai >= 0.27.8",
         "faiss-cpu",
         "PyCryptodome",
         "html2text",
-        "tiktoken",
+        "tiktoken>=0.4.0",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `paper-qa-3.0.0.dev2/tests/test_paperqa.py` & `paper-qa-3.0.0.dev3/tests/test_paperqa.py`

 * *Files 3% similar despite different names*

```diff
@@ -525,7 +525,36 @@
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What country is Bates from?")
+
+
+def test_memory():
+    docs = Docs(memory=True, k=3, max_sources=1, llm="gpt-3.5-turbo", key_filter=False)
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/Red_Army",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    answer1 = docs.query("When did the Soviet Union and Japan agree to a cease-fire?")
+    print(answer1.answer)
+    assert answer1.memory is not None
+    assert "1939" in answer1.answer
+    assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
+    answer2 = docs.query("When was the conflict resolved?")
+    assert "1941" in answer2.answer or "1945" in answer2.answer
+    assert answer2.memory is not None
+    assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
+    print(answer2.answer)
+
+    docs.clear_memory()
+
+    answer3 = docs.query("When was the conflict resolved?")
+    assert answer3.memory is not None
+    assert (
+        "I cannot answer" in answer3.answer
+        or "insufficient" in answer3.answer
+        or "does not provide" in answer3.answer
+    )
```

