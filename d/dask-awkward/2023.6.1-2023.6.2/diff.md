# Comparing `tmp/dask_awkward-2023.6.1.tar.gz` & `tmp/dask_awkward-2023.6.2.tar.gz`

## Comparing `dask_awkward-2023.6.1.tar` & `dask_awkward-2023.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    63654 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    63799 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16791 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dask_awkward-2023.6.2/PKG-INFO
```

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.6.2/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/typing.py` & `dask_awkward-2023.6.2/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/utils.py` & `dask_awkward-2023.6.2/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.6.2/src/dask_awkward/layers/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return ob
 
     def mock(self):
         layer = copy.copy(self)
         nb = layer.numblocks
         layer.numblocks = {k: tuple(1 for _ in v) for k, v in nb.items()}
         layer.__dict__.pop("_dims", None)
-        return layer
+        return layer, None
 
     def __getstate__(self) -> dict:
         d = self.__dict__.copy()
         try:
             pickle.dumps(d["_meta"])
         except (ValueError, TypeError, KeyError):
             d.pop(
@@ -209,22 +209,22 @@
         self.prev_name = previous_layer_name
         super().__init__(mapping, **kwargs)
 
     def mock(self):
         mapping = self.mapping.copy()
         if not mapping:
             # no partitions at all
-            return self
+            return self, None
         name = next(iter(mapping))[0]
 
         if (name, 0) in mapping:
             task = mapping[(name, 0)]
             task = tuple(
                 (self.prev_name, 0)
                 if isinstance(v, tuple) and len(v) == 2 and v[0] == self.prev_name
                 else v
                 for v in task
             )
-            return MaterializedLayer({(name, 0): task})
+            return MaterializedLayer({(name, 0): task}), None
 
         # failed to cull during column opt
-        return self
+        return self, None
```

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/core.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import inspect
 import keyword
 import logging
+import math
 import operator
 import sys
 import warnings
 from collections.abc import Callable, Hashable, Mapping, Sequence
 from functools import cached_property, partial
 from numbers import Number
 from typing import TYPE_CHECKING, Any, TypeVar
@@ -484,15 +485,15 @@
         meta: ak.Array,
         divisions: tuple[int | None, ...],
     ) -> None:
         self._dask: HighLevelGraph = dsk
         if hasattr(dsk, "layers"):
             # i.e., NOT matrializes/persisted state
             # output typetracer
-            lay = list(dsk.layers.values())[-1]
+            lay = dsk.layers[dsk._toposort_layers()[-1]]
             if isinstance(lay, AwkwardBlockwiseLayer):
                 lay._meta = meta  # type: ignore
         self._name: str = name
         self._divisions: tuple[int | None, ...] = divisions
         self._meta: ak.Array = meta
 
     def __dask_graph__(self) -> HighLevelGraph:
@@ -894,42 +895,46 @@
         remainder = 0
         outpart = 0
         divisions = [0]
         dask = {}
         # make low-level graph
         for i in range(self.npartitions):
             if start > self.divisions[i + 1]:
-                # first partition not found
+                # first partition not yet found
                 continue
             if stop < self.divisions[i] and dask:
                 # no more partitions with valid rows
                 # does **NOT** exit if there are no partitions yet, to make sure there is always
                 # at least one, needed to get metadata of empty output right
                 break
-            slice_start = max(start - self.divisions[i] + remainder, 0)
-            slice_end = min(stop - self.divisions[i], self.divisions[i + 1])
+            slice_start = max(start - self.divisions[i], 0 + remainder)
+            slice_end = min(
+                stop - self.divisions[i], self.divisions[i + 1] - self.divisions[i]
+            )
             if (
                 slice_end == slice_start
                 and (self.divisions[i + 1] - self.divisions[i])
                 and dask
             ):
                 # in case of zero-row last partition (if not only partition)
                 break
             dask[(name, outpart)] = (
                 _zero_getitem,
                 (self.name, i),
                 slice(slice_start, slice_end, step),
                 rest,
             )
             outpart += 1
