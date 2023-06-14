# Comparing `tmp/agency-1.0.0.tar.gz` & `tmp/agency-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.0.0.tar", max compression
+gzip compressed data, was "agency-1.0.1.tar", max compression
```

## Comparing `agency-1.0.0.tar` & `agency-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 agency-1.0.0/LICENSE
--rw-r--r--   0        0        0    24851 2023-06-12 21:57:53.079633 agency-1.0.0/README.md
--rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 agency-1.0.0/agency/__init__.py
--rw-r--r--   0        0        0    10606 2023-06-12 20:36:46.457220 agency-1.0.0/agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 agency-1.0.0/agency/agents/__init__.py
--rw-r--r--   0        0        0     2791 2023-06-12 21:57:53.079991 agency-1.0.0/agency/agents/chattyai.py
--rw-r--r--   0        0        0     2715 2023-06-12 20:36:46.457186 agency-1.0.0/agency/agents/demo_agent.py
--rw-r--r--   0        0        0     2202 2023-06-12 20:36:46.457242 agency-1.0.0/agency/agents/host.py
--rw-r--r--   0        0        0     1519 2023-06-12 20:36:46.457203 agency-1.0.0/agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 agency-1.0.0/agency/schema.py
--rwxr-xr-x   0        0        0     3232 2023-06-12 20:36:46.457170 agency-1.0.0/agency/space.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 agency-1.0.0/agency/spaces/__init__.py
--rw-r--r--   0        0        0     6149 2023-06-12 08:15:54.596300 agency-1.0.0/agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4010 2023-06-12 20:36:46.457499 agency-1.0.0/agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 agency-1.0.0/agency/util.py
--rw-r--r--   0        0        0      568 2023-06-12 21:57:53.080270 agency-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    25701 1970-01-01 00:00:00.000000 agency-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 agency-1.0.1/LICENSE
+-rw-r--r--   0        0        0    25810 2023-06-14 13:13:25.936547 agency-1.0.1/README.md
+-rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 agency-1.0.1/agency/__init__.py
+-rw-r--r--   0        0        0    10785 2023-06-14 13:13:25.936902 agency-1.0.1/agency/agent.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 agency-1.0.1/agency/agents/__init__.py
+-rw-r--r--   0        0        0     2791 2023-06-12 21:57:53.079991 agency-1.0.1/agency/agents/chattyai.py
+-rw-r--r--   0        0        0     2202 2023-06-12 20:36:46.457242 agency-1.0.1/agency/agents/host.py
+-rw-r--r--   0        0        0     2729 2023-06-14 13:13:25.937150 agency-1.0.1/agency/agents/openai_completion_agent.py
+-rw-r--r--   0        0        0     7797 2023-06-14 13:13:25.937407 agency-1.0.1/agency/agents/openai_function_agent.py
+-rw-r--r--   0        0        0     1519 2023-06-12 20:36:46.457203 agency-1.0.1/agency/agents/prompt_methods.py
+-rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 agency-1.0.1/agency/schema.py
+-rwxr-xr-x   0        0        0     3261 2023-06-14 13:13:25.937665 agency-1.0.1/agency/space.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 agency-1.0.1/agency/spaces/__init__.py
+-rw-r--r--   0        0        0     6646 2023-06-14 13:13:25.937925 agency-1.0.1/agency/spaces/templates/index.html
+-rw-r--r--   0        0        0     4027 2023-06-14 13:13:25.938200 agency-1.0.1/agency/spaces/web_app.py
+-rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 agency-1.0.1/agency/util.py
+-rw-r--r--   0        0        0      557 2023-06-14 13:17:07.822930 agency-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    26649 1970-01-01 00:00:00.000000 agency-1.0.1/PKG-INFO
```

### Comparing `agency-1.0.0/LICENSE` & `agency-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/README.md` & `agency-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: agency
+Version: 1.0.1
+Summary: A fast and minimal foundation for unifying human, AI, and other computing systems
+License: GPL-3.0
+Author: Daniel Rodriguez
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask-SocketIO (>=5.3,<6.0)
+Requires-Dist: asyncio (>=3.4,<4.0)
+Requires-Dist: colorama (>=0.4,<0.5)
+Requires-Dist: eventlet (>=0.33,<0.34)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pydantic (>=1.8,<2.0)
+Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: transformers (>=4.29,<5.0)
+Description-Content-Type: text/markdown
+
 # `agency`
 
 A fast and minimal foundation for unifying human, AI, and other computing
 systems, in python
 
 
 ## What is `agency`?
@@ -27,16 +49,16 @@
 - ...
 - anything
 
 
 # Install
 > **WARNING:**\
 Running `agency` may result in exposing your computer to access by any connected
-`Agent` class including AI agents. Please understand the risks before using this
-software and do not configure it for OS access otherwise.\
+`Agent` class. Please understand the risks before using this software and do not
+configure it for OS access otherwise.\
 \
 If you want to enable OS access, to allow for file I/O for example, I HIGHLY
 RECOMMEND running your project within a Docker container to prevent direct
 access to your host, allowing you to limit the resources and directories that
 may be accessed.
 
 ```sh
@@ -50,35 +72,31 @@
 model](https://en.wikipedia.org/wiki/Actor_model) intended for integrating AI,
 human, and traditional computing systems.
 
 In `agency`, all entities are called "agents" and represented as instances
 of the `Agent` class. This includes all humans, software, and AI-driven agents.
 
 The `Agent` class is a base class similar to "Object" in many object-oriented
-languages. All agents may expose "actions" which can be invoked by other
-agents, by simply defining instance methods on the class.
+languages. All agents may expose "actions" that other agents can discover and
+invoke at run time. Actions also specify an access policy, allowing you to
+monitor and control actions to ensure safety.
 
 A `Space` is also an `Agent` and is used to group multiple agents together.
 
 A space can be thought of as both a collection of agents and a "router" for
 their communication. An agent cannot communicate with others until it is first
 added to a space.
 
 Spaces may be nested, allowing for namespacing and hierarchical organization of
 the agents in your application.
 
-All agents may define public "actions" that other agents can discover and invoke
-at run time. Actions also specify an access policy, allowing you to monitor and
-control actions to ensure safety.
-
 To summarize, the two classes of `Agent` and `Space` together create a simple
-API for defining applications that may mix AI, human, and traditional computing
+API for creating applications that may mix AI, human, and traditional computing
 systems, in a way that is intended for all to equally understand and use.
 
-
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
 > Please note that the example classes used in this walkthrough are implemented
 for you to explore and try out, but should be considered "proof of concept"
@@ -203,23 +221,23 @@
 
 This is an example of the full message schema that is used for all messages sent
 between agents in `agency`. This format is intended to be simple and extensible
 enough to support any use case while remaining human readable.
 
 Note that the `"thoughts"` field is defined as a distinct argument for providing
 a natural language explanation to accompany any action, but as of this writing
-`ChattyAI` does not make use of it. `DemoAgent` discussed below, does.
+`ChattyAI` does not make use of it. `OpenAICompletionAgent` discussed below,
+does.
 
 For more details on the common message schema see
 [schema.py](./agency/schema.py).
 
 
 ## Access Control
 
-
 All actions must declare an access policy like the following example seen above
 the `ChattyAI._action__say()` method:
 
 ```python
 @access_policy(ACCESS_PERMITTED)
 def _action__say(self, content: str):
     """Use this action to say something to Chatty"""
