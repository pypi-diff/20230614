# Comparing `tmp/chatai-streamer-2.0.1.tar.gz` & `tmp/chatai-streamer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-streamer-2.0.1.tar", last modified: Mon Jun 12 17:53:24 2023, max compression
+gzip compressed data, was "chatai-streamer-2.0.2.tar", last modified: Wed Jun 14 20:50:18 2023, max compression
```

## Comparing `chatai-streamer-2.0.1.tar` & `chatai-streamer-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-2.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13838 2023-06-08 17:50:05.000000 chatai-streamer-2.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2555 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/ChatAIStreamer.py
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4821 2023-06-07 17:58:19.000000 chatai-streamer-2.0.1/src/GttsAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:53:24.008883 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:50:32.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-12 17:53:23.000000 chatai-streamer-2.0.1/src/chatai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:50:18.204445 chatai-streamer-2.0.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 12:23:33.000000 chatai-streamer-2.0.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-14 20:50:18.204445 chatai-streamer-2.0.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    13838 2023-06-14 20:44:17.000000 chatai-streamer-2.0.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-14 20:50:18.204445 chatai-streamer-2.0.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1172 2023-06-14 20:44:37.000000 chatai-streamer-2.0.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:50:18.204445 chatai-streamer-2.0.2/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     2555 2023-06-14 19:53:35.000000 chatai-streamer-2.0.2/src/ChatAIStreamer.py
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     4821 2023-06-07 17:58:19.000000 chatai-streamer-2.0.2/src/GttsAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       83 2023-06-14 20:44:51.000000 chatai-streamer-2.0.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-14 20:50:18.204445 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      604 2023-06-14 20:50:18.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      342 2023-06-14 20:50:18.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-14 20:50:18.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        2 2023-06-14 19:58:21.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      104 2023-06-14 20:50:18.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       39 2023-06-14 20:50:18.000000 chatai-streamer-2.0.2/src/chatai_streamer.egg-info/top_level.txt
```

### Comparing `chatai-streamer-2.0.1/LICENSE` & `chatai-streamer-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-streamer-2.0.1/PKG-INFO` & `chatai-streamer-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 2.0.1
+Version: 2.0.2
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-streamer-2.0.1/README.md` & `chatai-streamer-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,20 +128,20 @@
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
   # The voice generated by GttsGenerator is given.
   def answer_with_voice_cb(user_message, completion, voice):
```

### Comparing `chatai-streamer-2.0.1/setup.py` & `chatai-streamer-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-streamer",
-    version="2.0.1",
+    version="2.0.2",
     license="MIT",
     description="ChatGPT answer aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-streamer-2.0.1/src/ChatAIStreamer.py` & `chatai-streamer-2.0.2/src/ChatAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-2.0.1/src/GttsAIStreamer.py` & `chatai-streamer-2.0.2/src/GttsAIStreamer.py`

 * *Files identical despite different names*

### Comparing `chatai-streamer-2.0.1/src/chatai_streamer.egg-info/PKG-INFO` & `chatai-streamer-2.0.2/src/chatai_streamer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-streamer
-Version: 2.0.1
+Version: 2.0.2
 Summary: ChatGPT answer aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

