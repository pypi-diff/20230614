# Comparing `tmp/lazer-0.1.8.tar.gz` & `tmp/lazer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.8.tar", max compression
+gzip compressed data, was "lazer-0.1.9.tar", max compression
```

## Comparing `lazer-0.1.8.tar` & `lazer-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.8/LICENSE
--rw-r--r--   0        0        0     1427 2023-06-14 07:59:02.843905 lazer-0.1.8/README.md
--rw-r--r--   0        0        0     3979 2023-06-14 08:03:18.993905 lazer-0.1.8/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 08:03:26.433905 lazer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 lazer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1424 2023-06-14 08:04:56.453905 lazer-0.1.9/README.md
+-rw-r--r--   0        0        0     3979 2023-06-14 08:03:18.993905 lazer-0.1.9/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 08:05:02.063905 lazer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 lazer-0.1.9/PKG-INFO
```

### Comparing `lazer-0.1.8/LICENSE` & `lazer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lazer-0.1.8/README.md` & `lazer-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
-conversation = LazerConversation(backdoor, {"model": "gpt-3.5-turbo-0613"})
+conversation = LazerConversation(lazer, {"model": "gpt-3.5-turbo-0613"})
 response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
```

### Comparing `lazer-0.1.8/lazer/__init__.py` & `lazer-0.1.9/lazer/__init__.py`

 * *Files identical despite different names*

### Comparing `lazer-0.1.8/PKG-INFO` & `lazer-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazer
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
@@ -45,15 +45,15 @@
 
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
-conversation = LazerConversation(backdoor, {"model": "gpt-3.5-turbo-0613"})
+conversation = LazerConversation(lazer, {"model": "gpt-3.5-turbo-0613"})
 response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
```

