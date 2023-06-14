# Comparing `tmp/ansible-anonymizer-1.4.0.tar.gz` & `tmp/ansible-anonymizer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.4.0.tar", last modified: Tue Jun 13 18:36:14 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.4.1.tar", last modified: Wed Jun 14 17:23:02 2023, max compression
```

## Comparing `ansible-anonymizer-1.4.0.tar` & `ansible-anonymizer-1.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.gitleaks.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/ansible_anonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.591428 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.591428 ansible-anonymizer-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_anonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/ansible_anonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/ansible_anonymizer/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 17:23:02.000000 ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:23:02.667099 ansible-anonymizer-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/tests/test_anonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/tests/test_field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/tests/test_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-14 17:22:41.000000 ansible-anonymizer-1.4.1/tox.ini
```

### Comparing `ansible-anonymizer-1.4.0/.github/workflows/release.yml` & `ansible-anonymizer-1.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/.github/workflows/tox.yml` & `ansible-anonymizer-1.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/.gitignore` & `ansible-anonymizer-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/.pre-commit-config.yaml` & `ansible-anonymizer-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/CHANGELOG.rst` & `ansible-anonymizer-1.4.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 1.4.1 (2023-06-14)
+-------------
+
+- fix to ensure anonymize_struct() uses the right value_template when it anoymizes a text blocks
+
 Version 1.4.0 (2023-06-13)
 -------------
 
 - fix the parser when a string is an empty quoted string (``""``)
 - refactoring to properly isolate the parsing in ``ansible_anonymizer.parser``
 - add ability to customize the secret substitution
 - README: minor adjustments and a new "limitations" section
```

### Comparing `ansible-anonymizer-1.4.0/CONTRIBUTING.rst` & `ansible-anonymizer-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/LICENSE` & `ansible-anonymizer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/PKG-INFO` & `ansible-anonymizer-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.4.0/README.rst` & `ansible-anonymizer-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.4.1/ansible_anonymizer/anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     if is_password_field_name(name):
         if is_path(v):
             return value
         if is_jinja2_expression(unquote(v)):
             return unquote(v)
         variable_name = str_jinja2_variable_name(name)
         return value_template.substitute(variable_name=variable_name)
-    return anonymize_text_block(value)
+    return anonymize_text_block(value, value_template=value_template)
 
 
 def anonymize_struct(o: Any, key_name: str = "", value_template: Optional[Template] = None) -> Any:
     if not value_template:
         value_template = Template("{{ $variable_name }}")
 
     def key_name_str(k: Any) -> str:
```

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.4.1/ansible_anonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer/field_checks.py` & `ansible-anonymizer-1.4.1/ansible_anonymizer/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer/parser.py` & `ansible-anonymizer-1.4.1/ansible_anonymizer/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.4.0
+Version: 1.4.1
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.4.1/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/pyproject.toml` & `ansible-anonymizer-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/tests/test_anonymizer.py` & `ansible-anonymizer-1.4.1/tests/test_anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,17 @@
     changed = anonymize_struct(in_)
     assert in_ != changed
     assert isinstance(changed[0], str)
     assert "@" in changed[0]
 
 
 def test_anonymize_with_special_template():
-    original = {"password": ["first_password", "second_password"]}
-    expected = {"password": ["ö", "ö"]}
+    original = {"password": ["first_password", "second_password"], "block": 'password1: "bar"'}
+    expected = {"password": ["ö", "ö"], "block": 'password1: "ö"'}
+    value_template = Template("ö")
     value_template = Template("ö")
     assert anonymize_struct(original, value_template=value_template) == expected
 
 
 def test_anonymize_deprecated_function():
     in_ = ["my-email-address@somewhe.re"]
     changed = anonymize(in_)
```

### Comparing `ansible-anonymizer-1.4.0/tests/test_field_checks.py` & `ansible-anonymizer-1.4.1/tests/test_field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/tests/test_parser.py` & `ansible-anonymizer-1.4.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.4.0/tox.ini` & `ansible-anonymizer-1.4.1/tox.ini`

 * *Files identical despite different names*

