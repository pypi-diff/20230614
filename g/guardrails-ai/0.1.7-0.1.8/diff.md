# Comparing `tmp/guardrails-ai-0.1.7.tar.gz` & `tmp/guardrails-ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-ai-0.1.7.tar", last modified: Fri May 12 08:28:13 2023, max compression
+gzip compressed data, was "guardrails-ai-0.1.8.tar", last modified: Wed Jun 14 10:50:01 2023, max compression
```

## Comparing `guardrails-ai-0.1.7.tar` & `guardrails-ai-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.544013 guardrails-ai-0.1.7/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    11357 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/LICENSE
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      165 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/MANIFEST.in
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-05-12 08:28:13.543745 guardrails-ai-0.1.7/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7902 2023-05-12 07:21:55.000000 guardrails-ai-0.1.7/README.md
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.539687 guardrails-ai-0.1.7/guardrails/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      629 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/__init__.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.540119 guardrails-ai-0.1.7/guardrails/applications/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/applications/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6588 2023-05-12 07:21:55.000000 guardrails-ai-0.1.7/guardrails/applications/text2sql.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      778 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/applications/text2sql.rail
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1613 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/cli.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4694 2023-05-11 04:10:25.000000 guardrails-ai-0.1.7/guardrails/constants.xml
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    16775 2023-05-09 07:33:45.000000 guardrails-ai-0.1.7/guardrails/datatypes.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7361 2023-05-01 23:36:17.000000 guardrails-ai-0.1.7/guardrails/document_store.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6331 2023-05-09 04:21:53.000000 guardrails-ai-0.1.7/guardrails/embedding.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6816 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/guard.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4794 2023-05-09 04:21:53.000000 guardrails-ai-0.1.7/guardrails/llm_providers.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      295 2023-05-11 20:22:21.000000 guardrails-ai-0.1.7/guardrails/logging_utils.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.540934 guardrails-ai-0.1.7/guardrails/prompt/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      115 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/prompt/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3260 2023-05-09 04:21:49.000000 guardrails-ai-0.1.7/guardrails/prompt/base_prompt.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1279 2023-05-01 23:36:17.000000 guardrails-ai-0.1.7/guardrails/prompt/instructions.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      796 2023-05-09 03:35:20.000000 guardrails-ai-0.1.7/guardrails/prompt/prompt.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7373 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/rail.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    11145 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/run.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    18951 2023-05-08 17:19:07.000000 guardrails-ai-0.1.7/guardrails/schema.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.542219 guardrails-ai-0.1.7/guardrails/utils/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/utils/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1555 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/utils/constants.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2530 2023-04-27 15:53:00.000000 guardrails-ai-0.1.7/guardrails/utils/docs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6145 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/utils/logs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2567 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/utils/misc.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3349 2023-05-01 23:36:17.000000 guardrails-ai-0.1.7/guardrails/utils/pydantic_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8944 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/guardrails/utils/reask_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4030 2023-05-01 23:36:17.000000 guardrails-ai-0.1.7/guardrails/utils/sql_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    46681 2023-05-11 04:10:25.000000 guardrails-ai-0.1.7/guardrails/validators.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.542611 guardrails-ai-0.1.7/guardrails/vectordb/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       93 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/vectordb/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2953 2023-05-01 23:36:17.000000 guardrails-ai-0.1.7/guardrails/vectordb/base.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3244 2023-04-26 06:16:51.000000 guardrails-ai-0.1.7/guardrails/vectordb/faiss.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       22 2023-05-12 08:28:04.000000 guardrails-ai-0.1.7/guardrails/version.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-05-12 08:28:13.543399 guardrails-ai-0.1.7/guardrails_ai.egg-info/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1153 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/SOURCES.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        1 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/dependency_links.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       50 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/entry_points.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      550 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/requires.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       11 2023-05-12 08:28:13.000000 guardrails-ai-0.1.7/guardrails_ai.egg-info/top_level.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       38 2023-05-12 08:28:13.544063 guardrails-ai-0.1.7/setup.cfg
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4715 2023-05-05 04:48:05.000000 guardrails-ai-0.1.7/setup.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.662508 guardrails-ai-0.1.8/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    11357 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/LICENSE
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      165 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/MANIFEST.in
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-06-14 10:50:01.662299 guardrails-ai-0.1.8/PKG-INFO
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7902 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/README.md
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.657662 guardrails-ai-0.1.8/guardrails/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      629 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/__init__.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.658060 guardrails-ai-0.1.8/guardrails/applications/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/applications/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6588 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/applications/text2sql.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      778 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/applications/text2sql.rail
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1613 2023-05-19 21:55:45.000000 guardrails-ai-0.1.8/guardrails/cli.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4966 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/constants.xml
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    16754 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/datatypes.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7352 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/document_store.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6331 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/embedding.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7502 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/guard.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     5592 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/llm_providers.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      295 2023-05-19 22:08:29.000000 guardrails-ai-0.1.8/guardrails/logging_utils.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.658547 guardrails-ai-0.1.8/guardrails/prompt/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      115 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/prompt/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     3260 2023-06-06 19:33:09.000000 guardrails-ai-0.1.8/guardrails/prompt/base_prompt.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1279 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/prompt/instructions.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      796 2023-05-09 03:35:20.000000 guardrails-ai-0.1.8/guardrails/prompt/prompt.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8741 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/rail.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    11536 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/run.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    28902 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/schema.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.660814 guardrails-ai-0.1.8/guardrails/utils/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/utils/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1555 2023-06-08 19:52:05.000000 guardrails-ai-0.1.8/guardrails/utils/constants.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2530 2023-04-27 15:53:00.000000 guardrails-ai-0.1.8/guardrails/utils/docs_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6217 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/logs_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2567 2023-06-14 07:06:12.000000 guardrails-ai-0.1.8/guardrails/utils/misc.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    16550 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/pydantic_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7050 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/reask_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4018 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/utils/sql_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    48218 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/validators.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.661307 guardrails-ai-0.1.8/guardrails/vectordb/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       93 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/vectordb/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2956 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/guardrails/vectordb/base.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     3244 2023-04-26 06:16:51.000000 guardrails-ai-0.1.8/guardrails/vectordb/faiss.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       22 2023-06-14 10:49:41.000000 guardrails-ai-0.1.8/guardrails/version.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-06-14 10:50:01.662033 guardrails-ai-0.1.8/guardrails_ai.egg-info/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8607 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/PKG-INFO
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1153 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        1 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       50 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/entry_points.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      557 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/requires.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       11 2023-06-14 10:50:01.000000 guardrails-ai-0.1.8/guardrails_ai.egg-info/top_level.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       38 2023-06-14 10:50:01.662554 guardrails-ai-0.1.8/setup.cfg
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4722 2023-06-14 10:09:13.000000 guardrails-ai-0.1.8/setup.py
```

### Comparing `guardrails-ai-0.1.7/LICENSE` & `guardrails-ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/PKG-INFO` & `guardrails-ai-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `guardrails-ai-0.1.7/README.md` & `guardrails-ai-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/__init__.py` & `guardrails-ai-0.1.8/guardrails/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/applications/text2sql.py` & `guardrails-ai-0.1.8/guardrails/applications/text2sql.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/applications/text2sql.rail` & `guardrails-ai-0.1.8/guardrails/applications/text2sql.rail`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/cli.py` & `guardrails-ai-0.1.8/guardrails/cli.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/constants.xml` & `guardrails-ai-0.1.8/guardrails/constants.xml`

 * *Files 7% similar despite different names*

#### Comparing `guardrails-ai-0.1.7/guardrails/constants.xml` & `guardrails-ai-0.1.8/guardrails/constants.xml`

```diff
@@ -1,24 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <constants>
   <json_suffix_prompt>Return a valid JSON object that respects this XML format and extracts only the information requested in this document. Respect the types indicated in the XML -- the information you extract should be converted into the correct 'type'. Try to be as correct and concise as possible. Find all relevant information in the document. If you are unsure of the answer, enter 'None'. If you answer incorrectly, you will be asked again until you get it right which is expensive.</json_suffix_prompt>
   <xml_prefix_prompt>Given below is XML that describes the information to extract from this document and the tags to extract it into.</xml_prefix_prompt>
   <json_suffix_prompt_v2>ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter &quot;None&quot;.</json_suffix_prompt_v2>
   <json_suffix_prompt_v2_wo_none>ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise.</json_suffix_prompt_v2_wo_none>
-  <high_level_reask_prompt>I was given the following JSON response, which had problems due to incorrect values.
+  <high_level_json_reask_prompt>I was given the following JSON response, which had problems due to incorrect values.
 
 {previous_response}
 
-Help me correct the incorrect values based on the given error messages.</high_level_reask_prompt>
+Help me correct the incorrect values based on the given error messages.</high_level_json_reask_prompt>
   <complete_json_suffix>
     Given below is XML that describes the information to extract from this document and the tags to extract it into.
 
 {output_schema}
 
-ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `None`.
+ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `null`.
 
 Here are examples of simple (XML, JSON) pairs that show the expected behavior:
 - `
 <![CDATA[<string name='foo' format='two-words lower-case' />`]]>    =&gt; `{{{{'foo': 'example one'}}}}`
 - `
 <![CDATA[<list name='bar'><string format='upper-case' /></list>]]>    ` =&gt; `{{{{&quot;bar&quot;: ['STRING ONE', 'STRING TWO', etc.]}}}}`
 - `
@@ -36,18 +36,27 @@
 <![CDATA[<string name='foo' format='two-words lower-case' />`]]>    =&gt; `{{{{'foo': 'example one'}}}}`
 - `
 <![CDATA[<list name='bar'><string format='upper-case' /></list>]]>    ` =&gt; `{{{{&quot;bar&quot;: ['STRING ONE', 'STRING TWO', etc.]}}}}`
 - `
 <![CDATA[<object name='baz'><string name="foo" format="capitalize two-words" /><integer name="index" format="1-indexed" /></object>]]>    ` =&gt; `{{{{'baz': {{{{'foo': 'Some String', 'index': 1}}}}}}}}`
   </complete_json_suffix_v2>
   <json_suffix_prompt_examples>
-    ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `None`.
+    ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `null`.
 
 Here are examples of simple (XML, JSON) pairs that show the expected behavior:
 - `
 <![CDATA[<string name='foo' format='two-words lower-case' />`]]>    =&gt; `{{{{'foo': 'example one'}}}}`
 - `
 <![CDATA[<list name='bar'><string format='upper-case' /></list>]]>    ` =&gt; `{{{{&quot;bar&quot;: ['STRING ONE', 'STRING TWO', etc.]}}}}`
 - `
 <![CDATA[<object name='baz'><string name="foo" format="capitalize two-words" /><integer name="index" format="1-indexed" /></object>]]>    ` =&gt; `{{{{'baz': {{{{'foo': 'Some String', 'index': 1}}}}}}}}`
   </json_suffix_prompt_examples>
+  <high_level_string_reask_prompt>I was given the following string, delimited by +++:
+
++++
+{previous_response}
++++
+
+It had the following problems:
+{error_messages}</high_level_string_reask_prompt>
+  <complete_string_suffix>{output_schema}</complete_string_suffix>
 </constants>
```

### Comparing `guardrails-ai-0.1.7/guardrails/datatypes.py` & `guardrails-ai-0.1.8/guardrails/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import datetime
 from types import SimpleNamespace
-from typing import TYPE_CHECKING, Any, Dict, Generator, List, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Generator
+from typing import List as TypedList
+from typing import Tuple, Type, Union
 
 from lxml import etree as ET
 from pydantic import BaseModel
 
 if TYPE_CHECKING:
     from guardrails.schema import FormatAttr
 
@@ -17,15 +19,15 @@
         element: ET._Element,
     ) -> None:
         self._children = children
         self.format_attr = format_attr
         self.element = element
 
     @property
-    def validators(self) -> List:
+    def validators(self) -> TypedList:
         return self.format_attr.validators
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._children})"
 
     def __iter__(self) -> Generator[Tuple[str, "DataType", ET._Element], None, None]:
         """Return a tuple of (name, child_data_type, child_element) for each
@@ -38,18 +40,18 @@
             else:
                 assert len(self._children) == 1, "Must have exactly one child."
                 yield None, list(self._children.values())[0], el_child
 
     def iter(
         self, element: ET._Element
     ) -> Generator[Tuple[str, "DataType", ET._Element], None, None]:
-        """
-        Iterate over the children of an element.
+        """Iterate over the children of an element.
 
-        Yields tuples of (name, child_data_type, child_element) for each child.
+        Yields tuples of (name, child_data_type, child_element) for each
+        child.
         """
         for el_child in element:
             if element.tag == "list":
                 assert len(self._children) == 1, "Must have exactly one child."
                 yield None, list(self._children.values())[0], el_child
             else:
                 name: str = el_child.attrib["name"]
@@ -171,16 +173,16 @@
             raise ValueError(f"Invalid boolean value: {s}")
 
 
 @register_type("date")
 class Date(ScalarType):
     """Element tag: `<date>`
 
-    To configure the date format, create a date-format attribute on the element.
-    E.g. `<date name="..." ... date-format="%Y-%m-%d" />`
+    To configure the date format, create a date-format attribute on the
+    element. E.g. `<date name="..." ... date-format="%Y-%m-%d" />`
     """
 
     def __init__(
         self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
     ) -> None:
         self.date_format = "%Y-%m-%d"
         super().__init__(children, format_attr, element)
@@ -202,16 +204,16 @@
         return datatype
 
 
 @register_type("time")
 class Time(ScalarType):
     """Element tag: `<time>`
 
-    To configure the date format, create a date-format attribute on the element.
-    E.g. `<time name="..." ... time-format="%H:%M:%S" />`
+    To configure the date format, create a date-format attribute on the
+    element. E.g. `<time name="..." ... time-format="%H:%M:%S" />`
     """
 
     def __init__(
         self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
     ) -> None:
         self.time_format = "%H:%M:%S"
         super().__init__(children, format_attr, element)
@@ -354,15 +356,15 @@
     def set_children(self, element: ET._Element):
         for child in element:
             child_data_type = registry[child.tag]
             assert child_data_type == Case
             self._children[child.attrib["name"]] = child_data_type.from_xml(child)
 
     @property
-    def validators(self) -> List:
+    def validators(self) -> TypedList:
         from guardrails.validators import Choice as ChoiceValidator
 
         # Check if the <choice ... /> element has an `on-fail` attribute.
         # If so, use that as the `on_fail` argument for the PydanticValidator.
         on_fail = None
         on_fail_attr_name = "on-fail-choice"
         if on_fail_attr_name in self.element.attrib:
@@ -413,15 +415,15 @@
         assert isinstance(model, type) and issubclass(
             model, BaseModel
         ), "The `model` argument must be a Pydantic model."
 
         self.model = model
 
     @property
-    def validators(self) -> List:
+    def validators(self) -> TypedList:
         from guardrails.validators import Pydantic as PydanticValidator
 
         # Check if the <pydantic /> element has an `on-fail` attribute.
         # If so, use that as the `on_fail` argument for the PydanticValidator.
         on_fail = None
         on_fail_attr_name = "on-fail-pydantic"
         if on_fail_attr_name in self.element.attrib:
@@ -515,19 +517,14 @@
 
         # Convert the string to an XML element, making sure to format it.
         return ET.fromstring(
             xml, parser=ET.XMLParser(encoding="utf-8", remove_blank_text=True)
         )
 
 
-@register_type("field")
-class Field(ScalarType):
-    """Element tag: `<field>`"""
-
-
 # @register_type("key")
 # class Key(DataType):
 # """
 # Element tag: `<string>`
 # """
```

### Comparing `guardrails-ai-0.1.7/guardrails/document_store.py` & `guardrails-ai-0.1.8/guardrails/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
     orm = None
 
 
 @dataclass
 class Document:
     """Document holds text and metadata of a document.
 
-    Examples of documents are PDFs, Word documents, etc. A collection of related text
-    in an NLP application can be thought of a document as well.
+    Examples of documents are PDFs, Word documents, etc. A collection of
+    related text in an NLP application can be thought of a document as
+    well.
     """
 
     id: str
     pages: Dict[int, str]
     metadata: Dict[Any, Any] = None
 
 
@@ -32,24 +33,25 @@
 PageCoordinates = namedtuple("PageCoordinates", ["doc_id", "page_num"])
 
 
 @dataclass
 class Page:
     """Page holds text and metadata of a page in a document.
 
-    It also containts the coordinates of the page in the document."""
+    It also containts the coordinates of the page in the document.
+    """
 
     cordinates: PageCoordinates
     text: str
     metadata: Dict[Any, Any]
 
 
 class DocumentStoreBase(ABC):
-    """
-    Abstract class for a store that can store text, and metadata from documents.
+    """Abstract class for a store that can store text, and metadata from
+    documents.
 
     The store can be queried by text for similar documents.
     """
 
     @abstractmethod
     def add_document(self, document: Document):
         """Adds a document to the store.
@@ -60,16 +62,15 @@
         Returns:
             None if the document was added successfully
         """
         ...
 
     @abstractmethod
     def search(self, query: str, k: int = 4) -> List[Page]:
-        """Searches for pages which contain the text similar to
-        the query.
+        """Searches for pages which contain the text similar to the query.
 
         Args:
             query: Text to search for.
             k: Number of similar pages to return.
 
         Returns:
             List[Pages] List of pages which contains similar texts
@@ -102,18 +103,16 @@
     @abstractmethod
     def flush():
         """Flushes the store to disk."""
         ...
 
 
 class EphemeralDocumentStore(DocumentStoreBase):
