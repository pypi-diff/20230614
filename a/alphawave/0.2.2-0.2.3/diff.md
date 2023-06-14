# Comparing `tmp/alphawave-0.2.2.tar.gz` & `tmp/alphawave-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.2.tar", last modified: Sun Jun 11 21:16:53 2023, max compression
+gzip compressed data, was "alphawave-0.2.3.tar", last modified: Wed Jun 14 16:02:16 2023, max compression
```

## Comparing `alphawave-0.2.2.tar` & `alphawave-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,66 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.2/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-11 21:16:53.053576 alphawave-0.2.2/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.2/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-11 21:16:46.000000 alphawave-0.2.2/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-11 21:16:53.053576 alphawave-0.2.2/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.2/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.2/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.2/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.2/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.2/src/alphawave/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.2/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.2/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.2/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.2/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.2/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.2/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.2/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-09 18:39:01.000000 alphawave-0.2.2/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.2/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.2/src/alphawave/jsonParser.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.2/src/alphawave/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1316 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-11 21:16:53.000000 alphawave-0.2.2/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17857 2023-06-11 20:59:20.000000 alphawave-0.2.2/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.2/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2464 2023-06-11 20:48:55.000000 alphawave-0.2.2/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.2/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.2/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.2/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.2/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.2/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3142 2023-06-11 20:47:19.000000 alphawave-0.2.2/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.2/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.2/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.2/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.2/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.2/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:16:53.053576 alphawave-0.2.2/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.2/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.2/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.2/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.252409 alphawave-0.2.3/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.3/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-14 16:02:16.252409 alphawave-0.2.3/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.3/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-14 15:58:56.000000 alphawave-0.2.3/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-14 16:02:16.252409 alphawave-0.2.3/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.244409 alphawave-0.2.3/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.3/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.3/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.3/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.3/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.3/src/alphawave/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.3/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.3/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.3/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.3/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.3/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.3/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.3/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-13 18:50:06.000000 alphawave-0.2.3/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.3/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.3/src/alphawave/jsonParser.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.3/src/alphawave/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1775 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       36 2023-06-14 16:02:16.000000 alphawave-0.2.3/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17857 2023-06-11 20:59:20.000000 alphawave-0.2.3/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.3/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2464 2023-06-11 20:48:55.000000 alphawave-0.2.3/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.3/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.3/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.3/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.3/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.3/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3142 2023-06-11 20:47:19.000000 alphawave-0.2.3/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.3/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.3/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.3/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.3/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.3/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.248409 alphawave-0.2.3/src/aphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8822 2023-06-11 19:08:17.000000 alphawave-0.2.3/src/aphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.3/src/aphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-11 16:07:13.000000 alphawave-0.2.3/src/aphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4975 2023-06-11 19:09:29.000000 alphawave-0.2.3/src/aphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.3/src/aphawave/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.3/src/aphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.3/src/aphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.3/src/aphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3007 2023-06-11 03:54:19.000000 alphawave-0.2.3/src/aphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      788 2023-06-10 03:00:13.000000 alphawave-0.2.3/src/aphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1503 2023-06-09 18:41:13.000000 alphawave-0.2.3/src/aphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.3/src/aphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1347 2023-06-13 18:50:06.000000 alphawave-0.2.3/src/aphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.3/src/aphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.3/src/aphawave/jsonParser.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.3/src/aphawave/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 16:02:16.252409 alphawave-0.2.3/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.3/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.3/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.3/tests/testSchema.py
```

### Comparing `alphawave-0.2.2/LICENSE` & `alphawave-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/PKG-INFO` & `alphawave-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.2
+Version: 0.2.3
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.2/README.md` & `alphawave-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/pyproject.toml` & `alphawave-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.2/src/alphawave/AlphaWave.py` & `alphawave-0.2.3/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/Colorize.py` & `alphawave-0.2.3/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.3/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.3/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/LLMClient.py` & `alphawave-0.2.3/src/alphawave/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/MemoryFork.py` & `alphawave-0.2.3/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/OSClient.py` & `alphawave-0.2.3/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/OpenAIClient.py` & `alphawave-0.2.3/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/Response.py` & `alphawave-0.2.3/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/TestClient.py` & `alphawave-0.2.3/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/TestClientTest.py` & `alphawave-0.2.3/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.3/src/alphawave/alphawaveTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: 'PromptResponse', remaining_attempts: int) -> 'Promise[Validation]':
         pass
 
 @dataclass
 class PromptCompletionOptions:
     completion_type: str  # 'text' | 'chat'
     model: str
-    max_input_tokens: int =1000
+    max_input_tokens: int =2000
     temperature: float = 0.7
     top_p: float = 1.0
     max_tokens: int = 500
     stop: str = None
     presence_penalty: float = 1.0
     frequency_penalty: float = 1.0
     logit_bias = None
```

### Comparing `alphawave-0.2.2/src/alphawave/internalTypes.py` & `alphawave-0.2.3/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/jsonParser.py` & `alphawave-0.2.3/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave/utilityV2.py` & `alphawave-0.2.3/src/alphawave/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.3/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.2
+Version: 0.2.3
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.2/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.3/src/alphawave.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,10 +32,26 @@
 src/alphawave_agents/MathCommand.py
 src/alphawave_agents/PromptCommand.py
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
+src/aphawave/AlphaWave.py
+src/aphawave/Colorize.py
+src/aphawave/DefaultResponseValidator.py
+src/aphawave/JSONResponseValidator.py
+src/aphawave/LLMClient.py
+src/aphawave/MemoryFork.py
+src/aphawave/OSClient.py
+src/aphawave/OpenAIClient.py
+src/aphawave/Response.py
+src/aphawave/TestClient.py
+src/aphawave/TestClientTest.py
+src/aphawave/__init__.py
+src/aphawave/alphawaveTypes.py
+src/aphawave/internalTypes.py
+src/aphawave/jsonParser.py
+src/aphawave/utilityV2.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.2/src/alphawave_agents/Agent.py` & `alphawave-0.2.3/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.3/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.3/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.3/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.3/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.3/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.3/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.3/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.3/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.3/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.3/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.3/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.3/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/tests/testOSClient.py` & `alphawave-0.2.3/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/tests/testOpenAiClient.py` & `alphawave-0.2.3/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.2/tests/testSchema.py` & `alphawave-0.2.3/tests/testSchema.py`

 * *Files identical despite different names*

