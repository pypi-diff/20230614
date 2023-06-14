# Comparing `tmp/hin-0.1.0.tar.gz` & `tmp/hin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hin-0.1.0.tar", max compression
+gzip compressed data, was "hin-0.1.1.tar", max compression
```

## Comparing `hin-0.1.0.tar` & `hin-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-11 11:32:32.617796 hin-0.1.0/LICENSE
--rw-r--r--   0        0        0     2960 2023-06-11 11:33:23.152215 hin-0.1.0/README.rst
--rw-r--r--   0        0        0      123 2023-06-11 11:33:23.153167 hin-0.1.0/hin/__init__.py
--rw-r--r--   0        0        0      149 2023-06-11 11:33:23.153310 hin-0.1.0/hin/__main__.py
--rw-r--r--   0        0        0     3401 2023-06-11 11:33:23.153465 hin-0.1.0/hin/_actions.py
--rw-r--r--   0        0        0     3538 2023-06-11 11:33:23.153617 hin-0.1.0/hin/_add.py
--rw-r--r--   0        0        0      766 2023-06-11 11:33:23.153755 hin-0.1.0/hin/_clone.py
--rw-r--r--   0        0        0     1324 2023-06-11 11:33:23.153889 hin-0.1.0/hin/_commit.py
--rw-r--r--   0        0        0     2080 2023-06-11 11:33:23.154033 hin-0.1.0/hin/_config.py
--rw-r--r--   0        0        0     7744 2023-06-11 11:33:23.154196 hin-0.1.0/hin/_decorators.py
--rw-r--r--   0        0        0     5422 2023-06-11 11:33:23.154353 hin-0.1.0/hin/_file.py
--rw-r--r--   0        0        0     1650 2023-06-11 11:33:23.154493 hin-0.1.0/hin/_gitignore.py
--rw-r--r--   0        0        0     1916 2023-06-11 11:33:23.154643 hin-0.1.0/hin/_link.py
--rw-r--r--   0        0        0      676 2023-06-11 11:33:23.154775 hin-0.1.0/hin/_list.py
--rw-r--r--   0        0        0     5360 2023-06-11 11:33:23.154940 hin-0.1.0/hin/_main.py
--rw-r--r--   0        0        0     1132 2023-06-11 11:33:23.155077 hin-0.1.0/hin/_push.py
--rw-r--r--   0        0        0     1167 2023-06-11 11:33:23.155221 hin-0.1.0/hin/_remove.py
--rw-r--r--   0        0        0     2324 2023-06-11 11:33:23.155356 hin-0.1.0/hin/_status.py
--rw-r--r--   0        0        0     1268 2023-06-11 11:33:23.155509 hin-0.1.0/hin/_undo.py
--rw-r--r--   0        0        0      207 2023-06-11 11:33:23.155735 hin-0.1.0/hin/_version.py
--rw-r--r--   0        0        0        0 2023-06-11 11:33:23.155760 hin-0.1.0/hin/py.typed
--rw-r--r--   0        0        0     2231 2023-06-11 11:33:23.157226 hin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-14 10:28:55.233256 hin-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-14 10:28:55.233401 hin-0.1.1/README.rst
+-rw-r--r--   0        0        0      123 2023-06-14 10:28:55.233905 hin-0.1.1/hin/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-14 10:28:59.380763 hin-0.1.1/hin/__main__.py
+-rw-r--r--   0        0        0     3398 2023-06-14 10:28:59.380882 hin-0.1.1/hin/_actions.py
+-rw-r--r--   0        0        0     3535 2023-06-14 10:28:59.380994 hin-0.1.1/hin/_add.py
+-rw-r--r--   0        0        0      763 2023-06-14 10:28:59.381085 hin-0.1.1/hin/_clone.py
+-rw-r--r--   0        0        0     1321 2023-06-14 10:28:59.381194 hin-0.1.1/hin/_commit.py
+-rw-r--r--   0        0        0     2077 2023-06-14 10:28:59.381312 hin-0.1.1/hin/_config.py
+-rw-r--r--   0        0        0     7741 2023-06-14 10:28:59.381438 hin-0.1.1/hin/_decorators.py
+-rw-r--r--   0        0        0     5675 2023-06-14 10:29:01.034086 hin-0.1.1/hin/_file.py
+-rw-r--r--   0        0        0     1647 2023-06-14 10:28:59.381643 hin-0.1.1/hin/_gitignore.py
+-rw-r--r--   0        0        0     1913 2023-06-14 10:28:59.381747 hin-0.1.1/hin/_link.py
+-rw-r--r--   0        0        0      673 2023-06-14 10:28:59.381849 hin-0.1.1/hin/_list.py
+-rw-r--r--   0        0        0     5357 2023-06-14 10:28:59.381968 hin-0.1.1/hin/_main.py
+-rw-r--r--   0        0        0     1129 2023-06-14 10:28:59.382090 hin-0.1.1/hin/_push.py
+-rw-r--r--   0        0        0     1164 2023-06-14 10:28:59.382178 hin-0.1.1/hin/_remove.py
+-rw-r--r--   0        0        0     2496 2023-06-14 10:29:01.034230 hin-0.1.1/hin/_status.py
+-rw-r--r--   0        0        0     1265 2023-06-14 10:28:59.382378 hin-0.1.1/hin/_undo.py
+-rw-r--r--   0        0        0      204 2023-06-14 10:29:01.215534 hin-0.1.1/hin/_version.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:28:55.235217 hin-0.1.1/hin/py.typed
+-rw-r--r--   0        0        0     2231 2023-06-14 10:29:01.216119 hin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.1/PKG-INFO
```

### Comparing `hin-0.1.0/LICENSE` & `hin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hin-0.1.0/README.rst` & `hin-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hin-0.1.0/hin/_actions.py` & `hin-0.1.1/hin/_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._actions
-===============
+============
 """
 from __future__ import annotations
 
 import json as _json
 import shutil as _shutil
 import typing as _t
 from abc import ABC as _ABC
```

### Comparing `hin-0.1.0/hin/_add.py` & `hin-0.1.1/hin/_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._add
-===========
+========
 """
 from rich.console import Console as _Console
 
 from . import _decorators
 from ._actions import Move as _Move
 from ._config import Config as _Config
 from ._file import Entry as _Entry
