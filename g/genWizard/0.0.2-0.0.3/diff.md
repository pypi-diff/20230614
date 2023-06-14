# Comparing `tmp/genWizard-0.0.2.tar.gz` & `tmp/genWizard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genWizard-0.0.2.tar", last modified: Mon Jun 12 20:07:36 2023, max compression
+gzip compressed data, was "genWizard-0.0.3.tar", last modified: Wed Jun 14 15:46:58 2023, max compression
```

## Comparing `genWizard-0.0.2.tar` & `genWizard-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.361067 genWizard-0.0.2/
--rw-r--r--   0 yvonkim    (501) staff       (20)       66 2023-06-04 08:46:43.000000 genWizard-0.0.2/.gitattributes
--rw-r--r--   0 yvonkim    (501) staff       (20)      155 2023-06-12 09:36:43.000000 genWizard-0.0.2/CHANGELOG.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)     1065 2023-06-12 09:38:56.000000 genWizard-0.0.2/LICENSE.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)       49 2023-06-12 19:01:04.000000 genWizard-0.0.2/MANIFEST.in
--rw-r--r--   0 yvonkim    (501) staff       (20)     5567 2023-06-12 20:07:36.360504 genWizard-0.0.2/PKG-INFO
--rw-r--r--   0 yvonkim    (501) staff       (20)     4912 2023-06-12 20:00:41.000000 genWizard-0.0.2/README.txt
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.354697 genWizard-0.0.2/genWizard.egg-info/
--rw-r--r--   0 yvonkim    (501) staff       (20)     5567 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/PKG-INFO
--rw-r--r--   0 yvonkim    (501) staff       (20)      325 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/SOURCES.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        1 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/dependency_links.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        7 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/requires.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        8 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/top_level.txt
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.359350 genWizard-0.0.2/modules/
--rw-r--r--   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:33:40.000000 genWizard-0.0.2/modules/__init__.py
--rw-r--r--   0 yvonkim    (501) staff       (20)     2039 2023-06-12 08:57:22.000000 genWizard-0.0.2/modules/database_manager.py
--rw-r--r--   0 yvonkim    (501) staff       (20)      649 2023-06-12 09:38:56.000000 genWizard-0.0.2/modules/expander.py
--rw-r--r--   0 yvonkim    (501) staff       (20)     1236 2023-06-12 18:48:46.000000 genWizard-0.0.2/modules/generator.py
--rw-r--r--   0 yvonkim    (501) staff       (20)       38 2023-06-12 20:07:36.362184 genWizard-0.0.2/setup.cfg
--rw-r--r--   0 yvonkim    (501) staff       (20)      727 2023-06-12 20:07:33.000000 genWizard-0.0.2/setup.py
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-14 15:46:58.016908 genWizard-0.0.3/
+-rw-r--r--   0 yvonkim    (501) staff       (20)       66 2023-06-04 08:46:43.000000 genWizard-0.0.3/.gitattributes
+-rw-r--r--   0 yvonkim    (501) staff       (20)      371 2023-06-14 15:46:39.000000 genWizard-0.0.3/CHANGELOG.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)     1065 2023-06-12 09:38:56.000000 genWizard-0.0.3/LICENSE.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)       49 2023-06-12 19:01:04.000000 genWizard-0.0.3/MANIFEST.in
+-rw-r--r--   0 yvonkim    (501) staff       (20)     5882 2023-06-14 15:46:58.015536 genWizard-0.0.3/PKG-INFO
+-rw-r--r--   0 yvonkim    (501) staff       (20)     5011 2023-06-12 20:12:25.000000 genWizard-0.0.3/README.txt
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-14 15:46:57.949861 genWizard-0.0.3/genWizard.egg-info/
+-rw-r--r--   0 yvonkim    (501) staff       (20)     5882 2023-06-14 15:46:57.000000 genWizard-0.0.3/genWizard.egg-info/PKG-INFO
+-rw-r--r--   0 yvonkim    (501) staff       (20)      325 2023-06-14 15:46:57.000000 genWizard-0.0.3/genWizard.egg-info/SOURCES.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        1 2023-06-14 15:46:57.000000 genWizard-0.0.3/genWizard.egg-info/dependency_links.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        7 2023-06-14 15:46:57.000000 genWizard-0.0.3/genWizard.egg-info/requires.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        8 2023-06-14 15:46:57.000000 genWizard-0.0.3/genWizard.egg-info/top_level.txt
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-14 15:46:58.003091 genWizard-0.0.3/modules/
+-rw-r--r--   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:33:40.000000 genWizard-0.0.3/modules/__init__.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)     2039 2023-06-12 08:57:22.000000 genWizard-0.0.3/modules/database_manager.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)      649 2023-06-12 09:38:56.000000 genWizard-0.0.3/modules/expander.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)     1236 2023-06-12 18:48:46.000000 genWizard-0.0.3/modules/generator.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)       38 2023-06-14 15:46:58.020420 genWizard-0.0.3/setup.cfg
+-rw-r--r--   0 yvonkim    (501) staff       (20)      727 2023-06-14 15:46:50.000000 genWizard-0.0.3/setup.py
```

### Comparing `genWizard-0.0.2/LICENSE.txt` & `genWizard-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.2/PKG-INFO` & `genWizard-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genWizard
-Version: 0.0.2
+Version: 0.0.3
 Summary: genWizard allows for versatile usage of openAI generation and prompting management.
 Home-page: https://github.com/ykim336/genWizard
 Author: Isaac Moon
 Author-email: ykim336@ucr.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,19 @@
 
 'genWizard' is a complex project aimed at utilizing AI for text generation, particularly using OpenAI's language models. it is designed around the concept of generating content based on provided prompts, and involves a multi-stage process of expanding prompts, evaluating the reliability and validity of generated outputs, and comparing these outputs.
 
 The purpose of the project is the allow anyone with little to no experience in coding AI to utilize the features of OpenAI's LLMs. 
 
 -----------------------------------------------------------------------------------
 
