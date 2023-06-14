# Comparing `tmp/chatai-agent-1.0.0.tar.gz` & `tmp/chatai-agent-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-agent-1.0.0.tar", last modified: Sat May 27 02:05:35 2023, max compression
+gzip compressed data, was "chatai-agent-1.1.0.tar", last modified: Mon Jun 12 17:19:20 2023, max compression
```

## Comparing `chatai-agent-1.0.0.tar` & `chatai-agent-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-21 01:45:14.000000 chatai-agent-1.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     6097 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1176 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3230 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/src/ChatAIAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       49 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/src/chatai_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:19:20.358882 chatai-agent-1.1.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-28 02:02:45.000000 chatai-agent-1.1.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-12 17:19:20.358882 chatai-agent-1.1.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     6212 2023-06-12 17:17:48.000000 chatai-agent-1.1.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:19:20.358882 chatai-agent-1.1.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-06-12 17:17:48.000000 chatai-agent-1.1.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:19:20.358882 chatai-agent-1.1.0/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3302 2023-06-12 17:17:48.000000 chatai-agent-1.1.0/src/ChatAIAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       50 2023-06-12 17:17:48.000000 chatai-agent-1.1.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:19:20.358882 chatai-agent-1.1.0/src/chatai_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-06-12 17:19:20.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-06-12 17:19:20.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:19:20.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        2 2023-06-12 17:17:48.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-06-12 17:19:20.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-06-12 17:19:20.000000 chatai-agent-1.1.0/src/chatai_agent.egg-info/top_level.txt
```

### Comparing `chatai-agent-1.0.0/LICENSE` & `chatai-agent-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-agent-1.0.0/PKG-INFO` & `chatai-agent-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 1.0.0
+Version: 1.1.0
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-agent-1.0.0/README.md` & `chatai-agent-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ChatAIAgent
 Message broker between user and ChatGPT.
 
 ## The user of this library can
 - easily give role and messages to ChatGPT, and obtain answers.
 - spool messages which given before ChatGPT finish generating current answer.
 
-## Hou to install
+## How to install
 
 ### Install from PyPI
 - Install package to your environment.<br>
     ```install
     $ pip install chatai-agent
     ```
 
@@ -130,33 +130,37 @@
 - No arguments required, nothing returns.
 
 ### disconnect()
 - Request to terminate conversation and calling user callbacks.
 - Internal process will be terminated soon after.
 - No arguments required, nothing returns.
 
+### full_messages()
+- Indicate whether internal message queue is full or not.
+- No argments required, Boolean returns.
+
 And other [threading.Thread](https://docs.python.org/3/library/threading.html) public pethods are available.
 
 ## Callbacks
 ### ask_cb
 - Callback for getting questions that actually thrown to ChatGPT.
 - If you register external info to user message when you put it, you can obtain the external info here.
 - It's not be assumed that any values are returned.
 ### answer_cb
 - Callback for getting question and answer of ChatGPT
 - The type of completion is mentioned [here](https://platform.openai.com/docs/guides/chat).
 - It's not be assumed that any values are returned.
 
 ## Concept of design
-- User message is put on internal queue and treated on internal thiread.<br>
+- User message is put on internal queue and treated on internal thread.<br>
 This feature gives advantage when You put ChatGPT on chat stream.<br>
 Please try [this sample](samples/sample2.py) to experience the benefit.
   ```usage
   $ python3 ./sample2.py VIDEO-ID OpenAI-API-KEY
   ```
   ![](ReadMeParts/ChatAIAgent.gif)
 - The system role given by user remains ever as the oldest sentence of current context even if the number of messages is reached to the maximum, so ChatGPT doesn't forgot the role while current cunversation.
 
 ## Links
-StreamingChaatAgent uses following libraries internally.
+ChatAIAgent uses following libraries internally.
 
 - [streamchat-agent](https://github.com/GeneralYadoc/StreamChatAgent)<br> YouTube chat poller which can get massages very smothly by using internal queue.
```

### Comparing `chatai-agent-1.0.0/setup.py` & `chatai-agent-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-agent",
-    version="1.0.0",
+    version="1.1.0",
     license="MIT",
     description="Send messages to ChatGPT and get answers conveniently.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
@@ -30,8 +30,8 @@
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
     install_requires=_requires_from_file('requirements.txt'),
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov"]
-)
+)
```

### Comparing `chatai-agent-1.0.0/src/ChatAIAgent.py` & `chatai-agent-1.1.0/src/ChatAIAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     self.__keeping_connection = False
 
   def put_message(self, user_message):
     if self.__user_message_queue.full():
       self.__user_message_queue.get()
     self.__user_message_queue.put(user_message)
 
+  def full_messages(self):
+    return self.__user_message_queue.full()
+
   def run(self):
     self.__keeping_connection = True
     while self.__keeping_connection:
       start_time = time.time()
       while self.__keeping_connection and not self.__user_message_queue.empty():
         user_message = self.__user_message_queue.get()
         if self.__ask_cb:
```

### Comparing `chatai-agent-1.0.0/src/chatai_agent.egg-info/PKG-INFO` & `chatai-agent-1.1.0/src/chatai_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 1.0.0
+Version: 1.1.0
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

