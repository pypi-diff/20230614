# Comparing `tmp/pacman-prompts-1.1.1.tar.gz` & `tmp/pacman-prompts-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacman-prompts-1.1.1.tar", last modified: Mon Mar 27 18:07:30 2023, max compression
+gzip compressed data, was "pacman-prompts-1.2.0.tar", last modified: Thu Apr 27 21:37:16 2023, max compression
```

## Comparing `pacman-prompts-1.1.1.tar` & `pacman-prompts-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-03-27 18:07:30.148173 pacman-prompts-1.1.1/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-03-27 18:07:30.148015 pacman-prompts-1.1.1/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.1.1/README.md
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-03-27 18:07:30.147031 pacman-prompts-1.1.1/pacman/
--rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.1.1/pacman/__init__.py
--rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.1.1/pacman/file_utils.py
--rw-r--r--   0 anishthite   (501) staff       (20)      398 2023-03-17 19:44:52.000000 pacman-prompts-1.1.1/pacman/pacman.py
--rw-r--r--   0 anishthite   (501) staff       (20)     1122 2023-03-27 18:02:44.000000 pacman-prompts-1.1.1/pacman/prompt.py
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-03-27 18:07:30.147858 pacman-prompts-1.1.1/pacman_prompts.egg-info/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-03-27 18:07:30.000000 pacman-prompts-1.1.1/pacman_prompts.egg-info/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-03-27 18:07:30.000000 pacman-prompts-1.1.1/pacman_prompts.egg-info/SOURCES.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-03-27 18:07:30.000000 pacman-prompts-1.1.1/pacman_prompts.egg-info/dependency_links.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-03-27 18:07:30.000000 pacman-prompts-1.1.1/pacman_prompts.egg-info/requires.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-03-27 18:07:30.000000 pacman-prompts-1.1.1/pacman_prompts.egg-info/top_level.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-03-27 18:07:30.148216 pacman-prompts-1.1.1/setup.cfg
--rw-r--r--   0 anishthite   (501) staff       (20)      821 2023-03-27 18:07:22.000000 pacman-prompts-1.1.1/setup.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-04-27 21:37:16.306085 pacman-prompts-1.2.0/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-04-27 21:37:16.305924 pacman-prompts-1.2.0/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.2.0/README.md
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-04-27 21:37:16.304904 pacman-prompts-1.2.0/pacman/
+-rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.2.0/pacman/__init__.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.2.0/pacman/file_utils.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      637 2023-04-25 19:15:29.000000 pacman-prompts-1.2.0/pacman/pacman.py
+-rw-r--r--   0 anishthite   (501) staff       (20)     1646 2023-04-24 20:12:16.000000 pacman-prompts-1.2.0/pacman/prompt.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-04-27 21:37:16.305747 pacman-prompts-1.2.0/pacman_prompts.egg-info/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-04-27 21:37:16.000000 pacman-prompts-1.2.0/pacman_prompts.egg-info/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-04-27 21:37:16.000000 pacman-prompts-1.2.0/pacman_prompts.egg-info/SOURCES.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-04-27 21:37:16.000000 pacman-prompts-1.2.0/pacman_prompts.egg-info/dependency_links.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-04-27 21:37:16.000000 pacman-prompts-1.2.0/pacman_prompts.egg-info/requires.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-04-27 21:37:16.000000 pacman-prompts-1.2.0/pacman_prompts.egg-info/top_level.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-04-27 21:37:16.306127 pacman-prompts-1.2.0/setup.cfg
+-rw-r--r--   0 anishthite   (501) staff       (20)      821 2023-04-23 17:54:46.000000 pacman-prompts-1.2.0/setup.py
```

### Comparing `pacman-prompts-1.1.1/PKG-INFO` & `pacman-prompts-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.1.1
+Version: 1.2.0
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.1.1/README.md` & `pacman-prompts-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pacman-prompts-1.1.1/pacman/prompt.py` & `pacman-prompts-1.2.0/pacman/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,8 +38,23 @@
 
     def __call__(self, inputs, **kwargs):
         return self.run(inputs, **kwargs)
 
 def load_prompt(loaded_file):
     prompt = Prompt(**loaded_file)
 
+#make copy of Prompt class but use ChatCompletion in run method
+class ChatPrompt(Prompt):
+    def run(self, inputs, **kwargs):
+        #format string
+        complete_prompt = self.compile(inputs)
+        if  kwargs.get('debug', True):
+            print(complete_prompt)
+        #run in language model
+        res = openai.ChatCompletion.create(
+            messages=[{"role": "user","content": complete_prompt}],
+            **self.config.__dict__
+            #stop='\n'
+        )
+        return res
+        #return output
```

### Comparing `pacman-prompts-1.1.1/pacman_prompts.egg-info/PKG-INFO` & `pacman-prompts-1.2.0/pacman_prompts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.1.1
+Version: 1.2.0
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.1.1/setup.py` & `pacman-prompts-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pacman-prompts',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.1',
+  version = '1.2.0',
   license='MIT',
   description = 'Prompts As Code, man',
   long_description_content_type = 'text/markdown',
   author = 'Anish Thite',
   author_email = 'anishthite@gmail.com',
   url = 'https://github.com/anishthite/pacman',
   keywords = [
```