+SETUP:
+    -
+
+-----------------------------------------------------------------------------------
+
 DATABASE MANAGER CLASS:
     - `__init__(self)`: The constructor for the `DatabaseManager` class. This initializes the instance with a mapping of paths to different directories in your project.
 
     - `get_latest_file(self, path, number=1)`: This function retrieves the latest file(s) from a given directory, as determined by the `path` argument. If `number` is greater than 1, it will return the specified number of latest files. The returned files are sorted in descending order of creation time.
 
     - `write(self, id, content=None, filetype=".txt")`: This function writes content to a file in a directory specified by `id`. The file is named with the current timestamp and the provided `filetype`. If no content is given, it prompts the user to provide content.
 
@@ -56,15 +61,17 @@
 
     - `base_expansion(self, prompt_parts: list) -> str`: This function takes a list of string parts and joins them with two newline characters ("\n\n"). It is used for creating a prompt by joining multiple strings together in a specific format.
 
     - `expansion_generator(self, user_prompt: str, filename="expansion_generator_prompt.txt") -> list`: This function generates an expanded text based on a user-provided prompt. It reads an "expansion_prompt" from a file (default name "expansion_generator_prompt.txt") located in the directory associated with the ID 2 in the `DatabaseManager`'s path mapping. It then creates a full prompt by joining the "expansion_prompt" and the user's prompt using `base_expansion`. The full prompt is fed into the generator for text generation. The generated text is split by newline characters and returned as a list of strings. 
 
 In essence, the `Expander` class is used to expand a given prompt by adding additional content from a file and then generate text based on the expanded prompt.
 
+===================================================================================
 
-GENMAKE CHANGELOG
-===================
+GENWIZARD CHANGELOGS
 
-0.0.1
--------------------
+===================================================================================
+
+0.0.3
+-----------------------------------------------------------------------------------
 First Release
 - Includes the basic functions: Database Manager, Expander, and Generator.
```

### Comparing `genWizard-0.0.2/README.txt` & `genWizard-0.0.3/README.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 'genWizard' is a complex project aimed at utilizing AI for text generation, particularly using OpenAI's language models. it is designed around the concept of generating content based on provided prompts, and involves a multi-stage process of expanding prompts, evaluating the reliability and validity of generated outputs, and comparing these outputs.
 
 The purpose of the project is the allow anyone with little to no experience in coding AI to utilize the features of OpenAI's LLMs. 
 
 -----------------------------------------------------------------------------------
 
