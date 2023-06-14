# Comparing `tmp/talk_codebase-0.1.28.tar.gz` & `tmp/talk_codebase-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.28.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.29.tar", max compression
```

## Comparing `talk_codebase-0.1.28.tar` & `talk_codebase-0.1.29.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2866 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/README.md
--rw-r--r--   0        0        0      888 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/pyproject.toml
--rw-r--r--   0        0        0     4442 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/LLM.py
--rw-r--r--   0        0        0        0 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/cli.py
--rw-r--r--   0        0        0     1717 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/consts.py
--rw-r--r--   0        0        0     2474 2023-05-30 22:10:41.604071 talk_codebase-0.1.28/talk_codebase/utils.py
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 talk_codebase-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0     2866 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/README.md
+-rw-r--r--   0        0        0      896 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     4442 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/talk_codebase/LLM.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1722 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2474 2023-06-14 10:59:18.011864 talk_codebase-0.1.29/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 talk_codebase-0.1.29/PKG-INFO
```

### Comparing `talk_codebase-0.1.28/README.md` & `talk_codebase-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.28/pyproject.toml` & `talk_codebase-0.1.29/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.28"
+version = "0.1.29"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-langchain = "^0.0.181"
+python = ">=3.8.1,<4.0"
+langchain = "^0.0.200"
 fire = "^0.5.0"
 openai = "^0.27.7"
 tiktoken = "^0.4.0"
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
```

### Comparing `talk_codebase-0.1.28/talk_codebase/LLM.py` & `talk_codebase-0.1.29/talk_codebase/LLM.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.28/talk_codebase/cli.py` & `talk_codebase-0.1.29/talk_codebase/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             {"name": "OpenAI", "value": "openai"},
             {"name": "Local", "value": "local"},
         ]
     ).ask()
     config["model_type"] = model_type
     if model_type == "openai":
         api_key = input("🤖 Enter your OpenAI API key: ")
-        model_name = input("🤖 Enter your model name (default: gpt-3.5-turbo): ")
+        model_name = input(f"🤖 Enter your model name (default: {DEFAULT_CONFIG['model_name']}): ")
         config["model_name"] = model_name if model_name else DEFAULT_CONFIG["model_name"]
         config["api_key"] = api_key
     elif model_type == "local":
         model_path = input(f"🤖 Enter your model path: (default: {DEFAULT_CONFIG['model_path']}) ")
         config["model_path"] = model_path if model_path else DEFAULT_CONFIG["model_path"]
     save_config(config)
     print("🤖 Configuration saved!")
```

### Comparing `talk_codebase-0.1.28/talk_codebase/consts.py` & `talk_codebase-0.1.29/talk_codebase/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "LOCAL": "local",
 }
 DEFAULT_CONFIG = {
     "max_tokens": "1048",
     "chunk_size": "500",
     "chunk_overlap": "50",
     "k": "4",
-    "model_name": "gpt-3.5-turbo",
+    "model_name": "gpt-3.5-turbo-0613",
     "model_path": "models/ggml-gpt4all-j-v1.3-groovy.bin",
     "model_type": MODEL_TYPES["OPENAI"],
 }
 
 LOADER_MAPPING = {
     ".csv": {
         "loader": CSVLoader,
```

### Comparing `talk_codebase-0.1.28/talk_codebase/utils.py` & `talk_codebase-0.1.29/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.28/PKG-INFO` & `talk_codebase-0.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.28
+Version: 0.1.29
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: gpt4all (>=0.2.3,<0.3.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
-Requires-Dist: langchain (>=0.0.181,<0.0.182)
+Requires-Dist: langchain (>=0.0.200,<0.0.201)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: unstructured (>=0.6.10,<0.7.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
```

