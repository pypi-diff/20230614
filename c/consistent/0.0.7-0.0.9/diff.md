# Comparing `tmp/consistent-0.0.7.tar.gz` & `tmp/consistent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistent-0.0.7.tar", last modified: Fri Apr 28 10:31:17 2023, max compression
+gzip compressed data, was "consistent-0.0.9.tar", last modified: Fri Apr 28 13:08:53 2023, max compression
```

## Comparing `consistent-0.0.7.tar` & `consistent-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 10:31:02.000000 consistent-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-28 10:31:17.105385 consistent-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-28 10:31:02.000000 consistent-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/cache/chroma_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/base_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consisTent/validators/semantic_validators/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/consistency_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/semantic_validators/labels_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 10:31:02.000000 consistent-0.0.7/consisTent/validators/syntactic_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/consistent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 10:31:17.000000 consistent-0.0.7/consistent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 10:31:02.000000 consistent-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:31:17.105385 consistent-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:31:17.105385 consistent-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-28 10:31:02.000000 consistent-0.0.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.182628 consistent-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 13:08:39.000000 consistent-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-28 13:08:53.182628 consistent-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-28 13:08:39.000000 consistent-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.178629 consistent-0.0.9/consisTent/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.178629 consistent-0.0.9/consisTent/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/cache/chroma_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.182628 consistent-0.0.9/consisTent/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/base_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.182628 consistent-0.0.9/consisTent/validators/semantic_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/semantic_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/semantic_validators/consistency_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/semantic_validators/facts_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/semantic_validators/labels_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 13:08:39.000000 consistent-0.0.9/consisTent/validators/syntactic_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.182628 consistent-0.0.9/consistent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-28 13:08:53.000000 consistent-0.0.9/consistent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-28 13:08:53.000000 consistent-0.0.9/consistent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:08:53.000000 consistent-0.0.9/consistent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 13:08:53.000000 consistent-0.0.9/consistent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 13:08:53.000000 consistent-0.0.9/consistent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 13:08:39.000000 consistent-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:08:53.182628 consistent-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:08:53.182628 consistent-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-28 13:08:39.000000 consistent-0.0.9/tests/test.py
```

### Comparing `consistent-0.0.7/LICENSE` & `consistent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `consistent-0.0.7/PKG-INFO` & `consistent-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.7
+Version: 0.0.9
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -107,7 +107,18 @@
         "funny",
         "short",
         "about rabbits",
     ],
     model_output="What do you call a rabbit that tells jokes? A funny bunny!",
 )
 ```
+
+### facts validation
+
+```python
+OPENAI_KEY = "XXXXXXXXXXXXXXX"
+
+consisTent.FactsValidator(openai_key=OPENAI_KEY).validate(
+    facts=["this car weighs 1000KG"],
+    model_output="I can lift this car",
+)
+```
```

### Comparing `consistent-0.0.7/README.md` & `consistent-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,7 +71,18 @@
         "funny",
         "short",
         "about rabbits",
     ],
     model_output="What do you call a rabbit that tells jokes? A funny bunny!",
 )
 ```
+
+### facts validation
+
+```python
+OPENAI_KEY = "XXXXXXXXXXXXXXX"
+
+consisTent.FactsValidator(openai_key=OPENAI_KEY).validate(
+    facts=["this car weighs 1000KG"],
+    model_output="I can lift this car",
+)
+```
```

### Comparing `consistent-0.0.7/consisTent/cache/chroma_cache.py` & `consistent-0.0.9/consisTent/cache/chroma_cache.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.7/consisTent/validators/semantic_validators/consistency_validator.py` & `consistent-0.0.9/consisTent/validators/semantic_validators/consistency_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.7/consisTent/validators/semantic_validators/labels_validator.py` & `consistent-0.0.9/consisTent/validators/semantic_validators/labels_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.7/consisTent/validators/syntactic_validators.py` & `consistent-0.0.9/consisTent/validators/syntactic_validators.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.7/consistent.egg-info/PKG-INFO` & `consistent-0.0.9/consistent.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.7
+Version: 0.0.9
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -107,7 +107,18 @@
         "funny",
         "short",
         "about rabbits",
     ],
     model_output="What do you call a rabbit that tells jokes? A funny bunny!",
 )
 ```
+
+### facts validation
+
+```python
+OPENAI_KEY = "XXXXXXXXXXXXXXX"
+
+consisTent.FactsValidator(openai_key=OPENAI_KEY).validate(
+    facts=["this car weighs 1000KG"],
+    model_output="I can lift this car",
+)
+```
```

### Comparing `consistent-0.0.7/consistent.egg-info/SOURCES.txt` & `consistent-0.0.9/consistent.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 consisTent/cache/base_cache.py
 consisTent/cache/chroma_cache.py
 consisTent/validators/__init__.py
 consisTent/validators/base_validator.py
 consisTent/validators/syntactic_validators.py
 consisTent/validators/semantic_validators/__init__.py
 consisTent/validators/semantic_validators/consistency_validator.py
+consisTent/validators/semantic_validators/facts_validator.py
 consisTent/validators/semantic_validators/labels_validator.py
 consistent.egg-info/PKG-INFO
 consistent.egg-info/SOURCES.txt
 consistent.egg-info/dependency_links.txt
 consistent.egg-info/requires.txt
 consistent.egg-info/top_level.txt
 tests/test.py
```

### Comparing `consistent-0.0.7/pyproject.toml` & `consistent-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "consistent"
-version = "0.0.7"
+version = "0.0.9"
 description = "Make sure AI model outputs are consistent"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,15 +30,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "pre-commit", "pyflakes"]
 
 [project.urls]
 Homepage = "https://github.com/drorivry/consistent"
 
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `consistent-0.0.7/tests/test.py` & `consistent-0.0.9/tests/test.py`

 * *Files identical despite different names*

