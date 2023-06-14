# Comparing `tmp/lazer-0.1.6.tar.gz` & `tmp/lazer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.6.tar", max compression
+gzip compressed data, was "lazer-0.1.7.tar", max compression
```

## Comparing `lazer-0.1.6.tar` & `lazer-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.6/LICENSE
--rw-r--r--   0        0        0     1397 2023-06-14 05:54:08.013905 lazer-0.1.6/README.md
--rw-r--r--   0        0        0     3923 2023-06-14 05:32:15.583905 lazer-0.1.6/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 05:54:41.343905 lazer-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 lazer-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-14 00:37:54.243905 lazer-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1391 2023-06-14 06:13:54.883905 lazer-0.1.7/README.md
+-rw-r--r--   0        0        0     3923 2023-06-14 05:32:15.583905 lazer-0.1.7/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 06:15:31.853905 lazer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 lazer-0.1.7/PKG-INFO
```

### Comparing `lazer-0.1.6/LICENSE` & `lazer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lazer-0.1.6/README.md` & `lazer-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
 conversation = LazerConversation(lazer)
-response = await conversation.talk("What is the qux of 3 and steven")
+response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
 `.dispatch()` to build your own GPT frontend utilizing Lazer.
```

### Comparing `lazer-0.1.6/lazer/__init__.py` & `lazer-0.1.7/lazer/__init__.py`

 * *Files identical despite different names*

### Comparing `lazer-0.1.6/PKG-INFO` & `lazer-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazer
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
@@ -46,15 +46,15 @@
 # GPT is now made aware of your function `qux`
 @lazer.use
 def qux(num: int, name: str) -> str:
     """Retrieve a number and a name from the user and compute the qux of it"""
     return str(num + len(name) * 13)
 
 conversation = LazerConversation(lazer)
-response = await conversation.talk("What is the qux of 3 and steven")
+response = conversation.talk("What is the qux of 3 and steven")
 print(response)
 # ... 117 ...
 ```
 
 > **Note** You do not have to use the LazerConversation GPT frontend, you can simply use
 the Lazer functions `.use` (decorator) and `.get_functions()` as well as
 `.dispatch()` to build your own GPT frontend utilizing Lazer.
```

