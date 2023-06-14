# Comparing `tmp/paper-qa-3.0.0.dev1.tar.gz` & `tmp/paper-qa-3.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.0.0.dev1.tar", last modified: Sat Jun 10 11:20:01 2023, max compression
+gzip compressed data, was "paper-qa-3.0.0.dev2.tar", last modified: Tue Jun 13 16:48:09 2023, max compression
```

## Comparing `paper-qa-3.0.0.dev1.tar` & `paper-qa-3.0.0.dev2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 11:20:01.000000 paper-qa-3.0.0.dev1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20516 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:20:01.195564 paper-qa-3.0.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-10 11:19:26.000000 paper-qa-3.0.0.dev1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 16:48:09.000000 paper-qa-3.0.0.dev2/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20465 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:48:09.272610 paper-qa-3.0.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-13 16:47:35.000000 paper-qa-3.0.0.dev2/tests/test_paperqa.py
```

### Comparing `paper-qa-3.0.0.dev1/LICENSE` & `paper-qa-3.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/PKG-INFO` & `paper-qa-3.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev1
+Version: 3.0.0.dev2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.0.0.dev1/README.md` & `paper-qa-3.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.0.0.dev2/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.0.0.dev1
+Version: 3.0.0.dev2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.0.0.dev1/paperqa/chains.py` & `paper-qa-3.0.0.dev2/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/paperqa/contrib/zotero.py` & `paper-qa-3.0.0.dev2/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/paperqa/docs.py` & `paper-qa-3.0.0.dev2/paperqa/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     def add_texts(
         self,
         texts: List[Text],
         doc: Doc,
     ):
         """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself."""
         if doc.dockey in self.docs:
-            raise ValueError("Document already in collection.")
+            raise ValueError(f"Document {doc.dockey} already in collection.")
         if len(texts) == 0:
             raise ValueError("No texts to add.")
         if doc.docname in self.docnames:
             new_docname = self.get_unique_name(doc.docname)
             for t in texts:
                 t.name = t.name.replace(doc.docname, new_docname)
             doc.docname = new_docname
@@ -257,17 +257,15 @@
             self.doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         matches = self.doc_index.max_marginal_relevance_search(
             query, k=k + len(self.deleted_dockeys)
         )
         matched_docs = [self.docs[m.metadata["dockey"]] for m in matches]
-        chain = make_chain(
-            self.prompts.select, cast(BaseLanguageModel, self.summary_llm)
-        )
+        chain = make_chain(self.prompts.select, cast(BaseLanguageModel, self.llm))
         papers = [f"{d.docname}: {d.citation}" for d in matched_docs]
         result = await chain.arun(  # type: ignore
             question=query, papers="\n".join(papers), callbacks=get_callbacks("filter")
         )
         return set([d.dockey for d in matched_docs if d.docname in result])
 
     def __getstate__(self):
@@ -503,15 +501,14 @@
         if len(answer.context) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
             callbacks = get_callbacks("answer")
             qa_chain = make_chain(self.prompts.qa, self.llm)
-            print(self.prompts.qa)
             answer_text = await qa_chain.arun(
                 context=answer.context,
                 answer_length=answer.answer_length,
                 question=answer.question,
                 callbacks=callbacks,
             )
         # it still happens
```

### Comparing `paper-qa-3.0.0.dev1/paperqa/prompts.py` & `paper-qa-3.0.0.dev2/paperqa/prompts.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,29 @@
     input_variables=["context", "answer_length", "question"],
     template="Write an answer ({answer_length}) "
     "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
     "For each part of your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
-    "Answer in an unbiased, comp rehensive, and scholarly tone. "
+    "Answer in an unbiased, comprehensive, and scholarly tone. "
     "If the question is subjective, provide an opinionated answer in the concluding 1-2 sentences. \n\n"
     "{context}\n"
     "Question: {question}\n"
     "Answer: ",
 )
 
 select_paper_prompt = PromptTemplate(
     input_variables=["question", "papers"],
-    template="Select papers to help answer the question below. "
+    template="Select papers that may help answer the question below. "
     "Papers are listed as $KEY: $PAPER_INFO. "
     "Return a list of keys, separated by commas. "
     'Return "None", if no papers are applicable. '
-    "Choose papers that are relevant, from reputable sources, and timely. \n\n"
+    "Choose papers that are relevant, from reputable sources, and timely "
+    "(if the question requires timely information). \n\n"
     "Question: {question}\n\n"
     "{papers}\n\n"
     "Selected keys:",
 )
 
 
 def _get_datetime():
```

### Comparing `paper-qa-3.0.0.dev1/paperqa/readers.py` & `paper-qa-3.0.0.dev2/paperqa/readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,16 +124,16 @@
         )
     return texts
 
 
 def read_doc(
     path: Path,
     doc: Doc,
-    chunk_chars: int,
-    overlap: int,
+    chunk_chars: int = 3000,
+    overlap: int = 100,
     force_pypdf: bool = False,
 ) -> List[Text]:
     """Parse a document into chunks."""
     str_path = str(path)
     if str_path.endswith(".pdf"):
         if force_pypdf:
             return parse_pdf(path, doc, chunk_chars, overlap)
```

### Comparing `paper-qa-3.0.0.dev1/paperqa/types.py` & `paper-qa-3.0.0.dev2/paperqa/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Callable, List, Optional, Set, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Union
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain.prompts import PromptTemplate
@@ -102,11 +102,16 @@
     context: str = ""
     contexts: List[Context] = []
     references: str = ""
     formatted_answer: str = ""
     dockey_filter: Optional[Set[DocKey]] = None
     summary_length: str = "about 100 words"
     answer_length: str = "about 100 words"
+    # these two below are for convenience
+    # and are not set. But you can set them
+    # if you want to use them.
+    cost: Optional[float] = None
+    token_counts: Optional[Dict[str, List[int]]] = None
 
     def __str__(self) -> str:
         """Return the answer as a string."""
         return self.formatted_answer
```

### Comparing `paper-qa-3.0.0.dev1/paperqa/utils.py` & `paper-qa-3.0.0.dev2/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/setup.py` & `paper-qa-3.0.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.0.0.dev1/tests/test_paperqa.py` & `paper-qa-3.0.0.dev2/tests/test_paperqa.py`

 * *Files identical despite different names*

