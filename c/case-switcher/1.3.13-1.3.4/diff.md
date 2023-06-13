# Comparing `tmp/case-switcher-1.3.13.tar.gz` & `tmp/case-switcher-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "case-switcher-1.3.13.tar", max compression
+gzip compressed data, was "case-switcher-1.3.4.tar", max compression
```

## Comparing `case-switcher-1.3.13.tar` & `case-switcher-1.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-12 13:51:17.470536 case-switcher-1.3.13/LICENSE
--rw-r--r--   0        0        0     2224 2023-06-12 13:51:17.470536 case-switcher-1.3.13/README.md
--rw-r--r--   0        0        0     3904 2023-06-12 19:34:41.216943 case-switcher-1.3.13/caseswitcher/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 13:51:17.470536 case-switcher-1.3.13/caseswitcher/py.typed
--rw-r--r--   0        0        0      881 2023-06-12 21:45:23.373300 case-switcher-1.3.13/pyproject.toml
--rw-r--r--   0        0        0     2828 2023-06-13 22:24:17.562188 case-switcher-1.3.13/setup.py
--rw-r--r--   0        0        0     2917 2023-06-13 22:24:17.562378 case-switcher-1.3.13/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-03-25 18:47:58.296000 case-switcher-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2048 2022-04-03 17:41:18.926711 case-switcher-1.3.4/README.md
+-rw-r--r--   0        0        0     3181 2022-08-20 21:58:15.207397 case-switcher-1.3.4/caseswitcher/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-09 11:59:11.453000 case-switcher-1.3.4/caseswitcher/py.typed
+-rw-r--r--   0        0        0      880 2022-08-20 21:57:02.149432 case-switcher-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2644 2022-08-20 21:58:22.673778 case-switcher-1.3.4/setup.py
+-rw-r--r--   0        0        0     2740 2022-08-20 21:58:22.673983 case-switcher-1.3.4/PKG-INFO
```

### Comparing `case-switcher-1.3.13/LICENSE` & `case-switcher-1.3.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Matthew Burkard
+Copyright (c) 2022 Matthew Burkard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `case-switcher-1.3.13/README.md` & `case-switcher-1.3.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: case-switcher
+Version: 1.3.4
+Summary: Library to change the casing of strings.
+Home-page: https://gitlab.com/mburkard/case-switcher
+License: MIT
+Keywords: string,string manipulation,case convention,camel case,dot case,kebab case,pascal case,snake case,title case
+Author: Matthew Burkard
+Author-email: matthewjburkard@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Project-URL: Repository, https://gitlab.com/mburkard/case-switcher
+Description-Content-Type: text/markdown
+
 <div align=center>
 <!-- Title: -->
   <h1>Case Switcher</h1>
   <h3>Change the casing of a string.</h3>
 <!-- Labels: -->
   <!-- First row: -->
   <img src="https://img.shields.io/badge/license-MIT-green"
@@ -12,14 +29,19 @@
    alt="Code style: black">
   <img src="https://img.shields.io/pypi/v/case-switcher.svg"
    height="20"
    alt="PyPI version">
   <img src="https://img.shields.io/badge/coverage-100%25-success"
    height="20"
    alt="Code Coverage">
+  <a href="https://www.codefactor.io/repository/github/matthew-burkard/case-switcher">
+    <img
+     src="https://www.codefactor.io/repository/github/matthew-burkard/case-switcher/badge"
+     alt="CodeFactor" />
+  </a>
 </div>
 
 This library provides functions to change the casing convention of a string.
 
 Supported cases:
 
 - camelCase
@@ -53,23 +75,12 @@
 caseswitcher.to_camel(sample)  # -> "avocadoBagelCoffeeDONUTEclairFoodGravy"
 caseswitcher.to_dot(sample)  # -> "avocado.bagel.coffee.donut.eclair.food.gravy"
 caseswitcher.to_kebab(sample)  # -> "avocado-bagel-coffee-donut-eclair-food-gravy"
 caseswitcher.to_pascal(sample)  # -> "AvocadoBagelCoffeeDONUTEclairFoodGravy"
 caseswitcher.to_path(sample)  # -> "avocado/bagel/coffee/donut/eclair/food/gravy"
 caseswitcher.to_snake(sample)  # -> "avocado_bagel_coffee_donut_eclair_food_gravy"
 caseswitcher.to_title(sample)  # -> "Avocado Bagel Coffee DONUT Eclair Food Gravy"
-# Deprecated, use `to_dot(sample).upper()` instead.
 caseswitcher.to_upper_dot(sample)  # -> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"
-# Deprecated, use `to_kebab(sample).upper()` instead.
 caseswitcher.to_upper_kebab(sample)  # -> "AVOCADO-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-GRAVY"
-# Deprecated, use `to_snake(sample).upper()` instead.
 caseswitcher.to_upper_snake(sample)  # -> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY"
 ```
 
