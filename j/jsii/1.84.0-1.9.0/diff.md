# Comparing `tmp/jsii-1.84.0.tar.gz` & `tmp/jsii-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python/jsii-1.84.0.tar", last modified: Wed Jun 14 08:38:10 2023, max compression
+gzip compressed data, was "dist/python/jsii-1.9.0.tar", last modified: Fri Jul 17 05:14:53 2020, max compression
```

## Comparing `jsii-1.84.0.tar` & `jsii-1.9.0.tar`

### file list

```diff
@@ -1,48 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/
--rw-rw-r--   0 root         (0) root         (0)    11386 2023-06-14 08:10:58.000000 jsii-1.84.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       88 2023-06-14 08:10:58.000000 jsii-1.84.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)       77 2023-06-14 08:10:58.000000 jsii-1.84.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    72731 2023-06-14 08:38:10.000000 jsii-1.84.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    71709 2023-06-14 08:37:41.000000 jsii-1.84.0/README.md
--rw-rw-r--   0 root         (0) root         (0)      341 2023-06-14 08:10:58.000000 jsii-1.84.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 08:38:10.000000 jsii-1.84.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1803 2023-06-14 08:10:58.000000 jsii-1.84.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii/
--rw-rw-r--   0 root         (0) root         (0)     1568 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      348 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/__meta__.py
--rw-rw-r--   0 root         (0) root         (0)      107 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii/_embedded/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_embedded/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii/_embedded/jsii/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_embedded/jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   157127 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js
--rw-r--r--   0 root         (0) root         (0)   244005 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_embedded/jsii/bin__jsii-runtime.js.map
--rw-r--r--   0 root         (0) root         (0)   808766 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_embedded/jsii/lib__program.js
--rw-r--r--   0 root         (0) root         (0)  1186245 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_embedded/jsii/lib__program.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii/_kernel/
--rw-rw-r--   0 root         (0) root         (0)    17033 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_kernel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii/_kernel/providers/
--rw-rw-r--   0 root         (0) root         (0)      116 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_kernel/providers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2931 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_kernel/providers/base.py
--rw-rw-r--   0 root         (0) root         (0)    14293 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_kernel/providers/process.py
--rw-rw-r--   0 root         (0) root         (0)     4912 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_kernel/types.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-14 08:37:44.000000 jsii-1.84.0/src/jsii/_metadata.json
--rw-rw-r--   0 root         (0) root         (0)     6983 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_reference_map.py
--rw-rw-r--   0 root         (0) root         (0)     5405 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_runtime.py
--rw-rw-r--   0 root         (0) root         (0)      584 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/_utils.py
--rw-rw-r--   0 root         (0) root         (0)       96 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/compat.py
--rw-rw-r--   0 root         (0) root         (0)      387 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/errors.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/py.typed
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-06-14 08:10:58.000000 jsii-1.84.0/src/jsii/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/
--rw-r--r--   0 root         (0) root         (0)    72731 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 08:38:10.000000 jsii-1.84.0/src/jsii.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:38:10.000000 jsii-1.84.0/tests/
--rw-rw-r--   0 root         (0) root         (0)    38976 2023-06-14 08:10:58.000000 jsii-1.84.0/tests/test_compliance.py
--rw-rw-r--   0 root         (0) root         (0)     3978 2023-06-14 08:10:58.000000 jsii-1.84.0/tests/test_invoke_bin.py
--rw-rw-r--   0 root         (0) root         (0)     2316 2023-06-14 08:10:58.000000 jsii-1.84.0/tests/test_python.py
--rw-rw-r--   0 root         (0) root         (0)     8225 2023-06-14 08:10:58.000000 jsii-1.84.0/tests/test_runtime_type_checking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/
+-rw-rw-r--   0 root         (0) root         (0)    11386 2020-07-17 05:02:34.000000 jsii-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       88 2020-07-17 05:02:34.000000 jsii-1.9.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)       77 2020-07-17 05:02:34.000000 jsii-1.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15018 2020-07-17 05:14:53.000000 jsii-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11231 2020-07-17 05:14:39.000000 jsii-1.9.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       50 2020-07-17 05:02:34.000000 jsii-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2020-07-17 05:14:53.000000 jsii-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1578 2020-07-17 05:02:34.000000 jsii-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii/
+-rw-rw-r--   0 root         (0) root         (0)     1177 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      329 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/__meta__.py
+-rw-rw-r--   0 root         (0) root         (0)      202 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii/_embedded/
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_embedded/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii/_embedded/jsii/
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_embedded/jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431167 2020-07-17 05:13:48.000000 jsii-1.9.0/src/jsii/_embedded/jsii/jsii-runtime.js
+-rw-r--r--   0 root         (0) root         (0)   555676 2020-07-17 05:13:48.000000 jsii-1.9.0/src/jsii/_embedded/jsii/jsii-runtime.js.map
+-rw-r--r--   0 root         (0) root         (0)    48693 2020-07-17 05:13:48.000000 jsii-1.9.0/src/jsii/_embedded/jsii/mappings.wasm
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii/_kernel/
+-rw-rw-r--   0 root         (0) root         (0)    13734 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_kernel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii/_kernel/providers/
+-rw-rw-r--   0 root         (0) root         (0)      160 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_kernel/providers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2551 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_kernel/providers/base.py
+-rw-rw-r--   0 root         (0) root         (0)    13021 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_kernel/providers/process.py
+-rw-rw-r--   0 root         (0) root         (0)     4614 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_kernel/types.py
+-rw-r--r--   0 root         (0) root         (0)      322 2020-07-17 05:14:39.000000 jsii-1.9.0/src/jsii/_metadata.json
+-rw-rw-r--   0 root         (0) root         (0)     7433 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_reference_map.py
+-rw-rw-r--   0 root         (0) root         (0)     3918 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_runtime.py
+-rw-rw-r--   0 root         (0) root         (0)      571 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/_utils.py
+-rw-rw-r--   0 root         (0) root         (0)       96 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/compat.py
+-rw-rw-r--   0 root         (0) root         (0)      255 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/errors.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/py.typed
+-rw-rw-r--   0 root         (0) root         (0)      942 2020-07-17 05:02:34.000000 jsii-1.9.0/src/jsii/python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15018 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      803 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2020-07-17 05:14:53.000000 jsii-1.9.0/src/jsii.egg-info/top_level.txt
```

### Comparing `jsii-1.84.0/LICENSE` & `jsii-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsii-1.84.0/setup.py` & `jsii-1.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,56 +2,64 @@
 import setuptools
 
 
 with open("src/jsii/_metadata.json") as fp:
     metadata = json.load(fp)
 
 
