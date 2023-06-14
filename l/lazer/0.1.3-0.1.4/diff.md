# Comparing `tmp/lazer-0.1.3.tar.gz` & `tmp/lazer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazer-0.1.3.tar", max compression
+gzip compressed data, was "lazer-0.1.4.tar", max compression
```

## Comparing `lazer-0.1.3.tar` & `lazer-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      242 2023-06-14 04:20:08.313905 lazer-0.1.3/README.md
--rw-r--r--   0        0        0     3710 2023-06-14 04:40:37.133905 lazer-0.1.3/lazer/__init__.py
--rw-r--r--   0        0        0      377 2023-06-14 04:41:33.263905 lazer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 lazer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-14 04:56:06.903905 lazer-0.1.4/README.md
+-rw-r--r--   0        0        0     3715 2023-06-14 05:04:54.553905 lazer-0.1.4/lazer/__init__.py
+-rw-r--r--   0        0        0      377 2023-06-14 05:05:47.433905 lazer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 lazer-0.1.4/PKG-INFO
```

### Comparing `lazer-0.1.3/lazer/__init__.py` & `lazer-0.1.4/lazer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         self.args = chatCompletionArgs
 
         assert "messages" not in self.args
         assert "functions" not in self.args
         assert "function_call" not in self.args
 
         self.args["messages"] = self.messages
-        self.args["functions"] = lazer.get_functions()
         self.args["function_call"] = "auto"
 
     async def talk(self, content: str) -> str:
+        self.args["functions"] = self.lazer.get_functions()
         self.messages.append({"role": "user", "content": content})
 
         while True:
             response = openai.ChatCompletion.create(**self.args)
 
             message = response["choices"][0]["message"]  # type: ignore
             if not message.get("function_call"):
```

