# Comparing `tmp/codegenpt-0.4.0.tar.gz` & `tmp/codegenpt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.4.0.tar", max compression
+gzip compressed data, was "codegenpt-0.4.1.tar", max compression
```

## Comparing `codegenpt-0.4.0.tar` & `codegenpt-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-13 06:44:12.745350 codegenpt-0.4.0/LICENSE
--rw-r--r--   0        0        0     2323 2023-06-13 07:11:06.617618 codegenpt-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.4.0/codegenpt/__init__.py
--rw-r--r--   0        0        0     1337 2023-06-13 06:34:45.151133 codegenpt-0.4.0/codegenpt/cli.py
--rw-r--r--   0        0        0     1634 2023-06-13 07:05:46.474675 codegenpt-0.4.0/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.4.0/codegenpt/commands/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.4.0/codegenpt/commands/command.py
--rw-r--r--   0        0        0      572 2023-06-13 06:34:45.151534 codegenpt-0.4.0/codegenpt/commands/commands.py
--rw-r--r--   0        0        0     1592 2023-06-13 07:10:11.778638 codegenpt-0.4.0/codegenpt/commands/include.py
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.4.0/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.4.0/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.4.0/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     1417 2023-06-13 06:34:45.151764 codegenpt-0.4.0/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.4.0/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      415 2023-06-13 05:01:08.504508 codegenpt-0.4.0/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      578 2023-06-13 07:11:34.875758 codegenpt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 codegenpt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2323 2023-06-14 02:09:48.042507 codegenpt-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.4.1/codegenpt/__init__.py
+-rw-r--r--   0        0        0     1577 2023-06-14 03:48:47.790152 codegenpt-0.4.1/codegenpt/cli.py
+-rw-r--r--   0        0        0     1634 2023-06-14 02:09:48.042663 codegenpt-0.4.1/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.4.1/codegenpt/commands/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.4.1/codegenpt/commands/command.py
+-rw-r--r--   0        0        0      572 2023-06-13 06:34:45.151534 codegenpt-0.4.1/codegenpt/commands/commands.py
+-rw-r--r--   0        0        0     1592 2023-06-13 07:10:11.778638 codegenpt-0.4.1/codegenpt/commands/include.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.4.1/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.4.1/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.4.1/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     1417 2023-06-13 06:34:45.151764 codegenpt-0.4.1/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.4.1/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-13 05:01:08.504508 codegenpt-0.4.1/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      578 2023-06-14 04:09:44.521338 codegenpt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 codegenpt-0.4.1/PKG-INFO
```

### Comparing `codegenpt-0.4.0/LICENSE` & `codegenpt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/README.md` & `codegenpt-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/codegenpt/cli.py` & `codegenpt-0.4.1/codegenpt/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from threading import Thread
 import click
 from codegenpt.codegenpt_file import CodeGenPTFile
 
 from codegenpt.filesystem.file_discovery import find_codegenpt_files
 from codegenpt.generators.file_generator import generate_file
 
 
@@ -16,19 +17,27 @@
 def codegenpt(recursive=True, force=True, path='.'):
     if os.path.isdir(path):
         click.echo(f"🔎 Searching files...")
         files = find_codegenpt_files(recursive=recursive, path=path)
     else:
         files = [CodeGenPTFile(path)]
     
-    for file in files:
-        if os.path.exists(file.filename) and not force:
-            click.echo(f"👍 File already exists: {click.format_filename(file.filename)}")
-            continue
-        click.echo(f"⏳ Generating file: {click.format_filename(file.filename)}")
-        file.write(generate_file(file))
-        click.echo(f"🍺 File generated: {click.format_filename(file.filename)}")
+    generation_threads = [Thread(target=generate, args=(file, force)) for file in files]
     
+    for thread in generation_threads:
+        thread.start()
+
+    for thread in generation_threads:
+        thread.join()
+
     click.echo(f"🍻 Success")
 
+def generate(file: CodeGenPTFile, force=True):
+    if os.path.exists(file.filename) and not force:
+        click.echo(f"👍 File already exists: {click.format_filename(file.filename)}")
+        return
+    click.echo(f"⏳ Generating file: {click.format_filename(file.filename)}")
+    file.write(generate_file(file))
+    click.echo(f"🍺 File generated: {click.format_filename(file.filename)}")
+
 if __name__ == '__main__':
     cli()
```

### Comparing `codegenpt-0.4.0/codegenpt/codegenpt_file.py` & `codegenpt-0.4.1/codegenpt/codegenpt_file.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/codegenpt/commands/commands.py` & `codegenpt-0.4.1/codegenpt/commands/commands.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/codegenpt/commands/include.py` & `codegenpt-0.4.1/codegenpt/commands/include.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/codegenpt/generators/file_generator.py` & `codegenpt-0.4.1/codegenpt/generators/file_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.0/pyproject.toml` & `codegenpt-0.4.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codegenpt"
-version = "0.4.0"
+version = "0.4.1"
 description = "Autogenerate files and folders using ChatGPT API"
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [project.urls]
 homepage = "https://github.com/diegoquinteiro/codegenpt"
```

### Comparing `codegenpt-0.4.0/PKG-INFO` & `codegenpt-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codegenpt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Autogenerate files and folders using ChatGPT API
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

