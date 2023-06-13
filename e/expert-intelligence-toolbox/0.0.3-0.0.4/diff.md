# Comparing `tmp/expert_intelligence_toolbox-0.0.3.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.4.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.3.tar` & `expert_intelligence_toolbox-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/src/expert_intelligence_toolbox/expert_inteligence_toolbox.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/LICENSE
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.4/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.3/LICENSE` & `expert_intelligence_toolbox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.3/README.md` & `expert_intelligence_toolbox-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,11 @@
 `py -m build`
 `py -m twine upload dist/*`
 Username: __token__
 PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
 
 
 5 - What if you make any changes? Just repeat.
-Change version number.
+Change version number in pyproject.toml
+`py -m build`
 `twine upload --skip-existing dist/*`
 `twine upload --skip-existing --repository testpypi dist/*` (for testpypi)
```

### Comparing `expert_intelligence_toolbox-0.0.3/pyproject.toml` & `expert_intelligence_toolbox-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expert_intelligence_toolbox"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Arnold Kuersteiner", email="arnold.kuersteiner@expert-intelligence.com" },
 ]
 description = "This is (for now) a test."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `expert_intelligence_toolbox-0.0.3/PKG-INFO` & `expert_intelligence_toolbox-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expert_intelligence_toolbox
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is (for now) a test.
 Project-URL: Homepage, https://github.com/Point-Topic/expert_intelligence_toolbox
 Project-URL: Bug Tracker, https://github.com/Point-Topic/expert_intelligence_toolbox/issues
 Author-email: Arnold Kuersteiner <arnold.kuersteiner@expert-intelligence.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -54,10 +54,11 @@
 `py -m build`
 `py -m twine upload dist/*`
 Username: __token__
 PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
 
 
 5 - What if you make any changes? Just repeat.
-Change version number.
+Change version number in pyproject.toml
+`py -m build`
 `twine upload --skip-existing dist/*`
 `twine upload --skip-existing --repository testpypi dist/*` (for testpypi)
```

