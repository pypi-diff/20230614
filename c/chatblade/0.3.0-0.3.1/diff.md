# Comparing `tmp/chatblade-0.3.0.tar.gz` & `tmp/chatblade-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatblade-0.3.0.tar", last modified: Wed May  3 15:13:52 2023, max compression
+gzip compressed data, was "chatblade-0.3.1.tar", last modified: Wed Jun 14 08:06:10 2023, max compression
```

## Comparing `chatblade-0.3.0.tar` & `chatblade-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.346055 chatblade-0.3.0/
--rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.3.0/LICENSE
--rw-r--r--   0 npiv       (501) staff       (20)    10892 2023-05-03 15:13:52.346121 chatblade-0.3.0/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)    10588 2023-05-03 11:32:02.000000 chatblade-0.3.0/README.md
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.345312 chatblade-0.3.0/chatblade/
--rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.3.0/chatblade/__init__.py
--rw-r--r--   0 npiv       (501) staff       (20)      156 2023-04-25 05:44:29.000000 chatblade-0.3.0/chatblade/__main__.py
--rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/chat.py
--rw-r--r--   0 npiv       (501) staff       (20)     4613 2023-04-21 15:19:16.000000 chatblade-0.3.0/chatblade/cli.py
--rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.3.0/chatblade/errors.py
--rw-r--r--   0 npiv       (501) staff       (20)     6054 2023-05-03 11:20:12.000000 chatblade-0.3.0/chatblade/parser.py
--rw-r--r--   0 npiv       (501) staff       (20)     4644 2023-05-03 11:26:22.000000 chatblade-0.3.0/chatblade/printer.py
--rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/session.py
--rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.3.0/chatblade/storage.py
--rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.3.0/chatblade/utils.py
-drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-05-03 15:13:52.345966 chatblade-0.3.0/chatblade.egg-info/
--rw-r--r--   0 npiv       (501) staff       (20)    10892 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/PKG-INFO
--rw-r--r--   0 npiv       (501) staff       (20)      452 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/SOURCES.txt
--rw-r--r--   0 npiv       (501) staff       (20)        1 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/dependency_links.txt
--rw-r--r--   0 npiv       (501) staff       (20)       54 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/entry_points.txt
--rw-r--r--   0 npiv       (501) staff       (20)       49 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/requires.txt
--rw-r--r--   0 npiv       (501) staff       (20)       10 2023-05-03 15:13:52.000000 chatblade-0.3.0/chatblade.egg-info/top_level.txt
--rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.3.0/pyproject.toml
--rw-r--r--   0 npiv       (501) staff       (20)      567 2023-05-03 15:13:52.346512 chatblade-0.3.0/setup.cfg
--rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.3.0/setup.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-06-14 08:06:10.950891 chatblade-0.3.1/
+-rw-r--r--   0 npiv       (501) staff       (20)    34600 2023-03-19 21:07:18.000000 chatblade-0.3.1/LICENSE
+-rw-r--r--   0 npiv       (501) staff       (20)    10868 2023-06-14 08:06:10.950960 chatblade-0.3.1/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)    10564 2023-06-14 08:02:52.000000 chatblade-0.3.1/README.md
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-06-14 08:06:10.945004 chatblade-0.3.1/chatblade/
+-rw-r--r--   0 npiv       (501) staff       (20)        0 2023-03-21 01:08:04.000000 chatblade-0.3.1/chatblade/__init__.py
+-rw-r--r--   0 npiv       (501) staff       (20)      156 2023-04-25 05:44:29.000000 chatblade-0.3.1/chatblade/__main__.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4466 2023-04-02 07:58:37.000000 chatblade-0.3.1/chatblade/chat.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4613 2023-04-21 15:19:16.000000 chatblade-0.3.1/chatblade/cli.py
+-rw-r--r--   0 npiv       (501) staff       (20)       42 2023-03-21 01:25:46.000000 chatblade-0.3.1/chatblade/errors.py
+-rw-r--r--   0 npiv       (501) staff       (20)     6488 2023-06-14 08:02:52.000000 chatblade-0.3.1/chatblade/parser.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4644 2023-05-03 11:26:22.000000 chatblade-0.3.1/chatblade/printer.py
+-rw-r--r--   0 npiv       (501) staff       (20)     1106 2023-04-02 07:58:37.000000 chatblade-0.3.1/chatblade/session.py
+-rw-r--r--   0 npiv       (501) staff       (20)     4079 2023-04-11 09:29:23.000000 chatblade-0.3.1/chatblade/storage.py
+-rw-r--r--   0 npiv       (501) staff       (20)      683 2023-04-02 07:58:37.000000 chatblade-0.3.1/chatblade/utils.py
+drwxr-xr-x   0 npiv       (501) staff       (20)        0 2023-06-14 08:06:10.950794 chatblade-0.3.1/chatblade.egg-info/
+-rw-r--r--   0 npiv       (501) staff       (20)    10868 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/PKG-INFO
+-rw-r--r--   0 npiv       (501) staff       (20)      452 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/SOURCES.txt
+-rw-r--r--   0 npiv       (501) staff       (20)        1 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/dependency_links.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       54 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/entry_points.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       49 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/requires.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       10 2023-06-14 08:06:10.000000 chatblade-0.3.1/chatblade.egg-info/top_level.txt
+-rw-r--r--   0 npiv       (501) staff       (20)       90 2023-03-22 17:02:55.000000 chatblade-0.3.1/pyproject.toml
+-rw-r--r--   0 npiv       (501) staff       (20)      567 2023-06-14 08:06:10.951247 chatblade-0.3.1/setup.cfg
+-rw-r--r--   0 npiv       (501) staff       (20)       38 2023-03-18 13:34:51.000000 chatblade-0.3.1/setup.py
```

### Comparing `chatblade-0.3.0/LICENSE` & `chatblade-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/PKG-INFO` & `chatblade-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,20 +31,14 @@
 
 ### Via Brew
 
 ```
 brew install chatblade
 ```
 