-with open("README.md", encoding="utf8") as fp:
+with open("README.md") as fp:
     long_description = fp.read()
 
 
 setuptools.setup(
     name="jsii",
     version=metadata["version"],
     license=metadata["license"],
+
     url=metadata["homepage"],
     project_urls={
         "Bug Tracker": metadata["bugs"],
         "Source": metadata["repository"],
     },
+
     description=metadata["description"],
     long_description=long_description,
     long_description_content_type="text/markdown",
+
     author=metadata["author"],
+
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     package_data={
         "jsii": ["_metadata.json", "py.typed"],
-        "jsii._embedded.jsii": ["*.js", "*.js.map"],
+        "jsii._embedded.jsii": ["*.js", "*.js.map", "*.wasm"],
     },
+
     install_requires=[
-        "attrs>=21.2,<24.0",
-        "cattrs>=1.8,<23.2",
-        "importlib_resources>=5.2.0",
-        "publication>=0.0.3",  # This is used by all generated code.
-        "typeguard~=2.13.3",  # This is used by all generated code.
+        "attrs~=19.3.0",
+        "cattrs~=1.0.0",
+        "importlib_resources ; python_version < '3.7'",
         "python-dateutil",
-        "typing_extensions>=3.7,<5.0",
+        "typing_extensions~=3.7.4",
     ],
-    python_requires="~=3.7",
+
+    python_requires=">=3.6",
+
     classifiers=[
         "Development Status :: 5 - Production/Stable",
+
         "Intended Audience :: Developers",
+
         "License :: OSI Approved :: Apache Software License",
+
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
+
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
+
         "Typing :: Typed",
     ],
 )
```

### Comparing `jsii-1.84.0/src/jsii/_kernel/__init__.py` & `jsii-1.9.0/src/jsii/_kernel/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,289 +1,205 @@
 import datetime
 import inspect
 import itertools
 from types import FunctionType, MethodType, BuiltinFunctionType, LambdaType
 
-from typing import Callable, cast, Any, List, Optional, Sequence, Type
+from typing import Any, List, Optional, Type, Union
 
 import functools
 
 import attr
-import enum
 
