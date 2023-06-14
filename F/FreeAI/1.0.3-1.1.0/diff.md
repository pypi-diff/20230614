# Comparing `tmp/FreeAI-1.0.3.tar.gz` & `tmp/FreeAI-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeAI-1.0.3.tar", last modified: Wed Jun 14 16:15:16 2023, max compression
+gzip compressed data, was "FreeAI-1.1.0.tar", last modified: Wed Jun 14 18:36:21 2023, max compression
```

## Comparing `FreeAI-1.0.3.tar` & `FreeAI-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:15:16.344729 FreeAI-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     3698 2023-06-14 16:15:16.344729 FreeAI-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2869 2023-06-14 21:40:40.000000 FreeAI-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)      811 2023-06-14 21:41:56.000000 FreeAI-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 16:15:16.344729 FreeAI-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-14 15:32:12.000000 FreeAI-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:15:16.342729 FreeAI-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:15:16.343729 FreeAI-1.0.3/src/FreeAI/
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-14 15:38:00.000000 FreeAI-1.0.3/src/FreeAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-14 20:47:44.000000 FreeAI-1.0.3/src/FreeAI/generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:15:16.344729 FreeAI-1.0.3/src/FreeAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3698 2023-06-14 16:15:16.000000 FreeAI-1.0.3/src/FreeAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-14 16:15:16.000000 FreeAI-1.0.3/src/FreeAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 16:15:16.000000 FreeAI-1.0.3/src/FreeAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 16:15:16.000000 FreeAI-1.0.3/src/FreeAI.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-14 16:15:16.000000 FreeAI-1.0.3/src/FreeAI.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:36:21.595564 FreeAI-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-06-14 18:36:21.595564 FreeAI-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-06-14 23:33:02.000000 FreeAI-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      811 2023-06-14 23:56:32.000000 FreeAI-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 18:36:21.595564 FreeAI-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-14 23:30:50.000000 FreeAI-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:36:21.592563 FreeAI-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:36:21.594564 FreeAI-1.1.0/src/FreeAI/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-14 15:38:00.000000 FreeAI-1.1.0/src/FreeAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-06-14 23:30:14.000000 FreeAI-1.1.0/src/FreeAI/generator.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-14 23:29:06.000000 FreeAI-1.1.0/src/FreeAI/logger.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-14 23:29:26.000000 FreeAI-1.1.0/src/FreeAI/memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:36:21.595564 FreeAI-1.1.0/src/FreeAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-06-14 18:36:21.000000 FreeAI-1.1.0/src/FreeAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      291 2023-06-14 18:36:21.000000 FreeAI-1.1.0/src/FreeAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:36:21.000000 FreeAI-1.1.0/src/FreeAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-14 18:36:21.000000 FreeAI-1.1.0/src/FreeAI.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-14 18:36:21.000000 FreeAI-1.1.0/src/FreeAI.egg-info/top_level.txt
```

### Comparing `FreeAI-1.0.3/PKG-INFO` & `FreeAI-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: FreeAI
-Version: 1.0.3
+Version: 1.1.0
 Summary: FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 Author: Ashiq Hussain
 Author-email: Ashiq Hussain <imseldrith@gmail.com>
 Project-URL: Homepage, https://github.com/mir-ashiq/FreeAI
 Project-URL: Bug Tracker, https://github.com/mir-ashiq/FreeAI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# FreeAI: An Advanced GPT-based Text Generation Package
+# FreeAI: Advanced GPT-based Text Generation Package
 