```

### Comparing `hin-0.1.0/hin/_clone.py` & `hin-0.1.1/hin/_clone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._clone
-=============
+==========
 """
 from __future__ import annotations
 
 from os import environ as _e
 from pathlib import Path as _Path
 
 import git as _git
```

### Comparing `hin-0.1.0/hin/_commit.py` & `hin-0.1.1/hin/_commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._commit
-==============
+===========
 """
 from __future__ import annotations
 
 import git as _git
 from git import Repo as _Repo
 from rich.console import Console as _Console
```

### Comparing `hin-0.1.0/hin/_config.py` & `hin-0.1.1/hin/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._config
-==============
+===========
 """
 import os as _os
 import typing as _t
 from os import environ as _e
 from pathlib import Path as _Path
 
 from configobj import ConfigObj as _ConfigObj
```

### Comparing `hin-0.1.0/hin/_decorators.py` & `hin-0.1.1/hin/_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._decorators
-==================
+===============
 """
 from __future__ import annotations
 
 import functools as _functools
 import inspect as _inspect
 import os as _os
 import typing as _t
```

### Comparing `hin-0.1.0/hin/_file.py` & `hin-0.1.1/hin/_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._file
-============
+=========
 """
 from __future__ import annotations
 
 import hashlib as _hashlib
 import os as _os
 import re as _re
 from abc import ABC as _ABC
@@ -93,14 +93,23 @@
         return self._key
 
     @property
     def value(self) -> _File:
         """Path to the actual file or directory."""
         return self._value
 
+    @property
+    def isdotfile(self) -> bool:
+        """Boolean for whether file begins with a dot.
+
+        Some hidden files, such as ~/Library for OSX do not begin with a
+        dot.
+        """
+        return str(self._key.relpath).startswith(".")
+
     def is_child_of(self, other: Matrix) -> bool:
         """Check whether this is a child of a file matrix.
 
         :param other: Matrix to check against.
         :return: Boolean for whether this is the child of a matrix.
         """
         return (str(self.key.path).startswith(str(other.key.path))) or (
```

### Comparing `hin-0.1.0/hin/_gitignore.py` & `hin-0.1.1/hin/_gitignore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._gitignore
-=================
+==============
 """
 from __future__ import annotations
 
 from pathlib import Path as _Path
 
 
 class Gitignore:
