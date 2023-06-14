# Comparing `tmp/langkit-0.0.1b6.tar.gz` & `tmp/langkit-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1b6.tar", max compression
+gzip compressed data, was "langkit-0.0.1b7.tar", max compression
```

## Comparing `langkit-0.0.1b6.tar` & `langkit-0.0.1b7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b6/LICENSE
--rw-r--r--   0        0        0     2852 2023-06-09 23:51:13.157907 langkit-0.0.1b6/README.md
--rw-r--r--   0        0        0      998 2023-06-09 23:51:13.157907 langkit-0.0.1b6/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-06-09 23:51:13.157907 langkit-0.0.1b6/langkit/all_metrics.py
--rw-r--r--   0        0        0      140 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-06-09 23:51:13.157907 langkit-0.0.1b6/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1768 2023-06-09 23:51:13.157907 langkit-0.0.1b6/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-06-07 22:19:42.247907 langkit-0.0.1b6/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-06-07 22:19:42.247907 langkit-0.0.1b6/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    10756 2023-06-09 23:51:13.157907 langkit-0.0.1b6/langkit/docs/modules.md
--rw-r--r--   0        0        0    11219 2023-06-12 16:52:44.100690 langkit-0.0.1b6/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0     9391 2023-06-12 22:23:38.400690 langkit-0.0.1b6/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262428 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     5449 2023-06-12 16:56:49.630690 langkit-0.0.1b6/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0     1362 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/light_metrics.py
--rw-r--r--   0        0        0      499 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/llm_metrics.py
--rw-r--r--   0        0        0       75 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/openai/openai.py
--rw-r--r--   0        0        0     2441 2023-06-12 16:42:58.730690 langkit-0.0.1b6/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      793 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2962 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/sentiment.py
--rw-r--r--   0        0        0     3970 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/tests/conftest.py
--rw-r--r--   0        0        0     1078 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-06-12 16:42:58.730690 langkit-0.0.1b6/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b6/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b6/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-06-11 03:02:39.184198 langkit-0.0.1b6/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-06-11 03:52:57.364198 langkit-0.0.1b6/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b6/langkit/themes.json.txt
--rw-r--r--   0        0        0     3652 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-06-09 23:51:13.167907 langkit-0.0.1b6/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-06-11 01:28:15.324198 langkit-0.0.1b6/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b6/langkit/transformer.py
--rw-r--r--   0        0        0    30472 2023-06-11 21:55:45.901756 langkit-0.0.1b6/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-06-10 01:05:05.107906 langkit-0.0.1b6/langkit/whylogs/samples.py
--rw-r--r--   0        0        0      902 2023-06-12 22:13:34.620690 langkit-0.0.1b6/pyproject.toml
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 langkit-0.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0     3046 2023-06-10 01:05:05.107906 langkit-0.0.1b7/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b7/LICENSE
+-rw-r--r--   0        0        0      998 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/all_metrics.py
+-rw-r--r--   0        0        0      140 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1768 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-06-07 22:19:42.247907 langkit-0.0.1b7/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-06-07 22:19:42.247907 langkit-0.0.1b7/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    10756 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11219 2023-06-12 16:52:44.100690 langkit-0.0.1b7/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0     9391 2023-06-12 22:23:38.400690 langkit-0.0.1b7/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262428 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     5449 2023-06-12 16:56:49.630690 langkit-0.0.1b7/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0     1362 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/light_metrics.py
+-rw-r--r--   0        0        0      499 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/llm_metrics.py
+-rw-r--r--   0        0        0       75 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/openai/openai.py
+-rw-r--r--   0        0        0     2441 2023-06-12 16:42:58.730690 langkit-0.0.1b7/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      793 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2962 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/sentiment.py
+-rw-r--r--   0        0        0     3970 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     1078 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-06-12 16:42:58.730690 langkit-0.0.1b7/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b7/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-06-11 03:02:39.184198 langkit-0.0.1b7/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-06-11 03:52:57.364198 langkit-0.0.1b7/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/themes.json.txt
+-rw-r--r--   0        0        0     3652 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-06-11 01:28:15.324198 langkit-0.0.1b7/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/transformer.py
+-rw-r--r--   0        0        0    30472 2023-06-11 21:55:45.901756 langkit-0.0.1b7/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0      907 2023-06-12 22:38:57.550690 langkit-0.0.1b7/pyproject.toml
+-rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 langkit-0.0.1b7/PKG-INFO
```

### Comparing `langkit-0.0.1b6/LICENSE` & `langkit-0.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/__init__.py` & `langkit-0.0.1b7/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/all_metrics.py` & `langkit-0.0.1b7/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/config/environment.py` & `langkit-0.0.1b7/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/docs/features/quality.md` & `langkit-0.0.1b7/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/docs/features/relevance.md` & `langkit-0.0.1b7/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/docs/features/security.md` & `langkit-0.0.1b7/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/docs/features/sentiment.md` & `langkit-0.0.1b7/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/docs/modules.md` & `langkit-0.0.1b7/langkit/docs/modules.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.1b7/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.1b7/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.1b7/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.1b7/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.1b7/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/injections.py` & `langkit-0.0.1b7/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/input_output.py` & `langkit-0.0.1b7/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/openai/openai.py` & `langkit-0.0.1b7/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/openai_wrapper.py` & `langkit-0.0.1b7/langkit/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/pattern_groups.json` & `langkit-0.0.1b7/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/regexes.py` & `langkit-0.0.1b7/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/sentiment.py` & `langkit-0.0.1b7/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/conftest.py` & `langkit-0.0.1b7/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/test_injections.py` & `langkit-0.0.1b7/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/test_input_output.py` & `langkit-0.0.1b7/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/test_patterns.py` & `langkit-0.0.1b7/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/test_themes.py` & `langkit-0.0.1b7/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/tests/test_toxicity.py` & `langkit-0.0.1b7/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/textstat.py` & `langkit-0.0.1b7/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/themes.json` & `langkit-0.0.1b7/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/themes.py` & `langkit-0.0.1b7/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/topics.py` & `langkit-0.0.1b7/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/toxicity.py` & `langkit-0.0.1b7/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/whylogs/reference_chats.json` & `langkit-0.0.1b7/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/langkit/whylogs/samples.py` & `langkit-0.0.1b7/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b6/pyproject.toml` & `langkit-0.0.1b7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.1b6"
+version = "0.0.1b7"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
-readme = "README.md"
+readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 whylogs = {version = "1.1.45.dev4"}
 textstat = "^0.7.3"
 pandas = "*"
