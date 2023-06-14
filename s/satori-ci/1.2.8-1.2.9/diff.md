# Comparing `tmp/satori_ci-1.2.8.tar.gz` & `tmp/satori_ci-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.2.8.tar", last modified: Mon May 15 22:14:32 2023, max compression
+gzip compressed data, was "satori_ci-1.2.9.tar", last modified: Mon May 15 23:24:34 2023, max compression
```

## Comparing `satori_ci-1.2.8.tar` & `satori_ci-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.8/LICENSE
--rw-r--r--   0        0        0     4984 2023-05-15 15:49:56.139568 satori_ci-1.2.8/README.md
--rw-r--r--   0        0        0      646 2023-05-15 22:14:32.559456 satori_ci-1.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.8/src/satorici/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.8/src/satorici/classes/__init__.py
--rw-r--r--   0        0        0     4066 2023-05-15 12:33:16.870027 satori_ci-1.2.8/src/satorici/classes/api.py
--rw-r--r--   0        0        0     1770 2023-05-15 12:33:16.870199 satori_ci-1.2.8/src/satorici/classes/bundler.py
--rw-r--r--   0        0        0     2807 2023-05-15 12:33:16.870273 satori_ci-1.2.8/src/satorici/classes/playbooks.py
--rw-r--r--   0        0        0    20716 2023-05-15 22:14:04.481522 satori_ci-1.2.8/src/satorici/classes/satori.py
--rw-r--r--   0        0        0    10143 2023-05-15 15:49:56.139735 satori_ci-1.2.8/src/satorici/classes/utils.py
--rw-r--r--   0        0        0     1440 2023-05-15 12:33:16.870721 satori_ci-1.2.8/src/satorici/classes/validations.py
--rwxr-xr-x   0        0        0     6027 2023-05-15 12:33:16.870846 satori_ci-1.2.8/src/satorici/satori_module.py
--rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-28 19:49:33.588036 satori_ci-1.2.9/LICENSE
+-rw-r--r--   0        0        0     4984 2023-05-15 15:49:56.139568 satori_ci-1.2.9/README.md
+-rw-r--r--   0        0        0      646 2023-05-15 23:24:34.356210 satori_ci-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588599 satori_ci-1.2.9/src/satorici/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 19:49:33.588697 satori_ci-1.2.9/src/satorici/classes/__init__.py
+-rw-r--r--   0        0        0     4066 2023-05-15 12:33:16.870027 satori_ci-1.2.9/src/satorici/classes/api.py
+-rw-r--r--   0        0        0     1770 2023-05-15 12:33:16.870199 satori_ci-1.2.9/src/satorici/classes/bundler.py
+-rw-r--r--   0        0        0     2807 2023-05-15 12:33:16.870273 satori_ci-1.2.9/src/satorici/classes/playbooks.py
+-rw-r--r--   0        0        0    20716 2023-05-15 22:14:04.481522 satori_ci-1.2.9/src/satorici/classes/satori.py
+-rw-r--r--   0        0        0    10150 2023-05-15 23:24:06.860593 satori_ci-1.2.9/src/satorici/classes/utils.py
+-rw-r--r--   0        0        0     1440 2023-05-15 12:33:16.870721 satori_ci-1.2.9/src/satorici/classes/validations.py
+-rwxr-xr-x   0        0        0     6027 2023-05-15 12:33:16.870846 satori_ci-1.2.9/src/satorici/satori_module.py
+-rw-r--r--   0        0        0    46006 1970-01-01 00:00:00.000000 satori_ci-1.2.9/PKG-INFO
```

### Comparing `satori_ci-1.2.8/LICENSE` & `satori_ci-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/README.md` & `satori_ci-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/pyproject.toml` & `satori_ci-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.2.8"
+version = "1.2.9"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.2.8/src/satorici/classes/api.py` & `satori_ci-1.2.9/src/satorici/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/src/satorici/classes/bundler.py` & `satori_ci-1.2.9/src/satorici/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/src/satorici/classes/playbooks.py` & `satori_ci-1.2.9/src/satorici/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/src/satorici/classes/satori.py` & `satori_ci-1.2.9/src/satorici/classes/satori.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/src/satorici/classes/utils.py` & `satori_ci-1.2.9/src/satorici/classes/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rich.logging import RichHandler
 import logging
 from rich import print_json
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 import random
-from attr import dataclass
+from dataclasses import dataclass
 
 __decorations = "▢•○░"
 __random_colors = ["green", "blue", "red"]
 # IDs
 UUID4_REGEX = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}",
     re.I,
```

### Comparing `satori_ci-1.2.8/src/satorici/classes/validations.py` & `satori_ci-1.2.9/src/satorici/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/src/satorici/satori_module.py` & `satori_ci-1.2.9/src/satorici/satori_module.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.2.8/PKG-INFO` & `satori_ci-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.2.8
+Version: 1.2.9
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

