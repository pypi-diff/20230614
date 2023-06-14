# Comparing `tmp/pygus-2.0.2.tar.gz` & `tmp/pygus-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-2.0.2.tar", max compression
+gzip compressed data, was "pygus-2.0.3.tar", max compression
```

## Comparing `pygus-2.0.2.tar` & `pygus-2.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.2/LICENSE
--rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.2/README-pypi.md
--rw-r--r--   0        0        0      161 2023-06-14 13:00:54.096939 pygus-2.0.2/pygus/__init__.py
--rw-r--r--   0        0        0      183 2023-06-14 13:00:54.097675 pygus-2.0.2/pygus/gus/__init__.py
--rw-r--r--   0        0        0    27311 2023-06-07 17:14:01.717670 pygus-2.0.2/pygus/gus/agents.py
--rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.2/pygus/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.2/pygus/gus/inputs/allometrics.json
--rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees.csv
--rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_1000.csv
--rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_100000.csv
--rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_200.csv
--rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_20000.csv
--rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.2/pygus/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.2/pygus/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.2/pygus/gus/inputs/trees.csv
--rw-r--r--   0        0        0    16148 2023-06-14 13:17:00.376677 pygus-2.0.2/pygus/gus/models.py
--rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.2/pygus/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     4210 2023-06-14 13:00:54.098664 pygus-2.0.2/pygus/gus/utilities.py
--rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.2/pygus/gus/weather.py
--rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.2/pygus/impacts/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.2/pygus/impacts/carbon.py
--rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.2/pygus/impacts/water.py
--rw-r--r--   0        0        0     1501 2023-06-14 13:17:21.173060 pygus-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.2/setup.py
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.3/LICENSE
+-rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.3/README-pypi.md
+-rw-r--r--   0        0        0      161 2023-06-14 13:00:54.096939 pygus-2.0.3/pygus/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-14 13:00:54.097675 pygus-2.0.3/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27311 2023-06-07 17:14:01.717670 pygus-2.0.3/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.3/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.3/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees.csv
+-rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_1000.csv
+-rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_100000.csv
+-rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_200.csv
+-rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_20000.csv
+-rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.3/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.3/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.3/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    16148 2023-06-14 13:17:00.376677 pygus-2.0.3/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.3/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     4210 2023-06-14 13:00:54.098664 pygus-2.0.3/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.3/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.3/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.3/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.3/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1501 2023-06-14 13:40:01.257695 pygus-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.3/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.3/PKG-INFO
```

### Comparing `pygus-2.0.2/LICENSE` & `pygus-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/README-pypi.md` & `pygus-2.0.3/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/agents.py` & `pygus-2.0.3/pygus/gus/agents.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/allometrics.py` & `pygus-2.0.3/pygus/gus/allometrics.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/allometrics.json` & `pygus-2.0.3/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees.csv` & `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_1000.csv` & `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_1000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_100000.csv` & `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_100000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_200.csv` & `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_200.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/amsterdam_all_trees_20000.csv` & `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_20000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/inputs/trees.csv` & `pygus-2.0.3/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/models.py` & `pygus-2.0.3/pygus/gus/models.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/outputs/trees_yearly.json` & `pygus-2.0.3/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/utilities.py` & `pygus-2.0.3/pygus/gus/utilities.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/gus/weather.py` & `pygus-2.0.3/pygus/gus/weather.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/impacts/carbon.py` & `pygus-2.0.3/pygus/impacts/carbon.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pygus/impacts/water.py` & `pygus-2.0.3/pygus/impacts/water.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.2/pyproject.toml` & `pygus-2.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGUS"
-version = "2.0.2"
+version = "2.0.3"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
```

### Comparing `pygus-2.0.2/setup.py` & `pygus-2.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'termcolor>=2.1.1,<3.0.0',
  'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '2.0.2',
+    'version': '2.0.3',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-2.0.2/PKG-INFO` & `pygus-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 2.0.2
+Version: 2.0.3
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
```

