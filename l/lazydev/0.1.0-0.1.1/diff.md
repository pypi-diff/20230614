# Comparing `tmp/lazydev-0.1.0.tar.gz` & `tmp/lazydev-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.1.0.tar", last modified: Wed Jun 14 14:44:03 2023, max compression
+gzip compressed data, was "lazydev-0.1.1.tar", last modified: Wed Jun 14 16:39:02 2023, max compression
```

## Comparing `lazydev-0.1.0.tar` & `lazydev-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 14:44:03.630791 lazydev-0.1.0/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.1.0/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4977 2023-06-14 14:44:03.630576 lazydev-0.1.0/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     4307 2023-06-14 14:43:14.000000 lazydev-0.1.0/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 14:44:03.626458 lazydev-0.1.0/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.1.0/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1417 2023-06-14 14:36:14.000000 lazydev-0.1.0/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 14:44:03.630174 lazydev-0.1.0/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.1.0/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     7847 2023-06-13 08:30:21.000000 lazydev-0.1.0/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     6943 2023-06-13 08:36:03.000000 lazydev-0.1.0/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.1.0/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 14:44:03.629052 lazydev-0.1.0/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4977 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-14 14:44:03.000000 lazydev-0.1.0/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-14 14:44:03.630842 lazydev-0.1.0/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1579 2023-06-14 14:43:51.000000 lazydev-0.1.0/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 16:39:02.610561 lazydev-0.1.1/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.1.1/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4977 2023-06-14 16:39:02.610420 lazydev-0.1.1/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4307 2023-06-14 14:43:14.000000 lazydev-0.1.1/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 16:39:02.608150 lazydev-0.1.1/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.1.1/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1417 2023-06-14 14:36:14.000000 lazydev-0.1.1/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 16:39:02.610008 lazydev-0.1.1/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.1.1/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     8344 2023-06-14 16:35:25.000000 lazydev-0.1.1/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     8194 2023-06-14 16:33:10.000000 lazydev-0.1.1/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.1.1/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-14 16:39:02.609138 lazydev-0.1.1/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4977 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-14 16:39:02.000000 lazydev-0.1.1/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-14 16:39:02.610600 lazydev-0.1.1/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1579 2023-06-14 16:37:47.000000 lazydev-0.1.1/setup.py
```

### Comparing `lazydev-0.1.0/LICENSE` & `lazydev-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.1.0/PKG-INFO` & `lazydev-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.1.0/README.md` & `lazydev-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lazydev-0.1.0/lazydev/develop.py` & `lazydev-0.1.1/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.1.0/lazydev/modules/developer.py` & `lazydev-0.1.1/lazydev/modules/developer.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,15 +122,16 @@
             print("Sorry I was not able to create the folder structure in json correct format, check my instructions and try to refine it sothat i can understan the task better")
             sys.exit()
         self.root_folder_name, self.file_paths = Utilities.generate_files_and_folders(
             structure=folder_tree, root_dir=self.root_dir)
         return self.root_folder_name, self.file_paths
 
     def prioratize_files(self):
-        prompt = PromptBook.prioritise_file_list(self.file_paths)
+        prompt = PromptBook.prioritise_file_list(
+            self.file_paths, self.plannings)
         retry_count = 3
         while retry_count > 0:
             try:
                 file_paths_str = self.brain_storm(prompt, 'prioratize_files')
                 break
             except:
                 print("Opps messed up the json format, let me try again")
@@ -177,14 +178,25 @@
         compressed_code = self.brain_storm(PromptBook.get_compressed_code(
             code), f'code-compressed-{file_path.split("/")[-1]}')
         self.files_written.append((
             file_path,
             compressed_code
         ))
 
+    def final_instruction(self):
+        prompt = PromptBook.generate_instruction(
+            question=self.requirement,
+            clarifications=self.clarifications,
+            plan=self.plannings,
+            files_written=self.files_written,
+            file_paths=self.file_paths
+        )
+        instruction = self.brain_storm(prompt, f'instructions')
+        return instruction
+
     def develop(self):
         # clearing all doubts
         doubts, answers = self.clear_doubts()
         self.clarifications = self.get_clarifications(
             doubts=doubts, answers=answers)
         # planning the project
         print("Brainstorming ideas...")