-**Note**: if you were using the brew tap before, you will need to 
-```
-brew untap npiv/chatblade
-brew install chatblade
-```
-
 ## Documentation
 
 ### Making queries
 
 #### A new conversation
 
 You can begin any query by just typing. eg
@@ -73,14 +67,16 @@
 `-l` is shorthand for `-S last` or the last session. We can keep track of and continue various distinct conversations using the [session options](#session-options)
 
 
 #### Picking between gpt-3.5 and 4
 
 By default gpt-3.5 is used, you can switch at any point to 4 by using `-c 4`
 
+or you can pass any arbitrary full model name, eg `-c gpt-3.5-turbo-16k`
+
 #### Chatting interactively
 
 If you would prefer to chat interactively instead just use `chatblade -i`.
 
 #### Show streaming text (experimental)
 
 You can also stream the responses, just like in the webui. At the end of the stream it will format the result. This can be combined in an interactive session
@@ -233,42 +229,41 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
-                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
-                 [query ...]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c CHAT_GPT] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
-  query                           Query to send to chat GPT
+  query                            Query to send to chat GPT
 
 options:
-  -h, --help                      show this help message and exit
-  --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
-  --temperature t                 temperature (openai setting)
-  -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
-  -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
-  -s, --stream                    Stream the incoming text to the terminal
-  -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
+  -h, --help                       show this help message and exit
+  --openai-api-key key             the OpenAI API key can also be set as env variable OPENAI_API_KEY
+  --temperature t                  temperature (openai setting)
+  -c CHAT_GPT, --chat-gpt CHAT_GPT
+                                   chat GPT model 3.5/4 shorthand or full qualified model name, can also be set via env variable OPENAI_API_MODEL
+  -i, --interactive                start an interactive chat session. This will implicitly continue the conversation
+  -s, --stream                     Stream the incoming text to the terminal
+  -t, --tokens                     display what *would* be sent, how many tokens, and estimated costs
+  -p name, --prompt-file name      prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
-  -e, --extract                   extract content from response if possible (either json or code block)
-  -r, --raw                       print session as pure text, don't pretty print or format
-  -n, --no-format                 do not add pretty print formatting to output
-  -o, --only                      Only display the response, omit query
-  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
+  -e, --extract                    extract content from response if possible (either json or code block)
+  -r, --raw                        print session as pure text, don't pretty print or format
+  -n, --no-format                  do not add pretty print formatting to output
+  -o, --only                       Only display the response, omit query
+  --theme theme                    Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
-  -l, --last                      alias for '-S last', the default session if none is specified
-  -S sess, --session sess         initiate or continue named session
-  --session-list                  list sessions
-  --session-path                  show path to session file
-  --session-dump                  dump session to stdout
-  --session-delete                delete session
-  --session-rename newsess        rename session
+  -l, --last                       alias for '-S last', the default session if none is specified
+  -S sess, --session sess          initiate or continue named session
+  --session-list                   list sessions
+  --session-path                   show path to session file
+  --session-dump                   dump session to stdout
+  --session-delete                 delete session
+  --session-rename newsess         rename session
 ```
```