-from ..errors import JSIIError
-from .. import _reference_map
-from .._utils import Singleton
-from .providers import BaseProvider, ProcessProvider
-from .types import (
+from jsii.errors import JSIIError
+from jsii import _reference_map
+from jsii._utils import Singleton
+from jsii._kernel.providers import BaseProvider, ProcessProvider
+from jsii._kernel.types import JSClass, Referenceable
+from jsii._kernel.types import Callback
+from jsii._kernel.types import (
     EnumRef,
     LoadRequest,
     BeginRequest,
-    BeginResponse,
-    Callback,
     CallbacksRequest,
-    CompleteRequest,
-    CompleteRequest,
-    CompleteResponse,
     CreateRequest,
     CreateResponse,
+    CompleteRequest,
     DeleteRequest,
     EndRequest,
-    EnumRef,
     GetRequest,
-    GetResponse,
     InvokeRequest,
-    InvokeResponse,
-    GetScriptCommandRequest,
-    GetScriptCommandResponse,
-    InvokeScriptRequest,
-    InvokeScriptResponse,
-    KernelResponse,
-    LoadRequest,
-    ObjRef,
-    Override,
     SetRequest,
-    SetResponse,
     StaticGetRequest,
     StaticInvokeRequest,
     StaticSetRequest,
     StatsRequest,
+    ObjRef,
+    Override,
+    CompleteRequest,
+    CompleteResponse,
+    GetResponse,
+    SetResponse,
+    InvokeResponse,
+    KernelResponse,
+    BeginResponse
 )
-from .._utils import Singleton
 
 
 _nothing = object()
 
 
 class Object:
     __jsii_type__ = "Object"
 
 
-def _get_overides(klass: Type, obj: Any) -> List[Override]:
+def _get_overides(klass: JSClass, obj: Any) -> List[Override]:
     overrides: List[Override] = []
 
-    # We need to inspect each item in the MRO, until we get to our Type, at that
+    # We need to inspect each item in the MRO, until we get to our JSClass, at that
     # point we'll bail, because those methods are not the overriden methods, but the
     # "real" methods.
-    jsii_name = getattr(klass, "__jsii_type__", "Object")
-    jsii_classes = [
-        next(
-            (
-                m
-                for m in type(obj).mro()
-                if getattr(m, "__jsii_declared_type__", None) == jsii_name
-            ),
-            Object,
-        )
-    ] + list(
+    jsii_classes = [klass] + list(
         itertools.chain.from_iterable(
             (getattr(m, "__jsii_ifaces__", []) for m in type(obj).mro())
         )
     )
     for mro_klass in type(obj).mro():
-        if getattr(mro_klass, "__jsii_declared_type__", None) is not None:
-            # There is a jsii declared type, so we reached a "well known" object,
-            # and nothing from now on is an override.
+        if mro_klass is klass and getattr(mro_klass, "__jsii_type__", "Object") is not None:
             break
-        if mro_klass is Object or mro_klass is object:
+        if mro_klass is Object:
             break
 
         for name, item in mro_klass.__dict__.items():
-            # Ignore all "special" members (name starting with __)...
-            if name.startswith("__"):
-                continue
-
             # We're only interested in things that also exist on the JSII class or
             # interfaces, and which are themselves, jsii members.
             for jsii_class in jsii_classes:
                 original = getattr(jsii_class, name, _nothing)
                 if original is not _nothing:
                     if inspect.isfunction(item) and hasattr(original, "__jsii_name__"):
-                        if any(
-                            entry.method == cast(Any, original).__jsii_name__
-                            for entry in overrides
-                        ):
+                        if any(entry.method == original.__jsii_name__ for entry in overrides):
                             # Don't re-register an override we already discovered through a previous type
                             continue
                         overrides.append(
-                            Override(
-                                method=cast(Any, original).__jsii_name__, cookie=name
-                            )
+                            Override(method=original.__jsii_name__, cookie=name)
                         )
-                        break
                     elif inspect.isdatadescriptor(item) and hasattr(
                         getattr(original, "fget", None), "__jsii_name__"
                     ):
-                        if any(
-                            entry.property == cast(Any, original).fget.__jsii_name__
-                            for entry in overrides
-                        ):
+                        if any(entry.property == original.fget.__jsii_name__ for entry in overrides):
                             # Don't re-register an override we already discovered through a previous type
                             continue
                         overrides.append(
-                            Override(
-                                property=cast(Any, original).fget.__jsii_name__,
-                                cookie=name,
-                            )
+                            Override(property=original.fget.__jsii_name__, cookie=name)
                         )
-                        break
 
     return overrides
 
 
-def _recursize_dereference(kernel: "Kernel", d: Any) -> Any:
+def _recursize_dereference(kernel, d):
     if isinstance(d, dict):
         return {k: _recursize_dereference(kernel, v) for k, v in d.items()}
     elif isinstance(d, list):
         return [_recursize_dereference(kernel, i) for i in d]
     elif isinstance(d, ObjRef):
         return _reference_map.resolve_reference(kernel, d)
     elif isinstance(d, EnumRef):
         return _recursize_dereference(kernel, d.ref)(d.member)
     else:
         return d
 
 
-def _dereferenced(fn: Callable) -> Callable:
+def _dereferenced(fn):
     @functools.wraps(fn)
-    def wrapped(kernel: "Kernel", *args: Any, **kwargs: Any):
+    def wrapped(kernel, *args, **kwargs):
         return _recursize_dereference(kernel, fn(kernel, *args, **kwargs))
 
     return wrapped
 
 
 # We need to recurse through our data structure and look for anything that the JSII
 # doesn't natively handle. These items will be created as "Object" types in the JSII.
-def _make_reference_for_native(kernel: "Kernel", d: Any) -> Any:
+def _make_reference_for_native(kernel, d):
     if isinstance(d, dict):
-        return {
-            "$jsii.map": {
-                k: _make_reference_for_native(kernel, v) for k, v in d.items()
-            }
-        }
-
+        return {"$jsii.map": {k: _make_reference_for_native(kernel, v) for k, v in d.items()}}
     elif isinstance(d, list):
         return [_make_reference_for_native(kernel, i) for i in d]
 
     if getattr(d, "__jsii_type__", None) is not None:
-        typeFqn = getattr(d, "__jsii_type__")
-
-        if isinstance(d, enum.Enum):
-            return {"$jsii.enum": f"{typeFqn}/{d.value}"}
-
         # Ugly delayed import here because I can't solve the cyclic
         # package dependency right now :(.
-        from .._runtime import python_jsii_mapping
+        from jsii._runtime import python_jsii_mapping
 
+        typeFqn = getattr(d, "__jsii_type__")
         mapping = python_jsii_mapping(d)
-        if mapping is not None:  # This means we are handling a data_type (aka Struct)
+        if mapping: # This means we are handling a data_type (aka Struct)
             return {
                 "$jsii.struct": {
                     "fqn": typeFqn,
                     "data": {
-                        jsii_name: _make_reference_for_native(
-                            kernel, getattr(d, python_name)
-                        )
-                        for python_name, jsii_name in mapping.items()
-                    },
+                        jsii_name: _make_reference_for_native(kernel, getattr(d, python_name)) for python_name, jsii_name in mapping.items()
+                    }
                 }
             }
         return d
-
     elif isinstance(d, (int, type(None), str, float, bool, datetime.datetime)):
         return d
-
     elif isinstance(d, (FunctionType, MethodType, BuiltinFunctionType, LambdaType)):
         # Whether a given object is a function-like object.
         # We won't use iscallable() since objects may implement __call__()
         # but we still want to serialize them as normal.
-        raise JSIIError(
-            "Cannot pass function as argument here (did you mean to call this function?): %r"
-            % d
-        )
-
+        raise JSIIError("Cannot pass function as argument here (did you mean to call this function?): %r" % d)
     else:
         kernel.create(d.__class__, d)
         _reference_map.register_reference(d)
         return d
 
 
-def _handle_callback(kernel: "Kernel", callback: Callback) -> Any:
+def _handle_callback(kernel, callback):
     # need to handle get, set requests here as well as invoke requests
     if callback.invoke:
         obj = _reference_map.resolve_id(callback.invoke.objref.ref)
         method = getattr(obj, callback.cookie)
-        hydrated_args = [
-            _recursize_dereference(kernel, a) for a in callback.invoke.args or []
-        ]
-
-        # If keyword arguments are accepted, we may need to turn a struct into keywords...
-        kwargs = {}  # No keyword arguments by default
-        params = inspect.signature(method).parameters
-        params_kwargs = [
-            name
-            for (name, param) in params.items()
-            if param.kind == inspect.Parameter.KEYWORD_ONLY
-        ]
-        if len(params_kwargs) > 0:
-            params_pos_count = len(
-                [
-                    param
-                    for param in params.values()
-                    if param.kind == inspect.Parameter.POSITIONAL_OR_KEYWORD
-                    or param.kind == inspect.Parameter.POSITIONAL_ONLY
-                ]
-            )
-            if len(hydrated_args) > params_pos_count:
-                struct = hydrated_args.pop()
-                kwargs = {
-                    name: getattr(struct, name)
-                    for name in params_kwargs
-                    if hasattr(struct, name)
-                }
-
-        return method(*hydrated_args, **kwargs)
+        hydrated_args = [_recursize_dereference(kernel, a) for a in callback.invoke.args]
+        return method(*hydrated_args)
     elif callback.get:
         obj = _reference_map.resolve_id(callback.get.objref.ref)
         return getattr(obj, callback.cookie)
     elif callback.set:
         obj = _reference_map.resolve_id(callback.set.objref.ref)
         hydrated_value = _recursize_dereference(kernel, callback.set.value)
         return setattr(obj, callback.cookie, hydrated_value)
     else:
         raise JSIIError("Callback does not contain invoke|get|set")
 
 
-def _callback_till_result(
-    kernel: "Kernel", response: Callback, response_type: Type[KernelResponse]
-) -> Any:
+def _callback_till_result(kernel, response: Callback, response_type: Type[KernelResponse]) -> Any:
     while isinstance(response, Callback):
         try:
             result = _handle_callback(kernel, response)
         except Exception as exc:
-            response = kernel.sync_complete(
-                response.cbid, str(exc), None, response_type
-            )
+            response = kernel.sync_complete(response.cbid, str(exc), None, response_type)
         else:
             response = kernel.sync_complete(response.cbid, None, result, response_type)
 
     if isinstance(response, InvokeResponse):
         return response.result
     elif isinstance(response, GetResponse):
         return response.value
     else:
         return response
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Statistics:
+
     object_count: int
 
 
 class Kernel(metaclass=Singleton):
+
     # This class translates between the Pythonic interface for the kernel, and the
     # Kernel Provider interface that maps more directly to the JSII Kernel interface.
     # It currently only supports the idea of a process kernel provider, however it
     # should be possible to move to other providers in the future.
 
     # TODO: We don't currently have any error handling, but we need to. This should
     #       probably live at the provider layer though, maybe with something catching
@@ -294,109 +210,82 @@
         self.provider = provider_class()
 
     # TODO: Do we want to return anything from this method? Is the return value useful
     #       to anyone?
     def load(self, name: str, version: str, tarball: str) -> None:
         self.provider.load(LoadRequest(name=name, version=version, tarball=tarball))
 
-    def getBinScriptCommand(
-        self, pkgname: str, script: str, args: Optional[Sequence[str]] = None
-    ) -> GetScriptCommandResponse:
-        if args is None:
-            args = []
-
-        return self.provider.getScriptCommand(
-            GetScriptCommandRequest(
-                assembly=pkgname,
-                script=script,
-                args=_make_reference_for_native(self, args),
-            )
-        )
-
-    def invokeBinScript(
-        self, pkgname: str, script: str, args: Optional[Sequence[str]] = None
-    ) -> InvokeScriptResponse:
-        if args is None:
-            args = []
-
-        return self.provider.invokeBinScript(
-            InvokeScriptRequest(
-                assembly=pkgname,
-                script=script,
-                args=_make_reference_for_native(self, args),
-            )
-        )
-
     # TODO: Is there a way to say that obj has to be an instance of klass?
-    def create(self, klass: Type, obj: Any, args: Optional[List[Any]] = None) -> ObjRef:
+    def create(
+        self, klass: JSClass, obj: Any, args: Optional[List[Any]] = None
+    ) -> ObjRef:
         if args is None:
             args = []
 
         response = self.provider.create(
             CreateRequest(
                 fqn=klass.__jsii_type__ or "Object",
                 args=_make_reference_for_native(self, args),
                 overrides=_get_overides(klass, obj),
-                interfaces=[
-                    iface.__jsii_type__
-                    for iface in getattr(klass, "__jsii_ifaces__", [])
-                ],
+                interfaces=[iface.__jsii_type__ for iface in getattr(klass, "__jsii_ifaces__", [])],
             )
         )
         if isinstance(response, Callback):
-            obj.__jsii_ref__ = _callback_till_result(self, response, CreateResponse)
+            obj.__jsii_ref__ =  _callback_till_result(self, response, CreateResponse)
         else:
             obj.__jsii_ref__ = response
 
         # Register this to the reference map already (so it's available within the rest of the __init__)
         _reference_map.register_reference(obj)
 
         return obj.__jsii_ref__
 
     def delete(self, ref: ObjRef) -> None:
         self.provider.delete(DeleteRequest(objref=ref))
 
     @_dereferenced
-    def get(self, obj: Any, property: str) -> Any:
+    def get(self, obj: Referenceable, property: str) -> Any:
         response = self.provider.get(
             GetRequest(objref=obj.__jsii_ref__, property=property)
         )
         if isinstance(response, Callback):
             return _callback_till_result(self, response, GetResponse)
         else:
             return response.value
 
-    def set(self, obj: Any, property: str, value: Any) -> None:
+    def set(self, obj: Referenceable, property: str, value: Any) -> None:
         response = self.provider.set(
             SetRequest(
                 objref=obj.__jsii_ref__,
                 property=property,
                 value=_make_reference_for_native(self, value),
             )
         )
         if isinstance(response, Callback):
             _callback_till_result(self, response, SetResponse)
 
     @_dereferenced
-    def sget(self, klass: Type, property: str) -> Any:
+    def sget(self, klass: JSClass, property: str) -> Any:
         return self.provider.sget(
             StaticGetRequest(fqn=klass.__jsii_type__, property=property)
         ).value
 
-    def sset(self, klass: Type, property: str, value: Any) -> None:
+    def sset(self, klass: JSClass, property: str, value: Any) -> None:
         self.provider.sset(
             StaticSetRequest(
                 fqn=klass.__jsii_type__,
                 property=property,
                 value=_make_reference_for_native(self, value),
             )
         )
 
     @_dereferenced
-    def invoke(self, obj: Any, method: str, args: Optional[List[Any]] = None) -> Any:
+    def invoke(
+        self, obj: Referenceable, method: str, args: Optional[List[Any]] = None
+    ) -> Any:
         if args is None:
             args = []
 
         response = self.provider.invoke(
             InvokeRequest(
                 objref=obj.__jsii_ref__,
                 method=method,
@@ -406,15 +295,15 @@
         if isinstance(response, Callback):
             return _callback_till_result(self, response, InvokeResponse)
         else:
             return response.result
 
     @_dereferenced
     def sinvoke(
-        self, klass: Type, method: str, args: Optional[List[Any]] = None
+        self, klass: JSClass, method: str, args: Optional[List[Any]] = None
     ) -> Any:
         if args is None:
             args = []
 
         response = self.provider.sinvoke(
             StaticInvokeRequest(
                 fqn=klass.__jsii_type__,
@@ -424,37 +313,39 @@
         )
         if isinstance(response, Callback):
             return _callback_till_result(self, response, InvokeResponse)
         else:
             return response.result
 
     @_dereferenced
-    def complete(self, cbid: str, err: Optional[str], result: Any) -> Any:
+    def complete(
+        self, cbid: str, err: Optional[str], result: Any
+    ) -> Any:
         return self.provider.complete(
             CompleteRequest(
-                cbid=cbid, err=err, result=_make_reference_for_native(self, result)
+                cbid=cbid,
+                err=err,
+                result=_make_reference_for_native(self, result)
             )
         )
 
     def sync_complete(
-        self,
-        cbid: str,
-        err: Optional[str],
-        result: Any,
-        response_type: Type[KernelResponse],
+        self, cbid: str, err: Optional[str], result: Any, response_type: Type[KernelResponse]
     ) -> Any:
         return self.provider.sync_complete(
             CompleteRequest(
-                cbid=cbid, err=err, result=_make_reference_for_native(self, result)
-            ),
-            response_type=response_type,
+                cbid=cbid,
+                err=err,
+                result=_make_reference_for_native(self, result)),
+            response_type=response_type
         )
 
-    @_dereferenced
-    def ainvoke(self, obj: Any, method: str, args: Optional[List[Any]] = None) -> Any:
+    def ainvoke(
+        self, obj: Referenceable, method: str, args: Optional[List[Any]] = None
+    ) -> Any:
         if args is None:
             args = []
 
         promise = self.provider.begin(
             BeginRequest(
                 objref=obj.__jsii_ref__,
                 method=method,
```

### Comparing `jsii-1.84.0/src/jsii/_kernel/providers/base.py` & `jsii-1.9.0/src/jsii/_kernel/providers/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import abc
 
 from typing import Optional, Union, Type
 
-from ..types import (
+from jsii._kernel.types import (
     LoadRequest,
     LoadResponse,
     CreateRequest,
     CreateResponse,
     GetRequest,
     GetResponse,
     InvokeRequest,
     InvokeResponse,
-    GetScriptCommandRequest,
-    GetScriptCommandResponse,
-    InvokeScriptRequest,
-    InvokeScriptResponse,
     DeleteRequest,
     DeleteResponse,
     SetRequest,
     SetResponse,
     StaticGetRequest,
     StaticInvokeRequest,
     StaticSetRequest,
@@ -30,39 +26,30 @@
     CallbacksResponse,
     CompleteRequest,
     CompleteResponse,
     StatsRequest,
     StatsResponse,
     Callback,
     CompleteRequest,
-    KernelResponse,
+    KernelResponse
 )
 
 
 class BaseProvider(metaclass=abc.ABCMeta):
+
     # The API provided by this Provider is not very pythonic, however it is done to map
     # this API as closely to the JSII runtime as possible. Higher level abstractions
     # that layer ontop of the Provider will provide a translation layer that make this
     # much more Pythonic.
 
     @abc.abstractmethod
     def load(self, request: LoadRequest) -> LoadResponse:
         ...
 
     @abc.abstractmethod
-    def getScriptCommand(
-        self, request: GetScriptCommandRequest
-    ) -> GetScriptCommandResponse:
-        ...
-
-    @abc.abstractmethod
-    def invokeBinScript(self, request: InvokeScriptRequest) -> InvokeScriptResponse:
-        ...
-
-    @abc.abstractmethod
     def create(self, request: CreateRequest) -> CreateResponse:
         ...
 
     @abc.abstractmethod
     def get(self, request: GetRequest) -> GetResponse:
         ...
 
@@ -87,17 +74,15 @@
         ...
 
     @abc.abstractmethod
     def complete(self, request: CompleteRequest) -> CompleteResponse:
         ...
 
     @abc.abstractmethod
-    def sync_complete(
-        self, request: CompleteRequest, response_type: Type[KernelResponse]
-    ) -> Union[InvokeResponse, GetResponse]:
+    def sync_complete(self, request: CompleteRequest, response_type: Type[KernelResponse]) -> Union[InvokeResponse, GetResponse]:
         ...
 
     @abc.abstractmethod
     def delete(self, request: DeleteRequest) -> DeleteResponse:
         ...
 
     @abc.abstractmethod
```

### Comparing `jsii-1.84.0/src/jsii/_kernel/providers/process.py` & `jsii-1.9.0/src/jsii/_kernel/providers/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-import atexit
-import base64
 import datetime
 import contextlib
 import enum
+import importlib.machinery
 import json
 import os
 import os.path
-import pathlib
 import platform
 import subprocess
-import sys
 import tempfile
-import threading
 
-from typing import TYPE_CHECKING, Type, Union, Mapping, IO, Any, AnyStr, Optional
+from typing import TYPE_CHECKING, Type, Union, Mapping, Any, Optional
 
 import attr
 import cattr  # type: ignore
 import dateutil.parser
 
 import jsii._embedded.jsii
 
-from ...__meta__ import __jsii_runtime_version__
-from ..._compat import importlib_resources
-from ..._utils import memoized_property
-from .base import BaseProvider
-from ..types import (
+from jsii.__meta__ import __jsii_runtime_version__
+from jsii._compat import importlib_resources
+from jsii._utils import memoized_property
+from jsii._kernel.providers.base import BaseProvider
+from jsii._kernel.types import (
     ObjRef,
     EnumRef,
     Override,
     KernelRequest,
     KernelResponse,
     LoadRequest,
     LoadResponse,
@@ -37,18 +33,14 @@
     CreateResponse,
     DeleteRequest,
     DeleteResponse,
     GetRequest,
     GetResponse,
     InvokeRequest,
     InvokeResponse,
-    GetScriptCommandRequest,
-    GetScriptCommandResponse,
-    InvokeScriptRequest,
-    InvokeScriptResponse,
     SetRequest,
     SetResponse,
     StaticGetRequest,
     StaticInvokeRequest,
     StaticSetRequest,
     BeginRequest,
     BeginResponse,
@@ -60,50 +52,55 @@
     CompleteResponse,
     StatsRequest,
     StatsResponse,
     Callback,
     CompleteRequest,
     CompleteResponse,
 )
-from ...errors import ErrorType, JSIIError, JavaScriptError
+from jsii.errors import JSIIError, JavaScriptError
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class _HelloResponse:
+
     hello: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class _OkayResponse:
+
     # We could technically mark this as KernelResponse, because we know that
     # it is going to be one of those. However, we can't disambiguate the different
     # types because some of them have the same keys as each other, so the only way
     # to know what type the result is expected to be, is to know what method is
     # being called. Thus we'll expect Any here, and structure this value separately.
     ok: Any
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
-class _ErrorResponse:
+class _ErrorRespose:
+
     error: str
     stack: str
-    name: str
-
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class _CallbackResponse:
-    callback: Callback
 
+    callback: Callback
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class _CompleteRequest:
-    complete: CompleteRequest
 
+    complete: CompleteRequest
 
-_ProcessResponse = Union[_OkayResponse, _ErrorResponse, _CallbackResponse]
+_ProcessResponse = Union[_OkayResponse, _ErrorRespose, _CallbackResponse]
+# Workaround for mypy#5354
+_ProcessResponse_R: Type[Any]
+if not TYPE_CHECKING:
+    _ProcessResponse_R = _ProcessResponse
 
 
 def _with_api_key(api_name, asdict):
     def unstructurer(value):
         unstructured = asdict(value)
         unstructured["api"] = api_name
 
@@ -154,24 +151,14 @@
         self._serializer = cattr.Converter()
         self._serializer.register_unstructure_hook(enum.Enum, _unstructure_enum)
         self._serializer.register_unstructure_hook(
             LoadRequest,
             _with_api_key("load", self._serializer.unstructure_attrs_asdict),
         )
         self._serializer.register_unstructure_hook(
-            GetScriptCommandRequest,
-            _with_api_key(
-                "getBinScriptCommand", self._serializer.unstructure_attrs_asdict
-            ),
-        )
-        self._serializer.register_unstructure_hook(
-            InvokeScriptRequest,
-            _with_api_key("invokeBinScript", self._serializer.unstructure_attrs_asdict),
-        )
-        self._serializer.register_unstructure_hook(
             CreateRequest,
             _with_api_key("create", self._serializer.unstructure_attrs_asdict),
         )
         self._serializer.register_unstructure_hook(
             DeleteRequest,
             _with_api_key("del", self._serializer.unstructure_attrs_asdict),
         )
@@ -223,92 +210,86 @@
         self._serializer.register_structure_hook(ObjRef, _with_reference)
 
         self._ctx_stack = contextlib.ExitStack()
 
     def __del__(self):
         self.stop()
 
-    def _jsii_runtime(self) -> str:
-        tmpdir = self._ctx_stack.enter_context(tempfile.TemporaryDirectory())
-        resources = {
-            resname: os.path.join(tmpdir, filename.replace("/", os.sep))
-            for resname, filename in jsii._embedded.jsii.EMBEDDED_FILES.items()
-        }
-
-        for resname, filename in resources.items():
-            pathlib.Path(os.path.dirname(filename)).mkdir(exist_ok=True)
-            with open(filename, "wb") as fp:
-                fp.write(
-                    importlib_resources.files(jsii._embedded.jsii)
-                    .joinpath(resname)
-                    .read_bytes()
+    def _jsii_runtime(self):
+        # We have the JSII Runtime bundled with our package and we want to extract it,
+        # however if we just blindly use importlib.resources for this, we're going to
+        # have our jsii-runtime.js existing in a *different* temporary directory from
+        # the jsii-runtime.js.map, which we don't want. We can manually set up a
+        # temporary directory and extract our resources to there, but we don't want to
+        # pay the case of setting up a a temporary directory and shuffling bytes around
+        # in the common case where these files already exist on disk side by side. So
+        # we will check what loader the embedded package used, if it's a
+        # SourceFileLoader then we'll assume it's going to be on the filesystem and
+        # just use importlib.resources.path.
+
+        # jsii-runtime.js MUST be the first item in this list.
+        filenames = ["jsii-runtime.js", "jsii-runtime.js.map", "mappings.wasm"]
+
+        if isinstance(
+            jsii._embedded.jsii.__loader__, importlib.machinery.SourceFileLoader
+        ):
+            paths = [
+                self._ctx_stack.enter_context(
+                    importlib_resources.path(jsii._embedded.jsii, f)
                 )
+                for f in filenames
+            ]
+        else:
+            tmpdir = self._ctx_stack.enter_context(tempfile.TemporaryDirectory())
+            paths = [os.path.join(tmpdir, filename) for filename in filenames]
+
+            for path, filename in zip(paths, filenames):
+                with open(path, "wb") as fp:
+                    fp.write(
+                        importlib_resources.read_binary(jsii._embedded.jsii, filename)
+                    )
+
+        # Ensure that our jsii-runtime.js is the first entry in our paths, and that all
+        # of our paths, are in a commmon directory, and we didn't get them split into
+        # multiple directories somehow.
+        assert os.path.basename(paths[0]) == filenames[0]
+        assert os.path.commonpath(paths) == os.path.dirname(paths[0])
 
         # Return our first path, which should be the path for jsii-runtime.js
-        return resources[jsii._embedded.jsii.ENTRYPOINT]
+        return str(paths[0])
 
     def _next_message(self) -> Mapping[Any, Any]:
-        assert self._process.stdout is not None
         return json.loads(self._process.stdout.readline(), object_hook=ohook)
 
     def start(self):
         environ = os.environ.copy()
         environ["JSII_AGENT"] = f"Python/{platform.python_version()}"
 
-        jsii_node = environ.get("JSII_NODE", "node")
-        jsii_runtime = environ.get("JSII_RUNTIME", self._jsii_runtime())
+        jsii_runtime = environ.get('JSII_RUNTIME', self._jsii_runtime())
 
         self._process = subprocess.Popen(
-            [
-                jsii_node,
-                "--max-old-space-size=4069",
-                jsii_runtime,
-            ],
+            ["node", jsii_runtime],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
             env=environ,
         )
-
-        self.sink_thread = threading.Thread(
-            name="process.stderr_sink",
-            target=stderr_sink,
-            # Trailing comma here is important (this is a 1-value tuple, not a value between parentheses)
-            args=(self._process.stderr,),
-            # Thread is a daemon so it does not hold the VM from shutting down
-            daemon=True,
-        )
-        self.sink_thread.start()
-
-        # Clean this process up at exit, so it terminates "gracefully"
-        atexit.register(self.stop)
-
         self.handshake()
 
-    def stop(self) -> None:
-        # This process is closing already, un-registering the hook to not fire twice
-        atexit.unregister(self.stop)
-
-        assert self._process.stdin is not None
-        if not self._process.stdin.closed:
-            self._process.stdin.write(b'{"exit":0}\n')
-            # Close the process' STDIN, singaling we are done with it
-            self._process.stdin.close()
+    def stop(self):
+        # TODO: We can write an empty string here instead?
+        self._process.terminate()
 
         try:
             self._process.wait(timeout=5)
         except subprocess.TimeoutExpired:
-            self._process.terminate()
-
-        if self.sink_thread.is_alive():
-            self.sink_thread.join(timeout=5)
+            self._process.kill()
 
         self._ctx_stack.close()
 
-    def handshake(self) -> None:
+    def handshake(self):
         # Get the version of the runtime that we're using.
         resp: _HelloResponse = self._serializer.structure(
             self._next_message(), _HelloResponse
         )
 
         # TODO: Replace with proper error.
         assert (
@@ -318,51 +299,40 @@
     def send(
         self, request: KernelRequest, response_type: Type[KernelResponse]
     ) -> KernelResponse:
         req_dict = self._serializer.unstructure(request)
         data = json.dumps(req_dict, default=jdefault).encode("utf8")
 
         # Send our data, ensure that it is framed with a trailing \n
-        assert self._process.stdin is not None
         self._process.stdin.write(b"%b\n" % (data,))
         self._process.stdin.flush()
 
         resp: _ProcessResponse = self._serializer.structure(
-            self._next_message(), _ProcessResponse
+            self._next_message(), _ProcessResponse_R
         )
 
         if isinstance(resp, _OkayResponse):
             return self._serializer.structure(resp.ok, response_type)
         elif isinstance(resp, _CallbackResponse):
             return resp.callback
         else:
-            if resp.name == ErrorType.JSII_FAULT.value:
-                raise JSIIError(resp.error) from JavaScriptError(resp.stack)
-            raise RuntimeError(resp.error) from JavaScriptError(resp.stack)
+            raise JSIIError(resp.error) from JavaScriptError(resp.stack)
 
 
 class ProcessProvider(BaseProvider):
     @memoized_property
     def _process(self) -> _NodeProcess:
         process = _NodeProcess()
         process.start()
 
         return process
 
     def load(self, request: LoadRequest) -> LoadResponse:
         return self._process.send(request, LoadResponse)
 
-    def getScriptCommand(
-        self, request: GetScriptCommandRequest
-    ) -> GetScriptCommandResponse:
-        return self._process.send(request, GetScriptCommandResponse)
-
-    def invokeBinScript(self, request: InvokeScriptRequest) -> InvokeScriptResponse:
-        return self._process.send(request, InvokeScriptResponse)
-
     def create(self, request: CreateRequest) -> CreateResponse:
         return self._process.send(request, CreateResponse)
 
     def get(self, request: GetRequest) -> GetResponse:
         return self._process.send(request, GetResponse)
 
     def set(self, request: SetRequest) -> SetResponse:
@@ -391,32 +361,15 @@
 
     def callbacks(self, request: CallbacksRequest) -> CallbacksResponse:
         return self._process.send(request, CallbacksResponse)
 
     def complete(self, request: CompleteRequest) -> CompleteResponse:
         return self._process.send(request, CompleteResponse)
 
-    def sync_complete(
-        self, request: CompleteRequest, response_type: Type[KernelResponse]
-    ) -> Union[InvokeResponse, GetResponse]:
+    def sync_complete(self, request: CompleteRequest, response_type: Type[KernelResponse]) -> Union[InvokeResponse, GetResponse]:
         resp = self._process.send(_CompleteRequest(complete=request), response_type)
         return resp
 
     def stats(self, request: Optional[StatsRequest] = None) -> StatsResponse:
         if request is None:
             request = StatsRequest()
         return self._process.send(request, StatsResponse)
-
-
-def stderr_sink(reader: IO[AnyStr]) -> None:
-    # An empty string is used to signal EOF...
-    for line in iter(reader.readline, b""):
-        if line == b"":
-            break
-        try:
-            console = json.loads(line)
-            if console.get("stderr") is not None:
-                sys.stderr.buffer.write(base64.b64decode(console["stderr"]))
-            if console.get("stdout") is not None:
-                sys.stdout.buffer.write(base64.b64decode(console["stdout"]))
-        except:
-            print(line, file=sys.stderr)
```

### Comparing `jsii-1.84.0/src/jsii/_kernel/types.py` & `jsii-1.9.0/src/jsii/_kernel/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,243 +1,259 @@
-from typing import Any, Dict, Generic, List, Optional, Mapping, TypeVar, Union
-from typing_extensions import Protocol
+from typing import Union, List, Any, Optional, Mapping
 
 import attr
 
+from jsii.compat import Protocol
+
+
+# TODO:
+# - HelloResponse
+# - OkayResponse
+# - ErrorResponse
+
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class ObjRef:
+
     ref: str
     interfaces: Optional[List[str]] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class EnumRef:
+
     ref: ObjRef
     member: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Override:
+
     method: Optional[str] = None
     property: Optional[str] = None
     cookie: Optional[str] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class LoadRequest:
+
     name: str
     version: str
     tarball: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class LoadResponse:
-    assembly: str
-    types: int
-
 
-@attr.s(auto_attribs=True, frozen=True, slots=True)
-class GetScriptCommandRequest:
     assembly: str
-    script: str
-    args: List[Any] = attr.Factory(list)
-
-
-@attr.s(auto_attribs=True, frozen=True, slots=True)
-class GetScriptCommandResponse:
-    command: str
-    args: List[str] = attr.Factory(list)
-    env: Dict[str, str] = attr.Factory(dict)
-
-
-@attr.s(auto_attribs=True, frozen=True, slots=True)
-class InvokeScriptRequest:
-    assembly: str
-    script: str
-    args: List[Any] = attr.Factory(list)
-
-
-@attr.s(auto_attribs=True, frozen=True, slots=True)
-class InvokeScriptResponse:
-    status: int
-    stdout: str
-    stderr: str
-    signal: str
+    types: int
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CreateRequest:
+
     fqn: str
     args: List[Any] = attr.Factory(list)
     overrides: List[Override] = attr.Factory(list)
     interfaces: Optional[List[str]] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CreateResponse(ObjRef):
     ...
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class DeleteRequest:
+
     objref: ObjRef
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class DeleteResponse:
     ...
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class GetRequest:
+
     objref: ObjRef
     property: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class StaticGetRequest:
+
     fqn: str
     property: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class GetResponse:
+
     value: Any = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class StaticSetRequest:
+
     fqn: str
     property: str
     value: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class SetRequest:
+
     objref: ObjRef
     property: str
     value: Any
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class SetResponse:
     ...
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class StaticInvokeRequest:
+
     fqn: str
     method: str
     args: Optional[List[Any]] = attr.Factory(list)
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class InvokeRequest:
+
     objref: ObjRef
     method: str
     args: Optional[List[Any]] = attr.Factory(list)
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class InvokeResponse:
+
     result: Any = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class BeginRequest:
+
     objref: ObjRef
     method: str
     args: Optional[List[Any]] = attr.Factory(list)
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class BeginResponse:
+
     promiseid: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class EndRequest:
+
     promiseid: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class EndResponse:
-    result: Optional[Any] = None
+
+    result: Any
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Callback:
+
     cbid: str
-    cookie: str
+    cookie: Optional[str] = None
     invoke: Optional[InvokeRequest] = None
     get: Optional[GetRequest] = None
     set: Optional[SetRequest] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CallbacksRequest:
     ...
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CallbacksResponse:
+
     callbacks: List[Callback]
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CompleteRequest:
+
     cbid: str
     err: Optional[str] = None
     result: Optional[Any] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class CompleteResponse:
+
     cbid: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class NamingRequest:
+
     assembly: str
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class NamingResponse:
+
     naming: Mapping[str, Mapping[str, Optional[Any]]]
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class StatsRequest:
     ...
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class StatsResponse:
+
     objectCount: int
 
 
 KernelRequest = Union[
     LoadRequest,
     CreateRequest,
     DeleteRequest,
     GetRequest,
-    SetRequest,
     StaticGetRequest,
     InvokeRequest,
-    InvokeScriptRequest,
     StaticInvokeRequest,
     StatsRequest,
 ]
 
 KernelResponse = Union[
     BeginResponse,
     LoadResponse,
     CreateResponse,
     DeleteResponse,
     GetResponse,
     InvokeResponse,
-    InvokeScriptResponse,
     SetResponse,
     StatsResponse,
     Callback,
 ]
+
+
+class JSClass(Protocol):
+    @property
+    def __jsii_type__(self) -> str:
+        """
+        Returns a str that points to this class inside of the Javascript runtime.
+        """
+
+class Referenceable(Protocol):
+    @property
+    def __jsii_ref__(self) -> ObjRef:
+        """
+        Returns an ObjRef that points to this object on the JS side.
+        """
```

### Comparing `jsii-1.84.0/src/jsii/_runtime.py` & `jsii-1.9.0/src/jsii/_runtime.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,187 +1,132 @@
 import abc
 import os
-import sys
-import subprocess
 
 import attr
 
-from typing import (
-    Any,
-    Callable,
-    cast,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Type,
-    TypeVar,
-)
-
-from . import _reference_map
-from ._compat import importlib_resources
-from ._kernel import Kernel
-from .python import _ClassPropertyMeta
+from jsii import _reference_map
+from jsii._compat import importlib_resources
+from jsii._kernel import Kernel
+from jsii.python import _ClassPropertyMeta
 
 
 # Yea, a global here is kind of gross, however, there's not really a better way of
 # handling this. Fundamentally this is a global value, since we can only reasonably
 # have a single kernel active at any one time in a real program.
 kernel = Kernel()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class JSIIAssembly:
+
     name: str
     version: str
     module: str
     filename: str
 
     @classmethod
-    def load(cls, *args, _kernel=kernel, **kwargs) -> "JSIIAssembly":
+    def load(cls, *args, _kernel=kernel, **kwargs):
         # Our object here really just acts as a record for our JSIIAssembly, it doesn't
         # offer any functionality itself, besides this class method that will trigger
         # the loading of the given assembly in the JSII Kernel.
         assembly = cls(*args, **kwargs)
 
         # Actually load the assembly into the kernel, we're using the
-        # importlib.resources API here instead of manually constructing the path, in
+        # importlib.resources API here isntead of manually constructing the path, in
         # the hopes that this will make JSII modules able to be used with zipimport
         # instead of only on the FS.
-        with importlib_resources.as_file(
-            importlib_resources.files(f"{assembly.module}._jsii").joinpath(
-                assembly.filename
-            )
+        with importlib_resources.path(
+            f"{assembly.module}._jsii", assembly.filename
         ) as assembly_path:
             _kernel.load(assembly.name, assembly.version, os.fspath(assembly_path))
 
         # Give our record of the assembly back to the caller.
         return assembly
 
-    @classmethod
-    def invokeBinScript(
-        cls,
-        pkgname: str,
-        script: str,
-        args: Optional[Sequence[str]] = None,
-        _kernel=kernel,
-    ) -> int:
-        if args is None:
-            args = []
-
-        response = _kernel.getBinScriptCommand(pkgname, script, args)
-
-        result = subprocess.run(
-            " ".join([response.command, *response.args]),
-            encoding="utf-8",
-            shell=True,
-            env=response.env,
-        )
-        return result.returncode
-
 
 class JSIIMeta(_ClassPropertyMeta, type):
-    def __new__(
-        cls: Type["JSIIMeta"],
-        name: str,
-        bases: tuple,
-        attrs: dict,
-        *,
-        jsii_type: Optional[str] = None,
-    ) -> "JSIIMeta":
+    def __new__(cls, name, bases, attrs, *, jsii_type=None):
         # We want to ensure that subclasses of a JSII class do not require setting the
         # jsii_type keyword argument. They should be able to subclass it as normal.
         # Since their parent class will have the __jsii_type__ variable defined, they
         # will as well anyways.
         if jsii_type is not None:
             attrs["__jsii_type__"] = jsii_type
-        # The declared type should NOT be inherited by subclasses. This way we can identify whether
-        # an MRO entry corresponds to a possible overrides contributor or not.
-        attrs["__jsii_declared_type__"] = jsii_type
 
         obj = super().__new__(cls, name, bases, attrs)
 
         # Now that we've created the class, we'll need to register it with our reference
         # mapper. We only do this for types that are actually jsii types, and not any
         # subclasses of them.
         if jsii_type is not None:
             _reference_map.register_type(obj)
 
-        return cast("JSIIMeta", obj)
+        return obj
 
-    def __call__(cls: Type[Any], *args: Any, **kwargs) -> Any:
+    def __call__(cls, *args, **kwargs):
         inst = super().__call__(*args, **kwargs)
 
         # Register this instance with our reference map.
         _reference_map.register_reference(inst)
 
         return inst
 
 
 class JSIIAbstractClass(abc.ABCMeta, JSIIMeta):
     pass
 
 
-F = TypeVar("F", bound=Callable[..., Any])
-T = TypeVar("T", bound=Type[Any])
-
-
-def enum(*, jsii_type: str) -> Callable[[T], T]:
+def enum(*, jsii_type):
     def deco(cls):
         cls.__jsii_type__ = jsii_type
         _reference_map.register_enum(cls)
         return cls
 
     return deco
 
 
-def data_type(
-    *,
-    jsii_type: str,
-    jsii_struct_bases: List[Type[Any]],
-    name_mapping: Mapping[str, str],
-) -> Callable[[T], T]:
+def data_type(*, jsii_type, jsii_struct_bases, name_mapping):
     def deco(cls):
         cls.__jsii_type__ = jsii_type
         cls.__jsii_struct_bases__ = jsii_struct_bases
         cls.__jsii_name_mapping__ = name_mapping
         _reference_map.register_data_type(cls)
         return cls
 
     return deco
 
 
-def member(*, jsii_name: str) -> Callable[[F], F]:
+def member(*, jsii_name):
     def deco(fn):
         fn.__jsii_name__ = jsii_name
         return fn
 
     return deco
 
 
-def implements(*interfaces: Type[Any]) -> Callable[[T], T]:
+def implements(*interfaces):
     def deco(cls):
         cls.__jsii_type__ = getattr(cls, "__jsii_type__", None)
         cls.__jsii_ifaces__ = getattr(cls, "__jsii_ifaces__", []) + list(interfaces)
         return cls
 
     return deco
 
 
-def interface(*, jsii_type: str) -> Callable[[T], T]:
+def interface(*, jsii_type):
     def deco(iface):
         iface.__jsii_type__ = jsii_type
         _reference_map.register_interface(iface)
         return iface
 
     return deco
 
 
-def proxy_for(abstract_class: Type[Any]) -> Type[Any]:
+def proxy_for(abstract_class):
     if not hasattr(abstract_class, "__jsii_proxy_class__"):
         raise TypeError(f"{abstract_class} is not a JSII Abstract class.")
 
-    return cast(Any, abstract_class).__jsii_proxy_class__()
+    return abstract_class.__jsii_proxy_class__()
 
 
-def python_jsii_mapping(cls: Type[Any]) -> Optional[Mapping[str, str]]:
-    return getattr(cls, "__jsii_name_mapping__", None)
+def python_jsii_mapping(cls):
+    return getattr(cls, '__jsii_name_mapping__', None)
```

### Comparing `jsii-1.84.0/src/jsii.egg-info/SOURCES.txt` & `jsii-1.9.0/src/jsii.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -18,20 +18,15 @@
 src/jsii.egg-info/PKG-INFO
 src/jsii.egg-info/SOURCES.txt
 src/jsii.egg-info/dependency_links.txt
 src/jsii.egg-info/requires.txt
 src/jsii.egg-info/top_level.txt
 src/jsii/_embedded/__init__.py
 src/jsii/_embedded/jsii/__init__.py
-src/jsii/_embedded/jsii/bin__jsii-runtime.js
-src/jsii/_embedded/jsii/bin__jsii-runtime.js.map
-src/jsii/_embedded/jsii/lib__program.js
-src/jsii/_embedded/jsii/lib__program.js.map
+src/jsii/_embedded/jsii/jsii-runtime.js
+src/jsii/_embedded/jsii/jsii-runtime.js.map
+src/jsii/_embedded/jsii/mappings.wasm
 src/jsii/_kernel/__init__.py
 src/jsii/_kernel/types.py
 src/jsii/_kernel/providers/__init__.py
 src/jsii/_kernel/providers/base.py
-src/jsii/_kernel/providers/process.py
-tests/test_compliance.py
-tests/test_invoke_bin.py
-tests/test_python.py
-tests/test_runtime_type_checking.py
+src/jsii/_kernel/providers/process.py
```

