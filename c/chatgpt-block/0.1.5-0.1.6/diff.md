# Comparing `tmp/chatgpt_block-0.1.5.tar.gz` & `tmp/chatgpt_block-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_block-0.1.5.tar", last modified: Sat Apr  1 22:00:07 2023, max compression
+gzip compressed data, was "chatgpt_block-0.1.6.tar", last modified: Wed Jun 14 09:13:12 2023, max compression
```

## Comparing `chatgpt_block-0.1.5.tar` & `chatgpt_block-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-04-01 22:00:07.601549 chatgpt_block-0.1.5/
--rw-r--r--   0 suka-      (501) staff       (20)     1077 2023-03-28 22:53:10.000000 chatgpt_block-0.1.5/LICENSE
--rw-r--r--   0 suka-      (501) staff       (20)     5356 2023-04-01 22:00:07.601438 chatgpt_block-0.1.5/PKG-INFO
--rw-r--r--   0 suka-      (501) staff       (20)     5236 2023-03-29 23:31:34.000000 chatgpt_block-0.1.5/README.md
-drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-04-01 22:00:07.600736 chatgpt_block-0.1.5/chatgpt_block/
--rw-r--r--   0 suka-      (501) staff       (20)       63 2023-04-01 20:19:04.000000 chatgpt_block-0.1.5/chatgpt_block/__init__.py
--rw-r--r--   0 suka-      (501) staff       (20)    13777 2023-04-01 20:26:54.000000 chatgpt_block-0.1.5/chatgpt_block/chatgpt_block.py
-drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-04-01 22:00:07.601284 chatgpt_block-0.1.5/chatgpt_block.egg-info/
--rw-r--r--   0 suka-      (501) staff       (20)     5356 2023-04-01 22:00:07.000000 chatgpt_block-0.1.5/chatgpt_block.egg-info/PKG-INFO
--rw-r--r--   0 suka-      (501) staff       (20)      267 2023-04-01 22:00:07.000000 chatgpt_block-0.1.5/chatgpt_block.egg-info/SOURCES.txt
--rw-r--r--   0 suka-      (501) staff       (20)        1 2023-04-01 22:00:07.000000 chatgpt_block-0.1.5/chatgpt_block.egg-info/dependency_links.txt
--rw-r--r--   0 suka-      (501) staff       (20)       48 2023-04-01 22:00:07.000000 chatgpt_block-0.1.5/chatgpt_block.egg-info/requires.txt
--rw-r--r--   0 suka-      (501) staff       (20)       14 2023-04-01 22:00:07.000000 chatgpt_block-0.1.5/chatgpt_block.egg-info/top_level.txt
--rw-r--r--   0 suka-      (501) staff       (20)       38 2023-04-01 22:00:07.601592 chatgpt_block-0.1.5/setup.cfg
--rw-r--r--   0 suka-      (501) staff       (20)      497 2023-04-01 20:19:04.000000 chatgpt_block-0.1.5/setup.py
+drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-06-14 09:13:12.488367 chatgpt_block-0.1.6/
+-rw-r--r--   0 suka-      (501) staff       (20)     1077 2023-03-28 22:53:10.000000 chatgpt_block-0.1.6/LICENSE
+-rw-r--r--   0 suka-      (501) staff       (20)     5356 2023-06-14 09:13:12.488231 chatgpt_block-0.1.6/PKG-INFO
+-rw-r--r--   0 suka-      (501) staff       (20)     5236 2023-03-29 23:31:34.000000 chatgpt_block-0.1.6/README.md
+drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-06-14 09:13:12.487246 chatgpt_block-0.1.6/chatgpt_block/
+-rw-r--r--   0 suka-      (501) staff       (20)       63 2023-06-14 09:10:41.000000 chatgpt_block-0.1.6/chatgpt_block/__init__.py
+-rw-r--r--   0 suka-      (501) staff       (20)    13916 2023-06-14 09:11:24.000000 chatgpt_block-0.1.6/chatgpt_block/chatgpt_block.py
+drwxr-xr-x   0 suka-      (501) staff       (20)        0 2023-06-14 09:13:12.488043 chatgpt_block-0.1.6/chatgpt_block.egg-info/
+-rw-r--r--   0 suka-      (501) staff       (20)     5356 2023-06-14 09:13:12.000000 chatgpt_block-0.1.6/chatgpt_block.egg-info/PKG-INFO
+-rw-r--r--   0 suka-      (501) staff       (20)      267 2023-06-14 09:13:12.000000 chatgpt_block-0.1.6/chatgpt_block.egg-info/SOURCES.txt
+-rw-r--r--   0 suka-      (501) staff       (20)        1 2023-06-14 09:13:12.000000 chatgpt_block-0.1.6/chatgpt_block.egg-info/dependency_links.txt
+-rw-r--r--   0 suka-      (501) staff       (20)       48 2023-06-14 09:13:12.000000 chatgpt_block-0.1.6/chatgpt_block.egg-info/requires.txt
+-rw-r--r--   0 suka-      (501) staff       (20)       14 2023-06-14 09:13:12.000000 chatgpt_block-0.1.6/chatgpt_block.egg-info/top_level.txt
+-rw-r--r--   0 suka-      (501) staff       (20)       38 2023-06-14 09:13:12.488411 chatgpt_block-0.1.6/setup.cfg
+-rw-r--r--   0 suka-      (501) staff       (20)      497 2023-06-14 09:10:41.000000 chatgpt_block-0.1.6/setup.py
```

### Comparing `chatgpt_block-0.1.5/LICENSE` & `chatgpt_block-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_block-0.1.5/PKG-INFO` & `chatgpt_block-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_block
-Version: 0.1.5
+Version: 0.1.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPTBlock
 A Python package for interacting with OpenAI's chat models through the OpenAI API.
 
 ## Table Of Contents
```

### Comparing `chatgpt_block-0.1.5/README.md` & `chatgpt_block-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_block-0.1.5/chatgpt_block/chatgpt_block.py` & `chatgpt_block-0.1.6/chatgpt_block/chatgpt_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,18 +37,22 @@
 
     def __next__(self):
         return next(self.generator)
 
 
 class ChatGPTBlock:
     max_tokens_by_model = {
-        'gpt-3.5-turbo': 4097,
-        'gpt-3.5-turbo-0301': 4097,
-        'gpt-4': 8192,
-        'gpt-4-0314': 8192,
+        'gpt-3.5-turbo': 4096,
+        'gpt-3.5-turbo-0301':4096,
+        'gpt-3.5-turbo-0613': 4096,
+        'gpt-3.5-turbo-16k': 16384,
+        'gpt-3.5-turbo-16k-0613': 16384,
+        'gpt-4': 8096,
+        'gpt-4-0314': 8096,
+        'gpt-4-0613': 8096
     }
 
     """
     A class for interacting with OpenAI's chat model through the API.
     """
 
     def __init__(
```

### Comparing `chatgpt_block-0.1.5/chatgpt_block.egg-info/PKG-INFO` & `chatgpt_block-0.1.6/chatgpt_block.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-block
-Version: 0.1.5
+Version: 0.1.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPTBlock
 A Python package for interacting with OpenAI's chat models through the OpenAI API.
 
 ## Table Of Contents
```

