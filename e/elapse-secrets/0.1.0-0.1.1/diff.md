# Comparing `tmp/elapse_secrets-0.1.0.tar.gz` & `tmp/elapse_secrets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elapse_secrets-0.1.0.tar", max compression
+gzip compressed data, was "elapse_secrets-0.1.1.tar", max compression
```

## Comparing `elapse_secrets-0.1.0.tar` & `elapse_secrets-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2184 2023-06-14 14:38:38.451869 elapse_secrets-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 13:26:59.932979 elapse_secrets-0.1.0/elapse_secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 13:35:44.092844 elapse_secrets-0.1.0/elapse_secrets/db/__init__.py
--rw-r--r--   0        0        0     4874 2023-06-14 14:29:38.262009 elapse_secrets-0.1.0/elapse_secrets/db/rules-elapse-stable.yml
--rw-r--r--   0        0        0      396 2023-06-14 13:43:54.532718 elapse_secrets-0.1.0/elapse_secrets/debug.py
--rw-r--r--   0        0        0     1444 2023-06-14 14:34:00.841941 elapse_secrets-0.1.0/elapse_secrets/main.py
--rw-r--r--   0        0        0      411 2023-06-14 13:34:58.792856 elapse_secrets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 elapse_secrets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1982 2023-06-14 18:52:21.097937 elapse_secrets-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 13:26:59.932979 elapse_secrets-0.1.1/elapse_secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:35:44.092844 elapse_secrets-0.1.1/elapse_secrets/db/__init__.py
+-rw-r--r--   0        0        0     4874 2023-06-14 14:29:38.262009 elapse_secrets-0.1.1/elapse_secrets/db/rules-elapse-stable.yml
+-rw-r--r--   0        0        0      396 2023-06-14 13:43:54.532718 elapse_secrets-0.1.1/elapse_secrets/debug.py
+-rw-r--r--   0        0        0     1565 2023-06-14 18:52:21.107937 elapse_secrets-0.1.1/elapse_secrets/main.py
+-rw-r--r--   0        0        0      411 2023-06-14 18:52:17.127938 elapse_secrets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 elapse_secrets-0.1.1/PKG-INFO
```

### Comparing `elapse_secrets-0.1.0/README.md` & `elapse_secrets-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+Metadata-Version: 2.1
+Name: elapse-secrets
+Version: 0.1.1
+Summary: Detects and removes sensitive information from the client-side to secure a user's data.
+Author: kdcokenny
+Author-email: kenny@kdco.llc
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Description-Content-Type: text/markdown
+
 # Elapse Secrets Filters
 
 Elapse Secrets Filters is a Python package designed to help you search and mask sensitive information in a body of text using pre-defined regular expressions. This package includes filters for common secrets like AWS keys, Github tokens, API keys, and much more.
 
 The package provides two main functions:
 
 1. `filter_elapse_secrets(text: str) -> str` - Uses the predefined regex filters to search and mask (with asterisks) any matching sensitive information in the input text.
 
 2. `find_error_in_regex(yaml_file: str) -> None` - Checks the YAML file containing regex rules for any incorrect patterns and logs the error if any are found.
 
 ## Getting Started
 
-1. Clone this repository
-
-   ```bash
-   git clone https://github.com/username/elapse_secrets_filters.git
-   ```
-
-2. Navigate to the cloned repository
+1. Install elapse-secrets
 
    ```bash
-   cd elapse_secrets_filters
-   ```
-
-3. Install the required packages
-
-   ```bash
-   poetry install
+   pip install elapse-secrets
    ```
 
 ## Usage
 
 This is a basic usage example.
 
 ```python
-from elapse_secrets_filters import filter_elapse_secrets
+from elapse_secrets import filter_elapse_secrets
 
 text_with_secrets = "My AWS Access Key is AKIAYOURACCESSKEYHERE"
 filtered_text = filter_elapse_secrets(text_with_secrets)
 print(filtered_text)
 # Output: My AWS Access Key is ********
 ```
 
