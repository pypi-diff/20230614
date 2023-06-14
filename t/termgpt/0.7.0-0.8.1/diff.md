# Comparing `tmp/termgpt-0.7.0.tar.gz` & `tmp/termgpt-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termgpt-0.7.0.tar", last modified: Thu Apr 13 08:16:55 2023, max compression
+gzip compressed data, was "termgpt-0.8.1.tar", last modified: Wed Jun 14 16:26:47 2023, max compression
```

## Comparing `termgpt-0.7.0.tar` & `termgpt-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:16:55.257109 termgpt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-13 08:16:42.000000 termgpt-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:16:55.257109 termgpt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 08:16:42.000000 termgpt-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/termgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/termgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 16:26:47.817546 termgpt-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-14 16:26:16.000000 termgpt-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:26:47.817546 termgpt-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 16:26:16.000000 termgpt-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/models/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 16:26:16.000000 termgpt-0.8.1/termgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:26:47.817546 termgpt-0.8.1/termgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 16:26:47.000000 termgpt-0.8.1/termgpt.egg-info/top_level.txt
```

### Comparing `termgpt-0.7.0/PKG-INFO` & `termgpt-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.7.0
+Version: 0.8.1
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

### Comparing `termgpt-0.7.0/README.md` & `termgpt-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `termgpt-0.7.0/setup.py` & `termgpt-0.8.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,9 +26,10 @@
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
     ],
     entry_points={"console_scripts": ["gpt3=termgpt.chat:gpt3",
-                                      "gpt4=termgpt.chat:gpt4"]},
+                                      "gpt4=termgpt.chat:gpt4",
+                                      "claude=termgpt.chat:claude",]},
 )
```

### Comparing `termgpt-0.7.0/termgpt/roles.py` & `termgpt-0.8.1/termgpt/roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from textwrap import dedent
 from sys import platform
 
 assistant_role = "You are a helpful assistant."
 
 commander_role = dedent(f"""\
-    You are a terminal assistant, the will help me find the right command 
-    to execute to perform the given action.
+    You are a terminal assistant, you will help me find the right terminal
+    command to perform the given action.
     - We are running on {platform}.
     - Reply only with the terminal command required to perform the action. Nothing else. 
     - Reply in plain text, no fancy output.
     - Do not put quotes around the output.
     - If the question is not related to the terminal, just say "I'm not sure how to respond to that
     - If there are multiple ways of performing the same action, reply the simplest one.
     For example, if the questions is "How do I create a new file named "hello.txt?",
```

### Comparing `termgpt-0.7.0/termgpt.egg-info/PKG-INFO` & `termgpt-0.8.1/termgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.7.0
+Version: 0.8.1
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

