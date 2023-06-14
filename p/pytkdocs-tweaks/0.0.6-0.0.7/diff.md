# Comparing `tmp/pytkdocs_tweaks-0.0.6.tar.gz` & `tmp/pytkdocs_tweaks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytkdocs_tweaks-0.0.6.tar", last modified: Tue Jul 12 14:41:49 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytkdocs_tweaks-0.0.6.tar` & `pytkdocs_tweaks-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-x---   0 kidger   (1042332) primarygroup (89939)        0 2022-07-12 14:41:49.520883 pytkdocs_tweaks-0.0.6/
--rw-r-----   0 kidger   (1042332) primarygroup (89939)    11357 2022-07-12 14:27:21.000000 pytkdocs_tweaks-0.0.6/LICENSE
--rw-r-----   0 kidger   (1042332) primarygroup (89939)       16 2022-07-12 14:27:21.000000 pytkdocs_tweaks-0.0.6/MANIFEST.in
--rw-r-----   0 kidger   (1042332) primarygroup (89939)     3309 2022-07-12 14:41:49.520883 pytkdocs_tweaks-0.0.6/PKG-INFO
--rw-r-----   0 kidger   (1042332) primarygroup (89939)     2614 2022-07-12 14:27:21.000000 pytkdocs_tweaks-0.0.6/README.md
-drwxr-x---   0 kidger   (1042332) primarygroup (89939)        0 2022-07-12 14:41:49.520883 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks/
--rw-r-----   0 kidger   (1042332) primarygroup (89939)     9002 2022-07-12 14:35:46.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks/__init__.py
-drwxr-x---   0 kidger   (1042332) primarygroup (89939)        0 2022-07-12 14:41:49.520883 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/
--rw-r-----   0 kidger   (1042332) primarygroup (89939)     3309 2022-07-12 14:41:48.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/PKG-INFO
--rw-r-----   0 kidger   (1042332) primarygroup (89939)      298 2022-07-12 14:41:49.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/SOURCES.txt
--rw-r-----   0 kidger   (1042332) primarygroup (89939)        1 2022-07-12 14:41:48.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/dependency_links.txt
--rw-r-----   0 kidger   (1042332) primarygroup (89939)        1 2022-07-12 14:30:55.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/not-zip-safe
--rw-r-----   0 kidger   (1042332) primarygroup (89939)       17 2022-07-12 14:41:49.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/requires.txt
--rw-r-----   0 kidger   (1042332) primarygroup (89939)       16 2022-07-12 14:41:49.000000 pytkdocs_tweaks-0.0.6/pytkdocs_tweaks.egg-info/top_level.txt
--rw-r-----   0 kidger   (1042332) primarygroup (89939)       38 2022-07-12 14:41:49.520883 pytkdocs_tweaks-0.0.6/setup.cfg
--rw-r-----   0 kidger   (1042332) primarygroup (89939)     1537 2022-07-12 14:27:21.000000 pytkdocs_tweaks-0.0.6/setup.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/pytkdocs_tweaks/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/README.md
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    16270 2020-02-02 00:00:00.000000 pytkdocs_tweaks-0.0.7/PKG-INFO
```

### Comparing `pytkdocs_tweaks-0.0.6/LICENSE` & `pytkdocs_tweaks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytkdocs_tweaks-0.0.6/PKG-INFO` & `pytkdocs_tweaks-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pytkdocs_tweaks
-Version: 0.0.6
-Summary: Some custom tweaks to the results produced by pytkdocs (part of mkdocstrings).
-Home-page: https://github.com/patrick-kidger/pytkdocs_tweaks
-Author: Patrick Kidger
-Author-email: contact@kidger.site
-Maintainer: Patrick Kidger
-Maintainer-email: contact@kidger.site
-License: Apache-2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pytkdocs_tweaks
 
 Some custom tweaks for [pytkdocs](https://github.com/mkdocstrings/pytkdocs).
 
 _For use as part of the documentation-generation-for-Python stack that comprises [mkdocs](https://www.mkdocs.org/), [mkdocs-material](https://github.com/squidfunk/mkdocs-material), [mkdocstrings](https://github.com/mkdocstrings/mkdocstrings/) and [pytkdocs](https://github.com/mkdocstrings/pytkdocs)._
 
 - Types are ubiquitously displayed in the way you import them: `package.Foo` (rather than being a mix of where they're defined: `package.subpackage.foomodule.Foo` or just their name: `Foo`).
@@ -59,9 +39,7 @@
                     - pytkdocs_tweaks.main()
                 selection:
                     inherited_members: true  # allow looking up inherited members
                 rendering:
                     show_root_heading: true    #
                     show_root_full_path: true  # have e.g. `package.Foo` display correctly, rather than e.g. just `Foo`.
 ```
-
-
```

### Comparing `pytkdocs_tweaks-0.0.6/pytkdocs_tweaks/__init__.py` & `pytkdocs_tweaks-0.0.7/pytkdocs_tweaks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse
 import importlib
 import inspect
 import json
 import pathlib
-import sys
 import traceback
 import typing
 import warnings
 from typing import Any, Dict
 
 import pytkdocs
 import pytkdocs.cli
@@ -85,19 +84,25 @@
     else:
         for parameter in signature["parameters"]:
             if "annotation" in parameter:
                 for p in cache:
                     parameter["annotation"] = parameter["annotation"].replace(
                         p, p.rsplit(".", 1)[1]
                     )
+                parameter["annotation"] = parameter["annotation"].replace(
+                    "collections.abc.", ""
+                )
         if "return_annotation" in signature:
             for p in cache:
                 signature["return_annotation"] = signature["return_annotation"].replace(
                     p, p.rsplit(".", 1)[1]
                 )
+            signature["return_annotation"] = signature["return_annotation"].replace(
+                "collections.abc.", ""
+            )
 
     if "bases" in data:
         # Find those base classes which are part of our public documentation.
         # This is used for a couple of things lower down.
         bases = _find_public_bases(data["bases"], cache)
 
         # Display base classes in "import form" not "full form".
@@ -151,14 +156,15 @@
                 new_docstring = f"Inherited from [`{cache[base]}.{data['name']}`][]."
                 break
         else:
             _base_obj = _str_to_obj(data["path"])
             if isinstance(_base_obj, property):
                 # Property objects don't inherit module or qualname
                 _base_obj = _base_obj.fget
+            assert _base_obj is not None
             _base_path = _base_obj.__module__ + "." + _base_obj.__qualname__
             _base_config = {"objects": [{"path": _base_path}]}
             _base_result = pytkdocs.cli.process_config(_base_config)
             new_docstring = _base_result["objects"][0]["docstring"]
     if bases is not None:
         for base in bases:
             _base_obj = _str_to_obj(base)
@@ -246,12 +252,14 @@
             out["default"] = f"<function {parameter.default.__name__}>"
         return out
 
     pytkdocs.serializer.serialize_signature_parameter = serialize_signature_parameter
 
     # By default pytkdocs has some really weird behaviour in which the docstring for
     # inherited magic methods are removed. This removes that behaviour.
-    pytkdocs.loader.RE_SPECIAL = argparse.Namespace(match=lambda _: False)
+    pytkdocs.loader.RE_SPECIAL = argparse.Namespace(  # pyright: ignore
+        match=lambda _: False
+    )
 
     # Set a flag to say we're generating documentation, which the library can use to
     # customise how its types are displayed.
-    typing.GENERATING_DOCUMENTATION = True
+    typing.GENERATING_DOCUMENTATION = True  # pyright: ignore
```