-            remainder += (self.divisions[i + 1] - self.divisions[i]) % step
-            divisions.append(
-                (self.divisions[i + 1] - self.divisions[i]) // step + divisions[-1]
-            )
-            remainder = remainder % step
+            remainder = (
+                (self.divisions[i] + slice_start) - self.divisions[i + 1]
+            ) % step
+            remainder = step - remainder if remainder < 0 else remainder
+            nextdiv = math.ceil((slice_end - slice_start) / step)
+            divisions.append(divisions[-1] + nextdiv)
+
         hlg = HighLevelGraph.from_collections(
             name,
             AwkwardMaterializedLayer(dask, previous_layer_name=self.name),
             dependencies=[self],
         )
         return new_array_object(
             hlg,
```

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 log = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from awkward import Array as AwkwardArray
 
 
+COLUMN_OPT_FAILED_WARNING_MSG = """The necessary columns optimization failed; exception raised:
+
+{exception} with message {message}.
+
+Please see the FAQ section of the docs for more information:
+https://dask-awkward.readthedocs.io/en/stable/me-faq.html
+
+"""
+
+
 def all_optimizations(
     dsk: Mapping,
     keys: Hashable | list[Hashable] | set[Hashable],
     **_: Any,
 ) -> Mapping:
     """Run all optimizations that benefit dask-awkward computations.
 
@@ -344,15 +354,15 @@
     # make labelled report
     projectable = _projectable_input_layer_names(dsk)
     for name, lay in dsk.layers.copy().items():
         if name in projectable:
             layers[name], report = lay.mock()
             reports[name] = report
         elif hasattr(lay, "mock"):
-            layers[name] = lay.mock()
+            layers[name], _ = lay.mock()
 
     for name in _ak_output_layer_names(dsk):
         layers[name] = _mock_output(layers[name])
 
     for name in _opt_touch_all_layer_names(dsk):
         layers[name] = _touch_and_call(layers[name])
 
@@ -363,15 +373,17 @@
         for layer in hlg.layers.values():
             layer.__dict__.pop("_cached_dict", None)
         out = get_sync(hlg, list(outlayer.keys())[0])
     except Exception as err:
         on_fail = dask.config.get("awkward.optimization.on-fail")
         # this is the default, throw a warning but skip the optimization.
         if on_fail == "warn":
-            warnings.warn(f"Column projection optimization failed: {type(err)}, {err}")
+            warnings.warn(
+                COLUMN_OPT_FAILED_WARNING_MSG.format(exception=type(err), message=err)
+            )
             return {}
         # option "pass" means do not throw warning but skip the optimization.
         elif on_fail == "pass":
             log.debug("Column projection optimization failed; optimization skipped.")
             return {}
         # option "raise" to raise the exception here
         elif on_fail == "raise":
```

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/structure.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/unproject_layout.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.6.2/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/.gitignore` & `dask_awkward-2023.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/LICENSE` & `dask_awkward-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/README.md` & `dask_awkward-2023.6.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,7 +29,12 @@
 ```
 
 Documentation
 -------------
 
 Documentation is hosted at
 [https://dask-awkward.readthedocs.io/](https://dask-awkward.readthedocs.io/).
+
+Acknowledgements
+----------------
+
+Support for this work was provided by NSF grant [OAC-2103945](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2103945).
```

### Comparing `dask_awkward-2023.6.1/pyproject.toml` & `dask_awkward-2023.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.6.1/PKG-INFO` & `dask_awkward-2023.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -75,7 +75,12 @@
 ```
 
 Documentation
 -------------
 
 Documentation is hosted at
 [https://dask-awkward.readthedocs.io/](https://dask-awkward.readthedocs.io/).
+
+Acknowledgements
+----------------
+
+Support for this work was provided by NSF grant [OAC-2103945](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2103945).
```

