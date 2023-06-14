# Comparing `tmp/promptrix-0.2.2.tar.gz` & `tmp/promptrix-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.2.tar", last modified: Sun Jun 11 21:15:13 2023, max compression
+gzip compressed data, was "promptrix-0.2.3.tar", last modified: Wed Jun 14 15:57:19 2023, max compression
```

## Comparing `promptrix-0.2.2.tar` & `promptrix-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.2/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-11 21:15:13.767047 promptrix-0.2.2/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       78 2023-06-01 23:37:06.000000 promptrix-0.2.2/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-11 21:15:08.000000 promptrix-0.2.2/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-11 21:15:13.767047 promptrix-0.2.2/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.763047 promptrix-0.2.2/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-06-03 03:50:31.000000 promptrix-0.2.2/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2571 2023-06-08 00:11:30.000000 promptrix-0.2.2/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.2/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      551 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1181 2023-06-09 04:09:26.000000 promptrix-0.2.2/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-09 04:33:39.000000 promptrix-0.2.2/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2962 2023-06-09 04:34:31.000000 promptrix-0.2.2/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5352 2023-06-03 03:50:22.000000 promptrix-0.2.2/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      621 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-08 00:11:43.000000 promptrix-0.2.2/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.2/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/promptrixTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1733 2023-06-02 18:46:08.000000 promptrix-0.2.2/src/promptrix/types.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-11 21:15:13.767047 promptrix-0.2.2/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      648 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      733 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-11 21:15:13.000000 promptrix-0.2.2/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.3/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-14 15:57:19.440941 promptrix-0.2.3/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1655 2023-06-14 03:06:34.000000 promptrix-0.2.3/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-14 15:57:13.000000 promptrix-0.2.3/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-14 15:57:19.440941 promptrix-0.2.3/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.436941 promptrix-0.2.3/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.3/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2571 2023-06-08 00:11:30.000000 promptrix-0.2.3/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.3/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      679 2023-06-12 20:15:31.000000 promptrix-0.2.3/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1181 2023-06-09 04:09:26.000000 promptrix-0.2.3/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-13 18:46:29.000000 promptrix-0.2.3/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2491 2023-06-12 21:39:17.000000 promptrix-0.2.3/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5351 2023-06-12 21:38:53.000000 promptrix-0.2.3/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      640 2023-06-12 20:39:59.000000 promptrix-0.2.3/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-08 00:11:43.000000 promptrix-0.2.3/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.3/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.3/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-14 15:57:19.440941 promptrix-0.2.3/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-14 15:57:19.000000 promptrix-0.2.3/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.2/LICENSE` & `promptrix-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/pyproject.toml` & `promptrix-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
```

### Comparing `promptrix-0.2.2/src/promptrix/AssistantMessage.py` & `promptrix-0.2.3/src/promptrix/AssistantMessage.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     def __init__(self, template: str, tokens: Optional[int] = -1, assistant_prefix: Optional[str] = 'assistant: '):
         """
         Creates a new 'AssistantMessage' instance.
         :param template: Template to use for this section.
         :param tokens: Optional. Sizing strategy for this section. Defaults to `auto`.
         :param assistant_prefix: Optional. Prefix to use for assistant messages when rendering as text. Defaults to `assistant: `.
         """
-        super().__init__(template, 'assistant', tokens, True, '\n', assistant_prefix)
+        super().__init__(template, assistant_prefix, tokens, True, '\n', text_prefix=assistant_prefix)
```

### Comparing `promptrix-0.2.2/src/promptrix/ConversationHistory.py` & `promptrix-0.2.3/src/promptrix/ConversationHistory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.3/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/GroupSection.py` & `promptrix-0.2.3/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/LayoutEngine.py` & `promptrix-0.2.3/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.3/src/promptrix/PromptSectionBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,43 +15,37 @@
             raise Exception
 
     @abstractmethod
     async def renderAsMessages(self, memory, functions, tokenizer, max_tokens):
         pass
 
     async def renderAsText(self, memory, functions, tokenizer, max_tokens):
-        #print(f'\n\n***** PromptSectionBase renderAsText entry {type(self)}')
         as_messages = await self.renderAsMessages(memory, functions, tokenizer, max_tokens)