### Comparing `chatblade-0.3.0/README.md` & `chatblade-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,14 @@
 
 ### Via Brew
 
 ```
 brew install chatblade
 ```
 
-**Note**: if you were using the brew tap before, you will need to 
-```
-brew untap npiv/chatblade
-brew install chatblade
-```
-
 ## Documentation
 
 ### Making queries
 
 #### A new conversation
 
 You can begin any query by just typing. eg
@@ -63,14 +57,16 @@
 `-l` is shorthand for `-S last` or the last session. We can keep track of and continue various distinct conversations using the [session options](#session-options)
 
 
 #### Picking between gpt-3.5 and 4
 
 By default gpt-3.5 is used, you can switch at any point to 4 by using `-c 4`
 
+or you can pass any arbitrary full model name, eg `-c gpt-3.5-turbo-16k`
+
 #### Chatting interactively
 
 If you would prefer to chat interactively instead just use `chatblade -i`.
 
 #### Show streaming text (experimental)
 
 You can also stream the responses, just like in the webui. At the end of the stream it will format the result. This can be combined in an interactive session
@@ -223,42 +219,41 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
-                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
-                 [query ...]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c CHAT_GPT] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
-  query                           Query to send to chat GPT
+  query                            Query to send to chat GPT
 
 options:
-  -h, --help                      show this help message and exit
-  --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
-  --temperature t                 temperature (openai setting)
-  -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
-  -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
-  -s, --stream                    Stream the incoming text to the terminal
-  -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
+  -h, --help                       show this help message and exit
+  --openai-api-key key             the OpenAI API key can also be set as env variable OPENAI_API_KEY
+  --temperature t                  temperature (openai setting)
+  -c CHAT_GPT, --chat-gpt CHAT_GPT
+                                   chat GPT model 3.5/4 shorthand or full qualified model name, can also be set via env variable OPENAI_API_MODEL
+  -i, --interactive                start an interactive chat session. This will implicitly continue the conversation
+  -s, --stream                     Stream the incoming text to the terminal
+  -t, --tokens                     display what *would* be sent, how many tokens, and estimated costs
+  -p name, --prompt-file name      prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
-  -e, --extract                   extract content from response if possible (either json or code block)
-  -r, --raw                       print session as pure text, don't pretty print or format
-  -n, --no-format                 do not add pretty print formatting to output
-  -o, --only                      Only display the response, omit query
-  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
+  -e, --extract                    extract content from response if possible (either json or code block)
+  -r, --raw                        print session as pure text, don't pretty print or format
+  -n, --no-format                  do not add pretty print formatting to output
+  -o, --only                       Only display the response, omit query
+  --theme theme                    Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
-  -l, --last                      alias for '-S last', the default session if none is specified
-  -S sess, --session sess         initiate or continue named session
-  --session-list                  list sessions
-  --session-path                  show path to session file
-  --session-dump                  dump session to stdout
-  --session-delete                delete session
-  --session-rename newsess        rename session
+  -l, --last                       alias for '-S last', the default session if none is specified
+  -S sess, --session sess          initiate or continue named session
+  --session-list                   list sessions
+  --session-path                   show path to session file
+  --session-dump                   dump session to stdout
+  --session-delete                 delete session
+  --session-rename newsess         rename session
 ```
```

