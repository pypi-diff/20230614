# Comparing `tmp/janis pipelines-0.9.6.tar.gz` & `tmp/janis pipelines-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis pipelines-0.9.6.tar", last modified: Fri May 22 05:39:17 2020, max compression
+gzip compressed data, was "dist/janis pipelines-0.9.7.tar", last modified: Fri Jun 19 03:10:54 2020, max compression
```

## Comparing `janis pipelines-0.9.6.tar` & `janis pipelines-0.9.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/janis/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/janis/data_types/
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/janis/data_types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/janis/__meta__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/janis/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)      496 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/janis/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      970 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/janis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10748 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8706 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/toolbuilder/
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/parse_cwl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/cltconvert.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/toolbuilder/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      920 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/templates/tool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/templates/gatk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/templates/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8293 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/parse_help.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1887 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/test_cltbuilder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/toolbuilder/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2020-05-22 05:38:58.000000 janis pipelines-0.9.6/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10748 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      642 2020-05-22 05:39:17.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-05-22 05:39:16.000000 janis pipelines-0.9.6/janis_pipelines.egg-info/entry_points.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis/data_types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/janis/data_types/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/janis/__meta__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      496 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/janis/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      970 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/janis/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10748 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8706 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/toolbuilder/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/parse_cwl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/cltconvert.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/toolbuilder/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      920 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/templates/tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      780 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/templates/gatk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/templates/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8624 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/parse_help.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1887 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/test_cltbuilder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3573 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/toolbuilder/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2430 2020-06-19 03:10:36.000000 janis pipelines-0.9.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10748 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      642 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      291 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-06-19 03:10:54.000000 janis pipelines-0.9.7/janis_pipelines.egg-info/entry_points.txt
```

### Comparing `janis pipelines-0.9.6/janis/__init__.py` & `janis pipelines-0.9.7/janis/__init__.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/PKG-INFO` & `janis pipelines-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis pipelines
-Version: 0.9.6
+Version: 0.9.7
 Summary: Contains classes and helpers to build a workflow, and provide options to convert to CWL / WDL
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis
 Author: Michael Franklin, Richard Lupat
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis (janis-pipelines) (Alpha)
```

### Comparing `janis pipelines-0.9.6/README.md` & `janis pipelines-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/cltconvert.py` & `janis pipelines-0.9.7/toolbuilder/cltconvert.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/templates/tool.py` & `janis pipelines-0.9.7/toolbuilder/templates/tool.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/templates/gatk.py` & `janis pipelines-0.9.7/toolbuilder/templates/gatk.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/templates/__init__.py` & `janis pipelines-0.9.7/toolbuilder/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/parse_help.py` & `janis pipelines-0.9.7/toolbuilder/parse_help.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,18 @@
     Boolean,
     Filename,
 )
 from janis_core.tool.commandtool import ToolInput
 
 from .templates import ToolTemplateType
 
-container_exec = {
-    "docker": ["docker", "run"],
-    # "singularity": ["singularity", "exec"]
-}
+container_exec = {"docker": ["docker", "run"], "singularity": ["singularity", "exec"]}
 
-common_replacements = {
-    "input": "inp",
-    "output": "outputFilename",
-}
+
+common_replacements = {"input": "inp", "output": "outputFilename"}
 
 option_markers = {
     "options:",
     "arguments:",
     "required arguments:",
     "optional arguments:",
 }
@@ -39,24 +34,31 @@
     basecommand: Union[str, List[str]],
     help_param: Optional[str] = "--help",
     containersoftware="docker",
 ):
     import subprocess, os
 
     bc = basecommand if isinstance(basecommand, list) else [basecommand]
-    cmd = [*container_exec[containersoftware], container, *bc]
 
     if help_param:
-        cmd.append(help_param)
+        bc = [*bc, help_param]
+
+    cmd = [*container_exec[containersoftware]]
+
+    if containersoftware == "docker":
+        cmd.extend([container, *bc])
+    elif containersoftware == "singularity":
+        # this doesn't work: https://github.com/hpcng/singularity/issues/5316
+        cmd.extend(["docker://" + container, *bc])
 
     print("Running command: " + " ".join(f"'{x}'" for x in cmd))
     try:
         help = (
             subprocess.check_output(cmd, stderr=subprocess.STDOUT)
-            .decode("utf-8")
+            .decode("utf-16")
             .rstrip()
         )
     except subprocess.CalledProcessError as e:
         help = str(e.output)
     return help
 
 