-    """
-    EphemeralDocumentStore is a document store that stores the documents on
-    local disk and use a ephemeral vector store like Faiss
-    """
+    """EphemeralDocumentStore is a document store that stores the documents on
+    local disk and use a ephemeral vector store like Faiss."""
 
     def __init__(self, vector_db: VectorDBBase, path: Optional[str] = None):
         """Creates a new EphemeralDocumentStore.
 
         Args:
             vector_db: VectorDBBase instance to use for storing the vectors.
             path: Path to the database file store metadata.
```

### Comparing `guardrails-ai-0.1.7/guardrails/embedding.py` & `guardrails-ai-0.1.8/guardrails/embedding.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/guard.py` & `guardrails-ai-0.1.8/guardrails/guard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from string import Formatter
 from typing import Callable, Dict, Optional, Tuple, Union
 
 from eliot import add_destinations, start_action
+from pydantic import BaseModel
 
 from guardrails.llm_providers import PromptCallable, get_llm_ask
 from guardrails.prompt import Instructions, Prompt
 from guardrails.rail import Rail
 from guardrails.run import Runner
-from guardrails.schema import InputSchema, OutputSchema
+from guardrails.schema import Schema
 from guardrails.utils.logs_utils import GuardState
 from guardrails.utils.reask_utils import sub_reasks_with_fixed_values
 
 logger = logging.getLogger(__name__)
 actions_logger = logging.getLogger(f"{__name__}.actions")
 add_destinations(actions_logger.debug)
 
@@ -28,28 +29,30 @@
     the LLM and the validated output.
     """
 
     def __init__(
         self,
         rail: Rail,
         num_reasks: int = 1,
+        base_model: Optional[BaseModel] = None,
     ):
         """Initialize the Guard."""
         self.rail = rail
         self.num_reasks = num_reasks
         self.guard_state = GuardState([])
         self._reask_prompt = None
+        self.base_model = base_model
 
     @property
-    def input_schema(self) -> InputSchema:
+    def input_schema(self) -> Schema:
         """Return the input schema."""
         return self.rail.input_schema
 
     @property
-    def output_schema(self) -> OutputSchema:
+    def output_schema(self) -> Schema:
         """Return the output schema."""
         return self.rail.output_schema
 
     @property
     def instructions(self) -> Instructions:
         """Return the instruction-prompt."""
         return self.rail.instructions
@@ -127,44 +130,63 @@
             num_reasks: The max times to re-ask the LLM for invalid output.
 
         Returns:
             An instance of the `Guard` class.
         """
         return cls(Rail.from_string(rail_string), num_reasks=num_reasks)
 
+    @classmethod
+    def from_pydantic(
+        cls,
+        output_class: BaseModel,
+        prompt: str,
+        instructions: Optional[str] = None,
+        num_reasks: int = 1,
+    ) -> "Guard":
+        """Create a Guard instance from a Pydantic model and prompt."""
+        rail = Rail.from_pydantic(
+            output_class=output_class, prompt=prompt, instructions=instructions
+        )
+        return cls(rail, num_reasks=num_reasks, base_model=output_class)
+
     def __call__(
         self,
         llm_api: Callable,
         prompt_params: Dict = None,
-        num_reasks: int = 1,
+        num_reasks: Optional[int] = None,
         *args,
         **kwargs,
     ) -> Tuple[str, Dict]:
         """Call the LLM and validate the output.
 
         Args:
             llm_api: The LLM API to call (e.g. openai.Completion.create)
             prompt_params: The parameters to pass to the prompt.format() method.
             num_reasks: The max times to re-ask the LLM for invalid output.
 
         Returns:
             The raw text output from the LLM and the validated output.
         """
+
+        if num_reasks is None:
+            num_reasks = self.num_reasks
+
         with start_action(action_type="guard_call", prompt_params=prompt_params):
             if "instructions" in kwargs:
                 logger.info("Instructions overridden at call time")
                 # TODO(shreya): should we overwrite self.instructions for this run?
             runner = Runner(
                 instructions=kwargs.get("instructions", self.instructions),
                 prompt=self.prompt,
                 api=get_llm_ask(llm_api, *args, **kwargs),
                 input_schema=self.input_schema,
                 output_schema=self.output_schema,
                 num_reasks=num_reasks,
                 reask_prompt=self.reask_prompt,
+                base_model=self.base_model,
             )
             guard_history = runner(prompt_params=prompt_params)
             self.guard_state = self.guard_state.push(guard_history)
             return guard_history.output, guard_history.validated_output
 
     def __repr__(self):
         return f"Guard(RAIL={self.rail})"
```

### Comparing `guardrails-ai-0.1.7/guardrails/llm_providers.py` & `guardrails-ai-0.1.8/guardrails/llm_providers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from dataclasses import dataclass
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, cast
 
 import openai
+from pydantic import BaseModel
 from tenacity import retry, retry_if_exception_type, wait_exponential_jitter
 
 try:
     MANIFEST = True
     import manifest
 except ImportError:
     MANIFEST = False
@@ -64,27 +65,23 @@
 
 
 def nonchat_prompt(prompt: str, instructions: Optional[str] = None, **kwargs) -> str:
     """Prepare final prompt for nonchat engine."""
     if instructions:
         prompt = "\n\n".join([instructions, prompt])
 
-    return prompt + "\n\nJson Output:\n\n"
+    return prompt
 
 
 def chat_prompt(
     prompt: str, instructions: Optional[str] = None, **kwargs
 ) -> List[Dict[str, str]]:
     """Prepare final prompt for chat engine."""
     if not instructions:
-        instructions = (
-            "You are a helpful assistant, "
-            "able to express yourself purely through JSON, "
-            "strictly and precisely adhering to the provided XML schemas."
-        )
+        instructions = "You are a helpful assistant."
     return [
         {"role": "system", "content": instructions},
         {"role": "user", "content": prompt},
     ]
 
 
 def openai_wrapper(
@@ -105,26 +102,52 @@
     return openai_response["choices"][0]["text"]
 
 
 def openai_chat_wrapper(
     text: str,
     model="gpt-3.5-turbo",
     instructions: Optional[str] = None,
+    base_model: Optional[BaseModel] = None,
     *args,
     **kwargs,
 ):
+
+    if base_model:
+        base_model_schema = base_model.schema()
+        function_params = {
+            "name": base_model_schema["title"],
+            "description": base_model_schema["description"]
+            if "description" in base_model_schema
+            else None,
+            "parameters": base_model_schema,
+        }
+
     api_key = os.environ.get("OPENAI_API_KEY")
-    openai_response = openai.ChatCompletion.create(
-        api_key=api_key,
-        model=model,
-        messages=chat_prompt(text, instructions, **kwargs),
-        *args,
-        **kwargs,
-    )
-    return openai_response["choices"][0]["message"]["content"]
+
+    # TODO: update this as new models are released
+    if base_model and model in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
+        openai_response = openai.ChatCompletion.create(
+            api_key=api_key,
+            model=model,
+            messages=chat_prompt(text, instructions, **kwargs),
+            functions=[function_params],
+            function_call={"name": function_params["name"]},
+            *args,
+            **kwargs,
+        )
+        return openai_response["choices"][0]["message"]["function_call"]["arguments"]
+    else:
+        openai_response = openai.ChatCompletion.create(
+            api_key=api_key,
+            model=model,
+            messages=chat_prompt(text, instructions, **kwargs),
+            *args,
+            **kwargs,
+        )
+        return openai_response["choices"][0]["message"]["content"]
 
 
 def manifest_wrapper(
     text: str, client: Any, instructions: Optional[str] = None, *args, **kwargs
 ):
     """Wrapper for manifest client.
```

### Comparing `guardrails-ai-0.1.7/guardrails/prompt/base_prompt.py` & `guardrails-ai-0.1.8/guardrails/prompt/base_prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/prompt/instructions.py` & `guardrails-ai-0.1.8/guardrails/prompt/instructions.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from .base_prompt import BasePrompt
 
 
 class Instructions(BasePrompt):
     """Instructions class.
 
-    The instructions are passed to the LLM as secondary input.
-    Different model may use these differently. For example, chat models may receive
-    instructions in the system-prompt.
+    The instructions are passed to the LLM as secondary input. Different
+    model may use these differently. For example, chat models may
+    receive instructions in the system-prompt.
     """
 
     def __repr__(self) -> str:
         # Truncate the prompt to 50 characters and add ellipsis if it's longer.
         truncated_instructions = self.source[:50]
         if len(self.source) > 50:
             truncated_instructions += "..."
```

### Comparing `guardrails-ai-0.1.7/guardrails/prompt/prompt.py` & `guardrails-ai-0.1.8/guardrails/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/rail.py` & `guardrails-ai-0.1.8/guardrails/rail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Rail class."""
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import List, Optional, Type
 
 from lxml import etree as ET
+from lxml.etree import Element, SubElement
+from pydantic import BaseModel
 
 from guardrails.prompt import Instructions, Prompt
-from guardrails.schema import InputSchema, OutputSchema, Schema
+from guardrails.schema import JsonSchema, Schema, StringSchema
+from guardrails.utils.pydantic_utils import create_xml_element_for_base_model
 
 # TODO: Logging
 XMLPARSER = ET.XMLParser(encoding="utf-8")
 
 
 @dataclass
 class Script:
@@ -86,22 +89,29 @@
     that contains the following elements as children:
         1. `<script language="python">`, which contains the script to be executed
         2. `<input strict=True/False>`, which contains the input schema
         3. `<output strict=True/False>`, which contains the output schema
         4. `<prompt>`, which contains the prompt to be passed to the LLM
     """
 