@@ -245,37 +263,37 @@
 
 ```python
 def _request_permission(self, proposed_message: MessageSchema) -> bool:
     ...
 ```
 
 This method is called when an agent attempts to invoke an action that has been
-marked as `ACCESS_REQUESTED`. Your method should inspect the `proposed_message`
-and return a boolean indicating whether or not to permit the action.
+marked as `ACCESS_REQUESTED`. Your method should inspect `proposed_message` and
+return a boolean indicating whether or not to permit the action.
 
 You can use this approach to protect against dangerous actions being taken. For
 example if you allow terminal access, you may want to review commands before
 they are invoked.
 
 This implementation of access control is just a start, and further development
-of the mechanics is a priority for this project.
+of the functionality is a priority for this project.
 
 
 ## Adding Human Users With the `WebApp` Class
 
 A single chatting AI wouldn't be useful without someone to chat with, so now
 let's add humans into the space so that they can chat with "Chatty". To do
 this, we'll use the `WebApp` class, which is a subclass of `Space`.
 
 Why choose to subclass `Space` and not `Agent`? This is an arbitrary choice up
 to the developer, and may depend on what they want to accomplish.
 
 We could implement `WebApp` as a subclass of `Agent`. This would represent the
 web application as a single agent within the system. Users of the web
-application would not be able to be addressed individually by agents.
+application would not be able to be addressed individually by other agents.
 
 But since a typical web application serves multiple users, it may make sense to
 implement it as a `Space` subclass, so that individual users of the web
 application can be addressed by other agents using a namespace associated with
 the web application, as we'll see below.
 
 So this is _not_ the only way this could be accomplished but is intended as a
@@ -294,28 +312,29 @@
 `Agent` and is called `WebAppUser`.
 
 The `WebAppUser` class is where we define the actions that an individual web app
 user may expose to others.
 
 Using the `asyncio` library you'll see that we simply forward messages as-is to
 the `React` frontend, and allow the client code to handle rendering and parsing
-of input as actions back to the `Flask` application, which routes them to their
-intended receiver in the space.
+of input as actions back to the `Flask` application, which forwards them to
+their intended receiver in the space.
 
 This way, we allow individual web users to appear as individual agents to others
 in the space.
 
 
 ## Namespacing and Adding the Web Application
 
 Now that we've defined our new `WebApp` class, we can add it to `DemoSpace`
 with:
 
 ```python
-space.add(WebApp("WebApp", port=os.getenv('WEB_APP_PORT')))
+space.add(
+    WebApp("WebApp", port='8080'))
 ```
 
 Whenever any agent is added to a space, its fully qualified `id` becomes
 namespaced with the space's `id`.
 
 For example, after running the line above the `WebApp` being an agent as well,
 receives an `id` of `"WebApp.DemoSpace"`.
@@ -325,16 +344,17 @@
 
 - `"DemoSpace"` - The root space
 - `"ChattyAI.DemoSpace"` - ChattyAI's fully qualified `id`
 - `"WebApp.DemoSpace"` - the root of the `"WebApp"` space
 
 Users of the web application, as they log in or out, may be added dynamically
 under the `"WebApp"` namespace allowing them to be addressed with a fully
-qualified `id` of, for example `"Dan.WebApp.DemoSpace"`.
+qualified `id` of, for example:
 
+- `"Dan.WebApp.DemoSpace"`.
 
 _(Note that login/out functionality is not implemented as of this writing.)_
 
 
 ## Adding OS Access with the `Host` class
 
 At this point, we have a system where human users of the web application can
@@ -362,41 +382,41 @@
 
 By declaring this access policy, all actions on the host will require a
 confirmation from the terminal where the application is being run. This is
 thanks to the implementation of `_request_permission()` in the `Host` class.
 
 Note that this implementation of `_request_permission()` is just one
 possibility. We could have implemented, for example, a phone notification for a
-human to review from anywhere.
+human to review from elsewhere.
 
 
 ## Discovering Actions
 
 At this point, we can demonstrate how discovery works from the perspective of
 a human user of the web application.
 
 Once added to a space, each agent may send a `help` message to discover other
 agents and actions that are available in the space.
 
-The `WebApp` which hosts a simple chat UI supports a "slash" syntax summarized
-here:
+The `WebApp` application hosts a simple chat UI that supports a "slash" syntax
+summarized here:
 
 ```python
 /actionname arg1:val1 arg2:val2 ...
 ```
 
-So a person using the chat UI can discover available actions with:
+So a person using the chat UI can discover available actions by typing:
 
 ```
 /help
 ```
 
 This will broadcast a `help` action to all other agents, who will individually
 respond with a list of their available actions. The returned list of actions
-from the `Host` agent, would look something like:
+would look something like:
 
 ```python
 [
     {
         "to": "Host.DemoSpace",
         "action": "delete_file",
         "thoughts": "Delete a file",
@@ -408,14 +428,22 @@
         "to": "Host.DemoSpace",
         "action": "list_files",
         "thoughts": "List files in a directory",
         "args": {
           "directory_path": "str"
         }
     },
+    {
+        "to": "ChattyAI.DemoSpace",
+        "action": "say",
+        "thoughts": "Use this action to say something to Chatty",
+        "args": {
+          "content": "str"
+        }
+    },
     ...
 ]
 ```
 
 Notice that each action lists the fully qualified `id` of the agent in the
 `"to"` field, the docstring of the action's method in the `"thoughts"` field,
 and each argument along with its type in the `"args"` field.
@@ -425,18 +453,18 @@
 
 ```
 /list_files to:Host.DemoSpace directory_path:/app
 ```
 
 This will send the `list_files` action to the `Host` agent who will (after being
 granted permission) return the results back to `"Dan.WebApp.DemoSpace"`
-rendering it to the web user interface.
+rendering it to the web user interface as a message.
 
 Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
-field
+field.
 
 
 ## Broadcast vs Point-to-Point Messaging
 
 If we omit the `to:Host.DemoSpace` portion of the command above, the message
 will be broadcast, and any agents who implement a `list_files` action will
 respond.
@@ -459,120 +487,110 @@
 
 Finally we get to the good part!
 
 We'll now add an intelligent agent into this environment and see that it is able
 to understand and interact with any of the systems or humans we've connected
 thus far.
 
