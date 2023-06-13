# Comparing `tmp/gptbase-0.1.2.tar.gz` & `tmp/gptbase-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptbase-0.1.2.tar", last modified: Sun May 28 15:23:53 2023, max compression
+gzip compressed data, was "gptbase-0.2.3.tar", last modified: Tue Jun 13 22:38:25 2023, max compression
```

## Comparing `gptbase-0.1.2.tar` & `gptbase-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 15:23:53.424613 gptbase-0.1.2/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     2143 2023-05-28 15:23:53.424613 gptbase-0.1.2/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)     1699 2023-05-28 09:17:00.000000 gptbase-0.1.2/README.md
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 15:23:53.424613 gptbase-0.1.2/gptbase/
--rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.1.2/gptbase/__init__.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-05-28 09:02:05.000000 gptbase-0.1.2/gptbase/base.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)     6529 2023-05-28 09:47:37.000000 gptbase-0.1.2/gptbase/basev2.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      409 2023-05-28 08:51:32.000000 gptbase-0.1.2/gptbase/chat.py
--rw-r--r--   0 ershan    (1000) ershan    (1000)      110 2023-05-28 09:47:37.000000 gptbase-0.1.2/gptbase/const.py
-drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-05-28 15:23:53.424613 gptbase-0.1.2/gptbase.egg-info/
--rw-r--r--   0 ershan    (1000) ershan    (1000)     2143 2023-05-28 15:23:53.000000 gptbase-0.1.2/gptbase.egg-info/PKG-INFO
--rw-r--r--   0 ershan    (1000) ershan    (1000)      259 2023-05-28 15:23:53.000000 gptbase-0.1.2/gptbase.egg-info/SOURCES.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-05-28 15:23:53.000000 gptbase-0.1.2/gptbase.egg-info/dependency_links.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       44 2023-05-28 15:23:53.000000 gptbase-0.1.2/gptbase.egg-info/requires.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-05-28 15:23:53.000000 gptbase-0.1.2/gptbase.egg-info/top_level.txt
--rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-05-28 15:23:53.424613 gptbase-0.1.2/setup.cfg
--rw-r--r--   0 ershan    (1000) ershan    (1000)      811 2023-05-28 15:22:49.000000 gptbase-0.1.2/setup.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:38:25.238841 gptbase-0.2.3/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3455 2023-06-13 22:33:12.000000 gptbase-0.2.3/README.md
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/gptbase/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       80 2023-05-28 09:02:58.000000 gptbase-0.2.3/gptbase/__init__.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     1507 2023-06-04 12:19:20.000000 gptbase-0.2.3/gptbase/base.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)    10729 2023-06-13 22:17:25.000000 gptbase-0.2.3/gptbase/basev2.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      677 2023-06-13 22:35:49.000000 gptbase-0.2.3/gptbase/chat.py
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      110 2023-05-28 09:47:37.000000 gptbase-0.2.3/gptbase/const.py
+drwxr-xr-x   0 ershan    (1000) ershan    (1000)        0 2023-06-13 22:38:25.238841 gptbase-0.2.3/gptbase.egg-info/
+-rw-r--r--   0 ershan    (1000) ershan    (1000)     3899 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/PKG-INFO
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      293 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/SOURCES.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        1 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/dependency_links.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       51 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/entry_points.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       57 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/requires.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)        8 2023-06-13 22:38:25.000000 gptbase-0.2.3/gptbase.egg-info/top_level.txt
+-rw-r--r--   0 ershan    (1000) ershan    (1000)       38 2023-06-13 22:38:25.238841 gptbase-0.2.3/setup.cfg
+-rw-r--r--   0 ershan    (1000) ershan    (1000)      947 2023-06-13 22:36:37.000000 gptbase-0.2.3/setup.py
```

### Comparing `gptbase-0.1.2/gptbase/base.py` & `gptbase-0.2.3/gptbase/base.py`

 * *Files identical despite different names*

### Comparing `gptbase-0.1.2/setup.py` & `gptbase-0.2.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gptbase",
-    version="0.1.2",
+    version="0.2.3",
     author="callmexss",
     author_email="callmexss@126.com",
     description="A package for simplified interaction with OpenAI's GPT-3 and GPT-4 models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/callmexss/gptbase",
     packages=find_packages(include=["gptbase"]),
     install_requires=[
         "openai==0.27.7",
         "rich==13.0.1",
         "tiktoken==0.3.0",
+        "click==8.0.3",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
+    entry_points={
+        'console_scripts': [
+            'gptbase-chat=gptbase.chat:chat',
+        ],
+    },
 )
```

