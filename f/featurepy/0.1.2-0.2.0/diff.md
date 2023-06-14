# Comparing `tmp/featurepy-0.1.2.tar.gz` & `tmp/featurepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.1.2.tar", max compression
+gzip compressed data, was "featurepy-0.2.0.tar", max compression
```

## Comparing `featurepy-0.1.2.tar` & `featurepy-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,11 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.1.2/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.1.2/README.md
--rw-r--r--   0        0        0      788 2023-06-14 13:38:12.081583 featurepy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-11 09:55:40.361310 featurepy-0.1.2/src/featurepy/__init__.py
--rw-r--r--   0        0        0     1529 2023-06-14 00:06:33.902940 featurepy-0.1.2/src/featurepy/feature_class.py
--rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.1.2/src/featurepy/flask/__init__.py
--rw-r--r--   0        0        0      230 2023-05-18 14:59:44.476705 featurepy-0.1.2/src/featurepy/flask/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1901 2023-05-18 14:59:44.477827 featurepy-0.1.2/src/featurepy/flask/__pycache__/views.cpython-311.pyc
--rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.1.2/src/featurepy/flask/views.py
--rw-r--r--   0        0        0     3412 2023-06-13 23:31:59.687317 featurepy-0.1.2/src/featurepy/model_constraints.py
--rw-r--r--   0        0        0     1730 2023-06-11 15:46:14.698789 featurepy-0.1.2/src/featurepy/parametric_features.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.1.2/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      202 2023-06-03 17:07:40.240249 featurepy-0.1.2/src/featurepy/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1328 2023-06-03 17:07:40.240691 featurepy-0.1.2/src/featurepy/scripts/__pycache__/features.cpython-311.pyc
--rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.1.2/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.2.0/README.md
+-rw-r--r--   0        0        0      788 2023-06-06 10:57:15.617883 featurepy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      197 2023-06-05 07:46:53.683700 featurepy-0.2.0/src/featurepy/__init__.py
+-rw-r--r--   0        0        0     1346 2023-06-06 10:34:33.732327 featurepy-0.2.0/src/featurepy/feature_class.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.2.0/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.2.0/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0     2938 2023-06-06 10:52:23.396560 featurepy-0.2.0/src/featurepy/model_constraints.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.2.0/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.2.0/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.2.0/PKG-INFO
```

### Comparing `featurepy-0.1.2/LICENSE` & `featurepy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurepy-0.1.2/pyproject.toml` & `featurepy-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "featurepy"
-version = "0.1.2"
+version = "0.2.0"
 description = "Framework for building software product lines using feature-oriented programming (FOP) and aspect-oriented programming (AOP) in Python."
 authors = ["Adrian Wong <adrianwong227@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 featuremonkey3 = "^0.1.1"
```

### Comparing `featurepy-0.1.2/src/featurepy/feature_class.py` & `featurepy-0.2.0/src/featurepy/feature_class.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,46 +3,39 @@
 from functools import wraps
 from types import FunctionType
 
 import inspect
 
 
 def feature_method(func):
-    wraps(func)
-
     def wrapper(self, *args, **kwargs):
 
         cutpoint_aspects = self.aspects[func.__name__] if func.__name__ in self.aspects else {
         }
         result_func = func
         for cutpoint, aspects in cutpoint_aspects.items():
             base_func = result_func
-            # if isinstance(cutpoint, str):
-            #     cutpoint = eval(cutpoint)
 
             def weaved_func(self, *args, **kwargs):
                 with weave(cutpoint, aspects):
                     return base_func(self, *args, **kwargs)
 
             result_func = weaved_func
 
         return result_func(self, *args, **kwargs)
 
     return wrapper
 
 
-# TODO: weave aspects on methods
 def feature(cls):
-    wraps(cls)
-
     class Wrapper(cls):
         aspects = {}
 
         @classmethod
-        def register_aspect(clss, method, cutpoint, aspect, **kwargs):  # Missing options
+        def register_aspect(clss, method, cutpoint, aspect):
             if method not in clss.aspects:
                 clss.aspects[method] = {}
             if cutpoint not in clss.aspects[method]:
                 clss.aspects[method][cutpoint] = []
             clss.aspects[method][cutpoint].append(aspect)
 
         def __init__(self, *args, **kwargs):
```

### Comparing `featurepy-0.1.2/src/featurepy/flask/views.py` & `featurepy-0.2.0/src/featurepy/flask/views.py`

 * *Files identical despite different names*

### Comparing `featurepy-0.1.2/src/featurepy/model_constraints.py` & `featurepy-0.2.0/src/featurepy/model_constraints.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,71 +32,67 @@
     if fm is not None and 'children' in fm:
         for child in fm['children']:
             features += get_features(child)
 
     return features
 
 
-def _is_operator(token: str) -> bool:
-    return token in ["or", "and", "not"]
+def parse_reqs(reqs: str, selections):  # () not supported
+    if "!^|" not in reqs:
+        return reqs in selections
 
+    if '|' in reqs:
+        sub_reqs = reqs.split('|')
+        return any([parse_reqs(sr, selections) for sr in sub_reqs])
 
-def parse_reqs(reqs, selections):
-    tokens = reqs.split()
-    expr = " ".join([f"{token} in selections" if not _is_operator(
-        token) else token for token in tokens])
-    return eval(expr)
+    if '^' in reqs:
+        sub_reqs = reqs.split('^')
+        return all([parse_reqs(sr, selections) for sr in sub_reqs])
 
+    return reqs not in selections
 
-def validate_selections(fm, selections: list[str], remaining_selections: list[str]):
+
+def validate_selections(fm, selections, remaining_selections):
     if not is_optional(fm) and not is_abstract(fm) and fm['name'] not in selections:
         raise FeatureSelectionError(
             f"Mandatory feature not selected: {fm['name']}")
 
-    if 'cross-tree-reqs' in fm and fm['name'] in selections and not parse_reqs(fm['cross-tree-reqs'], selections):
+    if 'cross-tree-reqs' in fm and not parse_reqs(fm['cross-tree-reqs'], selections):
         raise FeatureSelectionError(
             f"Cross-tree requirements not satisfied for {fm['name']}")
 
     if fm['name'] in selections:
         remaining_selections.remove(fm['name'])
 
     if (is_abstract(fm) or fm['name'] in selections) and has_children(fm):
 
         if is_branch(fm, 'xor') and len(set([child['name'] for child in fm['children']]).intersection(set(selections))) != 1:
             raise FeatureSelectionError(
                 f"Incorrect number of xor features selected for branch {fm['name']}")
 
         for child in fm['children']:
-            if child['name'] in selections and selections.index(child['name']) > selections.index(fm['name']):
-                raise FeatureSelectionError(
-                    f"Child feature {child['name']} is selected before parent {fm['name']}.")
             if is_branch(fm, 'or'):
                 child['optional'] = True
             remaining_selections = validate_selections(
                 child, selections, remaining_selections)
 
     return remaining_selections
 
 
 @Aspect
 def model_constraints(composer, *features):
-    try:
-        with open('feature_model.yml') as fp:
-            feature_model = safe_load(fp)
+    with open('feature_model.yml') as fp:
+        feature_model = safe_load(fp)
 
-        all_features = get_features(feature_model)
-        selections = [feature.split("(")[0] for feature in features]
+    all_features = get_features(feature_model)
 
-        if not set(selections).issubset(set(all_features)):
-            raise FeatureSelectionError("Undefined features selected.")
+    if not set(features).issubset(set(all_features)):
+        raise FeatureSelectionError("Undefined features selected.")
 
-        unvalidated_selections = validate_selections(
-            feature_model, list(selections), list(selections))
+    unvalidated_selections = validate_selections(
+        feature_model, list(features), list(features))
 
-        if unvalidated_selections != []:
-            raise FeatureSelectionError(
-                f"Parent features not selected or the feature is selected more than once: {unvalidated_selections}")
-    except FileNotFoundError:
-        print("Feature model tree not found, proceeding without constraint checks...")
-        pass
+    if unvalidated_selections != []:
+        raise FeatureSelectionError(
+            f"Parent features not selected {unvalidated_selections}")
 
     yield Proceed(composer, *features)
```

