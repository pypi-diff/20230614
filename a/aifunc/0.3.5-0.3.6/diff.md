# Comparing `tmp/aifunc-0.3.5.tar.gz` & `tmp/aifunc-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.3.5.tar", max compression
+gzip compressed data, was "aifunc-0.3.6.tar", max compression
```

## Comparing `aifunc-0.3.5.tar` & `aifunc-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,8 @@
--rw-r--r--   0        0        0      126 2023-06-13 22:25:34.728002 aifunc-0.3.5/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.3.5/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      372 2023-06-13 21:47:21.569396 aifunc-0.3.5/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0     3180 2023-06-13 21:46:26.251737 aifunc-0.3.5/aifunc/evaluate_answer.yaml
--rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.3.5/aifunc/follow_up.py
--rw-r--r--   0        0        0     1812 2023-06-13 22:07:51.183195 aifunc-0.3.5/aifunc/follow_up.yaml
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.5/aifunc/generate_question.py
--rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.5/aifunc/generate_question.yaml
--rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.5/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-13 22:25:37.392275 aifunc-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      126 2023-06-13 22:25:34.728002 aifunc-0.3.6/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-13 22:04:13.296903 aifunc-0.3.6/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-14 01:36:26.006316 aifunc-0.3.6/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-13 22:08:50.857300 aifunc-0.3.6/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.6/aifunc/generate_question.py
+-rw-r--r--   0        0        0     3400 2023-06-14 01:42:54.282815 aifunc-0.3.6/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-14 01:44:00.869074 aifunc-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.6/PKG-INFO
```

### Comparing `aifunc-0.3.5/aifunc/add_ai_function.py` & `aifunc-0.3.6/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.3.5/aifunc/utility.py` & `aifunc-0.3.6/aifunc/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,25 @@
           raise e  # re-raise the last exception
 
   ai_function.__name__ = function_name  # Set the function name
   return ai_function
 
 
 def create_ai_function_from_yaml(yaml_file):
-  # get the current path of this file
+  # download from https://github.com/ZiyanWu93/sturdy-memory/blob/main/{yaml_file}
+  import urllib.request
+  url = "https://raw.githubusercontent.com/ZiyanWu93/sturdy-memory/main/{}".format(
+    yaml_file)
+  # save the file current_path + yaml_file
   current_path = os.path.dirname(os.path.abspath(__file__))
-  yaml_path = os.path.join(current_path, yaml_file)
-  with open(yaml_path, 'r') as stream:
-    data_loaded = yaml.safe_load(stream)
-
+  save_path = current_path + "/" + yaml_file
+  urllib.request.urlretrieve(url, save_path)
+  # load the yaml file
+  with open(current_path + "/" + yaml_file, "r") as f:
+    data_loaded = yaml.load(f, Loader=yaml.FullLoader)
   function_name = data_loaded['function_name']
   instruction = data_loaded['instruction']
   if 'temperature' in data_loaded:
     temperature = data_loaded['temperature']
   else:
     temperature = 0.7
   example_conversations = data_loaded['example_conversations']
```