-<!-- ![FreeAI Logo](/img/freeai_logo.png)-->
+![FreeAI Logo](/img/freeai_logo.png)
 
 FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT-3/4 (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 
 ## Features
 
 - **Advanced GPT Text Generation**: FreeAI leverages state-of-the-art GPT models to generate high-quality and contextually relevant text.
 - **Flexible Prompt Customization**: Users can easily provide their own prompts to guide the text generation process.
@@ -64,10 +64,10 @@
 
 ## License
 
 FreeAI is released under the MIT License. See the [LICENSE](https://github.com/mir-ashiq/FreeAI/blob/main/LICENSE) file for more details.
 
 ---
 
-FreeAI is developed and maintained by Ashiq Hussain(https://github.com/mir-ashiq). We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
+FreeAI is developed and maintained by Ashiq Hussain. We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
 
 Happy text generation with FreeAI!
```

### Comparing `FreeAI-1.0.3/README.md` & `FreeAI-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# FreeAI: An Advanced GPT-based Text Generation Package
+# FreeAI: Advanced GPT-based Text Generation Package
 
-<!-- ![FreeAI Logo](/img/freeai_logo.png)-->
+![FreeAI Logo](/img/freeai_logo.png)
 
 FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT-3/4 (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 
 ## Features
 
 - **Advanced GPT Text Generation**: FreeAI leverages state-of-the-art GPT models to generate high-quality and contextually relevant text.
 - **Flexible Prompt Customization**: Users can easily provide their own prompts to guide the text generation process.
@@ -50,10 +50,10 @@
 
 ## License
 
 FreeAI is released under the MIT License. See the [LICENSE](https://github.com/mir-ashiq/FreeAI/blob/main/LICENSE) file for more details.
 
 ---
 
-FreeAI is developed and maintained by Ashiq Hussain(https://github.com/mir-ashiq). We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
+FreeAI is developed and maintained by Ashiq Hussain. We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
 
 Happy text generation with FreeAI!
```

### Comparing `FreeAI-1.0.3/pyproject.toml` & `FreeAI-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "FreeAI"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="Ashiq Hussain", email="imseldrith@gmail.com" }
 ]
 description = "FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FreeAI-1.0.3/setup.py` & `FreeAI-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FreeAI',
-    version='1.0.2',
+    version='1.1.0',
     author='Ashiq Hussain',
     author_email='imseldrith@gmail.com',
     description='FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
         'requests',
+        'python-dateutil'
     ],
 )
```

### Comparing `FreeAI-1.0.3/src/FreeAI.egg-info/PKG-INFO` & `FreeAI-1.1.0/src/FreeAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: FreeAI
-Version: 1.0.3
+Version: 1.1.0
 Summary: FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 Author: Ashiq Hussain
 Author-email: Ashiq Hussain <imseldrith@gmail.com>
 Project-URL: Homepage, https://github.com/mir-ashiq/FreeAI
 Project-URL: Bug Tracker, https://github.com/mir-ashiq/FreeAI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# FreeAI: An Advanced GPT-based Text Generation Package
+# FreeAI: Advanced GPT-based Text Generation Package
 
-<!-- ![FreeAI Logo](/img/freeai_logo.png)-->
+![FreeAI Logo](/img/freeai_logo.png)
 
 FreeAI is a powerful Python package that utilizes the advanced capabilities of GPT-3/4 (Generative Pre-trained Transformer) models for text generation. It allows users to generate creative and context-aware text based on a given prompt. Whether you need to generate code snippets, creative writing pieces, or technical documentation, FreeAI has got you covered.
 
 ## Features
 
 - **Advanced GPT Text Generation**: FreeAI leverages state-of-the-art GPT models to generate high-quality and contextually relevant text.
 - **Flexible Prompt Customization**: Users can easily provide their own prompts to guide the text generation process.
@@ -64,10 +64,10 @@
 
 ## License
 
 FreeAI is released under the MIT License. See the [LICENSE](https://github.com/mir-ashiq/FreeAI/blob/main/LICENSE) file for more details.
 
 ---
 
-FreeAI is developed and maintained by Ashiq Hussain(https://github.com/mir-ashiq). We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
+FreeAI is developed and maintained by Ashiq Hussain. We are dedicated to providing advanced AI solutions to empower developers and enhance their productivity. If you have any questions or need support, feel free to reach out to us at imseldrith@gmail.com.
 
 Happy text generation with FreeAI!
```