@@ -198,8 +210,10 @@
         self.prioratize_files()
         self.files_written = []
         for file_path in self.file_paths:
             file_name = file_path.split("/")[-1]
             if (file_name.split(".")[-1] in ["png", "jpg", "jpeg", "bimp", "lock"]):
                 continue
             print(f"\nWriting Code for :{file_name}")
-            self.write_file_content(file_path, review_iteration=2)
+            self.write_file_content(file_path, review_iteration=1)
+        print("\n\nI am done!!!\n\n")
+        print(self.final_instruction())
```

### Comparing `lazydev-0.1.0/lazydev/modules/prompts.py` & `lazydev-0.1.1/lazydev/modules/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,23 +73,26 @@
         }}
     ]
 }}
 ```
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * only write the json nothing else, no expiation, no pretext 
-* do not write the contents of the files that will be done by the next developer
+* only write the folders and files structure
 Begin!
 """
 
     @staticmethod
-    def prioritise_file_list(filelist: List[str]) -> List[str]:
+    def prioritise_file_list(filelist: List[str], plan: str | None = None) -> List[str]:
         list_string = '\n'.join(filelist)
+        plan = 'below is the project plan:\n---'+plan+"\n---" if plan != None else ""
         return f"""
-you are a senior programmer. you going to write a api service.
+you are a senior programmer. you going to write a program for client.
+
+{plan}
 below are the file list that you are going to complete in future.
 
 reorder them in a way that most suitable based on how one will be dependent on other
 
 {list_string}
 
 As your response will go to an automated parser, things to keep in mind all the time:
@@ -137,15 +140,22 @@
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
 
 File:{file_path_to_write}
 Content:
 """
 
-    def get_code_feedback(draft: str, question, clarifications: str, plan: str, files_written: List[List[str]], file_path_to_write: str, file_paths: List[str]) -> str:
+    def get_code_feedback(
+            draft: str,
+            question,
+            clarifications: str,
+            plan: str,
+            files_written: List[List[str]],
+            file_path_to_write: str,
+            file_paths: List[str]) -> str:
         file_with_conent = "\n\n".join(
             [f"File:{file_path}\nContent:\n{content}" for file_path, content in files_written])
         all_files_list = "\n".join(file_paths)
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
@@ -208,7 +218,42 @@
 ```
 {text}
 ```
 As your response will go to an automated parser, things to keep in mind all the time:
 * only respond with the compressed text and nothing else
 Begin!
         """
+
+    def generate_instruction(question, clarifications: str, plan: str, files_written: List[List[str]], file_paths: List[str]) -> str:
+        file_with_conent = "\n\n".join(
+            [f"File:{file_path}\nContent:\n{content}" for file_path, content in files_written])
+        all_files_list = "\n".join(file_paths)
+        return f"""
+you are a senior programmer below is what your client have asked you to do:
+---
+{question}
+---
+here are some clarrification on the requirements
+---
+{clarifications}
+---
+below is the what you have already planed what to do:
+---
+{plan}
+---
+Below are the full files list that already has been or will be written
+--
+{all_files_list}
+--
+
+you are now writing the code below are the files that already written with content as follows:
+---
+{file_with_conent}
+---
+
+now you are need to give client further instruction on what you have developped and how to use it, basically write instruction for the client
+
+As your response will go to an automated parser, things to keep in mind all the time:
+* make the instruction clear and simple 
+
+Begin!
+"""
```

### Comparing `lazydev-0.1.0/lazydev/modules/utils.py` & `lazydev-0.1.1/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.1.0/lazydev.egg-info/PKG-INFO` & `lazydev-0.1.1/lazydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.1.0
+Version: 0.1.1
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.1.0/setup.py` & `lazydev-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