-To add the [`DemoAgent`](./agency/agents/demo_agent.py) class to the
+> Note that the following `OpenAIFunctionAgent` class uses the newly released
+[openai function calling
+API](https://platform.openai.com/docs/guides/gpt/function-calling).
+
+To add the [`OpenAIFunctionAgent`](./agency/agents/demo_agent.py) class to the
 environment:
 ```python
 space.add(
-    DemoAgent("Demo",
-        model="text-davinci-003",
-        openai_api_key=os.getenv("OPENAI_API_KEY")))
-```
-
-Note that the `DemoAgent` class is implemented to use the OpenAI API as a
-language model backend. I recommend using language models on par with GPT-3.5 or
-better for the best results with tool-using agents such as this.
-
-
-### The `DemoAgent` Prompt
-
-What makes the `DemoAgent` able to intelligently discover and interact with
-others is largely embodied in the `DemoAgent._prompt_head()` method. In it
-you'll notice a few things:
-
-1. The prompt is written from the first person perspective as though it is the
-agent's own thoughts. This differs slightly from common practice, which usually
-uses the second-person perspective. I do not think this makes a large difference
-but was worth mentioning. This is more of a personal preference.
-
-1. I frame the situation clearly and accurately for the agent, telling it enough
-about who it is, its goals, and the JSON format that it uses to communicate.
-
-1. I "pretend" that the bottom portion is a terminal application. By signaling a
-change in context with the `%%%%% Terminal %%%%%` header, we help make clear to
-the language model that this is a distinct section of content with its own text
-patterns to continue. I do not believe that this is a crucial technique either,
-but is worth noting.
-
-1. I use the `_message_log_to_list()` method to dynamically insert the previous
-conversation up to the current point. See the mixin class `PromptMethods` for
-the implementation. There is no summarization used, so the current
-implementation will eventually hit the context window after a short time.
-
-1. I insert a fake event at the beginning of the terminal portion of the prompt,
-pretending that the agent themself executed the `help` action proactively, and
-display the resulting list of available actions. This is just a neat way to
-insert the available actions while keeping the supposed context of the terminal,
-and providing a one-shot example to begin from.
-
-Note that `ChattyAI` uses a more typical prompt, showing that prompt style and
-technique need not be shared by all agents connected to a space, but can be
-entirely unique to each agent.
+    OpenAIFunctionAgent("FunctionAI",
+        model="gpt-3.5-turbo-16k",
+        openai_api_key=os.getenv("OPENAI_API_KEY"),
+        # user_id determines the "user" role in the chat API
+        user_id="Dan.WebApp.DemoSpace"))
+```
+
+The `user_id` argument determines which agent is represented as the "user" role
+to the chat API. Since the chat API is limited to a predefined set of roles, we
+need to indicate which is the main "user".
+
+For an implementation that uses a plain text completion API, see
+[`OpenAICompletionAgent`](./agency/agents/openai_completion_agent.py).
 
 
 ## Complete Demo Implementation
 
 The following is the full implementation (minus imports) of the above
-walkthrough that you can try out on your own. Note that `Space.run()` starts a
+walkthrough that you can try out on your own, including both OpenAI agent
+examples and the HuggingFace based "Chatty". Note that `Space.run()` starts a
 thread, so we simply keep the application alive with a while loop.
 
 ```python
 # demo.py
 
 if __name__ == '__main__':
 
     space = Space("DemoSpace") 
 
     space.add(
-        WebApp("WebApp", port=os.getenv('WEB_APP_PORT')))
+        WebApp("WebApp",
+            demo_user_id="Dan", # hardcoded for simplicity
+            port='8080'))
 
     space.add(
-        ChattyAI("Chatty", model="EleutherAI/gpt-neo-125m"))
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
 
     space.add(
         Host("Host"))
 
     space.add(
-        DemoAgent("Demo",
+        OpenAIFunctionAgent("FunctionAI",
+            model="gpt-3.5-turbo-16k",
+            openai_api_key=os.getenv("OPENAI_API_KEY"),
+            # user_id determines the "user" role in the OpenAI chat
+            user_id="Dan.WebApp.DemoSpace"))
+
+    space.add(
+        OpenAICompletionAgent("CompletionAI",
             model="text-davinci-003",
             openai_api_key=os.getenv("OPENAI_API_KEY")))
 
     space.run()
 
+    print("pop!")
+
     # keep alive
     while True:
         time.sleep(1)
 ```
 
 If you run the above python script, after a short boot time you can visit the
-web app at `localhost:$WEB_APP_PORT` and you should see a simple chat interface.
+web app at `http://localhost:8080` and you should see a simple chat interface.
 
-The following is a screenshot of a conversation that showcases `DemoAgent`'s
-ability to intelligently interact with the other agents in the environment,
-including running commands on the host, or chatting with "Chatty".
+The following is a screenshot of a conversation that showcases all the agents
+intelligently interacting and following orders.
 
 Note that my messages are broadcasted in the below conversation, which explains
-why Chatty responds to each message as does "Demo". There is an obvious
-difference in quality, of course.
+why all three respond to each message. There is an obvious difference in
+quality, of course.
 
-I also demonstrate the results of rejecting an action and asking Demo to use a
-different approach.
+I also demonstrate the results of rejecting an action and directing an agent to
+use a different approach.
 
-Behind the scenes, Demo messaged Chatty directly and correctly relayed her
-response, and after I explained my rejection of the `read_file` action, Demo
-used the `shell_command` action with `wc -l Dockerfile` which was more
-appropriate. And the file indeed has 75 lines.
+After I explained my rejection of the `read_file` action (which happened behind
+the scenes on the terminal), "FunctionAI" appropriately used the `shell_command`
+action with `wc -l Dockerfile`. The Dockerfile indeed has 73 lines.
+
+CompletionAI used that command on the first try. Anecdotally as of this writing,
+`CompletionAI` seems to be more accurate, even though it is using the text
+completion API vs the function calling feature of the chat API. This may be due
+to the implementation or issues arising from the translation into roles
+discussed elsewhere.
 
 <p align="center">
-  <img src="https://i.ibb.co/f1GMb5P/Screenshot-2023-06-10-at-11-50-42-PM.png"
-       alt="Screenshot-2023-06-10-at-11-50-42-PM" border="0" width=500>
+  <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
+       alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
 </p>
 
 
 # Hypothetical Examples
 
 The following examples are not implemented, but are presented as additional
 ideas for integrations that `agency` could support.
@@ -629,17 +647,17 @@
 
 
 # FAQ
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
-`agency` (see [`DemoAgent`](./agency/agents/demo_agent.py)), it is not intended
-to be a full-fledged agent toolset. It can be thought of as an "agent
-integration framework".
+`agency` (see [`agents/`](./agency/agents/)), it is not intended to be a
+full-fledged agent toolset. It can be thought of as an "agent integration
+framework".
 
 Projects like LangChain and others are exploring how to create purpose-built
 agents that solve diverse problems using tools.
 
 `agency` is concerned with creating a safe and dynamic _environment_ for these
 types of agents to work, where they can freely discover and communicate with the
 tools, each other, and any humans available in their environment.
@@ -656,14 +674,48 @@
 An additional benefit of its general design is that `agency` may also simplify
 some agent development workflows. See the hypothetical examples above.
 
 So, `agency` is a more general framework intended to support agent development
 and to ultimately enable agents to safely integrate with anything, in any way
 imaginable.
 
+## What are some known limitations or issues?
+
+* It's a new project, so keep that in mind in terms of completeness, but see
+the plans below for where this is heading. Core functionality is pretty
+well tested at the moment.
+
+* This library makes use of threads for each individual agent. Multithreading
+is limited by python's GIL, meaning if you run a CPU bound model other agents
+will have to wait for their "turn". This goes for anything else you might define
+as an "agent", if it is CPU heavy it will block other agents. Note that I/O does
+not block, so networked backends or services will execute in parallel.  Other
+forms of multiprocessing to avoid the GIL may eventually be considered.
+
+* This API does NOT assume or enforce predefined roles like "user", "system",
+  "assistant", etc. This is an intentional decision and is not likely to change.
+
+  `agency` is intended to allow potentially large numbers of agents, systems,
+  and people to come together. A small predefined set of roles gets in the way
+  of representing many things uniquely and independently.
+
+  This is a core feature of `agency`: that all things are treated the same and
+  may be interacted with through common means.
+
+  The lack of roles introduces some challenges in integrating with role based
+  APIs. See the implementation of
+  [`OpenAIFunctionAgent`](./agency/agents/openai_function_agent.py) for an
+  example.
+
+* There is not much by way of storage support. That is mostly left up to you and
+  I'd suggest looking at the many technologies that focus on that. The `Agent`
+  class implements a simple `_message_log` array which you can make use of or
+  overwrite to back it with longer term storage. More direct support for storage
+  APIs may be considered in the future.
+
 
 # Contributing
 
 Please do!
 
 If you have any questions, suggestions, or problems, please open an
 [issue](https://github.com/operand/agency/issues).
@@ -694,41 +746,41 @@
 human, artificial, and other computing systems together, with the following
 priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
-  Currently the limitations of pythong multi-threading are a bottleneck 
+  Currently the limitations of python multi-threading are a bottleneck.
 - **Access Control and Safety**:
-  Designing an effective access control solution for AI integrated systems is a
-  fundamental problem to solve in order to ensure safety. I believe I've
-  included a sane first attempt at such a pattern, but further exploration will
-  be a focus of this project.
+  An effective access control solution for agent-integrated systems is
+  fundamental to ensure safety. I believe I've included a sane first step at
+  such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
-  creating AI integrated systems. I intend to continually improve the API,
-  protocol, and other aspects of its design as needed based on feedback from
-  real world use. [So please let me
-  know!](https://github.com/operand/agency/issues)
+  creating agent systems. I hope to ensure ensure the API is kept small, and
+  compatible with a wide variety of use cases.
 - **Documentation**:
-  I hope to ensure documentation is kept small, accurate and up to date. This
+  I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add web app i/o examples
+- Add schema support for [OpenAI Function
+calling](https://platform.openai.com/docs/guides/gpt/function-calling)
+- Add web app multimodal i/o examples
   - image
   - audio
   - video
-- Add multimodal model example
+- Add multimodal model integration example
 - Add message broker/networking support (RabbitMQ)
 - Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
 - Add integration example for [gorilla](https://github.com/ShishirPatil/gorilla)
 - Add integration example for LangChain
 - Add model training example
 - Consider alternative multiprocessing approaches
 - Consider adding a storage API
 - Consider prior work on distributed access control
 - Add docker assets to encourage using it
 - [_feel free to make
 suggestions_](https://github.com/operand/agency/issues)
+
```

### Comparing `agency-1.0.0/agency/agent.py` & `agency-1.0.1/agency/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,25 @@
         self.running = threading.Event()
         self.stopping = threading.Event()
         # set by parent Space when added
         self.space = None
         # A basic approach to storing messages
         self._message_log = []
 
-    def id(self) -> str:
+    def id(self, fully_qualified=True) -> str:
         """
         Returns the fully qualified id of this agent
         """
-        _id = self.__id
-        if self.space is not None:
-            _id = f"{self.__id}.{self.space.id()}"
-        return _id
+        if fully_qualified:
+            _id = self.__id
+            if self.space is not None:
+                _id = f"{self.__id}.{self.space.id()}"
+            return _id
+        else:
+            return self.__id
 
     def run(self):
         """Starts the agent in a thread"""
         if not self.running.is_set():
             self.__thread = threading.Thread(target=self.__process)
             self.__thread.start()
             self.running.set()
@@ -90,18 +93,19 @@
         """
         while not self.stopping.is_set():
             try:
                 message = self.__message_queue.get(timeout=0.01)
                 try:
                     self.__commit_action(message)
                 except Exception as e:
-                    # Here we handle errors that occur while handling an action, including
-                    # access denial, by reporting the error back to the sender. If an error
-                    # occurs here, indicating that basic _send() functionality is broken,
-                    # the application will exit.
+                    # Here we handle exceptions that occur while committing an
+                    # action, including PermissionError's from access denial, by
+                    # reporting the error back to the sender. If an error occurs
+                    # here, indicating that basic _send() functionality is
+                    # broken, the application will exit.
                     self._send({
                       "to": message['from'],
                       "thoughts": "An error occurred",
                       "action": "error",
                       "args": {
                         "original_message": message,
                         "error": f"{e}",
@@ -120,15 +124,15 @@
             action_method = getattr(
               self, f"{ACTION_METHOD_PREFIX}{message['action']}")
         except AttributeError as e:
             # the action was not found
             if message['to'] == self.id():
                 # if it was point to point, raise an error
                 raise AttributeError(
-                    f"\"{message['action']}\" action not found")
+                    f"\"{message['action']}\" action not found on \"{self.id()}\"")
             else:
                 # broadcasts will not raise an error
                 return
 
         return_value = None
         error = None
         try:
@@ -283,15 +287,15 @@
         })
 
     def _after_action(self, original_message: MessageSchema, return_value: str, error: str):
         """
         Called after every action. Override and use this method for logging or other
         situations where you may want to pass through all actions.
 
-        Note that this is ONLY called if the action was actually attempted, meaning
+        Note that this is only called if the action was actually attempted, meaning
         BOTH the action exists AND is permitted.
         """
         pass
 
     @abstractmethod
     def _request_permission(self, proposed_message: MessageSchema) -> bool:
         """
```

### Comparing `agency-1.0.0/agency/agents/chattyai.py` & `agency-1.0.1/agency/agents/chattyai.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/agency/agents/demo_agent.py` & `agency-1.0.1/agency/agents/openai_completion_agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from agency.agent import Agent
 from agency.agents.prompt_methods import PromptMethods
 import json
 import openai
 import textwrap
 
 
-class DemoAgent(Agent, PromptMethods):
+class OpenAICompletionAgent(Agent, PromptMethods):
+    """
+    An agent which uses OpenAI's completion API for inference
+    """
 
     def __init__(self, id, model, openai_api_key, **kwargs):
         super().__init__(id, **kwargs)
         self.__model = model
         openai.api_key = openai_api_key
 
     def _prompt_head(self):
         return textwrap.dedent(f"""
-        I am "Demo". I am an early prototype of an "agent" system which can
-        freely interact with its environment.
+        I am "{self.id(fully_qualified=False)}". I am an early prototype of an
+        "agent" system which can freely interact with its environment.
 
         My creator has recently open-sourced my codebase intended to allow
         others to easily create their own AI integrated systems. He is
         demonstrating my abilities so that others can better understand agents
         like myself and how we may integrate with the world.
 
         My goal is to demonstrate my accurate understanding of the world and my
@@ -30,17 +33,14 @@
         problems at hand.
 
         In order to communicate, I use a simple terminal application where I can
         interact via JSON formatted messages. I can send messages to discover
         and interact with other systems, AI agents, or humans who may also be
         present.
 
-        It is {util.to_timestamp(datetime.now())}. I am ready to begin with our
-        demonstration.
-
         %%%%% Terminal App 1.0.0 %%%%%
         (Use the "help" action to see available commands")
         """) + \
             self._message_line({
                 "from": self.id(),
                 "to": None,
                 "thoughts": "I should see what commands are available.",
```

### Comparing `agency-1.0.0/agency/agents/host.py` & `agency-1.0.1/agency/agents/host.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/agency/agents/prompt_methods.py` & `agency-1.0.1/agency/agents/prompt_methods.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/agency/schema.py` & `agency-1.0.1/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/agency/space.py` & `agency-1.0.1/agency/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,11 +87,12 @@
                 recipient._receive(message)
 
     def _get_help__sync(self, action_name: str = None) -> list:
         """
         Returns an action list immediately without forwarding messages
         """
         help = [
-            agent._get_help(action_name)
+            item
             for agent in [self] + self.agents
+            for item in agent._get_help(action_name)
         ]
         return help
```

### Comparing `agency-1.0.0/agency/spaces/templates/index.html` & `agency-1.0.1/agency/spaces/templates/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -59,85 +59,88 @@
           ],
           input: ''
         };
         this.socket = io.connect('http://localhost:8080');
         this.chatbox = React.createRef()
       }
 
-      parseArguments(parts) {
-        let args = {};
-
-        for (let i = 1; i < parts.length; i++) {
-          let splitIndex = parts[i].indexOf(":");
-          let key = parts[i].substring(0, splitIndex);
-          let val = parts[i].substring(splitIndex + 1);
+      parseSlashSyntaxAction(action_text) {
+          action_text = action_text.trim();
+          let action = {};
 
-          if (val.startsWith('"') && val.endsWith('"')) {
-            val = val.slice(1, -1);
-          }
+          if (!action_text.startsWith("/")) {
+            action = {
+              "action": "say",
+              "thoughts": "",
+              "args": { "content": action_text }
+            }
+          } else {
+            let commandEndIndex = action_text.indexOf(" ");
+            let action_name = action_text.substring(1, commandEndIndex);
+            let args = {};
+
+            let currentArgName = "";
+            let currentArgValue = "";
+            let inQuotes = false;
+
+            for (let i = commandEndIndex + 1; i < action_text.length; i++) {
+              let char = action_text[i];
+
+              if (char === ':' && !inQuotes) {
+                currentArgName = currentArgValue.trim();
+                currentArgValue = "";
+              } else if (char === '"' && !inQuotes) {
+                inQuotes = true;
+              } else if (char === '"' && inQuotes) {
+                inQuotes = false;
+              } else if (char === ' ' && !inQuotes) {
+                args[currentArgName] = currentArgValue.trim();
+                currentArgValue = "";
+              } else {
+                currentArgValue += char;
+              }
+            }
 
-          try {
-            args[key] = JSON.parse(`"${val}"`);
-          } catch (e) {
-            args[key] = val;
+            if (currentArgName && currentArgValue) {
+              args[currentArgName] = currentArgValue.trim();
+            }
+
+            // pull out the "to" and "thoughts" args if they exist
+            let to = args['to'];
+            delete args['to'];
+            let thoughts = args['thoughts'];
+            delete args['thoughts'];
+
+            action = {
+              "to": to,
+              "thoughts": thoughts || "",
+              "action": action_name,
+              "args": args
+            };
           }
-        }
 
-        return args;
-      }
-
-      parseSlashSyntaxAction(action_text) {
-        action_text = action_text.trim();
-        let action = {};
-        if (!action_text.startsWith("/")) {
-          action = {
-            "action": "say",
-            "thoughts": "",
-            "args": { "content": action_text }
-          }
-        }
-        else {
-          let parts = action_text
-              .match(/"[^"]+"|\S+/g)
-              .map(part => part.replace(/"/g, ''));
-          let action_name = parts[0].substring(1);
-          let args = this.parseArguments(parts);
-
-          // pull out the "to" and "thoughts" args if they exist
-          let to = args['to']
-          delete args['to']
-          let thoughts = args['thoughts']
-          delete args['thoughts']
-
-          action = {
-            "to": to,
-            "thoughts": thoughts || "",
-            "action": action_name,
-            "args": args
-          };
+          console.log("sending action: ", action);
+          return action;
         }
-        console.log("sending action: ", action)
-        return action;
-      }
 
       componentDidMount() {
         this.socket.on('message', (msg) => {
           console.log('message: ', msg);
           this.setState(state => {
             const messages = [
               ...state.messages,
               msg
             ];
             return { messages };
           });
         });
 
-        this.socket.on('permission_request', (proposed_msg) => {
-          console.log('permission_request: ', proposed_msg);
-          const answer = window.confirm(`Do you permit the following?\n${proposed_msg}`);
+        this.socket.on('permission_request', (proposedMsg) => {
+          console.log('permission_request: ', proposedMsg);
+          const answer = window.confirm(`Do you permit the following?\n${proposedMsg}`);
           this.socket.emit('permission_response')
         });
       }
 
       componentDidUpdate() {
         this.chatbox.current.scrollTop = this.chatbox.current.scrollHeight;
       }
@@ -193,16 +196,20 @@
       render() {
         return (
           <div style={{ height: '100%', display: 'flex', flexDirection: 'column' }}>
             <div id="chatbox" ref={this.chatbox}>
               {
                 this.state.messages.map((message, index) => (
                   <div key={index}>
-                    {message.from ? `${message.from.split(".")[0]}: ` : ''}
-                    {this.messageToText(message)}
+                    <div style={{color: 'blue'}}>
+                      {message.from ? `${message.from.split(".")[0]}: ` : ''}
+                    </div>
+                    <div>
+                      {this.messageToText(message)}
+                    </div>
                   </div>
                 ))
               }
             </div>
             <div id="input-area">
               <textarea id="user-input" value={this.state.input} onChange={this.handleInputChange} onKeyDown={this.handleKeyDown} />
               <button onClick={this.sendMessage}>Send</button>
```

### Comparing `agency-1.0.0/agency/spaces/web_app.py` & `agency-1.0.1/agency/spaces/web_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         # start socketio server
         self.socketio = SocketIO(app, async_mode='eventlet',
                                  logger=False, engineio_logger=False)
 
         # NOTE: We're simplifying here by hardcoding a single agent named
         # "Dan" representing a user of the WebApp. In a real application this
         # could be handled dynamically as users log on/off.
-        self.add(WebAppUser("Dan"))
+        self.add(WebAppUser(kwargs['demo_user_id']))
 
         # Define routes
         @app.route('/')
         def index():
             return render_template(
                 'index.html',
                 agent_id=f"{self.current_agent().id()}")
```

### Comparing `agency-1.0.0/agency/util.py` & `agency-1.0.1/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.0/pyproject.toml` & `agency-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "agency"
-version = "1.0.0"
-description = "A fast and minimal foundation for unifying human, AI, and other computing systems, in python"
+version = "1.0.1"
+description = "A fast and minimal foundation for unifying human, AI, and other computing systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
```

### Comparing `agency-1.0.0/PKG-INFO` & `agency-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: agency
-Version: 1.0.0
-Summary: A fast and minimal foundation for unifying human, AI, and other computing systems, in python
-License: GPL-3.0
-Author: Daniel Rodriguez
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Flask-SocketIO (>=5.3,<6.0)
-Requires-Dist: asyncio (>=3.4,<4.0)
-Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: eventlet (>=0.33,<0.34)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: torch (>=2.0,<3.0)
-Requires-Dist: transformers (>=4.29,<5.0)
-Description-Content-Type: text/markdown
-
 # `agency`
 
 A fast and minimal foundation for unifying human, AI, and other computing
 systems, in python
 
 
 ## What is `agency`?
@@ -49,16 +27,16 @@
 - ...
 - anything
 
 
 # Install
 > **WARNING:**\
 Running `agency` may result in exposing your computer to access by any connected
-`Agent` class including AI agents. Please understand the risks before using this
-software and do not configure it for OS access otherwise.\
+`Agent` class. Please understand the risks before using this software and do not
+configure it for OS access otherwise.\
 \
 If you want to enable OS access, to allow for file I/O for example, I HIGHLY
 RECOMMEND running your project within a Docker container to prevent direct
 access to your host, allowing you to limit the resources and directories that
 may be accessed.
 
 ```sh
@@ -72,35 +50,31 @@
 model](https://en.wikipedia.org/wiki/Actor_model) intended for integrating AI,
 human, and traditional computing systems.
 
 In `agency`, all entities are called "agents" and represented as instances
 of the `Agent` class. This includes all humans, software, and AI-driven agents.
 
 The `Agent` class is a base class similar to "Object" in many object-oriented
-languages. All agents may expose "actions" which can be invoked by other
-agents, by simply defining instance methods on the class.
+languages. All agents may expose "actions" that other agents can discover and
+invoke at run time. Actions also specify an access policy, allowing you to
+monitor and control actions to ensure safety.
 
 A `Space` is also an `Agent` and is used to group multiple agents together.
 
 A space can be thought of as both a collection of agents and a "router" for
 their communication. An agent cannot communicate with others until it is first
 added to a space.
 
 Spaces may be nested, allowing for namespacing and hierarchical organization of
 the agents in your application.
 
-All agents may define public "actions" that other agents can discover and invoke
-at run time. Actions also specify an access policy, allowing you to monitor and
-control actions to ensure safety.
-
 To summarize, the two classes of `Agent` and `Space` together create a simple
-API for defining applications that may mix AI, human, and traditional computing
+API for creating applications that may mix AI, human, and traditional computing
 systems, in a way that is intended for all to equally understand and use.
 
-
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
 > Please note that the example classes used in this walkthrough are implemented
 for you to explore and try out, but should be considered "proof of concept"
@@ -225,23 +199,23 @@
 
 This is an example of the full message schema that is used for all messages sent
 between agents in `agency`. This format is intended to be simple and extensible
 enough to support any use case while remaining human readable.
 
 Note that the `"thoughts"` field is defined as a distinct argument for providing
 a natural language explanation to accompany any action, but as of this writing
-`ChattyAI` does not make use of it. `DemoAgent` discussed below, does.
+`ChattyAI` does not make use of it. `OpenAICompletionAgent` discussed below,
+does.
 
 For more details on the common message schema see
 [schema.py](./agency/schema.py).
 
 
 ## Access Control
 
-
 All actions must declare an access policy like the following example seen above
 the `ChattyAI._action__say()` method:
 
 ```python
 @access_policy(ACCESS_PERMITTED)
 def _action__say(self, content: str):
     """Use this action to say something to Chatty"""
@@ -267,37 +241,37 @@
 
 ```python
 def _request_permission(self, proposed_message: MessageSchema) -> bool:
     ...
 ```
 
 This method is called when an agent attempts to invoke an action that has been
-marked as `ACCESS_REQUESTED`. Your method should inspect the `proposed_message`
-and return a boolean indicating whether or not to permit the action.
+marked as `ACCESS_REQUESTED`. Your method should inspect `proposed_message` and
+return a boolean indicating whether or not to permit the action.
 
 You can use this approach to protect against dangerous actions being taken. For
 example if you allow terminal access, you may want to review commands before
 they are invoked.
 
 This implementation of access control is just a start, and further development
-of the mechanics is a priority for this project.
+of the functionality is a priority for this project.
 
 
 ## Adding Human Users With the `WebApp` Class
 
 A single chatting AI wouldn't be useful without someone to chat with, so now
 let's add humans into the space so that they can chat with "Chatty". To do
 this, we'll use the `WebApp` class, which is a subclass of `Space`.
 
 Why choose to subclass `Space` and not `Agent`? This is an arbitrary choice up
 to the developer, and may depend on what they want to accomplish.
 
 We could implement `WebApp` as a subclass of `Agent`. This would represent the
 web application as a single agent within the system. Users of the web
-application would not be able to be addressed individually by agents.
+application would not be able to be addressed individually by other agents.
 
 But since a typical web application serves multiple users, it may make sense to
 implement it as a `Space` subclass, so that individual users of the web
 application can be addressed by other agents using a namespace associated with
 the web application, as we'll see below.
 
 So this is _not_ the only way this could be accomplished but is intended as a
@@ -316,28 +290,29 @@
 `Agent` and is called `WebAppUser`.
 
 The `WebAppUser` class is where we define the actions that an individual web app
 user may expose to others.
 
 Using the `asyncio` library you'll see that we simply forward messages as-is to
 the `React` frontend, and allow the client code to handle rendering and parsing
-of input as actions back to the `Flask` application, which routes them to their
-intended receiver in the space.
+of input as actions back to the `Flask` application, which forwards them to
+their intended receiver in the space.
 
 This way, we allow individual web users to appear as individual agents to others
 in the space.
 
 
 ## Namespacing and Adding the Web Application
 
 Now that we've defined our new `WebApp` class, we can add it to `DemoSpace`
 with:
 
 ```python
-space.add(WebApp("WebApp", port=os.getenv('WEB_APP_PORT')))
+space.add(
+    WebApp("WebApp", port='8080'))
 ```
 
 Whenever any agent is added to a space, its fully qualified `id` becomes
 namespaced with the space's `id`.
 
 For example, after running the line above the `WebApp` being an agent as well,
 receives an `id` of `"WebApp.DemoSpace"`.
@@ -347,16 +322,17 @@
 
 - `"DemoSpace"` - The root space
 - `"ChattyAI.DemoSpace"` - ChattyAI's fully qualified `id`
 - `"WebApp.DemoSpace"` - the root of the `"WebApp"` space
 
 Users of the web application, as they log in or out, may be added dynamically
 under the `"WebApp"` namespace allowing them to be addressed with a fully
-qualified `id` of, for example `"Dan.WebApp.DemoSpace"`.
+qualified `id` of, for example:
 
+- `"Dan.WebApp.DemoSpace"`.
 
 _(Note that login/out functionality is not implemented as of this writing.)_
 
 
 ## Adding OS Access with the `Host` class
 
 At this point, we have a system where human users of the web application can
@@ -384,41 +360,41 @@
 
 By declaring this access policy, all actions on the host will require a
 confirmation from the terminal where the application is being run. This is
 thanks to the implementation of `_request_permission()` in the `Host` class.
 
 Note that this implementation of `_request_permission()` is just one
 possibility. We could have implemented, for example, a phone notification for a
-human to review from anywhere.
+human to review from elsewhere.
 
 
 ## Discovering Actions
 
 At this point, we can demonstrate how discovery works from the perspective of
 a human user of the web application.
 
 Once added to a space, each agent may send a `help` message to discover other
 agents and actions that are available in the space.
 
-The `WebApp` which hosts a simple chat UI supports a "slash" syntax summarized
-here:
+The `WebApp` application hosts a simple chat UI that supports a "slash" syntax
+summarized here:
 
 ```python
 /actionname arg1:val1 arg2:val2 ...
 ```
 
-So a person using the chat UI can discover available actions with:
+So a person using the chat UI can discover available actions by typing:
 
 ```
 /help
 ```
 
 This will broadcast a `help` action to all other agents, who will individually
 respond with a list of their available actions. The returned list of actions
-from the `Host` agent, would look something like:
+would look something like:
 
 ```python
 [
     {
         "to": "Host.DemoSpace",
         "action": "delete_file",
         "thoughts": "Delete a file",
@@ -430,14 +406,22 @@
         "to": "Host.DemoSpace",
         "action": "list_files",
         "thoughts": "List files in a directory",
         "args": {
           "directory_path": "str"
         }
     },
+    {
+        "to": "ChattyAI.DemoSpace",
+        "action": "say",
+        "thoughts": "Use this action to say something to Chatty",
+        "args": {
+          "content": "str"
+        }
+    },
     ...
 ]
 ```
 
 Notice that each action lists the fully qualified `id` of the agent in the
 `"to"` field, the docstring of the action's method in the `"thoughts"` field,
 and each argument along with its type in the `"args"` field.
@@ -447,18 +431,18 @@
 
 ```
 /list_files to:Host.DemoSpace directory_path:/app
 ```
 
 This will send the `list_files` action to the `Host` agent who will (after being
 granted permission) return the results back to `"Dan.WebApp.DemoSpace"`
-rendering it to the web user interface.
+rendering it to the web user interface as a message.
 
 Note the use of the fully qualified `id` of `Host.DemoSpace` used with the `to:`
-field
+field.
 
 
 ## Broadcast vs Point-to-Point Messaging
 
 If we omit the `to:Host.DemoSpace` portion of the command above, the message
 will be broadcast, and any agents who implement a `list_files` action will
 respond.
@@ -481,120 +465,110 @@
 
 Finally we get to the good part!
 
 We'll now add an intelligent agent into this environment and see that it is able
 to understand and interact with any of the systems or humans we've connected
 thus far.
 
-To add the [`DemoAgent`](./agency/agents/demo_agent.py) class to the
+> Note that the following `OpenAIFunctionAgent` class uses the newly released
+[openai function calling
+API](https://platform.openai.com/docs/guides/gpt/function-calling).
+
+To add the [`OpenAIFunctionAgent`](./agency/agents/demo_agent.py) class to the
 environment:
 ```python
 space.add(
-    DemoAgent("Demo",
-        model="text-davinci-003",
-        openai_api_key=os.getenv("OPENAI_API_KEY")))
-```
-
-Note that the `DemoAgent` class is implemented to use the OpenAI API as a
-language model backend. I recommend using language models on par with GPT-3.5 or
-better for the best results with tool-using agents such as this.
-
-
-### The `DemoAgent` Prompt
-
-What makes the `DemoAgent` able to intelligently discover and interact with
-others is largely embodied in the `DemoAgent._prompt_head()` method. In it
-you'll notice a few things:
-
-1. The prompt is written from the first person perspective as though it is the
-agent's own thoughts. This differs slightly from common practice, which usually
-uses the second-person perspective. I do not think this makes a large difference
-but was worth mentioning. This is more of a personal preference.
-
-1. I frame the situation clearly and accurately for the agent, telling it enough
-about who it is, its goals, and the JSON format that it uses to communicate.
-
-1. I "pretend" that the bottom portion is a terminal application. By signaling a
-change in context with the `%%%%% Terminal %%%%%` header, we help make clear to
-the language model that this is a distinct section of content with its own text
-patterns to continue. I do not believe that this is a crucial technique either,
-but is worth noting.
-
-1. I use the `_message_log_to_list()` method to dynamically insert the previous
-conversation up to the current point. See the mixin class `PromptMethods` for
-the implementation. There is no summarization used, so the current
-implementation will eventually hit the context window after a short time.
-
-1. I insert a fake event at the beginning of the terminal portion of the prompt,
-pretending that the agent themself executed the `help` action proactively, and
-display the resulting list of available actions. This is just a neat way to
-insert the available actions while keeping the supposed context of the terminal,
-and providing a one-shot example to begin from.
-
-Note that `ChattyAI` uses a more typical prompt, showing that prompt style and
-technique need not be shared by all agents connected to a space, but can be
-entirely unique to each agent.
+    OpenAIFunctionAgent("FunctionAI",
+        model="gpt-3.5-turbo-16k",
+        openai_api_key=os.getenv("OPENAI_API_KEY"),
+        # user_id determines the "user" role in the chat API
+        user_id="Dan.WebApp.DemoSpace"))
+```
+
+The `user_id` argument determines which agent is represented as the "user" role
+to the chat API. Since the chat API is limited to a predefined set of roles, we
+need to indicate which is the main "user".
+
+For an implementation that uses a plain text completion API, see
+[`OpenAICompletionAgent`](./agency/agents/openai_completion_agent.py).
 
 
 ## Complete Demo Implementation
 
 The following is the full implementation (minus imports) of the above
-walkthrough that you can try out on your own. Note that `Space.run()` starts a
+walkthrough that you can try out on your own, including both OpenAI agent
+examples and the HuggingFace based "Chatty". Note that `Space.run()` starts a
 thread, so we simply keep the application alive with a while loop.
 
 ```python
 # demo.py
 
 if __name__ == '__main__':
 
     space = Space("DemoSpace") 
 
     space.add(
-        WebApp("WebApp", port=os.getenv('WEB_APP_PORT')))
+        WebApp("WebApp",
+            demo_user_id="Dan", # hardcoded for simplicity
+            port='8080'))
 
     space.add(
-        ChattyAI("Chatty", model="EleutherAI/gpt-neo-125m"))
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
 
     space.add(
         Host("Host"))
 
     space.add(
-        DemoAgent("Demo",
+        OpenAIFunctionAgent("FunctionAI",
+            model="gpt-3.5-turbo-16k",
+            openai_api_key=os.getenv("OPENAI_API_KEY"),
+            # user_id determines the "user" role in the OpenAI chat
+            user_id="Dan.WebApp.DemoSpace"))
+
+    space.add(
+        OpenAICompletionAgent("CompletionAI",
             model="text-davinci-003",
             openai_api_key=os.getenv("OPENAI_API_KEY")))
 
     space.run()
 
+    print("pop!")
+
     # keep alive
     while True:
         time.sleep(1)
 ```
 
 If you run the above python script, after a short boot time you can visit the
-web app at `localhost:$WEB_APP_PORT` and you should see a simple chat interface.
+web app at `http://localhost:8080` and you should see a simple chat interface.
 
-The following is a screenshot of a conversation that showcases `DemoAgent`'s
-ability to intelligently interact with the other agents in the environment,
-including running commands on the host, or chatting with "Chatty".
+The following is a screenshot of a conversation that showcases all the agents
+intelligently interacting and following orders.
 
 Note that my messages are broadcasted in the below conversation, which explains
-why Chatty responds to each message as does "Demo". There is an obvious
-difference in quality, of course.
+why all three respond to each message. There is an obvious difference in
+quality, of course.
 
-I also demonstrate the results of rejecting an action and asking Demo to use a
-different approach.
+I also demonstrate the results of rejecting an action and directing an agent to
+use a different approach.
 
-Behind the scenes, Demo messaged Chatty directly and correctly relayed her
-response, and after I explained my rejection of the `read_file` action, Demo
-used the `shell_command` action with `wc -l Dockerfile` which was more
-appropriate. And the file indeed has 75 lines.
+After I explained my rejection of the `read_file` action (which happened behind
+the scenes on the terminal), "FunctionAI" appropriately used the `shell_command`
+action with `wc -l Dockerfile`. The Dockerfile indeed has 73 lines.
+
+CompletionAI used that command on the first try. Anecdotally as of this writing,
+`CompletionAI` seems to be more accurate, even though it is using the text
+completion API vs the function calling feature of the chat API. This may be due
+to the implementation or issues arising from the translation into roles
+discussed elsewhere.
 
 <p align="center">
-  <img src="https://i.ibb.co/f1GMb5P/Screenshot-2023-06-10-at-11-50-42-PM.png"
-       alt="Screenshot-2023-06-10-at-11-50-42-PM" border="0" width=500>
+  <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
+       alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
 </p>
 
 
 # Hypothetical Examples
 
 The following examples are not implemented, but are presented as additional
 ideas for integrations that `agency` could support.
@@ -651,17 +625,17 @@
 
 
 # FAQ
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
-`agency` (see [`DemoAgent`](./agency/agents/demo_agent.py)), it is not intended
-to be a full-fledged agent toolset. It can be thought of as an "agent
-integration framework".
+`agency` (see [`agents/`](./agency/agents/)), it is not intended to be a
+full-fledged agent toolset. It can be thought of as an "agent integration
+framework".
 
 Projects like LangChain and others are exploring how to create purpose-built
 agents that solve diverse problems using tools.
 
 `agency` is concerned with creating a safe and dynamic _environment_ for these
 types of agents to work, where they can freely discover and communicate with the
 tools, each other, and any humans available in their environment.
@@ -678,14 +652,48 @@
 An additional benefit of its general design is that `agency` may also simplify
 some agent development workflows. See the hypothetical examples above.
 
 So, `agency` is a more general framework intended to support agent development
 and to ultimately enable agents to safely integrate with anything, in any way
 imaginable.
 
+## What are some known limitations or issues?
+
+* It's a new project, so keep that in mind in terms of completeness, but see
+the plans below for where this is heading. Core functionality is pretty
+well tested at the moment.
+
+* This library makes use of threads for each individual agent. Multithreading
+is limited by python's GIL, meaning if you run a CPU bound model other agents
+will have to wait for their "turn". This goes for anything else you might define
+as an "agent", if it is CPU heavy it will block other agents. Note that I/O does
+not block, so networked backends or services will execute in parallel.  Other
+forms of multiprocessing to avoid the GIL may eventually be considered.
+
+* This API does NOT assume or enforce predefined roles like "user", "system",
+  "assistant", etc. This is an intentional decision and is not likely to change.
+
+  `agency` is intended to allow potentially large numbers of agents, systems,
+  and people to come together. A small predefined set of roles gets in the way
+  of representing many things uniquely and independently.
+
+  This is a core feature of `agency`: that all things are treated the same and
+  may be interacted with through common means.
+
+  The lack of roles introduces some challenges in integrating with role based
+  APIs. See the implementation of
+  [`OpenAIFunctionAgent`](./agency/agents/openai_function_agent.py) for an
+  example.
+
+* There is not much by way of storage support. That is mostly left up to you and
+  I'd suggest looking at the many technologies that focus on that. The `Agent`
+  class implements a simple `_message_log` array which you can make use of or
+  overwrite to back it with longer term storage. More direct support for storage
+  APIs may be considered in the future.
+
 
 # Contributing
 
 Please do!
 
 If you have any questions, suggestions, or problems, please open an
 [issue](https://github.com/operand/agency/issues).
@@ -716,42 +724,40 @@
 human, artificial, and other computing systems together, with the following
 priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
-  Currently the limitations of pythong multi-threading are a bottleneck 
+  Currently the limitations of python multi-threading are a bottleneck.
 - **Access Control and Safety**:
-  Designing an effective access control solution for AI integrated systems is a
-  fundamental problem to solve in order to ensure safety. I believe I've
-  included a sane first attempt at such a pattern, but further exploration will
-  be a focus of this project.
+  An effective access control solution for agent-integrated systems is
+  fundamental to ensure safety. I believe I've included a sane first step at
+  such a pattern, but further development will be a focus of this project.
 - **Compatibility and Usability**:
   In general, I believe this is a fair start in defining a set of patterns for
-  creating AI integrated systems. I intend to continually improve the API,
-  protocol, and other aspects of its design as needed based on feedback from
-  real world use. [So please let me
-  know!](https://github.com/operand/agency/issues)
+  creating agent systems. I hope to ensure ensure the API is kept small, and
+  compatible with a wide variety of use cases.
 - **Documentation**:
-  I hope to ensure documentation is kept small, accurate and up to date. This
+  I hope to ensure documentation is kept organized, clear, and accurate. This
   readme serves as a start.
 
 
 ## Planned Work
-- Add web app i/o examples
+- Add schema support for [OpenAI Function
+calling](https://platform.openai.com/docs/guides/gpt/function-calling)
+- Add web app multimodal i/o examples
   - image
   - audio
   - video
-- Add multimodal model example
+- Add multimodal model integration example
 - Add message broker/networking support (RabbitMQ)
 - Add integration example for [mlc-llm](https://github.com/mlc-ai/mlc-llm)
 - Add integration example for [gorilla](https://github.com/ShishirPatil/gorilla)
 - Add integration example for LangChain
 - Add model training example
 - Consider alternative multiprocessing approaches
 - Consider adding a storage API
 - Consider prior work on distributed access control
 - Add docker assets to encourage using it
 - [_feel free to make
 suggestions_](https://github.com/operand/agency/issues)
-
```