-        #print(f'n***** PromptSectionBase renderAsText {as_messages}')
         messages = as_messages.output
         #print(f'***** PromptSectionBase renderAsText messages len {len(messages)}')
-        #print(f'***** PromptSectionBase renderAsText messages[0] {messages[0]}')
         #print(f"***** PromptSectionBase renderAsText message {messages[0]['content']}")
         text = ''
         for message in messages:
             text += message['content']+'\n'
         #text = self.separator.join([message['content'] for message in messages])
         prefix_length = len(tokenizer.encode(self.text_prefix))
         separator_length = len(tokenizer.encode(self.separator))
         length = prefix_length + as_messages.length + ((len(as_messages.output) - 1) * separator_length)
         text = self.text_prefix + text
         if self.tokens > 1.0 and length > self.tokens:
             encoded = tokenizer.encode(text)
             text = tokenizer.decode(encoded[:self.tokens])
             length = self.tokens
-        #print(f"***** PromptSectionBase renderAsText exit\n")
         return RenderedPromptSection(output=text, length=length, tooLong=length > max_tokens)
 
     def return_messages(self, output, length, tokenizer, max_tokens):
-        #print(f'\n*** PromptSectionBase return_messages entry  {length}, {self.tokens}\n {output}\n')
         if self.tokens > 1.0:
             while length > self.tokens:
                 msg = output.pop()
                 encoded = tokenizer.encode(msg['content'])
                 length -= len(encoded)
                 if length < self.tokens:
                     delta = self.tokens - length
                     truncated = tokenizer.decode(encoded[:delta])
                     output.append(Message(role=msg.role, content=truncated))
                     length += delta
-        #print(f'***** PromptSectionBase return messages exit {output}')
         return RenderedPromptSection(output=output, length=length, tooLong=length > max_tokens)
```

### Comparing `promptrix-0.2.2/src/promptrix/TemplateSection.py` & `promptrix-0.2.3/src/promptrix/TemplateSection.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class TemplateSection(PromptSectionBase):
     def __init__(self, template, role, tokens = -1, required = True, separator='\n', text_prefix = ''):
         super().__init__(tokens, required, separator, text_prefix)
         self.template = template
         self.role = role
         self._parts = []
         self.parse_template()
-
     
     async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
         rendered_parts = [part(memory, functions, tokenizer, max_tokens) for part in self._parts]
         text = ''.join(rendered_parts)
         length = len(tokenizer.encode(text))
         return self.return_messages([{'role': self.role, 'content': text}], length, tokenizer, max_tokens)
```

### Comparing `promptrix-0.2.2/src/promptrix/TextSection.py` & `promptrix-0.2.3/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/UserMessage.py` & `promptrix-0.2.3/src/promptrix/UserMessage.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,8 +7,8 @@
     def __init__(self, template: str, tokens: int = -1, user_prefix: str = 'user: '):
         """
         Creates a new 'UserMessage' instance.
         :param template: Template to use for this section.
         :param tokens: Optional. Sizing strategy for this section. Defaults to `auto`.
         :param user_prefix: Optional. Prefix to use for user messages when rendering as text. Defaults to `user: `.
         """
-        super().__init__(template, 'user', tokens, True, '\n', user_prefix)
+        super().__init__(template, user_prefix, tokens, True, '\n', text_prefix = user_prefix)
```

### Comparing `promptrix-0.2.2/src/promptrix/Utilities.py` & `promptrix-0.2.3/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/VolatileMemory.py` & `promptrix-0.2.3/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix/promptrixTypes.py` & `promptrix-0.2.3/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.2/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.3/src/promptrix.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,13 +13,12 @@
 src/promptrix/TemplateSection.py
 src/promptrix/TextSection.py
 src/promptrix/UserMessage.py
 src/promptrix/Utilities.py
 src/promptrix/VolatileMemory.py
 src/promptrix/__init__.py
 src/promptrix/promptrixTypes.py
-src/promptrix/types.py
 src/promptrix.egg-info/PKG-INFO
 src/promptrix.egg-info/SOURCES.txt
 src/promptrix.egg-info/dependency_links.txt
 src/promptrix.egg-info/requires.txt
 src/promptrix.egg-info/top_level.txt
```

