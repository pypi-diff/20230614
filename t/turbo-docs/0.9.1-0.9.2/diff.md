# Comparing `tmp/turbo_docs-0.9.1.tar.gz` & `tmp/turbo_docs-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.9.1.tar", last modified: Mon Jun 12 21:25:56 2023, max compression
+gzip compressed data, was "turbo_docs-0.9.2.tar", last modified: Wed Jun 14 00:33:14 2023, max compression
```

## Comparing `turbo_docs-0.9.1.tar` & `turbo_docs-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.666760 turbo_docs-0.9.1/
--rw-rw-rw-   0        0        0     2252 2023-06-12 21:25:56.665753 turbo_docs-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-06-12 21:24:42.000000 turbo_docs-0.9.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 21:25:56.667755 turbo_docs-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-06-12 21:24:58.000000 turbo_docs-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.641359 turbo_docs-0.9.1/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.1/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.655746 turbo_docs-0.9.1/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.1/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0      818 2023-06-12 21:24:00.000000 turbo_docs-0.9.1/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0      914 2023-06-12 21:11:03.000000 turbo_docs-0.9.1/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.663752 turbo_docs-0.9.1/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.1/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      622 2023-06-12 21:10:08.000000 turbo_docs-0.9.1/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.1/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      991 2023-06-12 20:59:48.000000 turbo_docs-0.9.1/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:25:56.652748 turbo_docs-0.9.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2252 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 21:25:56.000000 turbo_docs-0.9.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.866591 turbo_docs-0.9.2/
+-rw-rw-rw-   0        0        0     2363 2023-06-14 00:33:14.865589 turbo_docs-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1866 2023-06-14 00:24:27.000000 turbo_docs-0.9.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:33:14.867594 turbo_docs-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-06-14 00:31:52.000000 turbo_docs-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.840824 turbo_docs-0.9.2/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.2/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.855582 turbo_docs-0.9.2/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.2/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0      840 2023-06-14 00:22:59.000000 turbo_docs-0.9.2/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0      914 2023-06-14 00:14:25.000000 turbo_docs-0.9.2/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.862590 turbo_docs-0.9.2/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.2/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-06-14 00:14:25.000000 turbo_docs-0.9.2/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.2/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      992 2023-06-14 00:20:44.000000 turbo_docs-0.9.2/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.851828 turbo_docs-0.9.2/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2363 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.9.1/PKG-INFO` & `turbo_docs-0.9.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs
 
-Turbo Docs is a Python package that helps you generate a well-formatted, user-friendly README.md file for your repository using GPT-3.5-turbo or GPT-4 (default). It also provides a command to copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
+Turbo Docs is a Python package that helps you generate a professional README.md file for your repository using GPT-3.5 Turbo or GPT-4. It can also copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
 
 ## Installation
 
-To install Turbo Docs, run the following command:
+To install Turbo Docs, you need to have Python 3.6 or higher. You can install the package using pip:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Requirements
+## Setup
 
-Turbo Docs requires the following packages:
+Before using Turbo Docs, you need to set up your OpenAI API key. If you don't have an API key, create an OpenAI account at https://platform.openai.com/overview. Then, set the API key as an environment variable:
 
-- requests
-- openai
-- llm-blocks
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
-- pathspec
-
-These packages will be installed automatically when you install Turbo Docs.
+```bash
+export OPENAI_API_KEY=<your_api_key>
+```
 
 ## Usage
 
