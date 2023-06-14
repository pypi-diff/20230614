# Comparing `tmp/python_urbandict-0.2.5.tar.gz` & `tmp/python_urbandict-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.2.5.tar", max compression
+gzip compressed data, was "python_urbandict-0.2.6.tar", max compression
```

## Comparing `python_urbandict-0.2.5.tar` & `python_urbandict-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1066 2022-12-20 21:06:26.944216 python_urbandict-0.2.5/LICENSE
--rw-r--r--   0        0        0     2325 2022-12-20 21:06:26.944216 python_urbandict-0.2.5/README.md
--rw-r--r--   0        0        0      947 2022-12-20 21:06:26.944216 python_urbandict-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       77 2022-12-20 21:06:26.944216 python_urbandict-0.2.5/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1018 2022-12-20 21:06:26.944216 python_urbandict-0.2.5/pyurbandict/parse.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 python_urbandict-0.2.5/setup.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 python_urbandict-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2325 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/README.md
+-rw-r--r--   0        0        0      923 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-14 19:19:50.924797 python_urbandict-0.2.6/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 python_urbandict-0.2.6/PKG-INFO
```

### Comparing `python_urbandict-0.2.5/LICENSE` & `python_urbandict-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.5/README.md` & `python_urbandict-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.5/pyproject.toml` & `python_urbandict-0.2.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.2.5"
+version = "0.2.6"
 description = "Python wrapper for the Urban Dictionary API."
-authors = ["Vitaman02"]
+authors = ["atbuy"]
 license = "MIT"
-homepage = "https://github.com/Vitaman02/pyurbandict"
-repository = "https://github.com/Vitaman02/pyurbandict"
+homepage = "https://github.com/atbuy/pyurbandict"
+repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
 readme = "README.md"
 packages = [
     {include = "pyurbandict"}
 ]
 
