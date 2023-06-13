# Comparing `tmp/gptbase-0.2.3.tar.gz` & `tmp/gptbase-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptbase-0.2.3.tar", last modified: Tue Jun 13 22:38:25 2023, max compression
+gzip compressed data, was "gptbase-0.2.4.tar", last modified: Tue Jun 13 22:42:21 2023, max compression
```

## Comparing `gptbase-0.2.3.tar` & `gptbase-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:38:25.238841 gptbase-0.2.3/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)     3455 2023-06-13 22:33:12.000000 gptbase-0.2.3/README.md
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/gptbase/
--rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.2.3/gptbase/__init__.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-06-04 12:19:20.000000 gptbase-0.2.3/gptbase/base.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)    10729 2023-06-13 22:17:25.000000 gptbase-0.2.3/gptbase/basev2.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      677 2023-06-13 22:35:49.000000 gptbase-0.2.3/gptbase/chat.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      110 2023-05-28 09:47:37.000000 gptbase-0.2.3/gptbase/const.py
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/gptbase.egg-info/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)      293 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/SOURCES.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/dependency_links.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       51 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/entry_points.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       57 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/requires.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/top_level.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-06-13 22:38:25.238841 gptbase-0.2.3/setup.cfg
--rw-r--r--   0 ershan    (1000) ershan    (1000)      947 2023-06-13 22:36:37.000000 gptbase-0.2.3/setup.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:42:21.448820 gptbase-0.2.4/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:42:21.448820 gptbase-0.2.4/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3455 2023-06-13 22:33:12.000000 gptbase-0.2.4/README.md
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:42:21.448820 gptbase-0.2.4/gptbase/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.2.4/gptbase/__init__.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-06-04 12:19:20.000000 gptbase-0.2.4/gptbase/base.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)    10729 2023-06-13 22:17:25.000000 gptbase-0.2.4/gptbase/basev2.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      784 2023-06-13 22:41:33.000000 gptbase-0.2.4/gptbase/chat.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      110 2023-05-28 09:47:37.000000 gptbase-0.2.4/gptbase/const.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:42:21.448820 gptbase-0.2.4/gptbase.egg-info/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      293 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/SOURCES.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/dependency_links.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       51 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/entry_points.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       57 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/requires.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-06-13 22:42:21.000000 gptbase-0.2.4/gptbase.egg-info/top_level.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-06-13 22:42:21.448820 gptbase-0.2.4/setup.cfg
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      947 2023-06-13 22:41:58.000000 gptbase-0.2.4/setup.py
```

### Comparing `gptbase-0.2.3/PKG-INFO` & `gptbase-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptbase
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.
 Home-page: https://github.com/callmexss/gptbase
 Author: callmexss
 Author-email: callmexss@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gptbase-0.2.3/README.md` & `gptbase-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gptbase-0.2.3/gptbase/base.py` & `gptbase-0.2.4/gptbase/base.py`

 * *Files identical despite different names*

### Comparing `gptbase-0.2.3/gptbase/basev2.py` & `gptbase-0.2.4/gptbase/basev2.py`

 * *Files identical despite different names*

### Comparing `gptbase-0.2.3/gptbase/chat.py` & `gptbase-0.2.4/gptbase/chat.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 @click.command()
 @click.option('--memory-turns', default=3, help='Number of memory turns.')
 @click.option('--system-prompt', default='', help='System prompt.')
 def chat(memory_turns, system_prompt):
     cm = CompletionParameters(stream=True)
     chat = ChatAssistant(memory_turns, system_prompt)
+    print("Welcome to Chat build with GPTBase!")
+    print("You can exit by hit ctrl c or typing `exit`.")
     while True:
         try:
             message = input(">>> ")
             if message == "exit":
                 break
             chat.chat(message, cm)
         except KeyboardInterrupt:
```

### Comparing `gptbase-0.2.3/gptbase.egg-info/PKG-INFO` & `gptbase-0.2.4/gptbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptbase
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.
 Home-page: https://github.com/callmexss/gptbase
 Author: callmexss
 Author-email: callmexss@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gptbase-0.2.3/setup.py` & `gptbase-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gptbase",
-    version="0.2.3",
+    version="0.2.4",
     author="callmexss",
     author_email="callmexss@126.com",
     description="A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/callmexss/gptbase",
     packages=find_packages(include=["gptbase"]),
```