-    input_schema: Optional[InputSchema] = (None,)
-    output_schema: Optional[OutputSchema] = (None,)
+    input_schema: Optional[Schema] = (None,)
+    output_schema: Optional[Schema] = (None,)
     instructions: Optional[Instructions] = (None,)
     prompt: Optional[Prompt] = (None,)
     script: Optional[Script] = (None,)
     version: Optional[str] = ("0.1",)
 
     @classmethod
+    def from_pydantic(
+        cls, output_class: BaseModel, prompt: str, instructions: Optional[str] = None
+    ):
+        xml = generate_xml_code(output_class, prompt, instructions)
+        return cls.from_xml(xml)
+
+    @classmethod
     def from_file(cls, file_path: str) -> "Rail":
         with open(file_path, "r") as f:
             xml = f.read()
         return cls.from_string(xml)
 
     @classmethod
     def from_string(cls, string: str) -> "Rail":
@@ -122,27 +132,26 @@
         else:
             script = Script()
 
         # Load <input /> schema
         raw_input_schema = xml.find("input")
         if raw_input_schema is None:
             # No input schema, so do no input checking.
-            input_schema = InputSchema()
+            input_schema = Schema()
         else:
             input_schema = cls.load_input_schema(raw_input_schema)
 
         # Load <output /> schema
         raw_output_schema = xml.find("output")
         if raw_output_schema is None:
             raise ValueError("RAIL file must contain a output-schema element.")
         # Replace all expressions in the <output /> schema.
         raw_output_schema = script.replace_expressions(ET.tostring(raw_output_schema))
         raw_output_schema = ET.fromstring(raw_output_schema, parser=XMLPARSER)
         output_schema = cls.load_output_schema(raw_output_schema)
-
         # Parse instructions for the LLM. These are optional but if given,
         # LLMs can use them to improve their output. Commonly these are
         # prepended to the prompt.
         instructions = xml.find("instructions")
         if instructions is not None:
             instructions = cls.load_instructions(instructions, output_schema)
 
@@ -164,40 +173,71 @@
     @staticmethod
     def load_schema(root: ET._Element) -> Schema:
         """Given the RAIL <input> or <output> element, create a Schema
         object."""
         return Schema(root)
 
     @staticmethod
-    def load_input_schema(root: ET._Element) -> InputSchema:
+    def load_input_schema(root: ET._Element) -> Schema:
         """Given the RAIL <input> element, create a Schema object."""
         # Recast the schema as an InputSchema.
-        return InputSchema(root)
+        return Schema(root)
 
     @staticmethod
-    def load_output_schema(root: ET._Element) -> OutputSchema:
+    def load_output_schema(root: ET._Element) -> Schema:
         """Given the RAIL <output> element, create a Schema object."""
-        # Recast the schema as an OutputSchema.
-        return OutputSchema(root)
+        # If root contains a `type="string"` attribute, then it's a StringSchema
+        if "type" in root.attrib and root.attrib["type"] == "string":
+            return StringSchema(root)
+        return JsonSchema(root)
 
     @staticmethod
-    def load_instructions(
-        root: ET._Element, output_schema: OutputSchema
-    ) -> Instructions:
+    def load_instructions(root: ET._Element, output_schema: Schema) -> Instructions:
         """Given the RAIL <instructions> element, create Instructions."""
         return Instructions(
             source=root.text,
             output_schema=output_schema.transpile(),
         )
 
     @staticmethod
-    def load_prompt(root: ET._Element, output_schema: OutputSchema) -> Prompt:
+    def load_prompt(root: ET._Element, output_schema: Schema) -> Prompt:
         """Given the RAIL <prompt> element, create a Prompt object."""
         return Prompt(
             source=root.text,
             output_schema=output_schema.transpile(),
         )
 
     @staticmethod
     def load_script(root: ET._Element) -> Script:
         """Given the RAIL <script> element, load and execute the script."""
         return Script.from_xml(root)
+
+
+def generate_xml_code(
+    output_class: Type[BaseModel],
+    prompt: str,
+    instructions: Optional[str] = None,
+) -> ET._Element:
+    """Generate XML RAIL Spec from a pydantic model and a prompt."""
+
+    # Create the root element
+    root = Element("rail")
+    root.set("version", "0.1")
+
+    # Create the output element
+    output_element = SubElement(root, "output")
+
+    # Create XML elements for the output_class
+    create_xml_element_for_base_model(output_class, output_element)
+
+    # Create the prompt element
+    prompt_element = SubElement(root, "prompt")
+    prompt_text = f"{prompt}"
+    prompt_element.text = prompt_text
+
+    if instructions is not None:
+        # Create the instructions element
+        instructions_element = SubElement(root, "instructions")
+        instructions_text = f"{instructions}"
+        instructions_element.text = instructions_text
+
+    return root
```

### Comparing `guardrails-ai-0.1.7/guardrails/run.py` & `guardrails-ai-0.1.8/guardrails/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-import json
 import logging
 from dataclasses import dataclass, field
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from eliot import add_destinations, start_action
+from pydantic import BaseModel
 
 from guardrails.llm_providers import PromptCallable
 from guardrails.prompt import Instructions, Prompt
-from guardrails.schema import InputSchema, OutputSchema
+from guardrails.schema import Schema
 from guardrails.utils.logs_utils import GuardHistory, GuardLogs
 from guardrails.utils.reask_utils import (
     ReAsk,
-    gather_reasks,
-    get_reask_prompt,
-    prune_json_for_reasking,
-    reask_json_as_dict,
+    prune_obj_for_reasking,
+    reasks_to_dict,
     sub_reasks_with_fixed_values,
 )
 
 logger = logging.getLogger(__name__)
 actions_logger = logging.getLogger(f"{__name__}.actions")
 add_destinations(actions_logger.debug)
 