+SETUP:
+    -
+
+-----------------------------------------------------------------------------------
+
 DATABASE MANAGER CLASS:
     - `__init__(self)`: The constructor for the `DatabaseManager` class. This initializes the instance with a mapping of paths to different directories in your project.
 
     - `get_latest_file(self, path, number=1)`: This function retrieves the latest file(s) from a given directory, as determined by the `path` argument. If `number` is greater than 1, it will return the specified number of latest files. The returned files are sorted in descending order of creation time.
 
     - `write(self, id, content=None, filetype=".txt")`: This function writes content to a file in a directory specified by `id`. The file is named with the current timestamp and the provided `filetype`. If no content is given, it prompts the user to provide content.
```

### Comparing `genWizard-0.0.2/genWizard.egg-info/PKG-INFO` & `genWizard-0.0.3/genWizard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genWizard
-Version: 0.0.2
+Version: 0.0.3
 Summary: genWizard allows for versatile usage of openAI generation and prompting management.
 Home-page: https://github.com/ykim336/genWizard
 Author: Isaac Moon
 Author-email: ykim336@ucr.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,19 @@
 
 'genWizard' is a complex project aimed at utilizing AI for text generation, particularly using OpenAI's language models. it is designed around the concept of generating content based on provided prompts, and involves a multi-stage process of expanding prompts, evaluating the reliability and validity of generated outputs, and comparing these outputs.
 
 The purpose of the project is the allow anyone with little to no experience in coding AI to utilize the features of OpenAI's LLMs. 
 
 -----------------------------------------------------------------------------------
 
+SETUP:
+    -
+
+-----------------------------------------------------------------------------------
+
 DATABASE MANAGER CLASS:
     - `__init__(self)`: The constructor for the `DatabaseManager` class. This initializes the instance with a mapping of paths to different directories in your project.
 
     - `get_latest_file(self, path, number=1)`: This function retrieves the latest file(s) from a given directory, as determined by the `path` argument. If `number` is greater than 1, it will return the specified number of latest files. The returned files are sorted in descending order of creation time.
 
     - `write(self, id, content=None, filetype=".txt")`: This function writes content to a file in a directory specified by `id`. The file is named with the current timestamp and the provided `filetype`. If no content is given, it prompts the user to provide content.
 
@@ -56,15 +61,17 @@
 
     - `base_expansion(self, prompt_parts: list) -> str`: This function takes a list of string parts and joins them with two newline characters ("\n\n"). It is used for creating a prompt by joining multiple strings together in a specific format.
 
     - `expansion_generator(self, user_prompt: str, filename="expansion_generator_prompt.txt") -> list`: This function generates an expanded text based on a user-provided prompt. It reads an "expansion_prompt" from a file (default name "expansion_generator_prompt.txt") located in the directory associated with the ID 2 in the `DatabaseManager`'s path mapping. It then creates a full prompt by joining the "expansion_prompt" and the user's prompt using `base_expansion`. The full prompt is fed into the generator for text generation. The generated text is split by newline characters and returned as a list of strings. 
 
 In essence, the `Expander` class is used to expand a given prompt by adding additional content from a file and then generate text based on the expanded prompt.
 
+===================================================================================
 
-GENMAKE CHANGELOG
-===================
+GENWIZARD CHANGELOGS
 
-0.0.1
--------------------
+===================================================================================
+
+0.0.3
+-----------------------------------------------------------------------------------
 First Release
 - Includes the basic functions: Database Manager, Expander, and Generator.
```

### Comparing `genWizard-0.0.2/modules/database_manager.py` & `genWizard-0.0.3/modules/database_manager.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.2/modules/expander.py` & `genWizard-0.0.3/modules/expander.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.2/modules/generator.py` & `genWizard-0.0.3/modules/generator.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.2/setup.py` & `genWizard-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='genWizard',
-    version='0.0.2',
+    version='0.0.3',
     description='genWizard allows for versatile usage of openAI generation and prompting management.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/ykim336/genWizard',
     license='MIT',
     classifiers=classifiers,
     keywords='machine learning',
     author='Isaac Moon',
```

