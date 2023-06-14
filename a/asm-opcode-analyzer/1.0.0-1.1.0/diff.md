# Comparing `tmp/asm-opcode-analyzer-1.0.0.tar.gz` & `tmp/asm-opcode-analyzer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asm-opcode-analyzer-1.0.0.tar", last modified: Thu Jun  8 10:36:23 2023, max compression
+gzip compressed data, was "asm-opcode-analyzer-1.1.0.tar", last modified: Wed Jun 14 06:52:31 2023, max compression
```

## Comparing `asm-opcode-analyzer-1.0.0.tar` & `asm-opcode-analyzer-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-08 10:36:23.599538 asm-opcode-analyzer-1.0.0/
--rw-r--r--   0 mustaqeem   (501) staff       (20)    35149 2023-06-08 09:18:28.000000 asm-opcode-analyzer-1.0.0/LICENSE
--rw-r--r--   0 mustaqeem   (501) staff       (20)     1064 2023-06-08 10:36:23.599294 asm-opcode-analyzer-1.0.0/PKG-INFO
--rw-r--r--   0 mustaqeem   (501) staff       (20)      292 2023-06-08 09:18:28.000000 asm-opcode-analyzer-1.0.0/README.md
-drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-08 10:36:23.597634 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer/
--rw-r--r--   0 mustaqeem   (501) staff       (20)        0 2023-06-08 09:21:15.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer/__init__.py
--rw-r--r--   0 mustaqeem   (501) staff       (20)     5513 2023-06-08 09:41:42.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer/parser.py
-drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-08 10:36:23.598973 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/
--rw-r--r--   0 mustaqeem   (501) staff       (20)     1064 2023-06-08 10:36:23.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 mustaqeem   (501) staff       (20)      260 2023-06-08 10:36:23.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 mustaqeem   (501) staff       (20)        1 2023-06-08 10:36:23.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 mustaqeem   (501) staff       (20)       20 2023-06-08 10:36:23.000000 asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/top_level.txt
--rw-r--r--   0 mustaqeem   (501) staff       (20)       38 2023-06-08 10:36:23.599583 asm-opcode-analyzer-1.0.0/setup.cfg
--rw-r--r--   0 mustaqeem   (501) staff       (20)      995 2023-06-08 10:33:47.000000 asm-opcode-analyzer-1.0.0/setup.py
+drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-14 06:52:31.050764 asm-opcode-analyzer-1.1.0/
+-rw-r--r--   0 mustaqeem   (501) staff       (20)    35149 2023-06-08 09:18:28.000000 asm-opcode-analyzer-1.1.0/LICENSE
+-rw-r--r--   0 mustaqeem   (501) staff       (20)     1064 2023-06-14 06:52:31.050498 asm-opcode-analyzer-1.1.0/PKG-INFO
+-rw-r--r--   0 mustaqeem   (501) staff       (20)      292 2023-06-08 09:18:28.000000 asm-opcode-analyzer-1.1.0/README.md
+drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-14 06:52:31.048973 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer/
+-rw-r--r--   0 mustaqeem   (501) staff       (20)        0 2023-06-08 09:21:15.000000 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer/__init__.py
+drwxr-xr-x   0 mustaqeem   (501) staff       (20)        0 2023-06-14 06:52:31.050161 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/
+-rw-r--r--   0 mustaqeem   (501) staff       (20)     1064 2023-06-14 06:52:31.000000 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 mustaqeem   (501) staff       (20)      230 2023-06-14 06:52:31.000000 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 mustaqeem   (501) staff       (20)        1 2023-06-14 06:52:31.000000 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 mustaqeem   (501) staff       (20)       20 2023-06-14 06:52:31.000000 asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 mustaqeem   (501) staff       (20)       38 2023-06-14 06:52:31.050810 asm-opcode-analyzer-1.1.0/setup.cfg
+-rw-r--r--   0 mustaqeem   (501) staff       (20)      995 2023-06-14 06:49:28.000000 asm-opcode-analyzer-1.1.0/setup.py
```

### Comparing `asm-opcode-analyzer-1.0.0/LICENSE` & `asm-opcode-analyzer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asm-opcode-analyzer-1.0.0/PKG-INFO` & `asm-opcode-analyzer-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asm-opcode-analyzer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package for analyzing ASM opcodes
 Home-page: https://github.com/muhammad-mustaqeem/ASM-Opcode-Analyzer
 Author: Mustaqeem
 Author-email: mustaqeem.whyne@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asm-opcode-analyzer-1.0.0/asm_opcode_analyzer.egg-info/PKG-INFO` & `asm-opcode-analyzer-1.1.0/asm_opcode_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asm-opcode-analyzer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package for analyzing ASM opcodes
 Home-page: https://github.com/muhammad-mustaqeem/ASM-Opcode-Analyzer
 Author: Mustaqeem
 Author-email: mustaqeem.whyne@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `asm-opcode-analyzer-1.0.0/setup.py` & `asm-opcode-analyzer-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="asm-opcode-analyzer",
-    version="1.0.0",
+    version="1.1.0",
     author="Mustaqeem",
     author_email="mustaqeem.whyne@gmail.com",
     description="Python package for analyzing ASM opcodes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muhammad-mustaqeem/ASM-Opcode-Analyzer",
     packages=["asm_opcode_analyzer"],
```