-To use Turbo Docs, run the following command in your terminal:
+To use Turbo Docs, navigate to your project directory and run the following command:
 
 ```bash
-turbo_docs [OPTIONS]
+turbo_docs
 ```
 
 ### Options
 
 - `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
 - `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
 - `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
 
-### Example
-
-To generate a README.md file using GPT-3.5 Turbo, run the following command:
-
-```bash
-turbo_docs --readme --gpt3
-```
-
 ## Configuration
 
-You can configure Turbo Docs by creating a `turbo_docs.toml` file in your repository. This file allows you to specify files and folders to ignore when generating the README.md file or copying the directory text to the clipboard.
-
-Example `turbo_docs.toml`:
+You can configure Turbo Docs to ignore specific files and folders by creating a `turbo_docs.toml` file in your project directory. Add the files and folders you want to ignore in the `ignore` list:
 
 ```toml
 ignore = [
     "__pycache__",
     "venv",
     "build",
     "dist",
     "*.egg-info",
     ".git",
     "README.md",  # This is recommended so that --readme doesn't include the readme file itself
 ]
 ```
 
+## Dependencies
+
+Turbo Docs requires the following packages:
+
+- requests
+- openai
+- llm-blocks
+- click
+- pyperclip
+- redbaron
+- gitpython
+- toml
+- pathspec
+
+These dependencies will be installed automatically when you install Turbo Docs using pip.
+
 ## License
 
 Turbo Docs is released under the MIT License.
```

### Comparing `turbo_docs-0.9.1/README.md` & `turbo_docs-0.9.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 # Turbo Docs
 
-Turbo Docs is a Python package that helps you generate a well-formatted, user-friendly README.md file for your repository using GPT-3.5-turbo or GPT-4 (default). It also provides a command to copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
+Turbo Docs is a Python package that helps you generate a professional README.md file for your repository using GPT-3.5 Turbo or GPT-4. It can also copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
 
 ## Installation
 
-To install Turbo Docs, run the following command:
+To install Turbo Docs, you need to have Python 3.6 or higher. You can install the package using pip:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Requirements
+## Setup
 
-Turbo Docs requires the following packages:
+Before using Turbo Docs, you need to set up your OpenAI API key. If you don't have an API key, create an OpenAI account at https://platform.openai.com/overview. Then, set the API key as an environment variable:
 
-- requests
-- openai
-- llm-blocks
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
-- pathspec
-
-These packages will be installed automatically when you install Turbo Docs.
+```bash
+export OPENAI_API_KEY=<your_api_key>
+```
 
 ## Usage
 
-To use Turbo Docs, run the following command in your terminal:
+To use Turbo Docs, navigate to your project directory and run the following command:
 
 ```bash
-turbo_docs [OPTIONS]
+turbo_docs
 ```
 
 ### Options
 
 - `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
 - `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
 - `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
 
-### Example
-
-To generate a README.md file using GPT-3.5 Turbo, run the following command:
-
-```bash
-turbo_docs --readme --gpt3
-```
-
 ## Configuration
 
-You can configure Turbo Docs by creating a `turbo_docs.toml` file in your repository. This file allows you to specify files and folders to ignore when generating the README.md file or copying the directory text to the clipboard.
-
-Example `turbo_docs.toml`:
+You can configure Turbo Docs to ignore specific files and folders by creating a `turbo_docs.toml` file in your project directory. Add the files and folders you want to ignore in the `ignore` list:
 
 ```toml
 ignore = [
     "__pycache__",
     "venv",
     "build",
     "dist",
     "*.egg-info",
     ".git",
     "README.md",  # This is recommended so that --readme doesn't include the readme file itself
 ]
 ```
 
+## Dependencies
+
+Turbo Docs requires the following packages:
+
+- requests
+- openai
+- llm-blocks
+- click
+- pyperclip
+- redbaron
+- gitpython
+- toml
+- pathspec
+
+These dependencies will be installed automatically when you install Turbo Docs using pip.
+
 ## License
 
 Turbo Docs is released under the MIT License.
```

### Comparing `turbo_docs-0.9.1/setup.py` & `turbo_docs-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.9.1",
+	version="0.9.2",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.9.1/turbo_docs/commands/readme.py` & `turbo_docs-0.9.2/turbo_docs/commands/readme.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from turbo_docs.utils import openai_api
 
 TEMPLATE = """
 "You are an expert software developement assistant.
 
-Create a well-formatted, user-firendly readme.md documenting the following repo:
+Create a formatted professional README.md documenting setup and usage of the following repo:
 {repo}
 """
 
 def readme(repo, gpt3=False, template=TEMPLATE):
     """
     Chose between GPT-3.5 Turbo and GPT-4, allow for template override, and
     generate a README.md file for the current repo.
     """
