# Comparing `tmp/lazydev-0.0.8.tar.gz` & `tmp/lazydev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.8.tar", last modified: Tue Jun 13 08:12:03 2023, max compression
+gzip compressed data, was "lazydev-0.0.9.tar", last modified: Tue Jun 13 22:31:23 2023, max compression
```

## Comparing `lazydev-0.0.8.tar` & `lazydev-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.665321 lazydev-0.0.8/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.8/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 08:12:03.665161 lazydev-0.0.8/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3883 2023-06-03 08:10:06.000000 lazydev-0.0.8/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.662711 lazydev-0.0.8/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.8/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.8/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.664739 lazydev-0.0.8/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.8/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     7760 2023-06-13 08:08:23.000000 lazydev-0.0.8/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     6898 2023-06-13 08:10:27.000000 lazydev-0.0.8/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.0.8/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.663775 lazydev-0.0.8/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-13 08:12:03.665367 lazydev-0.0.8/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1482 2023-06-13 08:10:38.000000 lazydev-0.0.8/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 22:31:23.684301 lazydev-0.0.9/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.9/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 22:31:23.684162 lazydev-0.0.9/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3883 2023-06-03 08:10:06.000000 lazydev-0.0.9/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 22:31:23.681809 lazydev-0.0.9/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.9/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.9/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 22:31:23.683822 lazydev-0.0.9/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.9/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     7847 2023-06-13 08:30:21.000000 lazydev-0.0.9/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     6943 2023-06-13 08:36:03.000000 lazydev-0.0.9/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.0.9/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 22:31:23.682997 lazydev-0.0.9/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-13 22:31:23.000000 lazydev-0.0.9/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-13 22:31:23.684337 lazydev-0.0.9/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1579 2023-06-13 08:45:32.000000 lazydev-0.0.9/setup.py
```

### Comparing `lazydev-0.0.8/LICENSE` & `lazydev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.8/PKG-INFO` & `lazydev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.8/README.md` & `lazydev-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.8/lazydev/develop.py` & `lazydev-0.0.9/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.8/lazydev/modules/developer.py` & `lazydev-0.0.9/lazydev/modules/developer.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,17 @@
                     plan=self.plannings,
                     files_written=self.files_written,
                     file_path_to_write=file_path,
                     file_paths=self.file_paths
                 )
                 response = self.brain_storm(
                     review_prompt, f'code-{file_path.split("/")[-1]}')
-                response = response.strip('"\'`-\n')
-                if (response.strip('"\'`-\n') == "NONE"):
+                response = response.strip('."\'`-\n')
+                nonecheck_response = response.split("\n")[0].split(" ")[0]
+                if (nonecheck_response.strip('."\'`-\n') == "NONE"):
                     break
                 code = response
 
         Utilities.write_to_file(code, file_path=file_path)
         # compress the code
         compressed_code = self.brain_storm(PromptBook.get_compressed_code(
             code), f'code-compressed-{file_path.split("/")[-1]}')
```

### Comparing `lazydev-0.0.8/lazydev/modules/prompts.py` & `lazydev-0.0.9/lazydev/modules/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,19 +175,23 @@
 ---
 {draft}
 ---
 
 your job is to find problems with the code and refine it. 
 
 As your response will go to an automated parser, things to keep in mind all the time:
-* if no refinement is required then just say NONE, and nothing else
+* if no refinement is required then just say "NONE", and nothing else
 * only write the file content, no expiation, no pretext as this will directly go as code.
 * if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
+
+File: {file_path_to_write}
+
+Refined code:
 """
 
     def get_compressed_code(code: str):
         return f"""
 compress the code below as best as you can, dont rename any data:
 ```
 {code}
```

### Comparing `lazydev-0.0.8/lazydev/modules/utils.py` & `lazydev-0.0.9/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.8/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.9/lazydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.8/setup.py` & `lazydev-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
@@ -42,7 +42,12 @@
 
     # # You can also specify additional non-package data files
     # data_files=[
     #     ('config', ['config.ini']),
     # ],
 
 )
+
+# steps to build and publish
+# source .venv/bin/activate
+# python -m bild
+# twine upload dist/*
```