-## Support The Developer
-
-<a href="https://www.buymeacoffee.com/mburkard" target="_blank">
-  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png"
-       width="217"
-       height="60"
-       alt="Buy Me A Coffee">
-</a>
```

#### html2text {}

```diff
@@ -1,24 +1,32 @@
+Metadata-Version: 2.1 Name: case-switcher Version: 1.3.4 Summary: Library to
+change the casing of strings. Home-page: https://gitlab.com/mburkard/case-
+switcher License: MIT Keywords: string,string manipulation,case
+convention,camel case,dot case,kebab case,pascal case,snake case,title case
+Author: Matthew Burkard Author-email: matthewjburkard@gmail.com Requires-
+Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.9
+Project-URL: Repository, https://gitlab.com/mburkard/case-switcher Description-
+Content-Type: text/markdown
                           ****** Case Switcher ******
                    **** Change the casing of a string. ****
-        [License: MIT] [Code style: black] [PyPI version] [Code Coverage]
+       [License: MIT] [Code style: black] [PyPI version] [Code Coverage]
+                                 [CodeFactor]
 This library provides functions to change the casing convention of a string.
 Supported cases: - camelCase - dot.case - kebab-case - PascalCase - path/case -
 snake_case - Title Case - UPPER.DOT.CASE - UPPER-KEBAB-CASE - UPPER_SNAKE_CASE
 ### Install ```shell poetry add case-switcher ``` ```shell pip install case-
 switcher ``` ### Demo ```python import caseswitcher sample = "avocado bagel-
 coffeeDONUTEclair_food.gravy" caseswitcher.to_camel(sample) # -
 > "avocadoBagelCoffeeDONUTEclairFoodGravy" caseswitcher.to_dot(sample) # -
 > "avocado.bagel.coffee.donut.eclair.food.gravy" caseswitcher.to_kebab(sample)
 # -> "avocado-bagel-coffee-donut-eclair-food-gravy" caseswitcher.to_pascal
 (sample) # -> "AvocadoBagelCoffeeDONUTEclairFoodGravy" caseswitcher.to_path
 (sample) # -> "avocado/bagel/coffee/donut/eclair/food/gravy"
 caseswitcher.to_snake(sample) # -
 > "avocado_bagel_coffee_donut_eclair_food_gravy" caseswitcher.to_title(sample)