### Comparing `chatblade-0.3.0/chatblade/chat.py` & `chatblade-0.3.1/chatblade/chat.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade/cli.py` & `chatblade-0.3.1/chatblade/cli.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade/parser.py` & `chatblade-0.3.1/chatblade/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,28 @@
     if options["openai_api_key"]:
         return options["openai_api_key"]
     elif "OPENAI_API_KEY" in os.environ:
         return os.environ["OPENAI_API_KEY"]
     else:
         return None
 
+model_mappings = {"3.5": "gpt-3.5-turbo-0613", "4": "gpt-4-0613"}
+def get_openai_model(options):
+    choice = options["chat_gpt"]
+    if not choice:
+        if "OPENAI_API_MODEL"in os.environ:
+            choice = os.environ["OPENAI_API_MODEL"]
+        else:
+            choice = "3.5"
+
+    if choice in model_mappings:
+        return model_mappings[choice]
+    else:
+        return choice
+
 def get_theme(options):
     if options["theme"]:
         return options["theme"]
     elif "CHATBLADE_THEME" in os.environ:
         return os.environ["CHATBLADE_THEME"]
     else:
         return None
@@ -44,15 +58,15 @@
         return None
 
 
 def extract_options(options):
     options = vars(options)  # to map
     options["openai_api_key"] = get_openai_key(options)
     options["theme"] = get_theme(options)
-    options["model"] = {"3.5": "gpt-3.5-turbo", "4": "gpt-4"}[options["chat_gpt"]]
+    options["model"] = get_openai_model(options)
     del options["query"]
     del options["chat_gpt"]
     return utils.DotDict(options)
 
 
 def valid_session(sess):
     if all(char not in sess for char in ["/", "\\", "\n"]):
@@ -88,15 +102,16 @@
         "--temperature",
         metavar="t",
         type=float,
         help="temperature (openai setting)",
         default=0.0,
     )
     parser.add_argument(
-        "-c", "--chat-gpt", choices=["3.5", "4"], help="chat GPT model", default="3.5"
+        "-c", "--chat-gpt", help="chat GPT model 3.5/4 shorthand or full qualified model name, can also be set via env variable OPENAI_API_MODEL",
+        type=str
     )
     parser.add_argument(
         "-i",
         "--interactive",
         help="start an interactive chat session. This will implicitly continue the conversation",
         action="store_true",
     )
```

### Comparing `chatblade-0.3.0/chatblade/printer.py` & `chatblade-0.3.1/chatblade/printer.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade/session.py` & `chatblade-0.3.1/chatblade/session.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade/storage.py` & `chatblade-0.3.1/chatblade/storage.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade/utils.py` & `chatblade-0.3.1/chatblade/utils.py`

 * *Files identical despite different names*

### Comparing `chatblade-0.3.0/chatblade.egg-info/PKG-INFO` & `chatblade-0.3.1/chatblade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatblade
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI Swiss Army Knife for ChatGPT
 Home-page: https://github.com/npiv/chatblade
 Project-URL: Documentation, https://github.com/npiv/chatblade
 Keywords: chatblade chatgpt cli python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,20 +31,14 @@
 
 ### Via Brew
 
 ```
 brew install chatblade
 ```
 
-**Note**: if you were using the brew tap before, you will need to 
-```
-brew untap npiv/chatblade
-brew install chatblade
-```
-
 ## Documentation
 
 ### Making queries
 
 #### A new conversation
 
 You can begin any query by just typing. eg