@@ -73,15 +75,15 @@
 
     print("Running command: " + " ".join(f"'{x}'" for x in cmd))
     try:
         help = subprocess.check_output(cmd, stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as e:
         return None
 
-    return help.decode("utf-8").rstrip()
+    return help.decode("utf-16").rstrip()
 
 
 def first_or_default(iterable, default=None):
     filtered = [f for f in iterable if f is not None]
     if len(filtered) > 0:
         return filtered[0]
     return default
@@ -138,15 +140,15 @@
         if (
             not requires_prev_line_blank_or_param or last_line_was_blank_or_param
         ) and line_args[0].startswith("-"):
             # sometimes this section has two items
             processed_tags = [
                 get_tag_and_cleanup_prefix(p) for p in line_args[0].split(",")
             ]
-            tags = sorted(processed_tags, key=lambda l: len(l[1]), reverse=True,)
+            tags = sorted(processed_tags, key=lambda l: len(l[1]), reverse=True)
             potential_type = first_or_default([p[3] for p in processed_tags])
 
             if len(tags) > 1:
                 tool_doc += "(" + ", ".join(t[0] for t in tags[1:]) + ") "
 
             if largs > 1:
                 tool_doc += " ".join(line_args[1:])
@@ -211,30 +213,34 @@
     # --adapter=ADAPTER
     # --quality-cutoff=[5'CUTOFF,]3'CUTOFF
     el = prefix.lstrip()
     has_equals = False
     pretag = None
     potential_type = None
 
-    if ":" in el:
-        parts = el.split(":")
+    # if prefix is split by ':' or split by
+    if ":" in el or "=" in el:
+        parts = None
+        if ":" in el:
+            parts = el.split(":")
+        elif "=" in el:
+            parts = el.split("=")
+            has_equals = True
+
         if len(parts) > 2:
             Logger.warn(
                 f"Unexpected number of components in the tag '{el}' to guess the type, using '{parts[0]}' and skipping type inference"
             )
         else:
             el, pt = parts[0], guess_type(parts[1])
 
             if not potential_type and pt:
                 potential_type = pt
 
-    if "=" in el:
-        has_equals = True
-        el = el.split("=")[0]
-    elif " " in el:
+    if " " in el:
         el = el.split(" ")[0]
 
     titleComponents = [l.strip().lower() for l in el.split("-") if l]
     if len(titleComponents) == 0:
         raise Exception(
             f"Title components for tag '{prefix}' does not have a component"
         )
```

### Comparing `janis pipelines-0.9.6/toolbuilder/test_cltbuilder.py` & `janis pipelines-0.9.7/toolbuilder/test_cltbuilder.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/toolbuilder/main.py` & `janis pipelines-0.9.7/toolbuilder/main.py`

 * *Files identical despite different names*

### Comparing `janis pipelines-0.9.6/setup.py` & `janis pipelines-0.9.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Version information is found in the __init__ file of `janis/`
 DESCRIPTION = "Contains classes and helpers to build a workflow, and provide options to convert to CWL / WDL"
 
-JANIS_CORE_VERSION = "v0.9.10"
-JANIS_ASSISTANT_VERSION = "v0.9.14"
-JANIS_UNIX_VERSION = "v0.9.1"
-JANIS_BIOINFORMATICS_VERSION = "v0.9.8"
+JANIS_CORE_VERSION = "v0.9.19"
+JANIS_ASSISTANT_VERSION = "v0.9.18"
+JANIS_UNIX_VERSION = "v0.9.2"
+JANIS_BIOINFORMATICS_VERSION = "v0.9.14"
 JANIS_PIPELINES_VERSION = "v0.9.5"
 JANIS_TEMPLATES_VERSION = "v0.9.4"
 
 
 ######## SHOULDN'T NEED EDITS BELOW THIS LINE ########
 
 min_core_version = f"janis-pipelines.core>=" + JANIS_CORE_VERSION
```

### Comparing `janis pipelines-0.9.6/janis_pipelines.egg-info/PKG-INFO` & `janis pipelines-0.9.7/janis_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines
-Version: 0.9.6
+Version: 0.9.7
 Summary: Contains classes and helpers to build a workflow, and provide options to convert to CWL / WDL
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis
 Author: Michael Franklin, Richard Lupat
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis (janis-pipelines) (Alpha)
```

### Comparing `janis pipelines-0.9.6/janis_pipelines.egg-info/SOURCES.txt` & `janis pipelines-0.9.7/janis_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

