# Comparing `tmp/xpystac-0.1.0.tar.gz` & `tmp/xpystac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpystac-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xpystac-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xpystac-0.1.0.tar` & `xpystac-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2041 2023-06-09 14:57:10.030114 xpystac-0.1.0/README.md
--rw-r--r--   0        0        0      622 2023-06-09 14:57:10.030114 xpystac-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/__init__.py
--rw-r--r--   0        0        0     2355 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/core.py
--rw-r--r--   0        0        0      235 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/utils.py
--rw-r--r--   0        0        0      656 2023-06-09 14:57:10.030114 xpystac-0.1.0/xpystac/xarray_plugin.py
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 xpystac-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2041 2023-06-14 19:41:11.943981 xpystac-0.1.1/README.md
+-rw-r--r--   0        0        0      682 2023-06-14 19:41:11.943981 xpystac-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/__init__.py
+-rw-r--r--   0        0        0     2513 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/core.py
+-rw-r--r--   0        0        0        0 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/py.typed
+-rw-r--r--   0        0        0      235 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/utils.py
+-rw-r--r--   0        0        0      754 2023-06-14 19:41:11.947981 xpystac-0.1.1/xpystac/xarray_plugin.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 xpystac-0.1.1/PKG-INFO
```

### Comparing `xpystac-0.1.0/README.md` & `xpystac-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xpystac-0.1.0/pyproject.toml` & `xpystac-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,7 +22,11 @@
 dev = [
   "pytest",
   "pre-commit",
 ]
 
 [project.entry-points."xarray.backends"]
 stac = "xpystac.xarray_plugin:STACBackend"
+
+[tool.ruff]
+line-length = 88
+select = ["E", "F", "W", "I"]
```

### Comparing `xpystac-0.1.0/xpystac/core.py` & `xpystac-0.1.1/xpystac/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 import functools
-from typing import List, Union
+from typing import List, Mapping, Union
 
 import pystac
 import xarray
 
 from xpystac.utils import _import_optional_dependency
 
 
 @functools.singledispatch
-def to_xarray(item, **kwargs) -> xarray.Dataset:
+def to_xarray(obj, **kwargs) -> xarray.Dataset:
     """Given a pystac object return an xarray dataset"""
-    is_pystac_client_obj = hasattr(item, "item_collection")
+    is_pystac_client_obj = hasattr(obj, "item_collection")
     if is_pystac_client_obj:
-        item_collection = item.item_collection()
+        item_collection = obj.item_collection()
         return to_xarray(item_collection, **kwargs)
     raise TypeError
 
 
 @to_xarray.register(pystac.Item)
 @to_xarray.register(pystac.ItemCollection)
 def _(
     obj: Union[pystac.Item, pystac.ItemCollection],
-    drop_variables: Union[str, List[str]] = None,
+    drop_variables: Union[str, List[str], None] = None,
     **kwargs,
 ) -> xarray.Dataset:
     stackstac = _import_optional_dependency("stackstac")
     if drop_variables is not None:
         raise KeyError("``drop_variables`` not implemented for pystac items")
     return stackstac.stack(obj, **kwargs).to_dataset(dim="band", promote_attrs=True)
 
 
 @to_xarray.register
 def _(obj: pystac.Asset, **kwargs) -> xarray.Dataset:
+    default_kwargs: Mapping
     open_kwargs = obj.extra_fields.get("xarray:open_kwargs", {})
 
     storage_options = obj.extra_fields.get("xarray:storage_options", None)
     if storage_options:
         open_kwargs["storage_options"] = storage_options
 
     if obj.media_type == pystac.MediaType.JSON and {"index", "references"}.intersection(
-        obj.roles
+        set(obj.roles) if obj.roles else set()
     ):
         requests = _import_optional_dependency("requests")
         fsspec = _import_optional_dependency("fsspec")
         r = requests.get(obj.href)
         r.raise_for_status()
         try:
-            import planetary_computer
+            import planetary_computer  # type: ignore
 
             refs = planetary_computer.sign(r.json())
         except ImportError:
             refs = r.json()
         mapper = fsspec.get_mapper("reference://", fo=refs)
-        default_kwargs = {"engine": "zarr", "consolidated": False, "chunks": {}}
-        return xarray.open_dataset(mapper, **default_kwargs, **open_kwargs, **kwargs)
+        default_kwargs = {
+            "engine": "zarr",
+            "consolidated": False,
+            "chunks": {},
+        }
+        return xarray.open_dataset(
+            mapper, **{**default_kwargs, **open_kwargs, **kwargs}
+        )
 
     if obj.media_type == pystac.MediaType.COG:
         _import_optional_dependency("rioxarray")
         default_kwargs = {"engine": "rasterio"}
     elif obj.media_type == "application/vnd+zarr":
         _import_optional_dependency("zarr")
         default_kwargs = {"engine": "zarr"}
```

### Comparing `xpystac-0.1.0/xpystac/xarray_plugin.py` & `xpystac-0.1.1/xpystac/xarray_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from typing import List, Union
+from typing import Any, Iterable, Union
 
 import pystac
 from xarray.backends import BackendEntrypoint
 
 from xpystac.core import to_xarray
 
 
 class STACBackend(BackendEntrypoint):
+    description = "Open pystac objects in Xarray"
+    open_dataset_parameters = ("filename_or_obj", "drop_variables")
+    url = "https://github.com/stac-utils/xpystac"
+
     def open_dataset(
         self,
-        obj,
-        *,
-        drop_variables: Union[str, List[str]] = None,
+        filename_or_obj: Any,
+        drop_variables: Union[str, Iterable[str], None] = None,
         **kwargs,
     ):
-        return to_xarray(obj, drop_variables=drop_variables, **kwargs)
-
-    open_dataset_parameters = ["obj", "drop_variables"]
+        return to_xarray(filename_or_obj, drop_variables=drop_variables, **kwargs)
 
-    def guess_can_open(self, obj):
-        return isinstance(obj, (pystac.Asset, pystac.Item, pystac.ItemCollection))
-
-    description = "Open pystac objects in Xarray"
-
-    url = "https://github.com/stac-utils/xpystac"
+    def guess_can_open(self, filename_or_obj: Any):
+        return isinstance(
+            filename_or_obj, (pystac.Asset, pystac.Item, pystac.ItemCollection)
+        )
```

### Comparing `xpystac-0.1.0/PKG-INFO` & `xpystac-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpystac
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extend xarray.open_dataset to accept pystac objects
 Author-email: Julia Signell <jsignell@element84.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: xarray
 Requires-Dist: pystac>=1.0.0b3
```