-# -> "Avocado Bagel Coffee DONUT Eclair Food Gravy" # Deprecated, use `to_dot
-(sample).upper()` instead. caseswitcher.to_upper_dot(sample) # -
-> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY" # Deprecated, use `to_kebab
-(sample).upper()` instead. caseswitcher.to_upper_kebab(sample) # -> "AVOCADO-
-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-GRAVY" # Deprecated, use `to_snake(sample).upper
-()` instead. caseswitcher.to_upper_snake(sample) # -
-> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY" ``` ## Support The Developer
-[Buy_Me_A_Coffee]
+# -> "Avocado Bagel Coffee DONUT Eclair Food Gravy" caseswitcher.to_upper_dot
+(sample) # -> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"
+caseswitcher.to_upper_kebab(sample) # -> "AVOCADO-BAGEL-COFFEE-DONUT-ECLAIR-
+FOOD-GRAVY" caseswitcher.to_upper_snake(sample) # -
+> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY" ```
```

### Comparing `case-switcher-1.3.13/caseswitcher/__init__.py` & `case-switcher-1.3.4/caseswitcher/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,77 @@
 """Module with functions to change casing of a string."""
+import re
+
+from typing import Union
 
 __all__ = (
     "get_words",
     "to_camel",
     "to_dot",
     "to_kebab",
     "to_pascal",
     "to_snake",
     "to_title",
+    "to_upper_dot",
+    "to_upper_kebab",
+    "to_upper_snake",
 )
 
-import re
-import warnings
-
-from typing import Union
-
 
 def to_camel(string: str) -> str:
     """Return a version of the string in camelCase format."""
-    preserve_upper = not string.isupper()
     words = get_words(string)
     first_word = ""
     if len(words) > 0:
-        first_word = (
-            words[0] if words[0].isupper() and preserve_upper else words[0].lower()
-        )
-    return first_word + "".join(_capitalize(w, preserve_upper) for w in words[1:])
+        first_word = words[0] if words[0].isupper() else words[0].lower()
+    return first_word + "".join(map(_capitalize, words[1:]))
 
 
 def to_dot(string: str) -> str:
     """Return a version of the string in dot.case format."""
     return ".".join(map(lambda w: w.lower(), get_words(string)))
 
 
 def to_kebab(string: str) -> str:
     """Return a version of the string in kebab-case format."""
     return "-".join(map(lambda w: w.lower(), get_words(string)))
 
 
 def to_pascal(string: str) -> str:
     """Return a version of the string in PascalCase format."""
-    preserve_upper = not string.isupper()
-    return "".join(_capitalize(w, preserve_upper) for w in get_words(string))
+    return "".join(map(_capitalize, get_words(string)))
 
 
 def to_path(string: str) -> str:
     """Return a version of the string in path/case format."""
     return "/".join(map(lambda w: w.lower(), get_words(string)))
 
 
 def to_snake(string: str) -> str:
     """Return a version of the string in snake_case format."""
     return "_".join(map(lambda w: w.lower(), get_words(string)))
 
 
 def to_title(string: str) -> str:
     """Return a version of the string in Title Case format."""
-    preserve_upper = not string.isupper()
-    return " ".join(_capitalize(w, preserve_upper) for w in get_words(string))
+    return " ".join(map(_capitalize, get_words(string)))
 
 
 def to_upper_dot(string: str) -> str:
     """Return a version of the string in UPPER.DOT.CASE format."""
-    warnings.warn(
-        f"to_upper_dot(...) is Deprecated. Use to_dot(...).upper() instead.",
-        category=DeprecationWarning,
-        stacklevel=2,
-    )
     return ".".join(map(lambda w: w.upper(), get_words(string)))
 
 
 def to_upper_kebab(string: str) -> str:
     """Return a version of the string in UPPER-KEBAB-CASE format."""
-    warnings.warn(
-        f"to_upper_kebab(...) is Deprecated. Use to_kebab(...).upper() instead.",
-        category=DeprecationWarning,
-        stacklevel=2,
-    )
     return "-".join(map(lambda w: w.upper(), get_words(string)))
 
 
 def to_upper_snake(string: str) -> str:
     """Return a version of the string in UPPER_SNAKE_CASE format."""