@@ -42,20 +40,21 @@
             where the output is already known.
         guard_history: The guard history to use, defaults to an empty history.
     """
 
     instructions: Optional[Instructions]
     prompt: Prompt
     api: PromptCallable
-    input_schema: InputSchema
-    output_schema: OutputSchema
+    input_schema: Schema
+    output_schema: Schema
     num_reasks: int = 0
     output: str = None
     reask_prompt: Optional[Prompt] = None
     guard_history: GuardHistory = field(default_factory=lambda: GuardHistory([]))
+    base_model: Optional[BaseModel] = None
 
     def _reset_guard_history(self):
         """Reset the guard history."""
         self.guard_history = GuardHistory([])
 
     def __post_init__(self):
         assert (self.prompt and self.api and not self.output) or (
@@ -114,20 +113,20 @@
                 )
 
             return self.guard_history
 
     def step(
         self,
         index: int,
-        api: Callable,
+        api: PromptCallable,
         instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
-        input_schema: InputSchema,
-        output_schema: OutputSchema,
+        input_schema: Schema,
+        output_schema: Schema,
         output: str = None,
     ):
         """Run a full step."""
         with start_action(
             action_type="step",
             index=index,
             instructions=instructions,
@@ -135,182 +134,204 @@
             prompt_params=prompt_params,
             input_schema=input_schema,
             output_schema=output_schema,
         ):
             # Prepare: run pre-processing, and input validation.
             if not output:
                 instructions, prompt = self.prepare(
-                    index, instructions, prompt, prompt_params, input_schema
+                    index,
+                    instructions,
+                    prompt,
+                    prompt_params,
+                    api,
+                    input_schema,
+                    output_schema,
                 )
             else:
                 instructions = None
                 prompt = None
 
-            # Call: run the API, and convert to dict.
-            output, output_as_dict = self.call(index, instructions, prompt, api, output)
+            # Call: run the API.
+            output = self.call(index, instructions, prompt, api, output)
+
+            # Parse: parse the output.
+            parsed_output = self.parse(index, output, output_schema)
 
             # Validate: run output validation.
-            validated_output = self.validate(index, output_as_dict, output_schema)
+            validated_output = self.validate(index, parsed_output, output_schema)
 
             # Introspect: inspect validated output for reasks.
-            reasks = self.introspect(index, validated_output)
+            reasks = self.introspect(index, validated_output, output_schema)
 
             # Replace reask values with fixed values if terminal step.
             if not self.do_loop(index, reasks):
                 validated_output = sub_reasks_with_fixed_values(validated_output)
 
             # Log: step information.
             self.log(
                 prompt=prompt,
                 instructions=instructions,
                 output=output,
-                output_as_dict=output_as_dict,
+                parsed_output=parsed_output,
                 validated_output=validated_output,
                 reasks=reasks,
             )
 
             return validated_output, reasks
 
     def prepare(
         self,
         index: int,
         instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
-        input_schema: InputSchema,
-    ) -> Prompt:
+        api: PromptCallable,
+        input_schema: Schema,
+        output_schema: Schema,
+    ) -> Tuple[Instructions, Prompt]:
         """Prepare by running pre-processing and input validation."""
         with start_action(action_type="prepare", index=index) as action:
             if prompt_params is None:
                 prompt_params = {}
 
-            if input_schema:
-                validated_prompt_params = input_schema.validate(prompt_params)
-            else:
-                validated_prompt_params = prompt_params
+            # if input_schema:
+            #     validated_prompt_params = input_schema.validate(prompt_params)
+            # else:
+            validated_prompt_params = prompt_params
 
             if isinstance(prompt, str):
                 prompt = Prompt(prompt)
 
             prompt = prompt.format(**validated_prompt_params)
 
             # TODO(shreya): should there be any difference to parsing params for prompt?
             if instructions is not None and isinstance(instructions, Instructions):
                 instructions = instructions.format(**validated_prompt_params)
 
+            instructions, prompt = output_schema.preprocess_prompt(
+                api, instructions, prompt
+            )
+
             action.log(
                 message_type="info",
                 instructions=instructions,
                 prompt=prompt,
                 prompt_params=prompt_params,
                 validated_prompt_params=validated_prompt_params,
             )
 
         return instructions, prompt
 
-    def post_process(self, output: str) -> str:
-        """Post-process the raw output before parsing it.
-
-        If the output is surrounded by triple backticks, remove them."""
-        output = output.strip()
-        if output.startswith("```"):
-            output = output[3:]
-            if output.startswith("json"):
-                output = output[4:]
-        if output.endswith("```"):
-            output = output[:-3]
-        return output
-
     def call(
         self,
         index: int,
-        instructions: Optional[str],
+        instructions: Optional[Instructions],
         prompt: Prompt,
         api: Callable,
         output: str = None,
-    ) -> Tuple[str, Optional[Dict]]:
+    ) -> str:
         """Run a step.
 
         1. Query the LLM API,
         2. Convert the response string to a dict,
         3. Log the output
         """
         with start_action(action_type="call", index=index, prompt=prompt) as action:
-            if prompt and instructions:
-                output = api(prompt.source, instructions=instructions.source)
-            elif prompt:
-                output = api(prompt.source)
-
-            # Post-process the output before loading it as JSON.
-            output = self.post_process(output)
-
-            error = None
-            # Treat the output as a JSON string, and load it into a dict.
             try:
-                output_as_dict = json.loads(output, strict=False)
-            except json.decoder.JSONDecodeError as e:
-                output_as_dict = None
-                error = e
+                if prompt and instructions:
+                    output = api(
+                        prompt.source,
+                        instructions=instructions.source,
+                        base_model=self.base_model,
+                    )
+                elif prompt:
+                    output = api(prompt.source, base_model=self.base_model)
+            except Exception:
+                # If the API call fails, try calling again without the instructions.
+                if prompt and instructions:
+                    output = api(prompt.source, instructions=instructions.source)
+                elif prompt:
+                    output = api(prompt.source)
 
             action.log(
                 message_type="info",
                 output=output,
-                output_as_dict=output_as_dict,
+            )
+
+            return output
+
+    def parse(
+        self,
+        index: int,
+        output: str,
+        output_schema: Schema,
+    ):
+        with start_action(action_type="parse", index=index) as action:
+            parsed_output, error = output_schema.parse(output)
+
+            action.log(
+                message_type="info",
+                parsed_output=parsed_output,
                 error=error,
             )
 
-            return output, output_as_dict
+            return parsed_output
 
     def validate(
         self,
         index: int,
-        output_as_dict: Dict,
-        output_schema: OutputSchema,
+        parsed_output: Any,
+        output_schema: Schema,
     ):
         """Validate the output."""
         with start_action(action_type="validate", index=index) as action:
-            validated_output = output_schema.validate(output_as_dict)
+            validated_output = output_schema.validate(parsed_output)
+
             action.log(
                 message_type="info",
-                validated_output=reask_json_as_dict(validated_output),
+                validated_output=reasks_to_dict(validated_output),
             )
+
             return validated_output
 
     def introspect(
         self,
         index: int,
-        validated_output: Optional[Dict],
+        validated_output: Any,
+        output_schema: Schema,
     ) -> List[ReAsk]:
         """Introspect the validated output."""
         with start_action(action_type="introspect", index=index) as action:
             if validated_output is None:
                 return []
-            reasks = gather_reasks(validated_output)
+            reasks = output_schema.introspect(validated_output)
+
             action.log(
                 message_type="info",
                 reasks=[r.__dict__ for r in reasks],
             )
+
             return reasks
 
     def log(
         self,
-        prompt: str,
+        prompt: Prompt,
         instructions: Optional[str],
         output: str,
-        output_as_dict: Dict,
-        validated_output: Dict,
+        parsed_output: Any,
+        validated_output: Any,
         reasks: list,
     ) -> None:
         """Log the step."""
         self.guard_history = self.guard_history.push(
             GuardLogs(
                 prompt=prompt,
                 instructions=instructions,
                 output=output,
-                output_as_dict=output_as_dict,
+                parsed_output=parsed_output,
                 validated_output=validated_output,
                 reasks=reasks,
             )
         )
 
     def do_loop(self, index: int, reasks: List[ReAsk]) -> bool:
         """Determine if we should loop again."""
@@ -318,17 +339,18 @@
             return True
         return False
 
     def prepare_to_loop(
         self,
         reasks: list,
         validated_output: Optional[Dict],
-        output_schema: OutputSchema,
-    ) -> Tuple[str, OutputSchema]:
+        output_schema: Schema,
+    ) -> Tuple[Prompt, Schema]:
         """Prepare to loop again."""
-        prompt, output_schema = get_reask_prompt(
-            parsed_rail=output_schema.root,
+        output_schema = output_schema.get_reask_schema(
             reasks=reasks,
-            reask_json=prune_json_for_reasking(validated_output),
+        )
+        prompt = output_schema.get_reask_prompt(
+            reask_value=prune_obj_for_reasking(validated_output),
             reask_prompt_template=self.reask_prompt,
         )
-        return prompt, OutputSchema(output_schema)
+        return prompt, output_schema
```

### Comparing `guardrails-ai-0.1.7/guardrails/schema.py` & `guardrails-ai-0.1.8/guardrails/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,30 @@
+import json
 import logging
 import pprint
 import re
 import warnings
 from copy import deepcopy
 from dataclasses import dataclass
 from types import SimpleNamespace
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from lxml import etree as ET
 from lxml.builder import E
 
-from guardrails.datatypes import DataType
+from guardrails.datatypes import DataType, String
+from guardrails.llm_providers import PromptCallable, openai_chat_wrapper, openai_wrapper
+from guardrails.prompt import Instructions, Prompt
+from guardrails.utils.constants import constants
+from guardrails.utils.reask_utils import (
+    ReAsk,
+    gather_reasks,
+    get_pruned_tree,
+    get_reasks_by_element,
+)
 from guardrails.validators import Validator, check_refrain_in_dict, filter_in_dict
 
 if TYPE_CHECKING:
     pass
 
 logger = logging.getLogger(__name__)
 
@@ -245,33 +255,22 @@
     """Schema class that holds a _schema attribute."""
 
     def __init__(
         self,
         root: Optional[ET._Element] = None,
         schema: Optional[Dict[str, DataType]] = None,
     ) -> None:
-        from guardrails.datatypes import registry as types_registry
-
         if schema is None:
             schema = {}
 
         self._schema = SimpleNamespace(**schema)
         self.root = root
 
         if root is not None:
-            strict = False
-            if "strict" in root.attrib and root.attrib["strict"] == "true":
-                strict = True
-
-            for child in root:
-                if isinstance(child, ET._Comment):
-                    continue
-                child_name = child.attrib["name"]
-                child_data = types_registry[child.tag].from_xml(child, strict=strict)
-                self[child_name] = child_data
+            self.setup_schema(root)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({pprint.pformat(vars(self._schema))})"
 
     def __getitem__(self, key: str) -> DataType:
         return getattr(self._schema, key)
 
@@ -298,14 +297,198 @@
         """Convert the schema to a dictionary."""
         return vars(self._schema)
 
     @property
     def parsed_rail(self) -> Optional[ET._Element]:
         return self.root
 
+    def setup_schema(self, root: ET._Element) -> None:
+        """Parse the schema specification.
+
+        Args:
+            root: The root element of the schema specification.
+        """
+        raise NotImplementedError
+
+    def validate(self, data: Any) -> Any:
+        """Validate a dictionary of data against the schema.
+
+        Args:
+            data: The data to validate.
+
+        Returns:
+            The validated data.
+        """
+        raise NotImplementedError
+
+    def transpile(self, method: str = "default") -> str:
+        """Convert the XML schema to a string that is used for prompting a
+        large language model.
+
+        Returns:
+            The prompt.
+        """
+        raise NotImplementedError
+
+    def get_reask_schema(
+        self,
+        reasks: List[ReAsk],
+    ) -> "Schema":
+        """Construct a schema for reasking.
+
+        Args:
+            reasks: List of tuples, where each tuple contains the path to the
+                reasked element, and the ReAsk object (which contains the error
+                message describing why the reask is necessary).
+
+        Returns:
+            The prompt.
+        """
+        raise NotImplementedError
+
+    def parse(self, output: str) -> Tuple[Any, Optional[Exception]]:
+        """Parse the output from the large language model.
+
+        Args:
+            output: The output from the large language model.
+
+        Returns:
+            The parsed output, and the exception that was raised (if any).
+        """
+        raise NotImplementedError
+
+    def introspect(self, data: Any) -> List[ReAsk]:
+        """Inspect the data for reasks.
+
+        Args:
+            data: The data to introspect.
+
+        Returns:
+            A list of ReAsk objects.
+        """
+        raise NotImplementedError
+
+    def get_default_reask_prompt(self) -> Prompt:
+        """Get the default reask prompt for the schema.
+
+        Returns:
+            The default reask prompt.
+        """
+        raise NotImplementedError
+
+    def get_reask_prompt(
+        self,
+        reask_value: Any,
+        reask_prompt_template: Optional[Prompt] = None,
+    ) -> Prompt:
+        """Get a reask prompt for the schema.
+
+        Args:
+            reask_value: The value that was returned from the API, with reasks.
+            reask_prompt_template: The template to use for the reask prompt.
+
+        Returns:
+            The reask prompt.
+        """
+        raise NotImplementedError
+
+    def preprocess_prompt(
+        self,
+        prompt_callable: PromptCallable,
+        instructions: Optional[Instructions],
+        prompt: Prompt,
+    ):
+        """Preprocess the instructions and prompt before sending it to the
+        model.
+
+        Args:
+            prompt_callable: The callable to be used to prompt the model.
+            instructions: The instructions to preprocess.
+            prompt: The prompt to preprocess.
+        """
+        raise NotImplementedError
+
+
+class JsonSchema(Schema):
+    def get_reask_schema(
+        self,
+        reasks: List[ReAsk],
+    ) -> "Schema":
+        parsed_rail = deepcopy(self.root)
+
+        # Get the elements that are to be reasked
+        reask_elements = get_reasks_by_element(reasks, parsed_rail)
+
+        # Get the pruned tree so that it only contains ReAsk objects
+        pruned_tree = get_pruned_tree(parsed_rail, list(reask_elements.keys()))
+        pruned_tree_schema = type(self)(pruned_tree)
+
+        return pruned_tree_schema
+
+    def get_reask_prompt(
+        self,
+        reask_value: Any,
+        reask_prompt_template: Optional[Prompt] = None,
+    ) -> Prompt:
+        pruned_tree_string = self.transpile()
+
+        if reask_prompt_template is None:
+            reask_prompt_template = self.get_default_reask_prompt()
+
+        def reask_decoder(obj):
+            return {
+                k: v for k, v in obj.__dict__.items() if k not in ["path", "fix_value"]
+            }
+
+        return reask_prompt_template.format(
+            previous_response=json.dumps(reask_value, indent=2, default=reask_decoder)
+            .replace("{", "{{")
+            .replace("}", "}}"),
+            output_schema=pruned_tree_string,
+        )
+
+    def setup_schema(self, root: ET._Element) -> None:
+        from guardrails.datatypes import registry as types_registry
+
+        strict = False
+        if "strict" in root.attrib and root.attrib["strict"] == "true":
+            strict = True
+
+        for child in root:
+            if isinstance(child, ET._Comment):
+                continue
+            child_name = child.attrib["name"]
+            child_data = types_registry[child.tag].from_xml(child, strict=strict)
+            self[child_name] = child_data
+
+    def parse(self, output: str) -> Tuple[Dict, Optional[Exception]]:
+        # Remove the triple backticks from the output
+        output = output.strip()
+        if output.startswith("```"):
+            output = output[3:]
+            if output.startswith("json"):
+                output = output[4:]
+        if output.endswith("```"):
+            output = output[:-3]
+
+        # Treat the output as a JSON string, and load it into a dict.
+        error = None
+        try:
+            output_as_dict = json.loads(output, strict=False)
+        except json.decoder.JSONDecodeError as e:
+            output_as_dict = None
+            error = e
+        return output_as_dict, error
+
+    def get_default_reask_prompt(self):
+        return Prompt(
+            constants["high_level_json_reask_prompt"]
+            + constants["complete_json_suffix"]
+        )
+
     def validate(
         self,
         data: Optional[Dict[str, Any]],
     ) -> Optional[Dict[str, Any]]:
         """Validate a dictionary of data against the schema.
 
         Args:
