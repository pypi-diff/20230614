# Comparing `tmp/parsita-1.7.1.tar.gz` & `tmp/parsita-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsita-1.7.1.tar", max compression
+gzip compressed data, was "parsita-1.7.2.tar", max compression
```

## Comparing `parsita-1.7.1.tar` & `parsita-1.7.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1062 2021-07-29 23:44:05.893031 parsita-1.7.1/LICENSE
--rw-r--r--   0        0        0     2647 2021-08-03 12:30:25.999096 parsita-1.7.1/README.md
--rw-r--r--   0        0        0     1782 2022-07-26 18:19:23.248092 parsita-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      403 2022-01-11 00:54:13.509244 parsita-1.7.1/src/parsita/__init__.py
--rw-r--r--   0        0        0     5422 2022-01-11 00:54:13.513244 parsita-1.7.1/src/parsita/metaclasses.py
--rw-r--r--   0        0        0     1234 2021-08-03 02:02:36.179483 parsita-1.7.1/src/parsita/options.py
--rw-r--r--   0        0        0    37469 2022-07-26 16:05:30.115208 parsita-1.7.1/src/parsita/parsers.py
--rw-r--r--   0        0        0    12297 2022-04-04 10:26:40.732520 parsita-1.7.1/src/parsita/state.py
--rw-r--r--   0        0        0     1689 2021-08-03 02:02:36.179483 parsita-1.7.1/src/parsita/util.py
--rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 parsita-1.7.1/setup.py
--rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 parsita-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-31 01:14:00.281278 parsita-1.7.2/LICENSE
+-rw-r--r--   0        0        0     2647 2023-03-31 00:36:25.902559 parsita-1.7.2/README.md
+-rw-r--r--   0        0        0     1786 2023-03-31 01:14:34.505270 parsita-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0      403 2023-03-31 00:36:25.910559 parsita-1.7.2/src/parsita/__init__.py
+-rw-r--r--   0        0        0     5404 2023-03-31 00:36:48.510626 parsita-1.7.2/src/parsita/metaclasses.py
+-rw-r--r--   0        0        0     1234 2023-03-31 00:36:25.906559 parsita-1.7.2/src/parsita/options.py
+-rw-r--r--   0        0        0    37497 2023-03-31 01:13:29.601287 parsita-1.7.2/src/parsita/parsers.py
+-rw-r--r--   0        0        0    12286 2023-03-31 01:13:29.601287 parsita-1.7.2/src/parsita/state.py
+-rw-r--r--   0        0        0     1689 2023-03-31 00:36:25.914559 parsita-1.7.2/src/parsita/util.py
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 parsita-1.7.2/PKG-INFO
```

### Comparing `parsita-1.7.1/LICENSE` & `parsita-1.7.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016-2021 David R Hagen
+Copyright (c) 2016-2023 David R Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `parsita-1.7.1/README.md` & `parsita-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `parsita-1.7.1/pyproject.toml` & `parsita-1.7.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsita"
-version = "1.7.1"
+version = "1.7.2"
 description = "Parser combinator library for Python"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://parsita.drhagen.com"
 repository = "https://github.com/drhagen/parsita"
 keywords = ["text", "parsing", "parser",  "combinator"]
@@ -16,36 +16,39 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
-poetry = "1.2.0b1"
-nox_poetry = "^0.9.0"
+nox_poetry = "^1.0.2"
 
 # Test
-pytest = "^7.1.1"
-coverage = { version = "^6.3.2", extras = ["toml"] }
-pytest-cov = "^3.0.0"
-pytest-timeout = "^2.1.0"
+pytest = "^7.2"
+coverage = { version = "^6.5", extras = ["toml"] }
+pytest-cov = "*"
+pytest-timeout = "*"
 
 # Black
-black = ">=22.3.0"
+black = ">=22.10"
 
 # Isort
-isort = "^5.9.3"
+isort = "^5.10"
 
 # Lint
-flakehell = "0.9.0"
-flake8 = "3.9.0"  # flakehell breaks on 3.9.1
-pep8-naming = "^0.11.1"
+flake8 = "^3.9"
+pep8-naming = "*"
+flake8-noqa = "*"
+flake8-bugbear = "*"
+flake8-broken-line = "*"
+flake8-comprehensions = "*"
+flake8-pyproject = "*"
 
 # Docs