-    warnings.warn(
-        f"to_upper_snake(...) is Deprecated. Use to_snake(...).upper() instead.",
-        category=DeprecationWarning,
-        stacklevel=2,
-    )
     return "_".join(map(lambda w: w.upper(), get_words(string)))
 
 
 def get_words(string: str) -> list[str]:
     """Get a list of the words in a string in the order they appear."""
     words = [it for it in re.split(r"\b|_", string) if re.match(r"\w", it)]
     # Split on lower then upper: "oneTwo" -> ["one", "Two"]
@@ -98,16 +79,16 @@
     # Split on upper then upper + lower: "JSONWord" -> ["JSON", "Word"]
     words = _split_words_on_regex(words, re.compile(r"(?<=[A-Z])(?=[A-Z][a-z])"))
     # Split on number + letter: "TO1Cat23dog" -> ["TO1", "Cat23", "dog"]
     words = _split_words_on_regex(words, re.compile(r"(?<=\d)(?=[A-Za-z])"))
     return words
 
 
-def _capitalize(word: str, preserve_upper: bool) -> str:
-    return word if preserve_upper and word.isupper() else word.capitalize()
+def _capitalize(word: str) -> str:
+    return word if word.isupper() else word.capitalize()
 
 
 def _split_words_on_regex(words: list[str], regex: Union[re.Pattern, str]) -> list[str]:
     words = words.copy()
     for i, word in enumerate(words):
         split_words = re.split(regex, word)
         if len(split_words) > 1:
```

### Comparing `case-switcher-1.3.13/pyproject.toml` & `case-switcher-1.3.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "case-switcher"
-version = "1.3.13"
+version = "1.3.4"
 description = "Library to change the casing of strings."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/case-switcher"
 homepage = "https://gitlab.com/mburkard/case-switcher"
 keywords = [
     "string",
     "string manipulation",
@@ -24,14 +24,14 @@
     { include = "caseswitcher/py.typed" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
-coverage = "^7.0.5"
-mypy = "^1.0.1"
+pytest = "^7.1.1"
+coverage = "^6.4.4"
+mypy = "^0.971"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `case-switcher-1.3.13/setup.py` & `case-switcher-1.3.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['__init__', 'py']
 setup_kwargs = {
     'name': 'case-switcher',
-    'version': '1.3.13',
+    'version': '1.3.4',
     'description': 'Library to change the casing of strings.',
-    'long_description': '<div align=center>\n<!-- Title: -->\n  <h1>Case Switcher</h1>\n  <h3>Change the casing of a string.</h3>\n<!-- Labels: -->\n  <!-- First row: -->\n  <img src="https://img.shields.io/badge/license-MIT-green"\n   height="20"\n   alt="License: MIT">\n  <img src="https://img.shields.io/badge/code%20style-black-000000.svg"\n   height="20"\n   alt="Code style: black">\n  <img src="https://img.shields.io/pypi/v/case-switcher.svg"\n   height="20"\n   alt="PyPI version">\n  <img src="https://img.shields.io/badge/coverage-100%25-success"\n   height="20"\n   alt="Code Coverage">\n</div>\n\nThis library provides functions to change the casing convention of a string.\n\nSupported cases:\n\n- camelCase\n- dot.case\n- kebab-case\n- PascalCase\n- path/case\n- snake_case\n- Title Case\n- UPPER.DOT.CASE\n- UPPER-KEBAB-CASE\n- UPPER_SNAKE_CASE\n\n### Install\n\n```shell\npoetry add case-switcher\n```\n\n```shell\npip install case-switcher\n```\n\n### Demo\n\n```python\nimport caseswitcher\n\nsample = "avocado bagel-coffeeDONUTEclair_food.gravy"\n\ncaseswitcher.to_camel(sample)  # -> "avocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_dot(sample)  # -> "avocado.bagel.coffee.donut.eclair.food.gravy"\ncaseswitcher.to_kebab(sample)  # -> "avocado-bagel-coffee-donut-eclair-food-gravy"\ncaseswitcher.to_pascal(sample)  # -> "AvocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_path(sample)  # -> "avocado/bagel/coffee/donut/eclair/food/gravy"\ncaseswitcher.to_snake(sample)  # -> "avocado_bagel_coffee_donut_eclair_food_gravy"\ncaseswitcher.to_title(sample)  # -> "Avocado Bagel Coffee DONUT Eclair Food Gravy"\n# Deprecated, use `to_dot(sample).upper()` instead.\ncaseswitcher.to_upper_dot(sample)  # -> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"\n# Deprecated, use `to_kebab(sample).upper()` instead.\ncaseswitcher.to_upper_kebab(sample)  # -> "AVOCADO-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-GRAVY"\n# Deprecated, use `to_snake(sample).upper()` instead.\ncaseswitcher.to_upper_snake(sample)  # -> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY"\n```\n\n## Support The Developer\n\n<a href="https://www.buymeacoffee.com/mburkard" target="_blank">\n  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png"\n       width="217"\n       height="60"\n       alt="Buy Me A Coffee">\n</a>\n',
+    'long_description': '<div align=center>\n<!-- Title: -->\n  <h1>Case Switcher</h1>\n  <h3>Change the casing of a string.</h3>\n<!-- Labels: -->\n  <!-- First row: -->\n  <img src="https://img.shields.io/badge/license-MIT-green"\n   height="20"\n   alt="License: MIT">\n  <img src="https://img.shields.io/badge/code%20style-black-000000.svg"\n   height="20"\n   alt="Code style: black">\n  <img src="https://img.shields.io/pypi/v/case-switcher.svg"\n   height="20"\n   alt="PyPI version">\n  <img src="https://img.shields.io/badge/coverage-100%25-success"\n   height="20"\n   alt="Code Coverage">\n  <a href="https://www.codefactor.io/repository/github/matthew-burkard/case-switcher">\n    <img\n     src="https://www.codefactor.io/repository/github/matthew-burkard/case-switcher/badge"\n     alt="CodeFactor" />\n  </a>\n</div>\n\nThis library provides functions to change the casing convention of a string.\n\nSupported cases:\n\n- camelCase\n- dot.case\n- kebab-case\n- PascalCase\n- path/case\n- snake_case\n- Title Case\n- UPPER.DOT.CASE\n- UPPER-KEBAB-CASE\n- UPPER_SNAKE_CASE\n\n### Install\n\n```shell\npoetry add case-switcher\n```\n\n```shell\npip install case-switcher\n```\n\n### Demo\n\n```python\nimport caseswitcher\n\nsample = "avocado bagel-coffeeDONUTEclair_food.gravy"\n\ncaseswitcher.to_camel(sample)  # -> "avocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_dot(sample)  # -> "avocado.bagel.coffee.donut.eclair.food.gravy"\ncaseswitcher.to_kebab(sample)  # -> "avocado-bagel-coffee-donut-eclair-food-gravy"\ncaseswitcher.to_pascal(sample)  # -> "AvocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_path(sample)  # -> "avocado/bagel/coffee/donut/eclair/food/gravy"\ncaseswitcher.to_snake(sample)  # -> "avocado_bagel_coffee_donut_eclair_food_gravy"\ncaseswitcher.to_title(sample)  # -> "Avocado Bagel Coffee DONUT Eclair Food Gravy"\ncaseswitcher.to_upper_dot(sample)  # -> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"\ncaseswitcher.to_upper_kebab(sample)  # -> "AVOCADO-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-GRAVY"\ncaseswitcher.to_upper_snake(sample)  # -> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY"\n```\n',
     'author': 'Matthew Burkard',
     'author_email': 'matthewjburkard@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/mburkard/case-switcher',
     'py_modules': modules,
     'python_requires': '>=3.9,<4.0',
```

#### html2text {}

```diff
@@ -1,39 +1,38 @@
 # -*- coding: utf-8 -*- from setuptools import setup modules = \ ['__init__',
-'py'] setup_kwargs = { 'name': 'case-switcher', 'version': '1.3.13',
+'py'] setup_kwargs = { 'name': 'case-switcher', 'version': '1.3.4',
 'description': 'Library to change the casing of strings.', 'long_description':
 '
                                      \n\n
                           ****** Case Switcher ******
                                       \n
                    **** Change the casing of a string. ****
                                    \n\n \n
                     n height="20"\n alt="License: MIT">\n
                   n height="20"\n alt="Code style: black">\n
                     n height="20"\n alt="PyPI version">\n
-                    n height="20"\n alt="Code Coverage">\n
+  n height="20"\n alt="Code Coverage">\n \n_n_src="https://www.codefactor.io/
+  repository/github/matthew-burkard/case-switcher/badge"\n_alt="CodeFactor"_/
+                                     >\n\n
 \n\nThis library provides functions to change the casing convention of a
 string.\n\nSupported cases:\n\n- camelCase\n- dot.case\n- kebab-case\n-
 PascalCase\n- path/case\n- snake_case\n- Title Case\n- UPPER.DOT.CASE\n- UPPER-
 KEBAB-CASE\n- UPPER_SNAKE_CASE\n\n### Install\n\n```shell\npoetry add case-
 switcher\n```\n\n```shell\npip install case-switcher\n```\n\n###
 Demo\n\n```python\nimport caseswitcher\n\nsample = "avocado bagel-
 coffeeDONUTEclair_food.gravy"\n\ncaseswitcher.to_camel(sample) # -
 > "avocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_dot(sample) # -
 > "avocado.bagel.coffee.donut.eclair.food.gravy"\ncaseswitcher.to_kebab(sample)
 # -> "avocado-bagel-coffee-donut-eclair-food-gravy"\ncaseswitcher.to_pascal
 (sample) # -> "AvocadoBagelCoffeeDONUTEclairFoodGravy"\ncaseswitcher.to_path
 (sample) # -> "avocado/bagel/coffee/donut/eclair/food/
 gravy"\ncaseswitcher.to_snake(sample) # -
 > "avocado_bagel_coffee_donut_eclair_food_gravy"\ncaseswitcher.to_title(sample)
-# -> "Avocado Bagel Coffee DONUT Eclair Food Gravy"\n# Deprecated, use `to_dot
-(sample).upper()` instead.\ncaseswitcher.to_upper_dot(sample) # -
-> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"\n# Deprecated, use `to_kebab
-(sample).upper()` instead.\ncaseswitcher.to_upper_kebab(sample) # -> "AVOCADO-
-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-GRAVY"\n# Deprecated, use `to_snake
-(sample).upper()` instead.\ncaseswitcher.to_upper_snake(sample) # -
-> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY"\n```\n\n## Support The
-Developer\n\n\n_n_width="217"\n_height="60"\n_alt="Buy_Me_A_Coffee">\n\n',
-'author': 'Matthew Burkard', 'author_email': 'matthewjburkard@gmail.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://gitlab.com/
-mburkard/case-switcher', 'py_modules': modules, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+# -> "Avocado Bagel Coffee DONUT Eclair Food Gravy"\ncaseswitcher.to_upper_dot
+(sample) # -
+> "AVOCADO.BAGEL.COFFEE.DONUT.ECLAIR.FOOD.GRAVY"\ncaseswitcher.to_upper_kebab
+(sample) # -> "AVOCADO-BAGEL-COFFEE-DONUT-ECLAIR-FOOD-
+GRAVY"\ncaseswitcher.to_upper_snake(sample) # -
+> "AVOCADO_BAGEL_COFFEE_DONUT_ECLAIR_FOOD_GRAVY"\n```\n', 'author': 'Matthew
+Burkard', 'author_email': 'matthewjburkard@gmail.com', 'maintainer': None,
+'maintainer_email': None, 'url': 'https://gitlab.com/mburkard/case-switcher',
+'py_modules': modules, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