@@ -342,31 +525,171 @@
             validated_response = {}
 
         # Remove all keys that have `Filter` values.
         validated_response = filter_in_dict(validated_response)
 
         return validated_response
 
+    def introspect(self, data: Dict) -> list:
+        return gather_reasks(data)
+
+    def preprocess_prompt(
+        self,
+        prompt_callable: PromptCallable,
+        instructions: Optional[Instructions],
+        prompt: Prompt,
+    ):
+        if not hasattr(prompt_callable.fn, "func"):
+            # Only apply preprocessing to guardrails wrappers.
+            return instructions, prompt
+
+        if prompt_callable.fn.func is openai_wrapper:
+            prompt.source += "\n\nJson Output:\n\n"
+        if prompt_callable.fn.func is openai_chat_wrapper and not instructions:
+            instructions = Instructions(
+                "You are a helpful assistant, "
+                "able to express yourself purely through JSON, "
+                "strictly and precisely adhering to the provided XML schemas."
+            )
+
+        return instructions, prompt
+
     def transpile(self, method: str = "default") -> str:
-        """Convert the XML schema to a string that is used for prompting a
-        large language model.
+        transpiler = getattr(Schema2Prompt, method)
+        return transpiler(self)
+
+
+class StringSchema(Schema):
+    def __init__(self, root: ET._Element) -> None:
+        self.string_key = "string"
+        super().__init__(root)
+
+    def setup_schema(self, root: ET._Element) -> None:
+        if len(root) != 0:
+            raise ValueError("String output schemas must not have children.")
+
+        if "name" in root.attrib:
+            self.string_key = root.attrib["name"]
+        else:
+            self.string_key = root.attrib["name"] = "string"
+
+        # make root tag into a string tag
+        root_string = ET.Element("string", root.attrib)
+        self[self.string_key] = String.from_xml(root_string)
+
+    def get_reask_schema(
+        self,
+        reasks: List[ReAsk],
+    ) -> "Schema":
+        return self
+
+    def get_default_reask_prompt(self):
+        return Prompt(
+            constants["high_level_string_reask_prompt"]
+            + constants["complete_string_suffix"]
+        )
+
+    def get_reask_prompt(
+        self,
+        reask_value: ReAsk,
+        reask_prompt_template: Optional[Prompt] = None,
+    ) -> Prompt:
+        pruned_tree_string = self.transpile()
+
+        if reask_prompt_template is None:
+            reask_prompt_template = self.get_default_reask_prompt()
+
+        return reask_prompt_template.format(
+            previous_response=reask_value.incorrect_value,
+            error_messages=f"- {reask_value.error_message}",
+            output_schema=pruned_tree_string,
+        )
+
+    def parse(self, output: str) -> Tuple[Any, Optional[Exception]]:
+        return output, None
+
+    def validate(
+        self,
+        data: Any,
+    ) -> Any:
+        """Validate a dictionary of data against the schema.
+
+        Args:
+            data: The data to validate.
 
         Returns:
-            The prompt.
+            The validated data.
         """
-        transpiler = getattr(Schema2Prompt, method)
-        return transpiler(self)
+        if data is None:
+            return None
 
+        if not isinstance(data, str):
+            raise TypeError(f"Argument `data` must be a string, not {type(data)}.")
 
-class InputSchema(Schema):
-    """Input schema class that holds a _schema attribute."""
+        validated_response = self[self.string_key].validate(
+            key=self.string_key,
+            value=data,
+            schema={
+                self.string_key: data,
+            },
+        )
 
+        if check_refrain_in_dict(validated_response):
+            # If the data contains a `Refain` value, we return an empty
+            # dictionary.
+            logger.debug("Refrain detected.")
+            validated_response = {}
+
+        # Remove all keys that have `Filter` values.
+        validated_response = filter_in_dict(validated_response)
 
-class OutputSchema(Schema):
-    """Output schema class that holds a _schema attribute."""
+        if self.string_key in validated_response:
+            return validated_response[self.string_key]
+        return None
+
+    def introspect(self, data: Any) -> List[ReAsk]:
+        if isinstance(data, ReAsk):
+            return [data]
+        return []
+
+    def preprocess_prompt(
+        self,
+        prompt_callable: PromptCallable,
+        instructions: Optional[Instructions],
+        prompt: Prompt,
+    ):
+        if not hasattr(prompt_callable.fn, "func"):
+            # Only apply preprocessing to guardrails wrappers.
+            return instructions, prompt
+
+        if prompt_callable.fn.func is openai_wrapper:
+            prompt.source += "\n\nString Output:\n\n"
+        if prompt_callable.fn.func is openai_chat_wrapper and not instructions:
+            instructions = Instructions(
+                "You are a helpful assistant, expressing yourself through a string."
+            )
+
+        return instructions, prompt
+
+    def transpile(self, method: str = "default") -> str:
+        obj = self[self.string_key]
+        schema = ""
+        if "description" in obj.element.attrib:
+            schema += f"""String description, delimited by +++:
+
++++
+{obj.element.attrib["description"]}
++++"""
+        if not obj.format_attr.empty:
+            schema += (
+                "\n\nYour generated response should satisfy the following properties:"
+            )
+            for validator in obj.format_attr.validators:
+                schema += f"\n- {validator.to_prompt()}"
+        return schema
 
 
 class Schema2Prompt:
     """Class that contains transpilers to go from a schema to its
     representation in a prompt.
 
     This is important for communicating the schema to a large language
