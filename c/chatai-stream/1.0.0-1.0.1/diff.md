# Comparing `tmp/chatai-stream-1.0.0.tar.gz` & `tmp/chatai-stream-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-stream-1.0.0.tar", last modified: Mon Jun 12 17:36:35 2023, max compression
+gzip compressed data, was "chatai-stream-1.0.1.tar", last modified: Wed Jun 14 21:10:06 2023, max compression
```

## Comparing `chatai-stream-1.0.0.tar` & `chatai-stream-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-1.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8218 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1695 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/ChatAIStream.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:36:35.188883 chatai-stream-1.0.0/src/chatai_stream.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:34:29.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-12 17:36:35.000000 chatai-stream-1.0.0/src/chatai_stream.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 11:25:30.000000 chatai-stream-1.0.1/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8218 2023-06-14 20:31:00.000000 chatai-stream-1.0.1/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1162 2023-06-14 20:29:35.000000 chatai-stream-1.0.1/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1695 2023-06-12 17:34:29.000000 chatai-stream-1.0.1/src/ChatAIStream.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       51 2023-06-14 20:29:47.000000 chatai-stream-1.0.1/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 21:10:06.084445 chatai-stream-1.0.1/src/chatai_stream.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      594 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      306 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        2 2023-06-14 19:57:58.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       44 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       22 2023-06-14 21:10:06.000000 chatai-stream-1.0.1/src/chatai_stream.egg-info/top_level.txt
```

### Comparing `chatai-stream-1.0.0/LICENSE` & `chatai-stream-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-stream-1.0.0/PKG-INFO` & `chatai-stream-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 1.0.0
+Version: 1.0.1
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-stream-1.0.0/README.md` & `chatai-stream-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,20 +44,20 @@
         break
       print(f"{st[i]}", end='')
       sys.stdout.flush()
       interruptible_sleep(interval_sec)
 
   # Customized sleep for making available of running flag interruption.
   def interruptible_sleep(time_sec):
-    counter = math.floor(time_sec / 0.01)
-    frac = time_sec - (counter * 0.01)
+    counter = math.floor(time_sec / 0.10)
+    frac = time_sec - (counter * 0.10)
     for i in range(counter):
       if not running:
         break
-      time.sleep(0.01)
+      time.sleep(0.10)
     if not running:
       return
     time.sleep(frac)
 
   # callback for getting answer of ChatGPT
   def answer_cb(user_message, completion):
     print(f"\n[{user_message.extern.author.name} {user_message.extern.datetime}] {user_message.message}\n")
```

### Comparing `chatai-stream-1.0.0/setup.py` & `chatai-stream-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-stream",
-    version="1.0.0",
+    version="1.0.1",
     license="MIT",
     description="ChatGPT reacts YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-stream-1.0.0/src/ChatAIStream.py` & `chatai-stream-1.0.1/src/ChatAIStream.py`

 * *Files identical despite different names*

### Comparing `chatai-stream-1.0.0/src/chatai_stream.egg-info/PKG-INFO` & `chatai-stream-1.0.1/src/chatai_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-stream
-Version: 1.0.0
+Version: 1.0.1
 Summary: ChatGPT reacts YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStream
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

