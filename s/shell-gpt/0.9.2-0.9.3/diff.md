# Comparing `tmp/shell_gpt-0.9.2.tar.gz` & `tmp/shell_gpt-0.9.3.tar.gz`

## Comparing `shell_gpt-0.9.2.tar` & `shell_gpt-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/LICENSE
--rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/__main__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/app.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/cache.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/client.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/config.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/role.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/test_integration.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/tests/test_unit.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/LICENSE
--rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    22140 2020-02-02 00:00:00.000000 shell_gpt-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/LICENSE
+-rw-r--r--   0        0        0    20106 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/__main__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/cache.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/client.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/config.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/role.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/test_integration.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/test_unit.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/LICENSE
+-rw-r--r--   0        0        0    20106 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/PKG-INFO
```

### Comparing `shell_gpt-0.9.2/LICENSE` & `shell_gpt-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/README.md` & `shell_gpt-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.2
+pip install shell-gpt
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -320,15 +320,15 @@
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --model    [gpt-4|gpt-4-32k|gpt-3.5|gpt-3.5-16k]    OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
 │ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
```

### Comparing `shell_gpt-0.9.2/pyproject.toml` & `shell_gpt-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/app.py` & `shell_gpt-0.9.3/sgpt/app.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/cache.py` & `shell_gpt-0.9.3/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/client.py` & `shell_gpt-0.9.3/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/config.py` & `shell_gpt-0.9.3/sgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 DEFAULT_CONFIG = {
     # TODO: Refactor it to CHAT_STORAGE_PATH.
     "CHAT_CACHE_PATH": os.getenv("CHAT_CACHE_PATH", str(CHAT_CACHE_PATH)),
     "CACHE_PATH": os.getenv("CACHE_PATH", str(CACHE_PATH)),
     "CHAT_CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "REQUEST_TIMEOUT": int(os.getenv("REQUEST_TIMEOUT", "60")),
-    "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT3.value),
+    "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT35TURBO.value),
     "OPENAI_API_HOST": os.getenv("OPENAI_API_HOST", "https://api.openai.com"),
     "DEFAULT_COLOR": os.getenv("DEFAULT_COLOR", "magenta"),
     "ROLE_STORAGE_PATH": os.getenv("ROLE_STORAGE_PATH", str(ROLE_STORAGE_PATH)),
     "SYSTEM_ROLES": os.getenv("SYSTEM_ROLES", "false"),
     "DEFAULT_EXECUTE_SHELL_CMD": os.getenv("DEFAULT_EXECUTE_SHELL_CMD", "false"),
     # New features might add their own config variables here.
 }
```

### Comparing `shell_gpt-0.9.2/sgpt/role.py` & `shell_gpt-0.9.3/sgpt/role.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/utils.py` & `shell_gpt-0.9.3/sgpt/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 from typing import Any, Callable
 
 import typer
 from click import BadParameter
 
 
 class ModelOptions(str, Enum):
-    GPT3 = "gpt-3.5-turbo"
+    """
+    Model endpoint compatibility
+    https://platform.openai.com/docs/models/model-endpoint-compatibility
+    """
+
     GPT4 = "gpt-4"
-    GPT4_32K = "gpt-4-32k"
+    GPT432k = "gpt-4-32k"
+    GPT35TURBO = "gpt-3.5-turbo"
+    GPT35TURBO16K = "gpt-3.5-turbo-16k"
 
 
 def get_edited_prompt() -> str:
     """
     Opens the user's default editor to let them
     input a prompt, and returns the edited text.
```

### Comparing `shell_gpt-0.9.2/sgpt/handlers/chat_handler.py` & `shell_gpt-0.9.3/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/handlers/default_handler.py` & `shell_gpt-0.9.3/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/handlers/handler.py` & `shell_gpt-0.9.3/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/sgpt/handlers/repl_handler.py` & `shell_gpt-0.9.3/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/tests/test_integration.py` & `shell_gpt-0.9.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/tests/test_unit.py` & `shell_gpt-0.9.3/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.2/PKG-INFO` & `shell_gpt-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.9.2
+Version: 0.9.3
 Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -45,15 +45,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.2
+pip install shell-gpt
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -364,15 +364,15 @@
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --model    [gpt-4|gpt-4-32k|gpt-3.5|gpt-3.5-16k]    OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
 │ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
```