-mkdocs-material = "^8.2.8"
+mkdocs-material = "^8.5"
 
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
@@ -66,23 +69,19 @@
 
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 
-[tool.flakehell]
-max_line_length = 120
-
-[tool.flakehell.plugins]
-# Allow binary operators before line breaks
-# Allow whitespace around `:` because black requires it
-pycodestyle = ["+*", "-W503", "-E203"]
-# Allow glob imports
-pyflakes = ["+*", "-F403", "-F405"]
-# Allow methods whose first argument isn't named `self`
-pep8-naming = ["+*", "-N805"]
+[tool.flake8]
+max-line-length = 120
+noqa-require-code = true
+# F821: undefined-name; Parsita triggers this, but code coverage will catch it
+# E203: whitespace-before-colon; Black formats it this way
+# N805: first-argument-self; Parsita tests and examples define functions in class bodies
+extend-ignore = ["F821", "E203", "N805"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `parsita-1.7.1/src/parsita/metaclasses.py` & `parsita-1.7.2/src/parsita/metaclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .parsers import Parser, RegexParser
 
 
 class ParsersDict(dict):
     def __init__(self, old_options: dict):
         super().__init__()
         self.old_options = old_options  # Holds state of options at start of definition
-        self.forward_declarations = dict()  # Stores forward declarations as they are discovered
+        self.forward_declarations = {}  # Stores forward declarations as they are discovered
 
     def __missing__(self, key):
         frame = inspect.currentframe()  # Should be the frame of __missing__
         while frame.f_code.co_name != "__missing__":  # pragma: no cover
             # But sometimes debuggers add frames on top of the stack; get back to `__missing__`'s frame
             frame = frame.f_back
 
@@ -76,15 +76,15 @@
         }
 
         options.handle_literal = options.wrap_literal
         options.parse_method = options.basic_parse
 
         return ParsersDict(old_options)
 
-    def __init__(cls, name, bases, dct, **_):  # noqa: N805
+    def __init__(cls, name, bases, dct, **_):
         old_options = dct.old_options
 
         super().__init__(name, bases, dct)
 
         # Resolve forward declarations, will raise if name not found
         for name, forward_declaration in dct.forward_declarations.items():
             obj = dct[name]
```

### Comparing `parsita-1.7.1/src/parsita/options.py` & `parsita-1.7.2/src/parsita/options.py`

 * *Files identical despite different names*

### Comparing `parsita-1.7.1/src/parsita/parsers.py` & `parsita-1.7.2/src/parsita/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,19 +192,19 @@
         super().__init__()
         self.pattern = pattern
 
     def consume(self, reader: Reader[Input]):
         remainder = reader
         for elem in self.pattern:
             if remainder.finished:
-                return Backtrack(remainder, lambda: str(elem))
+                return Backtrack(remainder, lambda: str(elem))  # noqa: B023
             elif elem == remainder.first:
                 remainder = remainder.rest
             else:
-                return Backtrack(remainder, lambda: str(elem))
+                return Backtrack(remainder, lambda: str(elem))  # noqa: B023
 
         return Continue(remainder, self.pattern)
 
     def __repr__(self):
         return self.name_or_nothing() + repr(self.pattern)
```

### Comparing `parsita-1.7.1/src/parsita/state.py` & `parsita-1.7.2/src/parsita/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
 class Backtrack(Generic[Input], Status[Input, None]):
     def __init__(self, farthest: Reader[Input], expected: Callable[[], str]):
         self.farthest = farthest
         self.expected = (expected,)
 
     def __repr__(self):
-        return f"Backtrack({self.farthest!r}, {list(map(lambda x: x(), self.expected))})"
+        return f"Backtrack({self.farthest!r}, {[x() for x in self.expected]})"
 
 
 __all__ = [
     "Input",
     "Output",
     "Convert",
     "Reader",
```

### Comparing `parsita-1.7.1/src/parsita/util.py` & `parsita-1.7.2/src/parsita/util.py`

 * *Files identical despite different names*

### Comparing `parsita-1.7.1/PKG-INFO` & `parsita-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsita
-Version: 1.7.1
+Version: 1.7.2
 Summary: Parser combinator library for Python
 Home-page: https://github.com/drhagen/parsita
 License: MIT
 Keywords: text,parsing,parser,combinator
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://parsita.drhagen.com
 Project-URL: Repository, https://github.com/drhagen/parsita
 Description-Content-Type: text/markdown
 
 # Parsita
```

