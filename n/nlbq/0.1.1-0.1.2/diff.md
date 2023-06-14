# Comparing `tmp/nlbq-0.1.1.tar.gz` & `tmp/nlbq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlbq-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nlbq-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nlbq-0.1.1.tar` & `nlbq-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      505 2023-06-13 15:46:24.829925 nlbq-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      878 2023-06-13 15:46:24.829925 nlbq-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3108 2023-06-13 15:46:24.829925 nlbq-0.1.1/.gitignore
--rw-r--r--   0        0        0      258 2023-06-13 15:46:24.829925 nlbq-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2023-06-13 15:46:24.829925 nlbq-0.1.1/LICENSE
--rw-r--r--   0        0        0     1039 2023-06-13 15:46:24.829925 nlbq-0.1.1/README.md
--rw-r--r--   0        0        0       58 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/__init__.py
--rw-r--r--   0        0        0     2431 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/api.py
--rw-r--r--   0        0        0     3675 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/cli.py
--rw-r--r--   0        0        0      631 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/config.py
--rw-r--r--   0        0        0     4333 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/core.py
--rw-r--r--   0        0        0     1476 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/helpers.py
--rw-r--r--   0        0        0      103 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/Dockerfile
--rw-r--r--   0        0        0     7354 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/index.html
--rw-r--r--   0        0        0     1460 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/prompt.txt
--rw-r--r--   0        0        0      760 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/prompt_template.txt
--rw-r--r--   0        0        0     1191 2023-06-13 15:46:24.833925 nlbq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 nlbq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      505 2023-06-14 10:23:25.853344 nlbq-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      878 2023-06-14 10:23:25.853344 nlbq-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3108 2023-06-14 10:23:25.853344 nlbq-0.1.2/.gitignore
+-rw-r--r--   0        0        0      258 2023-06-14 10:23:25.853344 nlbq-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-06-14 10:23:25.853344 nlbq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1039 2023-06-14 10:23:25.853344 nlbq-0.1.2/README.md
+-rw-r--r--   0        0        0       58 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/__init__.py
+-rw-r--r--   0        0        0     2431 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/api.py
+-rw-r--r--   0        0        0     3675 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/cli.py
+-rw-r--r--   0        0        0      631 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/config.py
+-rw-r--r--   0        0        0     4378 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/core.py
+-rw-r--r--   0        0        0     1476 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/helpers.py
+-rw-r--r--   0        0        0      103 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/templates/Dockerfile
+-rw-r--r--   0        0        0     7354 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/templates/index.html
+-rw-r--r--   0        0        0     1460 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/templates/prompt.txt
+-rw-r--r--   0        0        0      760 2023-06-14 10:23:25.853344 nlbq-0.1.2/nlbq/templates/prompt_template.txt
+-rw-r--r--   0        0        0     1191 2023-06-14 10:23:25.853344 nlbq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 nlbq-0.1.2/PKG-INFO
```

### Comparing `nlbq-0.1.1/.github/workflows/publish.yml` & `nlbq-0.1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/.gitignore` & `nlbq-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/LICENSE` & `nlbq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/README.md` & `nlbq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/api.py` & `nlbq-0.1.2/nlbq/api.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/cli.py` & `nlbq-0.1.2/nlbq/cli.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/config.py` & `nlbq-0.1.2/nlbq/config.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/core.py` & `nlbq-0.1.2/nlbq/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,9 +110,10 @@
                 "content": "Don't say what the query was, just answer the question.",
             },
         ]
         resp = await openai.ChatCompletion.acreate(
             model=self.model,
             messages=prompt_messages,
             temperature=0,
+            api_key=settings.openai_api_key,
         )
         return resp["choices"][0]["message"]["content"].strip()
```

### Comparing `nlbq-0.1.1/nlbq/helpers.py` & `nlbq-0.1.2/nlbq/helpers.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/templates/index.html` & `nlbq-0.1.2/nlbq/templates/index.html`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/templates/prompt.txt` & `nlbq-0.1.2/nlbq/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/nlbq/templates/prompt_template.txt` & `nlbq-0.1.2/nlbq/templates/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/pyproject.toml` & `nlbq-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.1/PKG-INFO` & `nlbq-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlbq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Natural language to BigQuery
 Author: Tom Dyson, Dan Braghis
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: openai
 Requires-Dist: fastapi
```

