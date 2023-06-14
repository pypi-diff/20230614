# Comparing `tmp/embedbase_client-0.1.9.tar.gz` & `tmp/embedbase_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.9.tar", max compression
+gzip compressed data, was "embedbase_client-0.2.0.tar", max compression
```

## Comparing `embedbase_client-0.1.9.tar` & `embedbase_client-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/README.md
--rw-r--r--   0        0        0      389 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/__init__.py
--rw-r--r--   0        0        0    19420 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/base.py
--rw-r--r--   0        0        0     1150 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/errors.py
--rw-r--r--   0        0        0     1645 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/split.py
--rw-r--r--   0        0        0    19348 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1005 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/README.md
+-rw-r--r--   0        0        0      389 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    21866 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1645 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/model.py
+-rw-r--r--   0        0        0     4525 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/split.py
+-rw-r--r--   0        0        0    21767 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3535 2023-06-14 20:09:37.326654 embedbase_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.2.0/PKG-INFO
```

### Comparing `embedbase_client-0.1.9/LICENSE` & `embedbase_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/README.md` & `embedbase_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/embedbase_client/async_client.py` & `embedbase_client-0.2.0/embedbase_client/async_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     AddDocument,
     ClientDatasets,
     Document,
     GenerateOptions,
     Metadata,
     SearchSimilarity,
 )
-from embedbase_client.split import split_text
+from embedbase_client.split import merge_and_return_tokens, split_text
 from embedbase_client.utils import CustomAsyncGenerator, async_stream
 
 
 class AsyncSearchBuilder:
     def __init__(
         self, client, dataset: str, query: str, options: Optional[Dict[str, Any]] = None
     ):
@@ -257,14 +257,34 @@
                 {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
                 {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
             ]
             results = await dataset.chunk_and_batch_add(documents)
         """
         return await self.client.chunk_and_batch_add(self.dataset, documents)
 
+    async def create_max_context(
+        self,
+        query: str,
+        max_tokens: int,
+    ) -> str:
+        """
+        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+
+        Args:
+            query: The query to search for.
+            max_tokens: The maximum number of tokens for the context.
+
+        Returns:
+            A string containing the context.
+
+        Example usage:
+            context = await dataset.create_max_context("What is Python?", max_tokens=100)
+        """
+        return await self.client.create_max_context(self.dataset, query, max_tokens)
+
 
 class EmbedbaseAsyncClient(BaseClient):
     def dataset(self, dataset: str) -> AsyncDataset:
         return AsyncDataset(client=self, dataset=dataset)
 
     async def create_context(
         self, dataset: str, query: str, limit: Optional[int] = None
@@ -552,7 +572,55 @@
             *[
                 self.batch_add(dataset, batch)
                 for batch in batch_chunks(chunks, parallel_batch_size)
             ]
         )
 
         return list(itertools.chain.from_iterable(results))
+
+    async def create_max_context(
+        self,
+        dataset: str,
+        query: str,
+        max_tokens: int,
+    ) -> str:
+        """
+        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+
+        Args:
+            dataset: The name of the dataset to search.
+            query: The query to search for.
+            max_tokens: the maximum number of tokens for the context.
+
+        Returns:
+            A string containing the context.
+
+        Example usage:
+            context = create_max_context("Python is a programming language.", max_tokens=30)
+            print(context)
+            # Python is a programming language.
+            # Python is a high-level, general-purpose programming language.
+            # Python is interpreted, dynamically typed and garbage-collected.
+            # Python is designed to be highly extensible.
+            # Python is a multi-paradig
+        """
+
+        # try to build a context until it's big enough by incrementing top_k
+        top_k = 100
+        context = await self.create_context(dataset, query, top_k)
+        merged_context, size = merge_and_return_tokens(context, max_tokens)
+
+        tries = 0
+        max_tries = 3
+        while size < max_tokens and tries < max_tries:
+            top_k *= 3
+            context = await self.create_context(dataset, query, top_k)
+            merged_context, size = merge_and_return_tokens(context, max_tokens)
+            tries += 1
+
+        if size < max_tokens:
+            # warn the user that the context is smaller than the max tokens
+            print(
+                f"Warning: context is smaller than the max tokens ({size} < {max_tokens})"
+            )
+
+        return merged_context
```

### Comparing `embedbase_client-0.1.9/embedbase_client/base.py` & `embedbase_client-0.2.0/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/embedbase_client/errors.py` & `embedbase_client-0.2.0/embedbase_client/errors.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/embedbase_client/model.py` & `embedbase_client-0.2.0/embedbase_client/model.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/embedbase_client/split.py` & `embedbase_client-0.2.0/embedbase_client/split.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from tiktoken import get_encoding
 
 MAX_CHUNK_LENGTH = 8191
 EMBEDDING_ENCODING = "cl100k_base"
 CHUNK_OVERLAP = 0
 
@@ -102,7 +102,44 @@
             break
         context.append(chunk)
 
     if separator is None:
         separator = "\n\n###\n\n"
 
     return separator.join(context)
+
+
+def merge_and_return_tokens(
+    chunks: List[str],
+    max_len: int,
+    encoding_name: str = EMBEDDING_ENCODING,
+) -> Tuple[str, int]:
+    """
+    This function takes a list of `chunks` and optional parameters `max_len`, `encoding_name`, and `separator`.
+    It encodes each chunk using the specified tokenizer, checks if the current length exceeds the `max_len`,
+    breaks if it does, and appends the chunk to the `context` list.
+    Finally, it joins the context list and returns the merged string.
+
+    For example,
+    ```python
+    chunks = ['Hello', 'world', '!']
+    merge_and_return_tokens(chunks, max_len=10)
+    ```
+    will return
+    ```
+    'Hello world!', 12
+    """
+    tokenizer = get_encoding(encoding_name)
+
+    cur_len = 0
+    context = []
+    for chunk in chunks:
+        n_tokens = len(tokenizer.encode(chunk))
+        if cur_len + n_tokens + ((len(context) - 1) * 4) > max_len:
+            break
+        cur_len += n_tokens
+        context.append(chunk)
+
+    separator = "\n\n"
+
+    # length is tokens + 4 tokens for each separator
+    return separator.join(context), cur_len + ((len(context) - 1) * 4)
```

### Comparing `embedbase_client-0.1.9/embedbase_client/sync_client.py` & `embedbase_client-0.2.0/embedbase_client/sync_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     AddDocument,
     ClientDatasets,
     Document,
     GenerateOptions,
     Metadata,
     SearchSimilarity,
 )
