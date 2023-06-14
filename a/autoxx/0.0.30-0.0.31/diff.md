# Comparing `tmp/autoxx-0.0.30.tar.gz` & `tmp/autoxx-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.30.tar", max compression
+gzip compressed data, was "autoxx-0.0.31.tar", max compression
```

## Comparing `autoxx-0.0.30.tar` & `autoxx-0.0.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.30/README.md
--rw-r--r--   0        0        0     7686 2023-06-13 13:41:17.104277 autoxx-0.0.30/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3617 2023-06-13 13:39:08.524255 autoxx-0.0.30/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.30/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.30/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.30/autoxx/setup.py
--rw-r--r--   0        0        0     7659 2023-06-14 01:42:51.264483 autoxx-0.0.30/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.30/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.30/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13243 2023-06-14 02:32:00.475100 autoxx-0.0.30/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.30/autoxx/utils/base.py
--rw-r--r--   0        0        0     3198 2023-06-14 02:49:33.778554 autoxx-0.0.30/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.30/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.30/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.30/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2676 2023-06-14 03:38:54.107786 autoxx-0.0.30/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      660 2023-06-14 04:24:59.228393 autoxx-0.0.30/pyproject.toml
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 autoxx-0.0.30/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.31/README.md
+-rw-r--r--   0        0        0     7686 2023-06-13 13:41:17.104277 autoxx-0.0.31/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.31/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.31/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.31/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.31/autoxx/setup.py
+-rw-r--r--   0        0        0     7659 2023-06-14 01:42:51.264483 autoxx-0.0.31/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.31/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.31/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13243 2023-06-14 02:32:00.475100 autoxx-0.0.31/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.31/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3198 2023-06-14 02:49:33.778554 autoxx-0.0.31/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.31/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.31/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.31/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2676 2023-06-14 03:38:54.107786 autoxx-0.0.31/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      660 2023-06-14 05:34:34.729665 autoxx-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 autoxx-0.0.31/PKG-INFO
```

### Comparing `autoxx-0.0.30/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.31/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.31/autoxx/agent/babyagi/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import threading
 import queue
 from uuid import uuid4
-from typing import Dict, Optional
+from typing import List, Dict, Optional
 from autoxx.agent.babyagi.agi import AGIExecutor
   
 class TaskManager:  
     def __init__(self, max_queue_length: int = 3):
         self.tasks = {}
         self.task_queue = queue.Queue(maxsize=max_queue_length)
         self.max_queue_length = max_queue_length
@@ -76,13 +76,13 @@
 
     def get_task_stat(self, task_id: str) -> Dict:
         if task_id not in self.tasks:
             raise ValueError(f"No task found with id: {task_id}")
   
         return self.tasks[task_id].stat()
 
-    def get_task_list(self) -> Dict:
+    def get_task_list(self) -> List:
         # Return a list of tasks [{task_id,objectivbe,status}, ...]
         task_list = []
         for task_id, task_info in self.tasks.items():
             task_list.append({'id': task_id, 'objective': task_info.objective, 'status': task_info.status})
         return task_list
```

### Comparing `autoxx-0.0.30/autoxx/agent/react/agent.py` & `autoxx-0.0.31/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/config/config.py` & `autoxx-0.0.31/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.31/autoxx/tools/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.31/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/tools/web_search/search.py` & `autoxx-0.0.31/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/base.py` & `autoxx-0.0.31/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/llm.py` & `autoxx-0.0.31/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/openai_models.py` & `autoxx-0.0.31/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/processing_html.py` & `autoxx-0.0.31/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/processing_text.py` & `autoxx-0.0.31/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/autoxx/utils/token_counter.py` & `autoxx-0.0.31/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.30/pyproject.toml` & `autoxx-0.0.31/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.30"
+version = "0.0.31"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.30/PKG-INFO` & `autoxx-0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.30
+Version: 0.0.31
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