@@ -73,14 +67,16 @@
 `-l` is shorthand for `-S last` or the last session. We can keep track of and continue various distinct conversations using the [session options](#session-options)
 
 
 #### Picking between gpt-3.5 and 4
 
 By default gpt-3.5 is used, you can switch at any point to 4 by using `-c 4`
 
+or you can pass any arbitrary full model name, eg `-c gpt-3.5-turbo-16k`
+
 #### Chatting interactively
 
 If you would prefer to chat interactively instead just use `chatblade -i`.
 
 #### Show streaming text (experimental)
 
 You can also stream the responses, just like in the webui. At the end of the stream it will format the result. This can be combined in an interactive session
@@ -233,42 +229,41 @@
 - `OPENAI_API_AZURE_ENGINE` :: name of your deployment in Azure, eg `my-gpt-35-turbo` (maps to a specific model)
 
 *Note*: that this will override any option for `-c 3.5` or `-c 4` which don't make sense in this case.
 
 ### Help
 
 ```
-usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c {3.5,4}] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
-                 [--session-path] [--session-dump] [--session-delete] [--session-rename newsess]
-                 [query ...]
+usage: Chatblade [-h] [--openai-api-key key] [--temperature t] [-c CHAT_GPT] [-i] [-s] [-t] [-p name] [-e] [-r] [-n] [-o] [--theme theme] [-l] [-S sess] [--session-list]
 
 a CLI Swiss Army Knife for ChatGPT
 
 positional arguments:
-  query                           Query to send to chat GPT
+  query                            Query to send to chat GPT
 
 options:
-  -h, --help                      show this help message and exit
-  --openai-api-key key            the OpenAI API key can also be set as env variable OPENAI_API_KEY
-  --temperature t                 temperature (openai setting)
-  -c {3.5,4}, --chat-gpt {3.5,4}  chat GPT model
-  -i, --interactive               start an interactive chat session. This will implicitly continue the conversation
-  -s, --stream                    Stream the incoming text to the terminal
-  -t, --tokens                    display what *would* be sent, how many tokens, and estimated costs
-  -p name, --prompt-file name     prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
+  -h, --help                       show this help message and exit
+  --openai-api-key key             the OpenAI API key can also be set as env variable OPENAI_API_KEY
+  --temperature t                  temperature (openai setting)
+  -c CHAT_GPT, --chat-gpt CHAT_GPT
+                                   chat GPT model 3.5/4 shorthand or full qualified model name, can also be set via env variable OPENAI_API_MODEL
+  -i, --interactive                start an interactive chat session. This will implicitly continue the conversation
+  -s, --stream                     Stream the incoming text to the terminal
+  -t, --tokens                     display what *would* be sent, how many tokens, and estimated costs
+  -p name, --prompt-file name      prompt name - will load the prompt with that name at ~/.config/chatblade/name or a path to a file
 
 result formatting options:
-  -e, --extract                   extract content from response if possible (either json or code block)
-  -r, --raw                       print session as pure text, don't pretty print or format
-  -n, --no-format                 do not add pretty print formatting to output
-  -o, --only                      Only display the response, omit query
-  --theme theme                   Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
+  -e, --extract                    extract content from response if possible (either json or code block)
+  -r, --raw                        print session as pure text, don't pretty print or format
+  -n, --no-format                  do not add pretty print formatting to output
+  -o, --only                       Only display the response, omit query
+  --theme theme                    Set the theme for syntax highlighting see https://pygments.org/styles/, can also be set with CHATBLADE_THEME
 
 session options:
-  -l, --last                      alias for '-S last', the default session if none is specified
-  -S sess, --session sess         initiate or continue named session
-  --session-list                  list sessions
-  --session-path                  show path to session file
-  --session-dump                  dump session to stdout
-  --session-delete                delete session
-  --session-rename newsess        rename session
+  -l, --last                       alias for '-S last', the default session if none is specified
+  -S sess, --session sess          initiate or continue named session
+  --session-list                   list sessions
+  --session-path                   show path to session file
+  --session-dump                   dump session to stdout
+  --session-delete                 delete session
+  --session-rename newsess         rename session
 ```
```

### Comparing `chatblade-0.3.0/setup.cfg` & `chatblade-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chatblade
-version = 0.3.0
+version = 0.3.1
 description = CLI Swiss Army Knife for ChatGPT
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/npiv/chatblade
 keywords = chatblade chatgpt cli python
 project_urls =
```