-from embedbase_client.split import split_text
+from embedbase_client.split import merge_and_return_tokens, split_text
 from embedbase_client.utils import sync_stream
 
 
 class SyncSearchBuilder:
     def __init__(
         self,
         client: BaseClient,
@@ -256,14 +256,34 @@
                 {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
                 {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
             ]
             results = dataset.chunk_and_batch_add(documents)
         """
         return self.client.chunk_and_batch_add(self.dataset, documents)
 
+    def create_max_context(
+        self,
+        query: str,
+        max_tokens: int,
+    ) -> str:
+        """
+        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+
+        Args:
+            query: The query to search for.
+            max_tokens: The maximum number of tokens for the context.
+
+        Returns:
+            A string containing the context.
+
+        Example usage:
+            context = dataset.create_max_context("What is Python?", max_tokens=100)
+        """
+        return self.client.create_max_context(self.dataset, query, max_tokens)
+
 
 class EmbedbaseClient(BaseClient):
     def __init__(
         self,
         embedbase_url: str = "https://api.embedbase.xyz",
         embedbase_key: Optional[str] = None,
         fastapi_app: Optional[Any] = None,
@@ -573,7 +593,55 @@
         def add_batch(batch):
             results.append(self.batch_add(dataset, batch))
 
         with ThreadPool() as pool:
             pool.map(add_batch, batch_chunks(chunks, parallel_batch_size))
 
         return list(itertools.chain.from_iterable(results))
+
+    def create_max_context(
+        self,
+        dataset: str,
+        query: str,
+        max_tokens: int,
+    ) -> str:
+        """
+        Create a context from a query by searching for similar documents and concatenating them up to the specified max tokens.
+
+        Args:
+            dataset: The name of the dataset to search.
+            query: The query to search for.
+            max_tokens: the maximum number of tokens for the context.
+
+        Returns:
+            A string containing the context.
+
+        Example usage:
+            context = embedbase.create_max_context("my_dataset", "What is Python?", max_tokens=30)
+            print(context)
+            # Python is a programming language.
+            # Python is a high-level, general-purpose programming language.
+            # Python is interpreted, dynamically typed and garbage-collected.
+            # Python is designed to be highly extensible.
+            # Python is a multi-paradig...
+        """
+
+        # try to build a context until it's big enough by incrementing top_k
+        top_k = 100
+        context = self.create_context(dataset, query, top_k)
+        merged_context, size = merge_and_return_tokens(context, max_tokens)
+
+        tries = 0
+        max_tries = 3
+        while size < max_tokens and tries < max_tries:
+            top_k *= 3
+            context = self.create_context(dataset, query, top_k)
+            merged_context, size = merge_and_return_tokens(context, max_tokens)
+            tries += 1
+
+        if size < max_tokens:
+            # warn the user that the context is smaller than the max tokens
+            print(
+                f"Warning: context is smaller than the max tokens ({size} < {max_tokens})"
+            )
+
+        return merged_context
```

### Comparing `embedbase_client-0.1.9/embedbase_client/utils.py` & `embedbase_client-0.2.0/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.9/pyproject.toml` & `embedbase_client-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.9"
+version = "0.2.0"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
```

### Comparing `embedbase_client-0.1.9/PKG-INFO` & `embedbase_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.9 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.2.0 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