+    from turbo_docs.utils import openai_api
+
     readme = "README.md"
     if gpt3:
-        model = "gpt-3.5-turbo"
+        model = "gpt-3.5-turbo-16k"
     else:
         model = "gpt-4"
 
     response = openai_api.gpt_completion(template, {"repo": repo}, model)
     if response is None:
         print("Unable to generate README.md, it seems like you have uploaded too many tokens.")
     else:
```

### Comparing `turbo_docs-0.9.1/turbo_docs/generate.py` & `turbo_docs-0.9.2/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.1/turbo_docs/utils/cli_options.py` & `turbo_docs-0.9.2/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.1/turbo_docs/utils/directory.py` & `turbo_docs-0.9.2/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.1/turbo_docs/utils/openai_api.py` & `turbo_docs-0.9.2/turbo_docs/utils/openai_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import openai
 
 if not os.environ.get("OPENAI_API_KEY"):
 	print("OpenAI API key is not set. Please set it as an environment variable (export OPENAI_API_KEY=<your_api_key>) or enter it below.")
 	print("If you have not done so already, create an OpenAI account at https://platform.openai.com/overview.")
-	os.environ['OPENAI_API_KEY'] = input("Secret key:")
+	os.environ['OPENAI_API_KEY'] = input("Secret key: ")
 
 from llm_blocks import chat_utils
 
 
 def gpt_completion(template, inputs, model="gpt-4"):
 	"""Genneric chat wrapper over the OpenAI API"""
```

### Comparing `turbo_docs-0.9.1/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.9.2/turbo_docs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs
 
-Turbo Docs is a Python package that helps you generate a well-formatted, user-friendly README.md file for your repository using GPT-3.5-turbo or GPT-4 (default). It also provides a command to copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
+Turbo Docs is a Python package that helps you generate a professional README.md file for your repository using GPT-3.5 Turbo or GPT-4. It can also copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
 
 ## Installation
 
-To install Turbo Docs, run the following command:
+To install Turbo Docs, you need to have Python 3.6 or higher. You can install the package using pip:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Requirements
+## Setup
 
-Turbo Docs requires the following packages:
+Before using Turbo Docs, you need to set up your OpenAI API key. If you don't have an API key, create an OpenAI account at https://platform.openai.com/overview. Then, set the API key as an environment variable:
 
-- requests
-- openai
-- llm-blocks
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
-- pathspec
-
-These packages will be installed automatically when you install Turbo Docs.
+```bash
+export OPENAI_API_KEY=<your_api_key>
+```
 
 ## Usage
 
-To use Turbo Docs, run the following command in your terminal:
+To use Turbo Docs, navigate to your project directory and run the following command:
 
 ```bash
-turbo_docs [OPTIONS]
+turbo_docs
 ```
 
 ### Options
 
 - `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
 - `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
 - `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
 
-### Example
-
-To generate a README.md file using GPT-3.5 Turbo, run the following command:
-
-```bash
-turbo_docs --readme --gpt3
-```
-
 ## Configuration
 
-You can configure Turbo Docs by creating a `turbo_docs.toml` file in your repository. This file allows you to specify files and folders to ignore when generating the README.md file or copying the directory text to the clipboard.
-
-Example `turbo_docs.toml`:
+You can configure Turbo Docs to ignore specific files and folders by creating a `turbo_docs.toml` file in your project directory. Add the files and folders you want to ignore in the `ignore` list:
 
 ```toml
 ignore = [
     "__pycache__",
     "venv",
     "build",
     "dist",
     "*.egg-info",
     ".git",
     "README.md",  # This is recommended so that --readme doesn't include the readme file itself
 ]
 ```
 
+## Dependencies
+
+Turbo Docs requires the following packages:
+
+- requests
+- openai
+- llm-blocks
+- click
+- pyperclip
+- redbaron
+- gitpython
+- toml
+- pathspec
+
+These dependencies will be installed automatically when you install Turbo Docs using pip.
+
 ## License
 
 Turbo Docs is released under the MIT License.
```

