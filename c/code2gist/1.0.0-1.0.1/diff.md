# Comparing `tmp/code2gist-1.0.0.tar.gz` & `tmp/code2gist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code2gist-1.0.0.tar", last modified: Wed Jun 14 03:05:06 2023, max compression
+gzip compressed data, was "code2gist-1.0.1.tar", last modified: Wed Jun 14 03:15:16 2023, max compression
```

## Comparing `code2gist-1.0.0.tar` & `code2gist-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.987349 code2gist-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4021 2023-06-14 03:05:06.987349 code2gist-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3650 2023-06-14 02:59:51.000000 code2gist-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.924815 code2gist-1.0.0/code2gist/
--rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-1.0.0/code2gist/__init__.py
--rw-rw-rw-   0        0        0     3520 2023-06-14 02:33:47.000000 code2gist-1.0.0/code2gist/main.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:05:06.987349 code2gist-1.0.0/code2gist.egg-info/
--rw-rw-rw-   0        0        0     4021 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 03:05:06.000000 code2gist-1.0.0/code2gist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      628 2023-06-14 03:03:42.000000 code2gist-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 03:05:06.987349 code2gist-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.636114 code2gist-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3961 2023-06-14 03:15:16.635114 code2gist-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2023-06-14 03:13:54.000000 code2gist-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.587160 code2gist-1.0.1/code2gist/
+-rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-1.0.1/code2gist/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-06-14 02:33:47.000000 code2gist-1.0.1/code2gist/main.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.632147 code2gist-1.0.1/code2gist.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      628 2023-06-14 03:14:07.000000 code2gist-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:15:16.636114 code2gist-1.0.1/setup.cfg
```

### Comparing `code2gist-1.0.0/LICENSE` & `code2gist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code2gist-1.0.0/PKG-INFO` & `code2gist-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <crspears@outlook.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
@@ -21,46 +21,42 @@
 In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
 
 ## Installation
 
 You can install the package via pip:
 
 ```
-bashCopy code
 pip install code2gist
 ```
 
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
-bashCopy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
-bashCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
 ### Deleting Gists
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
-bashCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
 ## GitHub Token
```

### Comparing `code2gist-1.0.0/README.md` & `code2gist-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,46 +9,42 @@
 In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
 
 ## Installation
 
 You can install the package via pip:
 
 ```
-bashCopy code
 pip install code2gist
 ```
 
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
-bashCopy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
-bashCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
 ### Deleting Gists
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
-bashCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
 ## GitHub Token
```

### Comparing `code2gist-1.0.0/code2gist/main.py` & `code2gist-1.0.1/code2gist/main.py`

 * *Files identical despite different names*

### Comparing `code2gist-1.0.0/code2gist.egg-info/PKG-INFO` & `code2gist-1.0.1/code2gist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <crspears@outlook.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
@@ -21,46 +21,42 @@
 In addition, `code2gist` comes with a `prune` feature that provides a clean way to remove all the gists created by this tool from your GitHub account.
 
 ## Installation
 
 You can install the package via pip:
 
 ```
-bashCopy code
 pip install code2gist
 ```
 
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
-bashCopy code
 code2gist .
 ```
 
 This command will upload all Python files in the current directory to a private Gist on your GitHub account. The Gist will be titled with the name of the current directory, followed by "[code2gist]".
 
 If you want to include files with different extensions, you can specify them using the `--ext` option:
 
 ```
-bashCopy code
 code2gist . --ext .txt .md .py
 ```
 
 This command will include all text, Markdown, and Python files in the upload.
 
 ### Deleting Gists
 
 The `prune` feature allows you to delete all gists created by `code2gist`:
 
 ```
-bashCopy code
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
 ## GitHub Token
```

### Comparing `code2gist-1.0.0/pyproject.toml` & `code2gist-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code2gist"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name = "Cameron Spears", email = "crspears@outlook.com"},
 ]
 description = "Upload Python files in a directory to a GitHub Gist."
 readme = "README.md"
 requires-python = ">=3.11.4"
 keywords = ["python", "github", "gist", "upload"]
```

