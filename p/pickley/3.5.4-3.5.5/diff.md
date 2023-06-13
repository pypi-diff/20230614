# Comparing `tmp/pickley-3.5.4.tar.gz` & `tmp/pickley-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.5.4.tar", last modified: Tue Jun 13 23:10:53 2023, max compression
+gzip compressed data, was "pickley-3.5.5.tar", last modified: Tue Jun 13 23:46:33 2023, max compression
```

## Comparing `pickley-3.5.4.tar` & `pickley-3.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.435780 pickley-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 23:09:07.000000 pickley-3.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 23:09:07.000000 pickley-3.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:10:53.435780 pickley-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 23:09:07.000000 pickley-3.5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 23:09:07.000000 pickley-3.5.4/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:09:07.000000 pickley-3.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:10:53.435780 pickley-3.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 23:09:07.000000 pickley-3.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31357 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 23:09:07.000000 pickley-3.5.4/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.431780 pickley-3.5.4/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 23:10:53.000000 pickley-3.5.4/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:10:53.435780 pickley-3.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 23:09:07.000000 pickley-3.5.4/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 23:45:03.000000 pickley-3.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 23:45:03.000000 pickley-3.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:46:33.645017 pickley-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 23:45:03.000000 pickley-3.5.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 23:45:03.000000 pickley-3.5.5/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:45:03.000000 pickley-3.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:46:33.645017 pickley-3.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 23:45:03.000000 pickley-3.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.641018 pickley-3.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36368 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31371 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 23:45:03.000000 pickley-3.5.5/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 23:46:33.000000 pickley-3.5.5/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:46:33.645017 pickley-3.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 23:45:03.000000 pickley-3.5.5/tests/test_venv.py
```

### Comparing `pickley-3.5.4/LICENSE` & `pickley-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/PKG-INFO` & `pickley-3.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.4
+Version: 3.5.5
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.4/README.rst` & `pickley-3.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/setup.py` & `pickley-3.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/src/pickley/__init__.py` & `pickley-3.5.5/src/pickley/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.5.4"
+__version__ = "3.5.5"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pk"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
@@ -469,14 +469,21 @@
         self.base = FolderBase("base", runez.resolved_path(base_path))
         self.meta = FolderBase("meta", os.path.join(self.base.path, DOT_META))
         self.cache = FolderBase("cache", os.path.join(self.meta.path, ".cache"))
         if self.cli:
             cli = runez.serialize.json_sanitized(self.cli.to_dict())
             self.configs.append(RawConfig(self, "cli", cli))
 
+        # TODO: Remove once pickley 3.4 is phased out
+        old_meta = self.base.full_path(".pickley")
+        old_cfg = os.path.join(old_meta, "config.json")
+        new_cfg = self.meta.full_path("config.json")
+        if not os.path.exists(new_cfg) and os.path.exists(old_cfg):
+            runez.move(old_cfg, new_cfg)
+
         self._add_config_file(self.config_path)
         self._add_config_file(self.meta.full_path("config.json"))
         defaults = dict(
             delivery="wrap",
             install_timeout=1800,
             min_python="3.6",
             preferred_min_python="3.7",
```

### Comparing `pickley-3.5.4/src/pickley/bstrap.py` & `pickley-3.5.5/src/pickley/bstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/src/pickley/cli.py` & `pickley-3.5.5/src/pickley/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         wrap = DeliveryMethodWrap()
         wrap.install(venv, {PICKLEY: PICKLEY})
 
         # TODO: Remove once pickley 3.4 is phased out
         old_meta = CFG.base.full_path(".pickley")
         if os.path.isdir(old_meta):
             runez.delete(old_meta)
-            runez.run(os.path.join(venv.folder, "bin", PICKLEY), "auto-heal")
+            runez.run(os.path.join(pspec.active_install_path, "bin", PICKLEY), "auto-heal")
 
         return
 
     if what:
         paths = {
             "audit": CFG.meta.full_path("audit.log"),
             "cache": CFG.cache.path,
```

### Comparing `pickley-3.5.4/src/pickley/delivery.py` & `pickley-3.5.5/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/src/pickley/package.py` & `pickley-3.5.5/src/pickley/package.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/src/pickley.egg-info/PKG-INFO` & `pickley-3.5.5/src/pickley.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.5.4
+Version: 3.5.5
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.5.4/src/pickley.egg-info/SOURCES.txt` & `pickley-3.5.5/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/tests/test_bootstrap.py` & `pickley-3.5.5/tests/test_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from unittest.mock import patch
 
 import pytest
 import runez
 
-from pickley import __version__, bstrap, DOT_META
+from pickley import bstrap, DOT_META
 
 
 def mocked_expanduser(path):
     if path and path.startswith("~/"):
         path = path[2:]
 
     return path
@@ -25,20 +25,21 @@
 
 
 def mocked_which(program):
     return None if program == "pickley" else program
 
 
 def test_bootstrap(cli, monkeypatch):
-    runez.touch(".pickley/foo")
+    runez.touch(".pickley/config.json")
     cli.run("-n base bootstrap-own-wrapper")
     assert cli.succeeded
+    assert f"Would move .pickley/config.json -> {DOT_META}/config.json" in cli.logged
     assert f"Would save {DOT_META}/pickley.manifest.json" in cli.logged
     assert "Would delete .pickley" in cli.logged
-    assert f"Would run: .pk/pickley-{__version__}/bin/pickley auto-heal" in cli.logged
+    assert f"Would run: {DOT_META}/pickley/bin/pickley auto-heal" in cli.logged
 
     with patch("pickley.bstrap.which", side_effect=mocked_which):
         with patch("pickley.bstrap.os.path.expanduser", side_effect=mocked_expanduser):
             runez.write(".local/bin/pickley", "#!/bin/sh\necho 0.1")  # Pretend we have an old pickley
             runez.make_executable(".local/bin/pickley")
 
             with patch("pickley.bstrap.get_python_version", return_value=(3, 6)):  # urllib fails
```

### Comparing `pickley-3.5.4/tests/test_config.py` & `pickley-3.5.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/tests/test_delivery.py` & `pickley-3.5.5/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/tests/test_ops.py` & `pickley-3.5.5/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/tests/test_run.py` & `pickley-3.5.5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.5.4/tests/test_venv.py` & `pickley-3.5.5/tests/test_venv.py`

 * *Files identical despite different names*

