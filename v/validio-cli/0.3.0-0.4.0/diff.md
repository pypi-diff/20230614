# Comparing `tmp/validio_cli-0.3.0.tar.gz` & `tmp/validio_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.3.0.tar", max compression
+gzip compressed data, was "validio_cli-0.4.0.tar", max compression
```

## Comparing `validio_cli-0.3.0.tar` & `validio_cli-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    11340 2023-06-14 12:04:49.257696 validio_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      227 2023-06-14 12:04:49.257696 validio_cli-0.3.0/README_PUBLIC.md
--rw-r--r--   0        0        0     1805 2023-06-14 12:04:59.561611 validio_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5590 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/__init__.py
--rw-r--r--   0        0        0     2390 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11640 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     4335 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2499 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     2306 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     7491 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2867 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3334 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     2913 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1902 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    26332 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3743 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     2806 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     3036 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-06-14 12:04:49.257696 validio_cli-0.3.0/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-14 13:46:49.212757 validio_cli-0.4.0/LICENSE
+-rw-r--r--   0        0        0      227 2023-06-14 13:46:49.212757 validio_cli-0.4.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     1987 2023-06-14 13:47:00.140614 validio_cli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5590 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2390 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11640 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2499 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     2306 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     7429 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2336 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     2867 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3334 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     2913 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1902 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    26332 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3743 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     2806 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     3114 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-06-14 13:46:49.212757 validio_cli-0.4.0/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.4.0/PKG-INFO
```

### Comparing `validio_cli-0.3.0/LICENSE` & `validio_cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/pyproject.toml` & `validio_cli-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
-version = "0.3.0"
+# This version does not represent the released version or any tag. For each
+# release we automatically bump this before building and publishing so this
+# should be kept at 0.0.1dev1
+version = "0.4.0"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
```

### Comparing `validio_cli-0.3.0/validio_cli/__init__.py` & `validio_cli-0.4.0/validio_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/channels.py` & `validio_cli-0.4.0/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/code.py` & `validio_cli-0.4.0/validio_cli/bin/entities/code.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/config.py` & `validio_cli-0.4.0/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/credentials.py` & `validio_cli-0.4.0/validio_cli/bin/entities/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/destinations.py` & `validio_cli-0.4.0/validio_cli/bin/entities/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/incidents.py` & `validio_cli-0.4.0/validio_cli/bin/entities/incidents.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,34 +135,14 @@
     else:
         print("You need to specify one of --validator and/or --segment or --source")
         raise typer.Exit(code=1)
 
     if output_format == OutputFormat.JSON:
         return output_json(incidents)
 
-    def calculate_operator(item: Any):
-        type_ = item.typename__[len("ValidatorMetricWith") :]
-        if type_ == "DynamicThreshold":
-            operator = item.decision_bounds_type
-        else:
-            operator = item.operator
-
-        return f"{type_}/{operator}"
-
-    def calculate_bound(item: Any):
-        type_ = item.typename__[len("ValidatorMetricWith") :]
-        if type_ == "DynamicThreshold":
-            bound = f"{item.lower_bound:.2f} - {item.upper_bound:.2f}"
-        elif type_ == "FixedThreshold":
-            bound = item.bound
-        else:
-            bound = "-"
-
-        return bound
-
     return output_text(
         incidents,
         fields={
             "operator": OutputSettings(
                 attribute_name="metric",
                 reformat=calculate_operator,
             ),
@@ -225,14 +205,36 @@
             "change_type": None,
             "old_value": None,
             "new_value": None,
         },
     )
 
 
+def calculate_operator(item: Any):
+    type_ = item.typename__[len("ValidatorMetricWith") :]
+    if type_ == "DynamicThreshold":
+        operator = item.decision_bounds_type
+    else:
+        operator = item.operator
+
+    return f"{type_}/{operator}"
+
+
+def calculate_bound(item: Any):
+    type_ = item.typename__[len("ValidatorMetricWith") :]
+    if type_ == "DynamicThreshold":
+        bound = f"{item.lower_bound:.2f} - {item.upper_bound:.2f}"
+    elif type_ == "FixedThreshold":
+        bound = item.bound
+    else:
+        bound = "-"
+
+    return bound
+
+
 def _output_text_source_incidents_segment_limit_exceeded(
     incidents: list[GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotification],
 ):
     return output_text(
         incidents,
         fields={
             "limit": None,
```

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.4.0/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.4.0/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.4.0/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/segments.py` & `validio_cli-0.4.0/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/sources.py` & `validio_cli-0.4.0/validio_cli/bin/entities/sources.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/users.py` & `validio_cli-0.4.0/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/validators.py` & `validio_cli-0.4.0/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/entities/windows.py` & `validio_cli-0.4.0/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/bin/main.py` & `validio_cli-0.4.0/validio_cli/bin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from validio_cli import ConfigDir
 from validio_cli.bin.entities import (
     channels,
     code,
     credentials,
     destinations,
     incidents,
+    metrics,
     notification_rules,
     recommendations,
     segmentations,
     segments,
     sources,
     users,
     validators,
@@ -31,14 +32,15 @@
 )
 
 app.add_typer(channels.app, no_args_is_help=True, name="channels")
 app.add_typer(code.app, no_args_is_help=True, name="code")
 app.add_typer(credentials.app, no_args_is_help=True, name="credentials")
 app.add_typer(destinations.app, no_args_is_help=True, name="destinations")
 app.add_typer(incidents.app, no_args_is_help=True, name="incidents")
+app.add_typer(metrics.app, no_args_is_help=True, name="metrics")
 app.add_typer(notification_rules.app, no_args_is_help=True, name="notification-rules")
 app.add_typer(recommendations.app, no_args_is_help=True, name="recommendations")
 app.add_typer(segmentations.app, no_args_is_help=True, name="segmentations")
 app.add_typer(segments.app, no_args_is_help=True, name="segments")
 app.add_typer(sources.app, no_args_is_help=True, name="sources")
 app.add_typer(users.app, no_args_is_help=True, name="users")
 app.add_typer(validators.app, no_args_is_help=True, name="validators")
```

### Comparing `validio_cli-0.3.0/validio_cli/components.py` & `validio_cli-0.4.0/validio_cli/components.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/namespace.py` & `validio_cli-0.4.0/validio_cli/namespace.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/validio_cli/schema.py` & `validio_cli-0.4.0/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.3.0/PKG-INFO` & `validio_cli-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.3.0
+Version: 0.4.0
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

