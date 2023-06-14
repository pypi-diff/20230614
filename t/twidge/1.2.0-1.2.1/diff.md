# Comparing `tmp/twidge-1.2.0.tar.gz` & `tmp/twidge-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twidge-1.2.0.tar", max compression
+gzip compressed data, was "twidge-1.2.1.tar", max compression
```

## Comparing `twidge-1.2.0.tar` & `twidge-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2022-08-12 02:08:32.474197 twidge-1.2.0/LICENSE
--rw-r--r--   0        0        0      753 2022-10-17 05:04:57.804049 twidge-1.2.0/README.md
--rw-r--r--   0        0        0      569 2023-06-13 23:47:57.238378 twidge-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-12 01:26:48.218522 twidge-1.2.0/twidge/__init__.py
--rw-r--r--   0        0        0     1194 2023-06-13 23:03:21.695436 twidge-1.2.0/twidge/__main__.py
--rw-r--r--   0        0        0     5735 2023-06-13 23:40:50.583409 twidge-1.2.0/twidge/core.py
--rw-r--r--   0        0        0     2939 2023-06-13 23:03:21.695436 twidge-1.2.0/twidge/terminal.py
--rw-r--r--   0        0        0      137 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/__init__.py
--rw-r--r--   0        0        0     8528 2023-06-13 23:40:50.673410 twidge-1.2.0/twidge/widgets/editors.py
--rw-r--r--   0        0        0     4311 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/filters.py
--rw-r--r--   0        0        0     1099 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/form.py
--rw-r--r--   0        0        0     4832 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/inline.py
--rw-r--r--   0        0        0     3590 2023-06-13 23:40:50.556743 twidge-1.2.0/twidge/widgets/simple.py
--rw-r--r--   0        0        0     3797 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/templater.py
--rw-r--r--   0        0        0     6641 2023-06-13 23:03:21.698769 twidge-1.2.0/twidge/widgets/wrappers.py
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 twidge-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-08-12 02:08:32.474197 twidge-1.2.1/LICENSE
+-rw-r--r--   0        0        0      977 2023-06-14 02:08:56.536980 twidge-1.2.1/README.md
+-rw-r--r--   0        0        0      569 2023-06-14 00:36:54.336833 twidge-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-12 01:26:48.218522 twidge-1.2.1/twidge/__init__.py
+-rw-r--r--   0        0        0     1194 2023-06-13 23:03:21.695436 twidge-1.2.1/twidge/__main__.py
+-rw-r--r--   0        0        0     5735 2023-06-13 23:40:50.583409 twidge-1.2.1/twidge/core.py
+-rw-r--r--   0        0        0     2939 2023-06-13 23:03:21.695436 twidge-1.2.1/twidge/terminal.py
+-rw-r--r--   0        0        0      137 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/__init__.py
+-rw-r--r--   0        0        0     9703 2023-06-14 02:04:25.559092 twidge-1.2.1/twidge/widgets/editors.py
+-rw-r--r--   0        0        0     4311 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/filters.py
+-rw-r--r--   0        0        0     1099 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/form.py
+-rw-r--r--   0        0        0     4832 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/inline.py
+-rw-r--r--   0        0        0     3590 2023-06-13 23:40:50.556743 twidge-1.2.1/twidge/widgets/simple.py
+-rw-r--r--   0        0        0     3797 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/templater.py
+-rw-r--r--   0        0        0     6641 2023-06-13 23:03:21.698769 twidge-1.2.1/twidge/widgets/wrappers.py
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 twidge-1.2.1/PKG-INFO
```

### Comparing `twidge-1.2.0/LICENSE` & `twidge-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/pyproject.toml` & `twidge-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twidge"
-version = "1.2.0"
+version = "1.2.1"
 description = "Terminal Widgets."
 authors = ["Aidan Courtney <aidanfc97@gmail.com>"]
 repository = 'https://github.com/aidaco/twidge'
 readme = 'README.md'
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `twidge-1.2.0/twidge/__main__.py` & `twidge-1.2.1/twidge/__main__.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/core.py` & `twidge-1.2.1/twidge/core.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/terminal.py` & `twidge-1.2.1/twidge/terminal.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/editors.py` & `twidge-1.2.1/twidge/widgets/editors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import re
 import typing
 from functools import partial
 from math import ceil, floor
 
+from rich.measure import Measurement
 from rich.style import Style
 from rich.styled import Styled
+from rich.table import Table
 from rich.text import Text
 
 from twidge.core import DispatchBuilder, RunBuilder
+from twidge.widgets.wrappers import FocusManager
 
 
 class EditString:
     run = RunBuilder()
     dispatch = DispatchBuilder()
 
     def __init__(
@@ -62,14 +65,18 @@
             if self.focus
             else Text(sstr) + Text(cstr) + Text(estr)
         )
 
         # Render lines after cursor, if any
         yield from (line[:width] for line in elines)
 
+    def __rich_measure__(self, console, options):
+        width = max(len(line) for line in self.lines) + 1
+        return Measurement(width, width)
+
     @dispatch.on("left")
     def cursor_left(self):
         if self.cursor[1] != 0:
             self.cursor[1] -= 1
         else:
             if self.cursor[0] != 0:
                 self.cursor[0] -= 1
@@ -139,15 +146,14 @@
                 self.cursor[0] -= 1
 
     @dispatch.on("ctrl+h")
     def delete_word(self):
         line = self.lines[self.cursor[0]]
         sec = line[: self.cursor[1]][::-1]
         m = re.search(r"(?>.)\b|$", sec)
-        print(sec, self.cursor, m)
         prev_non_word = m.end()
         n = self.cursor[1] - prev_non_word
         self.lines[self.cursor[0]] = (
             self.lines[self.cursor[0]][:n]
             + self.lines[self.cursor[0]][self.cursor[1] :]
         )
         self.cursor[1] = n
@@ -276,8 +282,42 @@
 EditNumericString = partial(ParsedEditString, parser=parse_numeric)
 
 
 def EditEnumString(enum_cls):
     return ParsedEditString(parser=enum_cls)
 
 
-__all__ = ["EditString"]
+class EditDict:
+    run = RunBuilder()
+    dispatch = DispatchBuilder()
+
+    def __init__(self, content: dict[str, str]):
+        self.content = content
+        self.editors = {EditString(k): EditString(v) for k, v in content.items()}
+        self.focuser = FocusManager(*(w for kv in self.editors.items() for w in kv))
+
+    @property
+    def result(self):
+        return {k.result: v.result for k, v in self.editors.items()}
+
+    def __rich__(self):
+        t = Table.grid(padding=(0, 1, 0, 0))
+        t.add_column()
+        t.add_column()
+        for k, v in self.editors.items():
+            t.add_row(Styled(k, style="bright_green"), v)
+        return t
+
+    @dispatch.on("tab")
+    def focus_advance(self):
+        self.focuser.forward()
+
+    @dispatch.on("shift+tab")
+    def focus_back(self):
+        self.focuser.back()
+
+    @dispatch.default
+    def passthrough(self, event):
+        self.focuser.focused.dispatch(event)
+
+
+__all__ = ["EditString", "EditDict"]
```

### Comparing `twidge-1.2.0/twidge/widgets/filters.py` & `twidge-1.2.1/twidge/widgets/filters.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/form.py` & `twidge-1.2.1/twidge/widgets/form.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/inline.py` & `twidge-1.2.1/twidge/widgets/inline.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/simple.py` & `twidge-1.2.1/twidge/widgets/simple.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/templater.py` & `twidge-1.2.1/twidge/widgets/templater.py`

 * *Files identical despite different names*

### Comparing `twidge-1.2.0/twidge/widgets/wrappers.py` & `twidge-1.2.1/twidge/widgets/wrappers.py`

 * *Files identical despite different names*