@@ -24,14 +24,14 @@
 black = "^22.6.0"
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/Vitaman02/pyurbandict/issues"
-"Source Code" = "https://github.com/Vitaman02/pyurbandict"
-"CI/CD" = "https://github.com/Vitaman02/pyurbandict/actions"
+"Bug Tracker" = "https://github.com/atbuy/pyurbandict/issues"
+"Source Code" = "https://github.com/atbuy/pyurbandict"
+"CI/CD" = "https://github.com/atbuy/pyurbandict/actions"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_urbandict-0.2.5/pyurbandict/parse.py` & `python_urbandict-0.2.6/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.2.5/setup.py` & `python_urbandict-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-urbandict
+Version: 0.2.6
+Summary: Python wrapper for the Urban Dictionary API.
+Home-page: https://github.com/atbuy/pyurbandict
+License: MIT
+Keywords: urban,dictionary,api,wrapper,python
+Author: atbuy
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/atbuy/pyurbandict/issues
+Project-URL: CI/CD, https://github.com/atbuy/pyurbandict/actions
+Project-URL: Repository, https://github.com/atbuy/pyurbandict
+Project-URL: Source Code, https://github.com/atbuy/pyurbandict
+Description-Content-Type: text/markdown
+
+# python-urbandict
+
+[![version](https://img.shields.io/pypi/v/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
+[![versions](https://img.shields.io/pypi/pyversions/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)
+[![Python package](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml/badge.svg)](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml)
+[![codecov](https://codecov.io/gh/Vitaman02/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)](https://codecov.io/gh/Vitaman02/pyurbandict)
+
+This is a python project, that fetches definitions of words from urban dictionary's public API.
+
+Future additions. PRs are always welcome :)
+* Calculate ratio of `thumbs_up` and `thumbs_down` and decide the probability of a correct definition.
+
+# Installation
+
+*Python 3.9 or higher is required*
+
+To install the library you can use the following command:
+
+```
+# Linux/MacOS
+python3 -m pip install --upgrade python-urbandict
+
+# Windows
+py -3 -m pip install --upgrade python-urbandict
+```
+
+Or just try:
+
+```
+pip install python-urbandict
+```
+
+# Quick Example
+
+You can create an instance of the `UrbanDict` class and pass a word to it. After that you can use the `search` method that will retrieve the definitions from UrbanDictionary.
+If you want to you can also leave the word attribute empty, in which case a random word is selected by UrbanDictionary.
+
+```python
+from pyurbandict import UrbanDict
+
+word = UrbanDict("python")
+results = word.search()
+print(results[0])
+
+>>> Definition(
+    word='python',
+    definition='The best thing to happen to [Computer Science] students in a data and [file] structures or [algorithms] class.',
+    example='Joe: "Man...I spent a week coding that [algorithm] in C."\r\nMoe: "I got it [done in one] evening with [Python]. It works great."\r\nJoe: "Say, what? Where can I download that?"',
+    author='TheNextBillGates',
+    thumbs_up=243,
+    thumbs_down=71,
+    sound_urls=['https://api.twilio.com/2008-08-01/Accounts/ACd09691b82112e4b26fce156d7c01d0ed/Recordings/RE7065a4ef810937cc16ae2b6e4b54b67d'],
+    written_on='2010-03-24T05:24:18.000Z',
+    permalink='http://python.urbanup.com/4826760',
+    defid=4826760,
+    current_vote=''
+)
+```
 
-packages = \
-['pyurbandict']
+# Links
+* [PyPi](https://pypi.org/project/python-urbandict/)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'python-urbandict',
-    'version': '0.2.5',
-    'description': 'Python wrapper for the Urban Dictionary API.',
-    'long_description': '# python-urbandict\n\n[![version](https://img.shields.io/pypi/v/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)\n[![versions](https://img.shields.io/pypi/pyversions/python-urbandict.svg)](https://pypi.org/project/python-urbandict/)\n[![Python package](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml/badge.svg)](https://github.com/Vitaman02/pyurbandict/actions/workflows/python-package.yml)\n[![codecov](https://codecov.io/gh/Vitaman02/pyurbandict/branch/main/graph/badge.svg?token=A244XBTUVH)](https://codecov.io/gh/Vitaman02/pyurbandict)\n\nThis is a python project, that fetches definitions of words from urban dictionary\'s public API.\n\nFuture additions. PRs are always welcome :)\n* Calculate ratio of `thumbs_up` and `thumbs_down` and decide the probability of a correct definition.\n\n# Installation\n\n*Python 3.9 or higher is required*\n\nTo install the library you can use the following command:\n\n```\n# Linux/MacOS\npython3 -m pip install --upgrade python-urbandict\n\n# Windows\npy -3 -m pip install --upgrade python-urbandict\n```\n\nOr just try:\n\n```\npip install python-urbandict\n```\n\n# Quick Example\n\nYou can create an instance of the `UrbanDict` class and pass a word to it. After that you can use the `search` method that will retrieve the definitions from UrbanDictionary.\nIf you want to you can also leave the word attribute empty, in which case a random word is selected by UrbanDictionary.\n\n```python\nfrom pyurbandict import UrbanDict\n\nword = UrbanDict("python")\nresults = word.search()\nprint(results[0])\n\n>>> Definition(\n    word=\'python\',\n    definition=\'The best thing to happen to [Computer Science] students in a data and [file] structures or [algorithms] class.\',\n    example=\'Joe: "Man...I spent a week coding that [algorithm] in C."\\r\\nMoe: "I got it [done in one] evening with [Python]. It works great."\\r\\nJoe: "Say, what? Where can I download that?"\',\n    author=\'TheNextBillGates\',\n    thumbs_up=243,\n    thumbs_down=71,\n    sound_urls=[\'https://api.twilio.com/2008-08-01/Accounts/ACd09691b82112e4b26fce156d7c01d0ed/Recordings/RE7065a4ef810937cc16ae2b6e4b54b67d\'],\n    written_on=\'2010-03-24T05:24:18.000Z\',\n    permalink=\'http://python.urbanup.com/4826760\',\n    defid=4826760,\n    current_vote=\'\'\n)\n```\n\n# Links\n* [PyPi](https://pypi.org/project/python-urbandict/)\n',
-    'author': 'Vitaman02',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Vitaman02/pyurbandict',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

