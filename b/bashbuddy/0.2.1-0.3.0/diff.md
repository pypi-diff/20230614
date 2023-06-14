# Comparing `tmp/bashbuddy-0.2.1.tar.gz` & `tmp/bashbuddy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bashbuddy-0.2.1.tar", max compression
+gzip compressed data, was "bashbuddy-0.3.0.tar", max compression
```

## Comparing `bashbuddy-0.2.1.tar` & `bashbuddy-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-03-26 09:35:47.932832 bashbuddy-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2670 2023-03-28 13:54:12.716994 bashbuddy-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-03-26 05:56:54.744694 bashbuddy-0.2.1/bashbuddy/__init__.py
--rw-r--r--   0        0        0      222 2023-03-26 08:58:51.323146 bashbuddy-0.2.1/bashbuddy/__main__.py
--rw-r--r--   0        0        0     1377 2023-03-28 13:48:44.787034 bashbuddy-0.2.1/bashbuddy/agent.py
--rw-r--r--   0        0        0      499 2023-03-28 13:48:17.777038 bashbuddy-0.2.1/bashbuddy/config.py
--rw-r--r--   0        0        0     1945 2023-03-26 08:31:50.853377 bashbuddy-0.2.1/bashbuddy/persistent_bash.py
--rw-r--r--   0        0        0      494 2023-03-28 14:00:05.976947 bashbuddy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 bashbuddy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-16 15:00:14.265517 bashbuddy-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     4123 2023-06-14 20:04:38.307645 bashbuddy-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 15:00:14.265517 bashbuddy-0.3.0/bashbuddy/__init__.py
+-rw-r--r--   0        0        0      594 2023-06-14 19:50:32.289914 bashbuddy-0.3.0/bashbuddy/__main__.py
+-rw-r--r--   0        0        0     2119 2023-06-14 17:05:58.583974 bashbuddy-0.3.0/bashbuddy/agent.py
+-rw-r--r--   0        0        0      504 2023-06-14 17:07:50.642527 bashbuddy-0.3.0/bashbuddy/config.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:03:23.780547 bashbuddy-0.3.0/bashbuddy/tools/__init__.py
+-rw-r--r--   0        0        0     3512 2023-06-14 19:19:28.881784 bashbuddy-0.3.0/bashbuddy/tools/file_tree.py
+-rw-r--r--   0        0        0     1945 2023-05-16 16:03:35.046193 bashbuddy-0.3.0/bashbuddy/tools/persistent_bash.py
+-rw-r--r--   0        0        0      620 2023-06-14 20:05:21.089120 bashbuddy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 bashbuddy-0.3.0/PKG-INFO
```

### Comparing `bashbuddy-0.2.1/LICENSE.md` & `bashbuddy-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bashbuddy-0.2.1/bashbuddy/persistent_bash.py` & `bashbuddy-0.3.0/bashbuddy/tools/persistent_bash.py`

 * *Files identical despite different names*

### Comparing `bashbuddy-0.2.1/PKG-INFO` & `bashbuddy-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,91 @@
 Metadata-Version: 2.1
 Name: bashbuddy
-Version: 0.2.1
+Version: 0.3.0
 Summary: Hook an LLM up to a Bash terminal
 License: MIT
 Author: Omegastick
 Author-email: isaac@poulton.dev
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.0.123,<0.0.124)
-Requires-Dist: openai (>=0.27.2,<0.28.0)
+Requires-Dist: langchain (>=0.0.200,<0.0.201)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: platformdirs (>=3.2.0,<4.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: pyfakefs (>=5.2.2,<6.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # bashbuddy
 
 bashbuddy is an LLM hooked up to a Bash terminal. It's as dangerous as it sounds, but it's also a lot of fun. It's pretty much a proof of concept right now, so expect jank.
 
 ## WARNING
 
 It's recommended to run bashbuddy in a VM. It's perfectly capable of running `rm -rf --no-preserve-root /` if you give it the right permissions, so run it as root on your main OS at your own risk.
 
 ## Installation
 
 ```
-poetry install
+pip install bashbuddy
 ```
 
-Or
+Or clone the repository and run:
 
 ```
-pip install -e .
+poetry install
 ```
 
 You'll also need to put your OpenAI API key in the `OPENAI_API_KEY` environment variable.
 
 ## Usage
 
+You can directly give bashbuddy a command with this:
+```
+bashbuddy -c "<command>"
+```
+
+Or, you can create a "script" for bashbuddy by creating a file with a shebang like this:
+```
+#!/usr/bin/env bashbuddy
+
+<command>
+```
+
+Then, make it executable and run it:
 ```
-bashbuddy "<command>"
+chmod +x <file>
+./<file>
+```
+
+Or you can run it with `bashbuddy <file>`.
+
+`.bb` is just a convention, you can use whatever extension you want. bashbuddy files like this are kind of like *"plain english shell scripts"*. They're super useful for quickly automating complex tasks that would normally require a lot of specicifity, edge case handling, or error handling. As an example:
+```
+#!/usr/bin/env bashbuddy
+
+Pick a random image from my wallpapers directory and set it as my wallpaper. I don't remember where the directory is, but it's probably somewhere in /home/omegastick. I use `feh` to set my wallpapers.
 ```
 
 ## Configuration
 
 You can change the model used by setting the `BASHBUDDY_MODEL` environment variable or setting it in `~/.config/bashbuddy/config.toml`:
 
 ```toml
-model = "gpt-4"  # defaults to gpt-3.5-turbo
+model = "gpt-4-0613"  # defaults to gpt-3.5-turbo-0613
 ```
 
+OpenAI's agent functions are supported, and will automatically be used if one of the `-0613` models is used. From my home testing, it pretty significantly improves capabilities (making `gpt-3.5-turbo` actually useful sometimes).
+
 ## Example
 
+### Manual command
 ````
-$ bashbuddy "Make a new directory called 'test', then put 3 files in it, each containing a haiku. The file name should be the title of the poem."
+$ bashbuddy -c "Make a new directory called 'test', then put 3 files in it, each containing a haiku. The file name should be the title of the poem."
 
 
 > Entering new AgentExecutor chain...
 Question: What is the task?
 Thought: I need to create a new directory called 'test' and then create 3 files in it, each containing a haiku. The file name should be the title of the poem.
 Action:
 ```
@@ -114,7 +141,22 @@
 Softly falling petals kiss
 The ground goodbye, love.
 Winter solitude -
 in a world of one color
 the sound of wind.
 ````
 
+### Command from a file
+```
+$ cat test.bb
+#!/usr/bin/env bashbuddy
+
+Make a new directory called 'test', then put 3 files in it, each containing a haiku. The file name should be the title of the poem.
+
+$ chmod +x test.bb
+$ ./test.bb
+
+
+> Entering new AgentExecutor chain...
+Question: What is the task?
+...
+```
```

