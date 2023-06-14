# Comparing `tmp/satori_playbook_validator-2.1.0.tar.gz` & `tmp/satori_playbook_validator-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.1.0.tar", last modified: Tue Jun 13 23:34:22 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.1.1.tar", last modified: Wed Jun 14 04:32:27 2023, max compression
```

## Comparing `satori_playbook_validator-2.1.0.tar` & `satori_playbook_validator-2.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/README.md
--rw-r--r--   0        0        0      474 2023-06-13 23:34:22.814902 satori_playbook_validator-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5253 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1837 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      537 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-13 23:34:08.111003 satori_playbook_validator-2.1.0/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/README.md
+-rw-r--r--   0        0        0      474 2023-06-14 04:32:27.104775 satori_playbook_validator-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5273 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1837 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      874 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-14 04:32:12.568708 satori_playbook_validator-2.1.1/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.1.1/PKG-INFO
```

### Comparing `satori_playbook_validator-2.1.0/src/satorici/validator/_validator.py` & `satori_playbook_validator-2.1.1/src/satorici/validator/_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,17 +135,18 @@
 
     while stack:
         path, current = stack.pop()
 
         for k, v in (i for i in current.items() if "^" not in i[0]):
             if isinstance(v, dict):
                 stack.append((path + (k,), v))
-            elif validate_commands(v) and get_reference_names(v):
-                validate_references(current, k)
+            elif validate_commands(v):
                 execution_found = True
+                if get_reference_names(v):
+                    validate_references(current, k)
 
     if not execution_found:
         raise PlaybookValidationError("No executions found.")
 
 
 def add_parent_info(d: dict):
     stack = [(d, None, None)]
```

### Comparing `satori_playbook_validator-2.1.0/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.0/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.0/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.1.1/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.0/tests/test_reference_finder.py` & `satori_playbook_validator-2.1.1/tests/test_reference_finder.py`

 * *Files identical despite different names*