```

### Comparing `guardrails-ai-0.1.7/guardrails/utils/constants.py` & `guardrails-ai-0.1.8/guardrails/utils/constants.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/utils/docs_utils.py` & `guardrails-ai-0.1.8/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/utils/logs_utils.py` & `guardrails-ai-0.1.8/guardrails/utils/logs_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from rich.console import Group
 from rich.panel import Panel
 from rich.pretty import pretty_repr
 from rich.tree import Tree
 
 from guardrails.prompt import Prompt
-from guardrails.utils.reask_utils import ReAsk, gather_reasks, prune_json_for_reasking
+from guardrails.utils.reask_utils import ReAsk, gather_reasks, prune_obj_for_reasking
 
 
 @dataclass
 class GuardLogs:
     prompt: Prompt
     instructions: Optional[str]
     output: str
-    output_as_dict: dict
+    parsed_output: dict
     validated_output: dict
     reasks: List[ReAsk]
 
     @property
     def failed_validations(self) -> List[ReAsk]:
         """Returns the failed validations."""
         return gather_reasks(self.validated_output)
@@ -88,15 +88,15 @@
     def output(self) -> str:
         """Returns the latest output."""
         return self.history[-1].output
 
     @property
     def output_as_dict(self) -> dict:
         """Returns the latest output as a dict."""
-        return self.history[-1].output_as_dict
+        return self.history[-1].parsed_output
 
     @property
     def failed_validations(self) -> List[ReAsk]:
         """Returns all failed validations."""
         return [log.failed_validations for log in self.history]
 
 
@@ -137,16 +137,19 @@
 
     Returns:
         The merged output.
     """
     from guardrails.validators import PydanticReAsk
 
     previous_response = prev_logs.validated_output
-    pruned_reask_json = prune_json_for_reasking(previous_response)
     reask_response = current_logs.validated_output
+    if isinstance(previous_response, ReAsk):
+        return reask_response
+
+    pruned_reask_json = prune_obj_for_reasking(previous_response)
 
     # Reask output and reask json have the same structure, except that values
     # of the reask json are ReAsk objects. We want to replace the ReAsk objects
     # with the values from the reask output.
     merged_json = deepcopy(previous_response)
 
     def update_reasked_elements(pruned_reask_json, reask_response_dict):
```

### Comparing `guardrails-ai-0.1.7/guardrails/utils/misc.py` & `guardrails-ai-0.1.8/guardrails/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails/utils/reask_utils.py` & `guardrails-ai-0.1.8/guardrails/utils/reask_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-import json
 from collections import defaultdict
-from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Union
 
 from lxml import etree as ET
 
-from guardrails.prompt import Prompt
-from guardrails.utils.constants import constants
-
 
 @dataclass
 class ReAsk:
     incorrect_value: Any
     error_message: str
     fix_value: Any
     path: List[Any] = None
@@ -135,128 +130,78 @@
             # Remove the format attribute
             if "format" in element.attrib:
                 del element.attrib["format"]
 
     return root
 
 
-def prune_json_for_reasking(json_object: Any) -> Union[None, Dict, List]:
-    """Validated JSON is a nested dictionary where some keys may be ReAsk
-    objects.
+def prune_obj_for_reasking(obj: Any) -> Union[None, Dict, List]:
+    """After validation, we get a nested dictionary where some keys may be
+    ReAsk objects.
 
-    This function prunes the validated JSON of any object that is not a ReAsk object.
+    This function prunes the validated form of any object that is not a ReAsk object.
     It also keeps all of the ancestors of the ReAsk objects.
 
     Args:
-        json_object: The validated JSON.
+        obj: The validated object.
 
     Returns:
-        The pruned validated JSON.
+        The pruned validated object.
     """
     from guardrails.validators import PydanticReAsk
 
-    if isinstance(json_object, ReAsk) or isinstance(json_object, PydanticReAsk):
-        return json_object
-    elif isinstance(json_object, list):
+    if isinstance(obj, ReAsk) or isinstance(obj, PydanticReAsk):
+        return obj
+    elif isinstance(obj, list):
         pruned_list = []
-        for item in json_object:
-            pruned_output = prune_json_for_reasking(item)
+        for item in obj:
+            pruned_output = prune_obj_for_reasking(item)
             if pruned_output is not None:
                 pruned_list.append(pruned_output)
         if len(pruned_list):
             return pruned_list
         return None
-    elif isinstance(json_object, dict):
+    elif isinstance(obj, dict):
         pruned_json = {}
-        for key, value in json_object.items():
+        for key, value in obj.items():
             if isinstance(value, ReAsk) or isinstance(value, PydanticReAsk):
                 pruned_json[key] = value
             elif isinstance(value, dict):
-                pruned_output = prune_json_for_reasking(value)
+                pruned_output = prune_obj_for_reasking(value)
                 if pruned_output is not None:
                     pruned_json[key] = pruned_output
             elif isinstance(value, list):
                 pruned_list = []
                 for item in value:
-                    pruned_output = prune_json_for_reasking(item)
+                    pruned_output = prune_obj_for_reasking(item)
                     if pruned_output is not None:
                         pruned_list.append(pruned_output)
                 if len(pruned_list):
                     pruned_json[key] = pruned_list
 
         if len(pruned_json):
             return pruned_json
 
         return None
 
 
-def get_reask_prompt(
-    parsed_rail: ET._Element,
-    reasks: List[ReAsk],
-    reask_json: Dict,
-    reask_prompt_template: Optional[Prompt] = None,
-) -> Tuple[Prompt, ET._Element]:
-    """Construct a prompt for reasking.
-
-    Args:
-        parsed_rail: The parsed RAIL.
-        reasks: List of tuples, where each tuple contains the path to the
-            reasked element, and the ReAsk object (which contains the error
-            message describing why the reask is necessary).
-        reask_json: Pruned JSON that contains only ReAsk objects.
-
-    Returns:
-        The prompt.
-    """
-    from guardrails.schema import OutputSchema
-
-    parsed_rail_copy = deepcopy(parsed_rail)
-
-    # Get the elements that are to be reasked
-    reask_elements = get_reasks_by_element(reasks, parsed_rail_copy)
+def reasks_to_dict(dict_with_reasks: Dict) -> Dict:
+    """If a ReAsk object exists in the dict, return it as a dictionary."""
 
-    # Get the pruned JSON so that it only contains ReAsk objects
-    # Get the pruned tree
-    pruned_tree = get_pruned_tree(parsed_rail_copy, list(reask_elements.keys()))
-    pruned_tree_string = OutputSchema(pruned_tree).transpile()
-
-    if reask_prompt_template is None:
-        reask_prompt_template = Prompt(
-            constants["high_level_reask_prompt"] + constants["complete_json_suffix"]
-        )
-
-    def reask_decoder(obj):
-        return {k: v for k, v in obj.__dict__.items() if k not in ["path", "fix_value"]}
-
-    reask_prompt = reask_prompt_template.format(
-        previous_response=json.dumps(reask_json, indent=2, default=reask_decoder)
-        .replace("{", "{{")
-        .replace("}", "}}"),
-        output_schema=pruned_tree_string,
-    )
-
-    return reask_prompt, pruned_tree
-
-
-def reask_json_as_dict(json: Dict) -> Dict:
-    """If a ReAsk object exists in the JSON, return it as a dictionary."""
-
-    def _reask_json_as_dict(json_object: Any) -> Any:
-        if isinstance(json_object, dict):
-            return {
-                key: _reask_json_as_dict(value) for key, value in json_object.items()
-            }
-        elif isinstance(json_object, list):
-            return [_reask_json_as_dict(item) for item in json_object]
-        elif isinstance(json_object, ReAsk):
-            return json_object.__dict__
+    def _(dict_object: Any) -> Any:
+        if isinstance(dict_object, dict):
+            return {key: _(value) for key, value in dict_object.items()}
+        elif isinstance(dict_object, list):
+            return [_(item) for item in dict_object]
+        elif isinstance(dict_object, ReAsk):
+            return dict_object.__dict__
         else:
-            return json_object
+            return dict_object
 
-    return _reask_json_as_dict(json)
+    return _(dict_with_reasks)
 
 
 def sub_reasks_with_fixed_values(value: Any) -> Any:
     """Substitute ReAsk objects with their fixed values recursively.
 
     Args:
         value: Either a list, a dictionary, a ReAsk object or a scalar value.
```

### Comparing `guardrails-ai-0.1.7/guardrails/utils/sql_utils.py` & `guardrails-ai-0.1.8/guardrails/utils/sql_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 
     _HAS_SQLALCHEMY = True
 except ImportError:
     _HAS_SQLALCHEMY = False
 
 
 class SQLDriver(ABC):
-    """
-    Abstract class for SQL drivers. The expose common functionality
-    for validating SQL queries.
+    """Abstract class for SQL drivers.
+
+    The expose common functionality for validating SQL queries.
     """
 
     @abstractmethod
     def validate_sql(self, query: str) -> List[str]:
         ...
 
     @abstractmethod
     def get_schema(self) -> str:
         ...
 
 
 class SimpleSqlDriver(SQLDriver):