@@ -78,7 +79,8 @@
 ## Contact
 
 Please feel free to contact the maintainers of this project if you have any questions.
 
 ## Acknowledgments
 
 We would like to thank all the contributors who have been part of this project.
+
```

### Comparing `elapse_secrets-0.1.0/elapse_secrets/db/rules-elapse-stable.yml` & `elapse_secrets-0.1.1/elapse_secrets/db/rules-elapse-stable.yml`

 * *Files identical despite different names*

### Comparing `elapse_secrets-0.1.0/elapse_secrets/main.py` & `elapse_secrets-0.1.1/elapse_secrets/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import yaml
 import re
 import logging
+import os
+
+current_dir = os.path.dirname(os.path.abspath(__file__))
 
 logging.basicConfig(level=logging.INFO)
 
 def clean_regex(regex):
     # remove leading and trailing slashes
     cleaned = regex.strip('/')
     # remove unsupported flag (?-i)
     cleaned = cleaned.replace("(?-i)", "")
     return cleaned
 
-def process_regex(yaml_file, text):
+def process_regex(folder,filename, text):
+    yaml_file = os.path.join(current_dir,folder,filename)
     with open(yaml_file, 'r') as stream:
         y = yaml.safe_load(stream)
 
     assert type(y) == dict
     assert "patterns" in y
 
     for i in y["patterns"]:
@@ -40,8 +44,9 @@
         except re.error as e:
             logging.error(f"Invalid regex pattern '{r}' for '{name}'. Error: {str(e)}")
 
     stripped_text = text.strip()
     return stripped_text
 
 def filter_elapse_secrets(text: str):
-    return process_regex('elapse_secrets/db/rules-elapse-stable.yml', text)
+    return process_regex('db','rules-elapse-stable.yml', text)
+
```

### Comparing `elapse_secrets-0.1.0/PKG-INFO` & `elapse_secrets-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,31 @@
-Metadata-Version: 2.1
-Name: elapse-secrets
-Version: 0.1.0
-Summary: Detects and removes sensitive information from the client-side to secure a user's data.
-Author: kdcokenny
-Author-email: kenny@kdco.llc
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Description-Content-Type: text/markdown
-
 # Elapse Secrets Filters
 
 Elapse Secrets Filters is a Python package designed to help you search and mask sensitive information in a body of text using pre-defined regular expressions. This package includes filters for common secrets like AWS keys, Github tokens, API keys, and much more.
 
 The package provides two main functions:
 
 1. `filter_elapse_secrets(text: str) -> str` - Uses the predefined regex filters to search and mask (with asterisks) any matching sensitive information in the input text.
 
 2. `find_error_in_regex(yaml_file: str) -> None` - Checks the YAML file containing regex rules for any incorrect patterns and logs the error if any are found.
 
 ## Getting Started
 
-1. Clone this repository
-
-   ```bash
-   git clone https://github.com/username/elapse_secrets_filters.git
-   ```
-
-2. Navigate to the cloned repository
+1. Install elapse-secrets
 
    ```bash
-   cd elapse_secrets_filters
-   ```
-
-3. Install the required packages
-
-   ```bash
-   poetry install
+   pip install elapse-secrets
    ```
 
 ## Usage
 
 This is a basic usage example.
 
 ```python
-from elapse_secrets_filters import filter_elapse_secrets
+from elapse_secrets import filter_elapse_secrets
 
 text_with_secrets = "My AWS Access Key is AKIAYOURACCESSKEYHERE"
 filtered_text = filter_elapse_secrets(text_with_secrets)
 print(filtered_text)
 # Output: My AWS Access Key is ********
 ```
 
@@ -91,8 +66,7 @@
 ## Contact
 
 Please feel free to contact the maintainers of this project if you have any questions.
 
 ## Acknowledgments
 
 We would like to thank all the contributors who have been part of this project.
-
```

