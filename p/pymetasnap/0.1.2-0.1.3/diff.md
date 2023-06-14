# Comparing `tmp/pymetasnap-0.1.2.tar.gz` & `tmp/pymetasnap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.1.2.tar", max compression
+gzip compressed data, was "pymetasnap-0.1.3.tar", max compression
```

## Comparing `pymetasnap-0.1.2.tar` & `pymetasnap-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/LICENSE
--rw-r--r--   0        0        0     3034 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/extractor/__init__.py
--rw-r--r--   0        0        0     2403 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/extractor/core.py
--rw-r--r--   0        0        0     1286 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/extractor/main.py
--rw-r--r--   0        0        0     2550 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/extractor/render.py
--rw-r--r--   0        0        0     1916 2023-06-14 14:21:34.602188 pymetasnap-0.1.2/extractor/utils.py
--rw-r--r--   0        0        0      823 2023-06-14 14:21:34.606188 pymetasnap-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 pymetasnap-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/__init__.py
+-rw-r--r--   0        0        0     2403 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/core.py
+-rw-r--r--   0        0        0     1286 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/main.py
+-rw-r--r--   0        0        0     2550 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/render.py
+-rw-r--r--   0        0        0     1916 2023-06-14 14:41:25.952432 pymetasnap-0.1.3/extractor/utils.py
+-rw-r--r--   0        0        0      823 2023-06-14 14:41:25.956433 pymetasnap-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.1.3/PKG-INFO
```

### Comparing `pymetasnap-0.1.2/LICENSE` & `pymetasnap-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.2/README.md` & `pymetasnap-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,19 +30,14 @@
 ```
 
 Replace the following placeholders in the command:
 
 - `<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
 - `<output_path>`: Path to store the extracted metadata file.
 - `<input_format>`: Format of the input requirements file (pip_list or pip_freeze).
-Example usage:
-
-```bash
-pymetasnap --source-path ./requirements.txt --output metadata.csv --format csv
-```
 
 #### Interactive mode
 
 Additionally, an interactive mode is available, allowing you to provide the required values through user prompts as follows:
 
 [![asciicast](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh.svg)](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh)
```

### Comparing `pymetasnap-0.1.2/extractor/core.py` & `pymetasnap-0.1.3/extractor/core.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.2/extractor/main.py` & `pymetasnap-0.1.3/extractor/main.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.2/extractor/render.py` & `pymetasnap-0.1.3/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.2/extractor/utils.py` & `pymetasnap-0.1.3/extractor/utils.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.2/pyproject.toml` & `pymetasnap-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.1.2"
+version = "0.1.3"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.1.2/PKG-INFO` & `pymetasnap-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,19 +55,14 @@
 ```
 
 Replace the following placeholders in the command:
 
 - `<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
 - `<output_path>`: Path to store the extracted metadata file.
 - `<input_format>`: Format of the input requirements file (pip_list or pip_freeze).
-Example usage:
-
-```bash
-pymetasnap --source-path ./requirements.txt --output metadata.csv --format csv
-```
 
 #### Interactive mode
 
 Additionally, an interactive mode is available, allowing you to provide the required values through user prompts as follows:
 
 [![asciicast](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh.svg)](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh)
```