-    """
-    Simple SQL driver which uses sqlvalidator to validate SQL queries.
+    """Simple SQL driver which uses sqlvalidator to validate SQL queries.
+
     Does not understands dialects and is not connected to a database.
     """
 
     def validate_sql(self, query: str) -> List[str]:
         import sqlvalidator
 
         sql_query = sqlvalidator.parse(query)
@@ -43,16 +43,16 @@
         return sql_query.errors
 
     def get_schema(self) -> str:
         raise NotImplementedError
 
 
 class SqlAlchemyDriver(SQLDriver):
-    """
-    SQL driver which uses sqlalchemy to validate SQL queries.
+    """SQL driver which uses sqlalchemy to validate SQL queries.
+
     It can setup the database schema and check if the queries are valid
     by connecting to the database.
     """
 
     def __init__(self, schema_file: Optional[str], conn: Optional[str]) -> None:
         if not _HAS_SQLALCHEMY:
             raise ImportError(
```

### Comparing `guardrails-ai-0.1.7/guardrails/validators.py` & `guardrails-ai-0.1.8/guardrails/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,33 @@
                 kwargs[k] = str(v)
 
         params = " ".join(list(kwargs.values()))
         if with_keywords:
             params = " ".join([f"{k}={v}" for k, v in kwargs.items()])
         return f"{self.rail_alias}: {params}"
 
+    def to_xml_attrib(self):
+        """Convert the validator to an XML attribute."""
+
+        if not len(self._kwargs):
+            return self.rail_alias
+
+        validator_args = []
+        for arg in self.__init__.__code__.co_varnames[1:]:
+            if arg not in ("on_fail", "args", "kwargs"):
+                str_arg = str(self._kwargs[arg])
+                str_arg = "{" + str_arg + "}" if " " in str_arg else str_arg
+                validator_args.append(str_arg)
+
+        params = " ".join(validator_args)
+        return f"{self.rail_alias}: {params}"
+
+    def __call__(self, v: Any) -> Any:
+        return self.validate("dummy_key", v, {"dummy_key": v})["dummy_key"]
+
 
 # @register_validator('required', 'all')
 # class Required(Validator):
 #     """Validate that a value is not None."""
 
 #     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> bool:
 #         """Validate that a value is not None."""
@@ -392,14 +411,41 @@
             # Insert the new `value` dictionary into the schema.
             # This now contains e.g. ReAsk objects.
             schema[key] = PydanticReAsk(new_value)
 
         return schema
 
 
+@register_validator(name="pydantic_field_validator", data_type="all")
+class PydanticFieldValidator(Validator):
+    def __init__(
+        self,
+        field_validator: Callable,
+        on_fail: Optional[Callable[..., Any]] = None,
+        **kwargs,
+    ):
+        self.field_validator = field_validator
+        super().__init__(on_fail, **kwargs)
+
+    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+        try:
+            return self.field_validator(value)
+        except Exception as e:
+            raise EventDetail(
+                key=key,
+                value=value,
+                schema=schema,
+                error_message=str(e),
+                fix_value=None,
+            )
+
+    def to_prompt(self, with_keywords: bool = True) -> str:
+        return self.field_validator.__func__.__name__
+
+
 @register_validator(name="choice", data_type="choice")
 class Choice(Validator):
     """Validate that a value is one of a set of choices.
 
     - Name for `format` attribute: `choice`
     - Supported data types: `string`
     - Programmatic fix: Closest value within the set of choices.
@@ -633,15 +679,15 @@
             )
 
         return schema
 
 
 @register_validator(name="two-words", data_type="string")
 class TwoWords(Validator):
-    """Validate that a value is upper case.
+    """Validate that a value is two words.
 
     - Name for `format` attribute: `two-words`
     - Supported data types: `string`
     - Programmatic fix: Pick the first two words.
     """
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
@@ -1118,15 +1164,16 @@
 
     def to_prompt(self, with_keywords: bool = True) -> str:
         return ""
 
 
 @register_validator(name="reading-time", data_type="string")
 class ReadingTime(Validator):
-    """Validate that the a string can be read in less than a certain amount of time."""
+    """Validate that the a string can be read in less than a certain amount of
+    time."""
 
     def __init__(self, reading_time: int, on_fail: str = "fix"):
         super().__init__(on_fail=on_fail, max_time=reading_time)
         self._max_time = reading_time
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         logger.debug(
@@ -1148,21 +1195,23 @@
             )
 
         return schema
 
 
 @register_validator(name="extractive-summary", data_type="string")
 class ExtractiveSummary(Validator):
-    """Validate that a string is a valid extractive summary of a given document.
+    """Validate that a string is a valid extractive summary of a given
+    document.
 
-    This validator does a fuzzy match between the sentences in the summary and the
-    sentences in the document. Each sentence in the summary must be similar to at
-    least one sentence in the document. After the validation, the summary is updated
-    to include the sentences from the document that were matched, and the citations
-    for those sentences are added to the end of the summary.
+    This validator does a fuzzy match between the sentences in the
+    summary and the sentences in the document. Each sentence in the
+    summary must be similar to at least one sentence in the document.
+    After the validation, the summary is updated to include the
+    sentences from the document that were matched, and the citations for
+    those sentences are added to the end of the summary.
     """
 
     def __init__(
         self,
         documents_dir: str,
         threshold: int = 85,
         on_fail: Optional[Callable] = None,
@@ -1240,16 +1289,17 @@
         return schema
 
 
 @register_validator(name="remove-redundant-sentences", data_type="string")
 class RemoveRedundantSentences(Validator):
     """Remove redundant sentences from a string.
 
-    This validator removes sentences from a string that are similar to other sentences
-    in the string. This is useful for removing repetitive sentences from a string.
+    This validator removes sentences from a string that are similar to
+    other sentences in the string. This is useful for removing
+    repetitive sentences from a string.
     """
 
     def __init__(
         self, threshold: int = 70, on_fail: Optional[Callable] = None, **kwargs
     ):
         super().__init__(on_fail, **kwargs)
         self.threshold = threshold
@@ -1303,15 +1353,16 @@
             )
 
         return schema
 
 
 @register_validator(name="saliency-check", data_type="string")
 class SaliencyCheck(Validator):
-    """Check that the summary covers the list of topics present in the document."""
+    """Check that the summary covers the list of topics present in the
+    document."""
 
     def __init__(
         self,
         docs_dir: str,
         llm_callable: Callable = None,
         on_fail: Optional[Callable] = None,
         threshold: int = 0.25,
```

### Comparing `guardrails-ai-0.1.7/guardrails/vectordb/base.py` & `guardrails-ai-0.1.8/guardrails/vectordb/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 
 # TODO Parameterize the init with the distance algorithm to use: cosine, L2, etc.
 class VectorDBBase(ABC):
     """Base class for vector databases."""
 
     def __init__(self, embedder: EmbeddingBase, path: str = None) -> None:
         """Creates a new VectorDBBase.
+
         Args:
             embedder: EmbeddingBase instance to use for embedding the text.
             path: Path to store or load the vector database.
         """
         self._embedder = embedder
         self._path = path
 
     @abstractmethod
     def add_vectors(self, vectors: List[List[float]]) -> None:
         """Adds a list of vectors to the store.
+
         Args:
             vectors: List of vectors to add.
         Returns:
             None
         """
         ...
 
     @abstractmethod
     def similarity_search_vector(self, vector: List[float], k: int) -> List[int]:
         """Searches for vectors which are similar to the given vector.
+
         Args:
             vector: Vector to search for.
             k: Number of similar vectors to return.
         """
         ...
 
     @abstractmethod
```

### Comparing `guardrails-ai-0.1.7/guardrails/vectordb/faiss.py` & `guardrails-ai-0.1.8/guardrails/vectordb/faiss.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails_ai.egg-info/PKG-INFO` & `guardrails-ai-0.1.8/guardrails_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `guardrails-ai-0.1.7/guardrails_ai.egg-info/SOURCES.txt` & `guardrails-ai-0.1.8/guardrails_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.7/guardrails_ai.egg-info/requires.txt` & `guardrails-ai-0.1.8/guardrails_ai.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 openai
 rich
 eliot
 eliot-tree
 pydantic
 typer
 griffe
-tenacity
+tenacity>=8.1.0
 
 [critique]
 inspiredco
 
 [dev]
 black==22.12.0
 isort>=5.12.0
```

### Comparing `guardrails-ai-0.1.7/setup.py` & `guardrails-ai-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "openai",
     "rich",
     "eliot",
     "eliot-tree",
     "pydantic",
     "typer",
     "griffe",
-    "tenacity",
+    "tenacity>=8.1.0",
 ]
 
 # Read in docs/requirements.txt
 with open("docs/requirements.txt") as f:
     DOCS_REQUIREMENTS = f.read().splitlines()
 
 SQL_REQUIREMENTS = ["sqlvalidator", "sqlalchemy>=2.0.9", "sqlglot"]
```