```

### Comparing `langkit-0.0.1b6/PKG-INFO` & `langkit-0.0.1b7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -19,70 +19,69 @@
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
 Requires-Dist: whylogs (==1.1.45.dev4)
 Description-Content-Type: text/markdown
 
-# LangKit
+LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
-![LangKit graphic](static/img/LangKit_graphic.png)
+## Table of Contents 📖
 
-**LangKit** is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
+- [Motivation](#motivation-)
+- [Features](#features-)
+- [Installation](#installation-)
+- [Usage](#usage-)
+- [Modules](#modules-)
 
-The generated profiles can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
-
-## Motivation
+## Motivation 🎯
 
 Productionizing language models, including LLMs, comes with a range of risks due to the infinite amount of input combinations, which can elicit an infinite amount of outputs. The unstructured nature of text poses a challenge in the ML observability space - a challenge worth solving, since the lack of visibility on the model's behavior can have serious consequences.
 
-## Features
+## Features 🛠️
 
 The currently supported metrics include:
 
-- [Text Quality](langkit/docs/features/quality.md)
+- [Text Quality](https://github.com/whylabs/langkit/blob/main/langkit/docs/features/quality.md)
   - readability score
   - complexity and grade scores
-- [Text Relevance](langkit/docs/features/relevance.md)
+- [Text Relevance](https://github.com/whylabs/langkit/blob/main/langkit/docs/features/relevance.md)
   - Similarity scores between prompt/responses
   - Similarity scores against user-defined themes
-- [Security and Privacy](langkit/docs/features/security.md)
+- [Security and Privacy](https://github.com/whylabs/langkit/blob/main/langkit/docs/features/security.md)
   - patterns - count of strings matching a user-defined regex pattern group
   - jailbreaks - similarity scores with respect to known jailbreak attempts
   - prompt injection - similarity scores with respect to known prompt injection attacks
   - refusals - similarity scores with respect to known LLM refusal of service responses
-- [Sentiment and Toxicity](langkit/docs/features/sentiment.md)
+- [Sentiment and Toxicity](https://github.com/whylabs/langkit/blob/main/langkit/docs/features/sentiment.md)
   - sentiment analysis
   - toxicity analysis
 
-## Installation
+## Installation 💻
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 
-```bash
+```
 pip install langkit
 ```
 
-## Usage
+## Usage 🚀
 
 LangKit modules contain UDFs that automatically wire into the collection of UDFs on String features provided by whylogs by default. All we have to do is import the LangKit modules and then instantiate a custom schema as shown in the example below.
 
 ```python
-from whylogs.experimental.core.metrics.udf_metric import generate_udf_schema
-from whylogs.core.schema import DeclarativeSchema
 import whylogs as why
-from langkit.sentiment import *
-from langkit.textstat import *
-
-text_schema = DeclarativeSchema(generate_udf_schema())
-results = why.log({"prompt": "hello!", "response": "world!"}, schema=text_schema)
+from whylogs.experimental.core.udf_schema import udf_schema
+from langkit import sentiment
+from langkit import textstat
 
+results = why.log({"prompt": "Hello!", "response": "World!"}, schema=udf_schema())
 ```
 
-The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules.
+The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules. This profile can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
 
-More examples are available [here](https://github.com/whylabs/LanguageToolkit/tree/main/langkit/examples).
+More examples are available [here](https://github.com/whylabs/langkit/tree/main/langkit/examples).
 
-## Modules
+## Modules 📦
 
-You can have more information about the different modules and their metrics [here](langkit/docs/modules.md).
+You can have more information about the different modules and their metrics [here](https://github.com/whylabs/langkit/blob/main/langkit/docs/modules.md).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