```

### Comparing `hin-0.1.0/hin/_link.py` & `hin-0.1.1/hin/_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._link
-============
+=========
 """
 from rich.console import Console as _Console
 
 from . import _decorators
 from ._config import Config as _Config
 from ._file import Custom as _Custom
 from ._gitignore import unignore as _unignore
```

### Comparing `hin-0.1.0/hin/_list.py` & `hin-0.1.1/hin/_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._list
-============
+=========
 """
 from rich.console import Console as _Console
 
 from . import _decorators
 from ._config import Config as _Config
 from ._file import Custom as _Custom
```

### Comparing `hin-0.1.0/hin/_main.py` & `hin-0.1.1/hin/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._main
-============
+=========
 """
 # pylint: disable=no-value-for-parameter
 from __future__ import annotations
 
 import getpass as _getpass
 import socket as _socket
 import sys as _sys
```

### Comparing `hin-0.1.0/hin/_push.py` & `hin-0.1.1/hin/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._push
-============
+=========
 """
 from __future__ import annotations
 
 import git as _git
 from rich.console import Console as _Console
 
 from . import _decorators
```

### Comparing `hin-0.1.0/hin/_remove.py` & `hin-0.1.1/hin/_remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._remove
-==============
+===========
 """
 from rich.console import Console as _Console
 
 from . import _decorators
 from ._actions import Move as _Move
 from ._config import Config as _Config
 from ._file import Entry as _Entry
```

### Comparing `hin-0.1.0/hin/_status.py` & `hin-0.1.1/hin/_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._status
-==============
+===========
 """
 from __future__ import annotations
 
 import re as _re
 from os import environ as _e
 from pathlib import Path as _Path
 
@@ -31,24 +31,32 @@
 
     @property
     def path(self) -> str:
         """Changed path."""
         return self._path
 
 
+def _print_paths(line: str, config: _Config) -> None:
+    if line.startswith("\t"):
+        path_ref = _PathRef(_re.sub(" +", " ", line).strip())
+        for existing in config.values():
+            if path_ref.path.startswith(str(existing.value.relpath)):
+                path = str(path_ref.path)
+                if existing.isdotfile:
+                    path = f".{path}"
+
+                print(path_ref.kind, path)
+
+
 def _print_status(out: _Console, output: str, config: _Config) -> None:
     for line in output.splitlines():
         if _re.match(r"((\w+(?: \w+)*):)", line):
             out.print(f"[green bold]{line}[/green bold]")
 
-        if line.startswith("\t"):
-            path_ref = _PathRef(_re.sub(" +", " ", line).strip())
-            for existing in config.values():
-                if path_ref.path.startswith(str(existing.value.relpath)):
-                    print(path_ref.kind, existing.key.relpath)
+        _print_paths(line, config)
 
 
 @_decorators.console
 @_decorators.config
 @_decorators.repository
 def status(
     config: _Config, out: _Console, file: str | None, repo: _git.Repo
```

### Comparing `hin-0.1.0/hin/_undo.py` & `hin-0.1.1/hin/_undo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 hin._undo
-============
+=========
 """
 from os import environ as _e
 from pathlib import Path as _Path
 
 import git as _git
 from rich.console import Console as _Console
```

### Comparing `hin-0.1.0/pyproject.toml` & `hin-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "hin"
 readme = "README.rst"
 repository = "https://github.com/jshwi/hin"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 appdirs = "^1.4.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 configobj = "^5.0.8"
 gitpython = "^3.1.31"
```

### Comparing `hin-0.1.0/PKG-INFO` & `hin-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dotfile manager
 Home-page: https://pypi.org/project/hin/
 License: MIT
 Keywords: config,dot,dotfile,file,hin
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```

