# Comparing `tmp/muutils-0.4.2.tar.gz` & `tmp/muutils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.4.2.tar", max compression
+gzip compressed data, was "muutils-0.4.3.tar", max compression
```

## Comparing `muutils-0.4.2.tar` & `muutils-0.4.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.2/LICENSE
--rw-r--r--   0        0        0       22 2023-06-13 21:17:33.202116 muutils-0.4.2/muutils/__init__.py
--rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.4.2/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.2/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.4.2/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.4.2/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.4.2/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.4.2/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.4.2/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.2/muutils/dictmagic.py
--rw-r--r--   0        0        0     1613 2023-06-13 20:39:10.110554 muutils-0.4.2/muutils/group_equiv.py
--rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.2/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.2/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.4.2/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.2/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.2/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.2/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.2/muutils/jsonlines.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.2/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.2/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.2/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.2/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.2/muutils/logger/logger.py
--rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.2/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.2/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.2/muutils/logger/timing.py
--rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.2/muutils/misc.py
--rw-r--r--   0        0        0     3356 2023-06-13 21:17:26.051156 muutils-0.4.2/muutils/mlutils.py
--rw-r--r--   0        0        0        0 2023-06-13 21:17:26.051156 muutils-0.4.2/muutils/nbutils/__init__.py
--rw-r--r--   0        0        0     1452 2023-06-13 21:17:26.052156 muutils-0.4.2/muutils/nbutils/configure_notebook.py
--rw-r--r--   0        0        0    12374 2023-06-13 20:43:08.425478 muutils-0.4.2/muutils/nbutils/convert_ipynb_to_script.py
--rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.2/muutils/nbutils/print_tex.py
--rw-r--r--   0        0        0     3693 2023-06-13 21:17:26.054178 muutils-0.4.2/muutils/nbutils/run_notebook_tests.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.2/muutils/py.typed
--rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.2/muutils/statcounter.py
--rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.4.2/muutils/sysinfo.py
--rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.2/muutils/tensor_utils.py
--rw-r--r--   0        0        0      990 2023-06-13 21:17:28.966629 muutils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2341 2023-05-28 07:16:04.858712 muutils-0.4.2/README.md
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 muutils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.3/LICENSE
+-rw-r--r--   0        0        0       22 2023-06-14 07:25:08.958584 muutils-0.4.3/muutils/__init__.py
+-rw-r--r--   0        0        0     4014 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.3/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5834 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23255 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3281 2023-06-14 07:24:44.656519 muutils-0.4.3/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0    10195 2023-06-14 07:24:44.656731 muutils-0.4.3/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7415 2023-06-14 07:24:44.657732 muutils-0.4.3/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.3/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1950 2023-06-14 07:24:44.658733 muutils-0.4.3/muutils/group_equiv.py
+-rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.3/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.3/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    11124 2023-06-14 07:24:44.659732 muutils-0.4.3/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.3/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.3/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.3/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.3/muutils/jsonlines.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.3/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.3/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.3/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.3/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.3/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.3/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.3/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.3/muutils/logger/timing.py
+-rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.3/muutils/misc.py
+-rw-r--r--   0        0        0     3356 2023-06-13 21:17:26.051156 muutils-0.4.3/muutils/mlutils.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:17:26.051156 muutils-0.4.3/muutils/nbutils/__init__.py
+-rw-r--r--   0        0        0     1452 2023-06-13 21:17:26.052156 muutils-0.4.3/muutils/nbutils/configure_notebook.py
+-rw-r--r--   0        0        0    12383 2023-06-14 07:24:44.660732 muutils-0.4.3/muutils/nbutils/convert_ipynb_to_script.py
+-rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.3/muutils/nbutils/print_tex.py
+-rw-r--r--   0        0        0     3860 2023-06-14 07:24:44.661730 muutils-0.4.3/muutils/nbutils/run_notebook_tests.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.3/muutils/py.typed
+-rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.3/muutils/statcounter.py
+-rw-r--r--   0        0        0     6376 2023-06-14 07:24:44.661730 muutils-0.4.3/muutils/sysinfo.py
+-rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.3/muutils/tensor_utils.py
+-rw-r--r--   0        0        0     1344 2023-06-14 07:25:17.339614 muutils-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-06-14 02:35:51.207754 muutils-0.4.3/README.md
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 muutils-0.4.3/PKG-INFO
```

### Comparing `muutils-0.4.2/LICENSE` & `muutils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/_wip/dataclass_validator.py` & `muutils-0.4.3/muutils/_wip/dataclass_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-from typing import Optional, Callable, Union, Literal
+from typing import Callable, Literal, Optional, Union
+
 
 def dataclass_validator_factory(
-        cls,
-        checks: Optional[list[tuple[
-            Callable[[object], bool], # method taking self as argument and returning True if valid
-            Optional[str], # error message
-        ]]] = None,
-        default_throw_except : bool = False,
-        field_check_types : Union[bool, list[str]] = True,
-        type_strictness : Literal['except', 'check', 'ignore'] = 'except',
-    ) -> Callable:
+    cls,
+    checks: Optional[
+        list[
+            tuple[
+                Callable[
+                    [object], bool
+                ],  # method taking self as argument and returning True if valid
+                Optional[str],  # error message
+            ]
+        ]
+    ] = None,
+    default_throw_except: bool = False,
+    field_check_types: Union[bool, list[str]] = True,
+    type_strictness: Literal["except", "check", "ignore"] = "except",
+) -> Callable:
     """validate dataclass through type checking and a list of checks
-    
+
     # Args
     - cls: dataclass to validate (so, define MyClass.validate outside of the class defn. see example)
     - `checks`: a list of tuples of the form (method, error_message). the method should take self as argument and return True if valid
     - `default_throw_except: bool` : if True, will throw an exception if any check in `checks` fails. does not apply to type checking
     - `field_check_types: Union[bool, list[str]]`: if True, will check the type of each field. if a list, will check the type of only the fields in the list. if False, will not check the type of any field.
     - `type_strictness: Literal['except', 'check', 'ignore']` : if 'except', will throw an exception if any type is incorrect. if 'check', will return false if a type check fails, but will not raise an exception. if 'ignore', will not check type at all.
-    
+
     # Returns
     - `validator: Callable` : a function that takes a dataclass instance and a boolean indicating whether to throw an exception or not, and returns `True` if the dataclass is valid, `False` otherwise.
 
     # Usage:
     ```python
     # define our class
     @dataclass
@@ -36,58 +43,59 @@
         checks = [
             (lambda x: x.a > 0, "a must be greater than 0"),
         ],
         field_check_types = ['a'],
         default_throw_except = True,
         type_strictness = 'except',
     )
-    ```    
+    ```
 
     """
 
     # check type strictness value
-    if type_strictness not in ('except', 'check', 'ignore'):
-        raise ValueError(f"type_strictness must be one of 'except', 'check', 'ignore'. got {type_strictness = }")
-
+    if type_strictness not in ("except", "check", "ignore"):
+        raise ValueError(
+            f"type_strictness must be one of 'except', 'check', 'ignore'. got {type_strictness = }"
+        )
 
     # if set to True and no list given, set to all the keys
     if field_check_types and isinstance(field_check_types, bool):
         field_check_types = list(cls.__dataclass_fields__.keys())
 
     # filter and convert the fields and their types
-    fields_types : dict[str, type] = {
+    fields_types: dict[str, type] = {
         key: (
             # if complex type, list `list[int]`, get `list`
-            field.type.__origin__ 
-            if hasattr(field.type, '__origin__')
+            field.type.__origin__
+            if hasattr(field.type, "__origin__")
             else field.type
         )
-        for key,field in cls.__dataclass_fields__.items()
-        if key in field_check_types # filter by 
+        for key, field in cls.__dataclass_fields__.items()
+        if key in field_check_types  # filter by
     }
 
-
     def validate(self, throw_except: bool = default_throw_except) -> bool:
         f"""automagically created validator function for {cls.__name__}"""
         valid: bool = True
 
         # type checking
         for field_name, field_type in fields_types.items():
-           if not isinstance(getattr(self, field_name), field_type):
+            if not isinstance(getattr(self, field_name), field_type):
                 # if incorrect type
                 valid = False
-                if type_strictness == 'except':
-                    raise TypeError(f"`{cls.__name__}.{field_name}` must be of type `{field_type}`, is of type `{type(getattr(self, field_name))}`")
-
+                if type_strictness == "except":
+                    raise TypeError(
+                        f"`{cls.__name__}.{field_name}` must be of type `{field_type}`, is of type `{type(getattr(self, field_name))}`"
+                    )
 
         # custom checks
         if checks is not None:
             for check_func, error_msg in checks:
                 # call the function and check output
                 if not check_func(self):
                     valid = False
                     if throw_except:
-                        raise ValueError(error_msg.format(self) + f'\n\t{self = }')
-        
+                        raise ValueError(error_msg.format(self) + f"\n\t{self = }")
+
         return valid
-    
-    return validate
+
+    return validate
```

### Comparing `muutils-0.4.2/muutils/_wip/experiments.ipynb` & `muutils-0.4.3/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/_wip/gptdataset.py` & `muutils-0.4.3/muutils/_wip/gptdataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import abc
 import os
 from dataclasses import dataclass, field
 from typing import Sequence
 
-import numpy as np
 import jaxtyping
+import numpy as np
 import torch
 from torch.utils.data import Dataset
 
 
-
 # "error: Only concrete class can be given where Type[Abstract] is expected"
 # this is a mypy issue, see
 # https://github.com/python/mypy/issues/5374
 # https://github.com/python/mypy/issues/4717
 @dataclass(kw_only=True)  # type: ignore
 class GPTDatasetConfig(metaclass=abc.ABCMeta):
     """base config class"""
```

### Comparing `muutils-0.4.2/muutils/_wip/json_serialize_old.py` & `muutils-0.4.3/muutils/_wip/json_serialize_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import functools
-from pathlib import Path
-import types
-from typing import Any, Optional, Union, Callable, Literal, Iterable
-from dataclasses import dataclass, is_dataclass
 import inspect
+import types
 import typing
 import warnings
+from dataclasses import dataclass, is_dataclass
+from pathlib import Path
+from typing import Any, Callable, Iterable, Literal, Optional, Union
 
 from muutils.json_serialize.util import JSONdict
 
-
 _NUMPY_WORKING: bool
 try:
     import numpy as np
+
     _NUMPY_WORKING = True
 except ImportError:
     warnings.warn("numpy not found, cannot serialize numpy arrays!")
     _NUMPY_WORKING = False
 
 JSONitem = Union[bool, int, float, str, list, dict, None]
 Hashableitem = Union[bool, int, float, str, tuple]
 
 
 class UniversalContainer:
     """contains everything -- `x in UniversalContainer()` is always True"""
+
     def __contains__(self, x: Any) -> bool:
         return True
 
 
 def isinstance_namedtuple(x):
     """checks if `x` is a `namedtuple`
 
@@ -41,17 +42,18 @@
     if not isinstance(f, tuple):
         return False
     return all(type(n) == str for n in f)
 
 
 def try_catch(func: Callable):
     """wraps the function to catch exceptions, returns serialized error message on exception
-    
+
     returned func will return normal result on success, or error message on exception
     """
+
     @functools.wraps(func)
     def newfunc(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             return f"{e.__class__.__name__}: {e}"
 
@@ -99,30 +101,30 @@
         "dtype": str(arr.dtype),
         "data": <arr.tolist()|arr.tobytes().hex()>,
     }
     ```
 
     # Parameters:
      - `arr : Any` array to serialize
-     - `array_mode : ArrayMode` mode in which to serialize the array  
-       (defaults to `"array_list_meta"`)  
-    
+     - `array_mode : ArrayMode` mode in which to serialize the array
+       (defaults to `"array_list_meta"`)
+
     # Returns:
-     - `JSONitem` 
+     - `JSONitem`
        json serialized array
-    
+
     # Raises:
      - `KeyError` : if the array mode is not valid
 
     # TODO: allow external-file storage of large arrays?
-    """    
+    """
 
     if len(arr.shape) == 0:
         return arr.item()
-    
+
     if array_mode == "array_list_meta":
         return {
             "__format__": "array_list_meta",
             "shape": arr.shape,
             "dtype": str(arr.dtype),
             "data": arr.tolist(),
         }
@@ -134,17 +136,18 @@
             "shape": arr.shape,
             "dtype": str(arr.dtype),
             "data": arr.tobytes().hex(),
         }
     else:
         raise KeyError(f"invalid array_mode: {array_mode}")
 
+
 def infer_array_mode(arr: JSONitem) -> ArrayMode:
     """given a serialized array, infer the mode
-    
+
     assumes the array was serialized via `serialize_array()`
     """
     if isinstance(arr, typing.Mapping):
         fmt: Optional[str] = arr.get("__format__", None)
         if fmt == "array_list_meta":
             if type(arr["data"]) != list:
                 raise ValueError(f"invalid list format: {arr}")
@@ -157,22 +160,25 @@
             raise ValueError(f"invalid format: {arr}")
 
     elif isinstance(arr, list):
         return "list"
     else:
         raise ValueError(f"cannot infer array_mode from {arr}")
 
+
 def load_array(arr: JSONitem, array_mode: Optional[ArrayMode] = None) -> Any:
     """load a json-serialized array, infer the mode if not specified"""
     # try to infer the array_mode
     array_mode_inferred: ArrayMode = infer_array_mode(arr)
     if array_mode is None:
         array_mode = array_mode_inferred
     elif array_mode != array_mode_inferred:
-        warnings.warn(f"array_mode {array_mode} does not match inferred array_mode {array_mode_inferred}")        
+        warnings.warn(
+            f"array_mode {array_mode} does not match inferred array_mode {array_mode_inferred}"
+        )
 
     # actually load the array
     if array_mode == "array_list_meta":
         data = np.array(arr["data"], dtype=arr["dtype"])
         if tuple(arr["shape"]) != tuple(data.shape):
             raise ValueError(f"invalid shape: {arr}")
         return data
@@ -180,37 +186,40 @@
         data = np.frombuffer(bytes.fromhex(arr["data"]), dtype=arr["dtype"])
         return data.reshape(arr["shape"])
     elif array_mode == "list":
         return np.array(arr)
     else:
         raise ValueError(f"invalid array_mode: {array_mode}")
 
+
 SERIALIZE_DIRECT_AS_STR: set[str] = (
-    "<class 'torch.device'>", "<class 'torch.dtype'>",
+    "<class 'torch.device'>",
+    "<class 'torch.dtype'>",
 )
 
+
 def json_serialize(
     obj: Any,
     depth: int = -1,
     array_mode: ArrayMode = "array_list_meta",
     error_mode: ErrorMode = "except",
     direct_as_str: tuple[str] = SERIALIZE_DIRECT_AS_STR,
     **kwargs,
 ) -> JSONitem:
     """serialize __any__ python object to json, not guaranteed to be recoverable
-    
+
     in general, tries the following (recursive) serialization:
     - try to call a `.serialize()` method on the object (if present)
     - serialize as a base type (bool, int, float, str)
     - recursively serialize dicts
     - if a namedtuple, serialize as a dict with the namedtuple fields as keys
     - if a dataclass, serialize as a dict with the dataclass fields as keys ( but call this function recursively, not just `asdict(obj)` )
     - if an iterable, call this function recursively on each element and return a list
     - if numpy or torch array, call `serialize_array()`
-    - if none of the above, serialize as a dict with 
+    - if none of the above, serialize as a dict with
       - the items at `SERIALIZER_SPECIAL_KEYS` as keys
       - the results of calling `SERIALIZER_SPECIAL_FUNCS` as values
     - if there is an exception in the above
       - if `error_mode == "ignore"`, ignore the exception and return `repr(obj)`
       - if `error_mode == "warn"`, warn and return `repr(obj)`
       - if `error_mode == "except"`, raise the exception
     """
@@ -256,16 +265,15 @@
             # if namedtuple, treat as dict
             return json_serialize(dict(obj._asdict()), newdepth)
 
         elif is_dataclass(obj):
             # if dataclass, treat as dict
             # print(f'\n### reading obj as dataclass: {str(obj)}')
             return {
-                k: json_serialize(getattr(obj, k)) 
-                for k in obj.__dataclass_fields__
+                k: json_serialize(getattr(obj, k)) for k in obj.__dataclass_fields__
             }
         elif isinstance(obj, Path):
             return obj.as_posix()
 
         elif str_type_obj in direct_as_str:
             return str(obj)
 
@@ -276,135 +284,124 @@
             return serialize_array(obj, array_mode)
         elif str_type_obj == "<class 'torch.Tensor'>":
             # same for torch tensors
             return serialize_array(obj.detach().cpu().numpy())
         elif isinstance(obj, (set, list, tuple)) or isinstance(obj, Iterable):
             # if iterable, recurse
             # print(f'\n### reading obj as iterable: {str(obj)}')
-            return [json_serialize(x, newdepth) for x in obj]            
+            return [json_serialize(x, newdepth) for x in obj]
         else:
             # if not basic type, serialize it however we can
             return {
                 **{k: str(getattr(obj, k, None)) for k in SERIALIZER_SPECIAL_KEYS},
                 **{k: f(obj) for k, f in SERIALIZER_SPECIAL_FUNCS.items()},
             }
     except Exception as e:
         if error_mode == "except":
             raise e
         elif error_mode == "warn":
-            warnings.warn(f"error serializing, will return as string\n{obj = }\nexception = {e}")
+            warnings.warn(
+                f"error serializing, will return as string\n{obj = }\nexception = {e}"
+            )
 
         return repr(obj)
 
 
 def _recursive_hashify(obj: Any, force: bool = True) -> Hashableitem:
     if isinstance(obj, typing.Mapping):
-        return tuple(
-            (k, _recursive_hashify(v)) 
-            for k, v in obj.items()
-        )
+        return tuple((k, _recursive_hashify(v)) for k, v in obj.items())
     elif isinstance(obj, (tuple, list, Iterable)):
-        return tuple(
-            _recursive_hashify(v)
-            for v in obj
-        )
+        return tuple(_recursive_hashify(v) for v in obj)
     elif isinstance(obj, (bool, int, float, str)):
         return obj
     else:
         if force:
             return str(obj)
         else:
-            raise ValueError(f"cannot hashify:\n{obj}")        
+            raise ValueError(f"cannot hashify:\n{obj}")
 
 
 def hashify(obj: Any, force: bool = True) -> Hashableitem:
     """try to turn any object into something hashable"""
     data = json_serialize(obj, depth=-1)
 
     # recursive hashify, turning dicts and lists into tuples
     return _recursive_hashify(data, force=force)
 
 
 def serialize_torch_module(
-        obj: "torch.nn.Module", 
-        *,
-        member_typecasts: dict[str, Callable],
-        array_mode: ArrayMode = "array_list_meta",
-    ) -> JSONitem:
+    obj: "torch.nn.Module",
+    *,
+    member_typecasts: dict[str, Callable],
+    array_mode: ArrayMode = "array_list_meta",
+) -> JSONitem:
     """serialize an instance of `torch.nn.Module`
-    
+
     you'll need to specify `member_typecasts`, which is a dict mapping
     member names to functions to call on the member value before serializing it
 
     the state dict will be saved separately under `state_dict`
     """
     return {
         "__format__": "torch_module",
         "name": obj.__class__.__name__,
         "state_dict": {
-            k : serialize_array(v.cpu().numpy(), array_mode=array_mode)
+            k: serialize_array(v.cpu().numpy(), array_mode=array_mode)
             for k, v in obj.state_dict().items()
         },
         "members_dict": {
-            k : (
+            k: (
                 json_serialize(v)
                 if k not in member_typecasts
                 else json_serialize(member_typecasts[k](v))
             )
             for k, v in obj.__dict__.items()
             if not k.startswith("_")
         },
     }
 
+
 def load_torch_module_factory(
-        cls, 
-        *,
-        members_exclude: list[str],
-        typecasts: dict[str, Callable],
-    ) -> Callable[[Any, JSONitem], "torch.nn.Module"]:
+    cls,
+    *,
+    members_exclude: list[str],
+    typecasts: dict[str, Callable],
+) -> Callable[[Any, JSONitem], "torch.nn.Module"]:
     """create a function which allows for loading a torch module from `JSONitem`
 
     - everything from the `members_dict` not in `members_exclude` will be passed to the `__init__` method of the module
     - everything from the `state_dict` will be passed to the `load_state_dict` method of the module
     """
     import torch
 
     @classmethod
     def load(cls, item: JSONitem) -> "torch.nn.Module":
         assert item["__format__"] == "torch_module"
         assert item["name"] == cls.__name__
 
         module_obj = cls(
             **{
-                k: (
-                    v 
-                    if k not in typecasts 
-                    else typecasts[k](v)
-                )
+                k: (v if k not in typecasts else typecasts[k](v))
                 for k, v in item["members_dict"].items()
                 if k not in members_exclude
             }
         )
         module_obj.load_state_dict(
-            {
-                k: torch.from_numpy(load_array(v))
-                for k, v in item["state_dict"].items()
-            },
+            {k: torch.from_numpy(load_array(v)) for k, v in item["state_dict"].items()},
         )
         return module_obj
 
     return load
 
 
-
 def dataclass_serializer_factory(
-        cls, 
-        special_serializers: Optional[dict[str, Callable]] = None,
-        fields_exclude: Optional[Iterable[str]] = None,
-    ) -> Callable[[Any], JSONitem]:
+    cls,
+    special_serializers: Optional[dict[str, Callable]] = None,
+    fields_exclude: Optional[Iterable[str]] = None,
+) -> Callable[[Any], JSONitem]:
     """outputs a `.serialize` method for a dataclass,
     where fields present in `special_serializers` are serialized using the corresponding function.
 
     each function in `special_serializers` should take the class itself as an argument, and return a JSONitem.
     """
     # make it an empty dict if not provided
     if special_serializers is None:
@@ -412,48 +409,44 @@
 
     if fields_exclude is None:
         fields_exclude = list()
 
     def serialize(self):
         # get the base outputs for all keys in the dataclass but which dont have a special serializer
         base_output: JSONdict = {
-            k: (
-                json_serialize(getattr(self, k))
-            )
+            k: (json_serialize(getattr(self, k)))
             for k in self.__dataclass_fields__
-            if (
-                (k not in special_serializers)
-                and (k not in fields_exclude)
-            )
+            if ((k not in special_serializers) and (k not in fields_exclude))
         }
 
         # update with the special serializers
         return {
             **base_output,
             **{
                 k: special_serializers[k](self)
                 for k in special_serializers
                 if k not in fields_exclude
             },
         }
 
     return serialize
 
+
 TypeErrorMode = Union[ErrorMode, Literal["try_convert"]]
 
 
 def loader_typecheck_factory(
-        key: str,
-        expected_type: type, 
-        error_mode: TypeErrorMode = "except",
-    ) -> Callable[[JSONitem], Any]:
+    key: str,
+    expected_type: type,
+    error_mode: TypeErrorMode = "except",
+) -> Callable[[JSONitem], Any]:
     """outputs a loader function, which checks the type of the argument
-    
+
     if the argument `data` to the loader is not of the expected type:
-    - if `error_mode == "except"`, raises a TypeError 
+    - if `error_mode == "except"`, raises a TypeError
     - if `error_mode == "try_convert"` return `expected_type(data)`. this might raise further exceptions
     - if `error_mode == "warn"`, print a warning and return `data`
     - if `error_mode == "ignore"`, return `data`
 
     TODO: perhaps an option to warn, but try to convert?
     """
 
@@ -468,73 +461,79 @@
     try:
         if origin_type in (Union, types.UnionType, Optional):
             # TODO: this is incomplete
             pass
         elif isinstance(None, origin_type):
             pass
     except TypeError as e:
-        warnings.warn(f"error processing {origin_type = } for {key = }, loader will return raw data\n\t{e}")
+        warnings.warn(
+            f"error processing {origin_type = } for {key = }, loader will return raw data\n\t{e}"
+        )
         return_raw = True
 
     def loader(data: JSONitem) -> Any:
         if key not in data:
-            raise KeyError(f"while executing `.load(data)`, key {key} not found in data: {data = }")
+            raise KeyError(
+                f"while executing `.load(data)`, key {key} not found in data: {data = }"
+            )
 
         if return_raw:
             return data[key]
 
         # TODO: make unions work correctly
         if (
-                (origin_type is Union) 
-                or (origin_type is types.UnionType)
-                or isinstance(data[key], origin_type)
-            ):
-                return data[key]
+            (origin_type is Union)
+            or (origin_type is types.UnionType)
+            or isinstance(data[key], origin_type)
+        ):
+            return data[key]
         else:
             if error_mode == "warn":
                 warnings.warn(f"error loading, will return raw data")
                 return data[key]
             elif error_mode == "except":
-                raise TypeError(f"expected {origin_type} for {key = }, got {type(data)}\n\t{data = }")
+                raise TypeError(
+                    f"expected {origin_type} for {key = }, got {type(data)}\n\t{data = }"
+                )
             elif error_mode == "try_convert":
                 return origin_type(data)
             elif error_mode == "ignore":
                 return data[key]
             else:
                 raise ValueError(f"error mode {error_mode} not recognized")
 
     return loader
 
 
 def dataclass_loader_factory(
-        cls,
-        special_loaders: Optional[dict[str, Callable[[JSONitem], Any]]] = None,
-        loader_types_override: Optional[dict[str, type]] = None,
-        # key_error_mode: ErrorMode = "except",
-        type_error_mode: TypeErrorMode = "except",
-    ) -> Callable[[JSONitem], Any]:
+    cls,
+    special_loaders: Optional[dict[str, Callable[[JSONitem], Any]]] = None,
+    loader_types_override: Optional[dict[str, type]] = None,
+    # key_error_mode: ErrorMode = "except",
+    type_error_mode: TypeErrorMode = "except",
+) -> Callable[[JSONitem], Any]:
     """returns a `.load()` method for a dataclass, recursively calling loader functions if found
-    
+
     where arguments present in `special_loaders` are loaded using the corresponding function
     functions in `special_loaders` should take a JSONitem (the whole dataset) and return an item
-    
+
 
     `type_error_mode` determines how to handle the JSON item type not matching the type hint of the dataclass field.
 
     ```
-    (not working) 
+    (not working)
     `key_error_mode` determines how to handle not being able to find the key in the JSONitem.
     for "warn" or "ignore", a `None` value is given to the key, unless a default exists~
     ```
     """
 
     # make it an empty dict if not provided
     if special_loaders is None:
         special_loaders = dict()
-    
+
     if loader_types_override is None:
         loader_types_override = dict()
 
     # check all loaders make sense
     for key in special_loaders:
         if key not in cls.__dataclass_fields__:
             raise ValueError(f"{key} is not a field of {cls}")
@@ -552,20 +551,27 @@
         # get the type hint for the field
         elif k in type_hints:
             # if it is a class with a `.load()` method, use that
             if isinstance(type_hints[k], type) and hasattr(type_hints[k], "load"):
                 k_loader: Callable = lambda data: type_hints[k].load(data[k])
                 # check the `load()` has the correct signature
                 k_loader_signature: inspect.Signature = inspect.signature(k_loader)
-                if len([
-                    True
-                    for p_name, p_cls in k_loader_signature.parameters.items()
-                    if p_cls.default == inspect._empty
-                ]) != 1:
-                    raise TypeError(f"`.load()` method for {k} has incorrect signature, expected exactly 1 argument without a default value:\n\t{k = }\n\t{k_loader = }\n\t{k_loader_signature = }\n\t{k_loader_signature.parameters = }")
+                if (
+                    len(
+                        [
+                            True
+                            for p_name, p_cls in k_loader_signature.parameters.items()
+                            if p_cls.default == inspect._empty
+                        ]
+                    )
+                    != 1
+                ):
+                    raise TypeError(
+                        f"`.load()` method for {k} has incorrect signature, expected exactly 1 argument without a default value:\n\t{k = }\n\t{k_loader = }\n\t{k_loader_signature = }\n\t{k_loader_signature.parameters = }"
+                    )
 
                 # set the load function if everything works
                 loader_funcs[k] = k_loader
             else:
                 # attempt to create a loader function for the type hint
                 typehint_k = type_hints[k]
                 if k in loader_types_override:
@@ -596,23 +602,22 @@
             raise TypeError(f"expected {cls}, got {type(loaded)}")
 
         return loaded
 
     return load
 
 
-
-
 def augement_dataclass_serializer_loader(
-        cls: Any = None,
-        /, *,
-        special_serializers: Optional[dict[str, Callable]] = None,
-        special_loaders: Optional[dict[str, Callable[[JSONitem], Any]]] = None,
-        load_type_error_mode: TypeErrorMode = "except",
-    ) -> Any:
+    cls: Any = None,
+    /,
+    *,
+    special_serializers: Optional[dict[str, Callable]] = None,
+    special_loaders: Optional[dict[str, Callable[[JSONitem], Any]]] = None,
+    load_type_error_mode: TypeErrorMode = "except",
+) -> Any:
     """adds a `.serialize()` and `.load()` method to a dataclass,
     using `dataclass_serializer_factory` and `dataclass_loader_factory`
 
     TODO: dynamically added methods dont show up as attributes during linting, and this makes the decorator suck.
     """
 
     def wrap(cls):
@@ -624,41 +629,41 @@
             cls,
             special_loaders=special_loaders,
             type_error_mode=load_type_error_mode,
         )
 
         return cls
 
-    # See if we're being called as `@augement_dataclass_serializer_loader` 
+    # See if we're being called as `@augement_dataclass_serializer_loader`
     # or `@augement_dataclass_serializer_loader()`.
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as `@augement_dataclass_serializer_loader` without parens.
     return wrap(cls)
 
-def _test():
 
+def _test():
     # @augement_dataclass_serializer_loader(
     #     special_serializers=dict(rand_data=lambda self: str(self.rand_data)),
     # )
     @dataclass
     class TestClass:
         a: int
         b: str
         c: float
         rand_data: Any = None
-    
+
     TestClass.serialize = dataclass_serializer_factory(
         TestClass,
         special_serializers=dict(rand_data=lambda self: str(self.rand_data)),
     )
     TestClass.load = dataclass_loader_factory(TestClass)
-    
+
     # @augement_dataclass_serializer_loader
     @dataclass
     class OuterTestClass:
         a2: int
         b2: str
         c2: float
         d2: TestClass
@@ -669,24 +674,22 @@
     item_a: TestClass = TestClass(a=1, b="x", c=3.0)
     item_b: OuterTestClass = OuterTestClass(a2=2, b2="y", c2=4.0, d2=item_a)
 
     print(f"{item_a = }")
     print(f"{item_a.serialize() = }")
     print(f"{item_b = }")
     print(f"{item_b.serialize() = }")
-    
+
     item_b_ser: JSONitem = item_b.serialize()
 
     item_b_loaded: OuterTestClass = OuterTestClass.load(item_b_ser)
 
     # assert item_b_loaded == item_b
     # assert item_b_loaded.d2 == item_a
 
     print(f"{item_b_loaded = }")
     print(f"{item_b_loaded.serialize() = }")
 
-if __name__ == '__main__':
-    print('# running tests')
-    _test()
-
 
-    
+if __name__ == "__main__":
+    print("# running tests")
+    _test()
```

### Comparing `muutils-0.4.2/muutils/_wip/lazy_externals.py` & `muutils-0.4.3/muutils/_wip/lazy_externals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class LazyExternalLoader:
     """lazy load np arrays or jsonl files, similar tp NpzFile from np.lib
 
     initialize with zipfile object and zanj metadata (for list of externals)
     """
 
     def __init__(
@@ -28,30 +27,27 @@
     def __getitem__(self, key: str) -> Any:
         if key in self._externals_types:
             item_type: str = self._externals_types[key]
             with self._zipf.open(key, "r") as fp:
                 return GET_EXTERNAL_LOAD_FUNC(item_type)(self._loaded_zanj, fp)
 
 
-
-
-# TODO: this needs to be refactored 
+# TODO: this needs to be refactored
 class LoadedZANJ(typing.Mapping):
     """object loaded from ZANJ archive. acts like a dict."""
 
     def __init__(
         self,
         # config
         path: str | Path,
         zanj: _ZANJ_pre,
         loader_handlers: dict[str, LoaderHandler] | None = None,
         externals_mode: ExternalsLoadingMode = "lazy",
         format_error_mode: ErrorMode = "warn",
     ) -> None:
-
         # copy handlers
         self._loader_handlers: dict[str, LoaderHandler]
         if loader_handlers is not None:
             self._loader_handlers = loader_handlers
         else:
             self._loader_handlers = LOADER_MAP
```

### Comparing `muutils-0.4.2/muutils/_wip/newargparser.py` & `muutils-0.4.3/muutils/_wip/newargparser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,368 @@
-from typing import (
-	Callable, get_type_hints, Any, Union, Annotated, Optional, _SpecialForm, _type_check
-)
 import inspect
 import sys
 from copy import deepcopy
 from dataclasses import dataclass
+from typing import (
+    Annotated,
+    Any,
+    Callable,
+    Optional,
+    Union,
+    _SpecialForm,
+    _type_check,
+    get_type_hints,
+)
 
 
+class Description(str):
+    pass
 
 
-class Description(str): pass
 class ArgProcessor:
-	def __init__(self, func) -> None:
-		self.func = func
-	
-	def __call__(self, *args, **kwargs) -> Any:
-		return self.func(*args, **kwargs)
+    def __init__(self, func) -> None:
+        self.func = func
+
+    def __call__(self, *args, **kwargs) -> Any:
+        return self.func(*args, **kwargs)
+
 
 # Description: Callable[[str], type] = lambda x : NewType(x, str)(x)
 
-class NoValue: pass
+
+class NoValue:
+    pass
+
 
 @_SpecialForm
 def NoValueOptional(self, parameters):
     arg = _type_check(parameters, f"{self} requires a single type.")
     return Union[arg, NoValue]
 
+
 @dataclass
 class ArgumentSignature:
-	"""signature and metadata about a function argument"""
-	name : str
-	keyword_only : bool
-	positional_only : bool
-	type : NoValueOptional[type] = NoValue
-	default : NoValueOptional[Any] = NoValue
-	description : Optional[str] = None
-	processor : NoValueOptional[ArgProcessor] = NoValue
-
-	def to_docstring_item(self) -> str:
-		desc_processed: str = self.description.replace('\n', '\n\t') if self.description is not None else ''
-		if not isinstance(self.default, NoValue):
-			return f" - `{self.name} : {self.type.__name__}` {desc_processed} "
-		else:
-			return f" - `{self.name} : {self.type.__name__} = {self.default}` {desc_processed} "
+    """signature and metadata about a function argument"""
+
+    name: str
+    keyword_only: bool
+    positional_only: bool
+    type: NoValueOptional[type] = NoValue
+    default: NoValueOptional[Any] = NoValue
+    description: Optional[str] = None
+    processor: NoValueOptional[ArgProcessor] = NoValue
+
+    def to_docstring_item(self) -> str:
+        desc_processed: str = (
+            self.description.replace("\n", "\n\t")
+            if self.description is not None
+            else ""
+        )
+        if not isinstance(self.default, NoValue):
+            return f" - `{self.name} : {self.type.__name__}` {desc_processed} "
+        else:
+            return f" - `{self.name} : {self.type.__name__} = {self.default}` {desc_processed} "
+
 
 @dataclass
 class FunctionSignature:
-	"""signature and metadata about a function"""
-	name : str
-	doc : str
-	args : list[ArgumentSignature]
-	return_type : type
-
-	@property
-	def args_positional(self) -> list[ArgumentSignature]:
-		return [a for a in self.args if not a.keyword_only]
-	
-	@property
-	def args_pos_only(self) -> list[ArgumentSignature]:
-		return [x for x in self.args if x.positional_only]
-	
-	@property
-	def args_kw_only(self) -> list[ArgumentSignature]:
-		return [x for x in self.args if x.keyword_only]
-
-
-	def to_docstring(self) -> str:
-		return '\n'.join([
-			self.doc or '',
-			'# Arguments:',
-			'\n'.join([x.to_docstring_item() for x in self.args]),
-			'# Returns:',
-			f'return : {self.return_type}',
-		])
-
-
-
-
-def process_signature(func : Callable) -> None:
-
-	argspec: inspect.FullArgSpec = inspect.getfullargspec(func)
-
-	# print(json.dumps(json_serialize(argspec), indent=4))
-	args_all_names: list[str] = argspec.args
-	if argspec.varargs is not None:
-		args_all_names.append('*' + argspec.varargs)
-	args_all_names.extend(argspec.kwonlyargs)
-	if argspec.varkw is not None:
-		args_all_names.append('**' + argspec.varkw)
-	
-	# get the base type signatures
-	# ==============================
-	args_types : dict[str,type] = get_type_hints(func)
-
-	# get default values
-	# ==============================
-	args_defaults : dict[str, Any] = dict()
-	# chop the values without default values from `argspec.args`
-	ordered_args_with_defaults : list[str] = deepcopy(argspec.args[:-len(argspec.defaults)])
-	# zip them up with defaults and add them to dict
-	for arg, default in zip(ordered_args_with_defaults, argspec.defaults):
-		args_defaults[arg] = default
-	# add keyword only args
-	args_defaults.update({
-		arg : default
-		for arg, default in zip(argspec.kwonlyargs, argspec.kwonlydefaults)
-	})
-
-	
-	# get the annotations
-	# ==============================
-	args_annotations : dict[str,tuple] = {
-		k : v.__metadata__
-		for k,v in get_type_hints(func, include_extras=True).items()
-		if hasattr(v, '__metadata__')
-	}
-
-	# get the descriptions, by getting all strings in the annotation
-	# ==============================
-	args_descriptions : dict[str, Description] = dict()
-	for k,v in args_annotations.items():
-		desc_items : list[str] = [
-			x
-			for x in v
-			if isinstance(x, (str, Description))
-		]
-		# if anything found
-		if len(desc_items) > 0:
-			args_descriptions[k] = Description('\n'.join(desc_items))
-
-	# get the processors, by getting only things marked as `ArgProcessor`
-	# ==============================
-	args_processors : dict[str,ArgProcessor] = dict()
-	for k,v in args_annotations.items():
-		if isinstance(v, ArgProcessor):
-			args_processors[k] = v
-
-
-	args: list[ArgumentSignature] = [
-		ArgumentSignature(
-			name = arg,
-			keyword_only = arg in argspec.kwonlyargs,
-			positional_only = False,
-			type = args_types.get(arg, Any),
-			default = args_defaults.get(arg, NoValue),
-			description = args_descriptions.get(arg, None),
-			processor = args_processors.get(arg, NoValue),
-		)
-		for arg in argspec.args
-	]
-	
-	return FunctionSignature(
-		name=func.__name__,
-		doc=func.__doc__,
-		args=args,
-		return_type=func.__annotations__['return'],
-	)
+    """signature and metadata about a function"""
 
+    name: str
+    doc: str
+    args: list[ArgumentSignature]
+    return_type: type
+
+    @property
+    def args_positional(self) -> list[ArgumentSignature]:
+        return [a for a in self.args if not a.keyword_only]
+
+    @property
+    def args_pos_only(self) -> list[ArgumentSignature]:
+        return [x for x in self.args if x.positional_only]
+
+    @property
+    def args_kw_only(self) -> list[ArgumentSignature]:
+        return [x for x in self.args if x.keyword_only]
+
+    def to_docstring(self) -> str:
+        return "\n".join(
+            [
+                self.doc or "",
+                "# Arguments:",
+                "\n".join([x.to_docstring_item() for x in self.args]),
+                "# Returns:",
+                f"return : {self.return_type}",
+            ]
+        )
+
+
+def process_signature(func: Callable) -> None:
+    argspec: inspect.FullArgSpec = inspect.getfullargspec(func)
+
+    # print(json.dumps(json_serialize(argspec), indent=4))
+    args_all_names: list[str] = argspec.args
+    if argspec.varargs is not None:
+        args_all_names.append("*" + argspec.varargs)
+    args_all_names.extend(argspec.kwonlyargs)
+    if argspec.varkw is not None:
+        args_all_names.append("**" + argspec.varkw)
+
+    # get the base type signatures
+    # ==============================
+    args_types: dict[str, type] = get_type_hints(func)
+
+    # get default values
+    # ==============================
+    args_defaults: dict[str, Any] = dict()
+    # chop the values without default values from `argspec.args`
+    ordered_args_with_defaults: list[str] = deepcopy(
+        argspec.args[: -len(argspec.defaults)]
+    )
+    # zip them up with defaults and add them to dict
+    for arg, default in zip(ordered_args_with_defaults, argspec.defaults):
+        args_defaults[arg] = default
+    # add keyword only args
+    args_defaults.update(
+        {
+            arg: default
+            for arg, default in zip(argspec.kwonlyargs, argspec.kwonlydefaults)
+        }
+    )
+
+    # get the annotations
+    # ==============================
+    args_annotations: dict[str, tuple] = {
+        k: v.__metadata__
+        for k, v in get_type_hints(func, include_extras=True).items()
+        if hasattr(v, "__metadata__")
+    }
+
+    # get the descriptions, by getting all strings in the annotation
+    # ==============================
+    args_descriptions: dict[str, Description] = dict()
+    for k, v in args_annotations.items():
+        desc_items: list[str] = [x for x in v if isinstance(x, (str, Description))]
+        # if anything found
+        if len(desc_items) > 0:
+            args_descriptions[k] = Description("\n".join(desc_items))
+
+    # get the processors, by getting only things marked as `ArgProcessor`
+    # ==============================
+    args_processors: dict[str, ArgProcessor] = dict()
+    for k, v in args_annotations.items():
+        if isinstance(v, ArgProcessor):
+            args_processors[k] = v
+
+    args: list[ArgumentSignature] = [
+        ArgumentSignature(
+            name=arg,
+            keyword_only=arg in argspec.kwonlyargs,
+            positional_only=False,
+            type=args_types.get(arg, Any),
+            default=args_defaults.get(arg, NoValue),
+            description=args_descriptions.get(arg, None),
+            processor=args_processors.get(arg, NoValue),
+        )
+        for arg in argspec.args
+    ]
+
+    return FunctionSignature(
+        name=func.__name__,
+        doc=func.__doc__,
+        args=args,
+        return_type=func.__annotations__["return"],
+    )
 
 
 # use functools.wraps
-def docstring_updater(func : Callable) -> Callable:
-	signature: FunctionSignature = process_signature(func)
-	func.__doc__ = signature.to_docstring()
-	return func
+def docstring_updater(func: Callable) -> Callable:
+    signature: FunctionSignature = process_signature(func)
+    func.__doc__ = signature.to_docstring()
+    return func
 
 
 @docstring_updater
 def main(
-        dumb_file : str,
-        /,
-		no_default : Annotated[str, 'this has no deafault', 'lol'],
-        use_erdos: Annotated[bool, 
-			'asdkljasdkljsad',
-			ArgProcessor(lambda x: 
-				bool(x.lower() == 'true')
-				if isinstance(x,str)
-				else bool(x)
-			),
-		] = False,
-        # index_file: str = 'example_data/example_index.index',
-        index_file: str = "/mnt/ssd-0/lichess/preprocessed/25M_high_elo.index",
-        output_folder: str = "example_data",
-        num_games: int = 100,
-        *,
-        keyword_only_arg : str = "default string",
-    ) -> bool:
-	"""base docstring"""
+    dumb_file: str,
+    /,
+    no_default: Annotated[str, "this has no deafault", "lol"],
+    use_erdos: Annotated[
+        bool,
+        "asdkljasdkljsad",
+        ArgProcessor(
+            lambda x: bool(x.lower() == "true") if isinstance(x, str) else bool(x)
+        ),
+    ] = False,
+    # index_file: str = 'example_data/example_index.index',
+    index_file: str = "/mnt/ssd-0/lichess/preprocessed/25M_high_elo.index",
+    output_folder: str = "example_data",
+    num_games: int = 100,
+    *,
+    keyword_only_arg: str = "default string",
+) -> bool:
+    """base docstring"""
 
-	pass
+    pass
 
 
 @docstring_updater
 def main_other(
-        dumb_file : str,
-        /,
-		use_erdos: bool = False,
-        *args,
-		keyword_only_arg : str = "default string",
-        **kwargs,
-    ) -> bool:
-
-	pass
+    dumb_file: str,
+    /,
+    use_erdos: bool = False,
+    *args,
+    keyword_only_arg: str = "default string",
+    **kwargs,
+) -> bool:
+    pass
 
 
 @docstring_updater
 def main_third(
-		another_dumb : str,
-        dumb_file : str = 'default value for no-keyword arg',
-		n_things : int = 10,
-        /,
-        use_erdos: Annotated[bool, 
-			'asdkljasdkljsad',
-			ArgProcessor(lambda x: 
-				bool(x.lower() == 'true')
-				if isinstance(x,str)
-				else bool(x)
-			),
-		] = False,
-        # index_file: str = 'example_data/example_index.index',
-        index_file: str = "/mnt/ssd-0/lichess/preprocessed/25M_high_elo.index",
-        output_folder: str = "example_data",
-        num_games: int = 100,
-        *,
-        keyword_only_arg : str = "default string",
-    ) -> bool:
+    another_dumb: str,
+    dumb_file: str = "default value for no-keyword arg",
+    n_things: int = 10,
+    /,
+    use_erdos: Annotated[
+        bool,
+        "asdkljasdkljsad",
+        ArgProcessor(
+            lambda x: bool(x.lower() == "true") if isinstance(x, str) else bool(x)
+        ),
+    ] = False,
+    # index_file: str = 'example_data/example_index.index',
+    index_file: str = "/mnt/ssd-0/lichess/preprocessed/25M_high_elo.index",
+    output_folder: str = "example_data",
+    num_games: int = 100,
+    *,
+    keyword_only_arg: str = "default string",
+) -> bool:
+    pass
 
-	pass
 
+JSONData = Union[bool, int, float, str, list, dict]
 
 
-JSONData = Union[bool, int, float, str, list, dict]
+def substring_mask(data: str, quote_symbol: str = "'") -> list[bool]:
+    """iterate over a string, returning a list of bools on whether each character is within quotes"""
 
+    output: list[bool] = list()
 
-def substring_mask(data: str, quote_symbol:str = "'") -> list[bool]:
-	"""iterate over a string, returning a list of bools on whether each character is within quotes"""
+    # start by assuming we're not in a string
+    in_string_current: bool = False
+    in_string_next: bool = False
+    is_escaped: bool = False
+
+    # iterate over the string
+    for i, c in enumerate(data):
+        # handle escape chars
+        if is_escaped:
+            is_escaped = False
+        elif c == "\\":
+            is_escaped = True
+        elif not in_string_current and c == quote_symbol:
+            # if we're not in a string and we see a quote, we're in a string
+            in_string_current = True
+            in_string_next = True
+        elif in_string_current and c == quote_symbol:
+            # if we're in a string and we see a quote, we're no longer in a string
+            in_string_current = True
+            in_string_next = False
+        elif not in_string_current:
+            # if we're not in a string, add the character to the output
+            pass
+        else:
+            # if we're in a string, ignore the character
+            pass
 
-	output: list[bool] = list()
-	
-	# start by assuming we're not in a string
-	in_string_current: bool = False
-	in_string_next: bool = False
-	is_escaped: bool = False
-
-	# iterate over the string
-	for i,c in enumerate(data):
-		# handle escape chars
-		if is_escaped:
-			is_escaped = False
-		elif c == '\\':
-			is_escaped = True
-		elif not in_string_current and c == quote_symbol:
-			# if we're not in a string and we see a quote, we're in a string
-			in_string_current = True
-			in_string_next = True
-		elif in_string_current and c == quote_symbol:
-			# if we're in a string and we see a quote, we're no longer in a string
-			in_string_current = True
-			in_string_next = False
-		elif not in_string_current:
-			# if we're not in a string, add the character to the output
-			pass
-		else:
-			# if we're in a string, ignore the character
-			pass
-		
-		print(i, c, '\t', in_string_current)
-		output.append(in_string_current)
+        print(i, c, "\t", in_string_current)
+        output.append(in_string_current)
 
-		in_string_current = in_string_next
+        in_string_current = in_string_next
 
-	return output
+    return output
 
 
 def split_Lmask(data: str, mask: bool) -> tuple[list[str], list[bool]]:
-	"""given a mask, split the data into runs of strings which either are or are not masked"""
+    """given a mask, split the data into runs of strings which either are or are not masked"""
 
-	output_strings: list[str] = list()
-	output_masks: list[bool] = list()
-	
-	prev_mask: Optional[bool] = None
-
-	for (c,m) in zip(data, mask):
-		if prev_mask is None:
-			# if none, we are at the start of a string. start a new run
-			prev_mask = m
-			output_masks.append(m)
-			output_strings.append(c)
-		
-		elif m == prev_mask:
-			# continue the last run
-			assert m == output_masks[-1]
-			output_strings[-1] += c
-			
-		else:
-			# start a new run
-			output_masks.append(m)
-			output_strings.append(c)
-			prev_mask = m
+    output_strings: list[str] = list()
+    output_masks: list[bool] = list()
 
-	return output_strings, output_masks
+    prev_mask: Optional[bool] = None
 
-def invert_mask(mask: list[bool]) -> list[bool]:
-	"""invert a mask"""
-	return [not x for x in mask]
+    for c, m in zip(data, mask):
+        if prev_mask is None:
+            # if none, we are at the start of a string. start a new run
+            prev_mask = m
+            output_masks.append(m)
+            output_strings.append(c)
+
+        elif m == prev_mask:
+            # continue the last run
+            assert m == output_masks[-1]
+            output_strings[-1] += c
+
+        else:
+            # start a new run
+            output_masks.append(m)
+            output_strings.append(c)
+            prev_mask = m
 
+    return output_strings, output_masks
 
-def display_str_with_mask(data: str) -> None:
 
-	mask = substring_mask(data)
-	print(data)
-	print(''.join(['*' if x else ' ' for x in mask]))
+def invert_mask(mask: list[bool]) -> list[bool]:
+    """invert a mask"""
+    return [not x for x in mask]
+
 
+def display_str_with_mask(data: str) -> None:
+    mask = substring_mask(data)
+    print(data)
+    print("".join(["*" if x else " " for x in mask]))
 
 
 def apply_replace_within_Lmask(
-		data: list[str], 
-		mask: list[bool], 
-		replace_from: str,
-		replace_to: str,
-	) -> str:
-	"""apply a replace to a string, but only within a mask"""
-	
-	output: list[str] = list()
-
-	for (c,m) in zip(data, mask):
-		if m:
-			output.append(c.replace(replace_from, replace_to))
-		else:
-			output.append(c)
-		
-	return output
+    data: list[str],
+    mask: list[bool],
+    replace_from: str,
+    replace_to: str,
+) -> str:
+    """apply a replace to a string, but only within a mask"""
+
+    output: list[str] = list()
+
+    for c, m in zip(data, mask):
+        if m:
+            output.append(c.replace(replace_from, replace_to))
+        else:
+            output.append(c)
 
+    return output
 
-def argv_json_preprocessor(data: str) -> str:
-	pass
 
+def argv_json_preprocessor(data: str) -> str:
+    pass
 
 
 def custom_json_loader(data: str) -> JSONData:
-	# first, isolate all indices
-
-	pass
-
-if __name__ == '__main__':
-	data = ' '.join(sys.argv)
-	display_str_with_mask(data)
-	print(split_into_runs(data, substring_mask(data)))
-
+    # first, isolate all indices
 
+    pass
 
 
+if __name__ == "__main__":
+    data = " ".join(sys.argv)
+    display_str_with_mask(data)
+    print(split_into_runs(data, substring_mask(data)))
 
 
-# process_signature(main)	
+# process_signature(main)
 # process_signature(main_other)
 # process_signature(main_third)
 
 
 # print(main.__name__)
 # print(main.__doc__)
 # print('\n\n\n')
```

### Comparing `muutils-0.4.2/muutils/_wip/torch_util_old.py` & `muutils-0.4.3/muutils/_wip/torch_util_old.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -200,8 +200,8 @@
         "state_dict": jser.json_serialize(
             data.state_dict(), tuple(path) + ("state_dict",)
         ),
         "_modules": {k: str(v) for k, v in data._modules.items()},
         "__dict__": {k: str(v) for k, v in data.__dict__.items()},
     }
 
-    return jser.json_serialize(output)
+    return jser.json_serialize(output)
```

### Comparing `muutils-0.4.2/muutils/dictmagic.py` & `muutils-0.4.3/muutils/dictmagic.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/group_equiv.py` & `muutils-0.4.3/muutils/group_equiv.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,24 @@
 def group_by_equivalence(
     items_in: Sequence[T],
     eq_func: Callable[[T, T], bool],
 ) -> list[list[T]]:
     """group items by assuming that `eq_func` implies an equivalence relation but might not be transitive
 
     so, if f(a,b) and f(b,c) then f(a,c) might be false, but we still want to put [a,b,c] in the same class
+
+    note that lists are used to avoid the need for hashable items, and to allow for duplicates
+
+    # Arguments
+     - `items_in: Sequence[T]` the items to group
+     - `eq_func: Callable[[T, T], bool]` a function that returns true if two items are equivalent. need not be transitive
     """
 
     items: list[T] = list(items_in)
+    items.reverse()
     output: list[list[T]] = list()
 
     while items:
         x: T = items.pop()
 
         # try to add to an existing class
         found_classes: list[int] = list()
@@ -42,13 +49,14 @@
                     output_new.append(c)
 
             # then merge them back in, along with the element `x`
             merged: list[T] = list(chain.from_iterable(to_merge))
             merged.append(x)
 
             output_new.append(merged)
+            output = output_new
 
         # if no class found, make a new one
         else:
             output.append([x])
 
     return output
```

### Comparing `muutils-0.4.2/muutils/json_serialize/__init__.py` & `muutils-0.4.3/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/json_serialize/array.py` & `muutils-0.4.3/muutils/json_serialize/array.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/json_serialize/dataclass_factories.py` & `muutils-0.4.3/muutils/json_serialize/dataclass_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import typing
 import warnings
 from typing import Any, Callable, Optional, Sequence, Union
 
 from muutils.json_serialize.json_serialize import JsonSerializer
 from muutils.json_serialize.util import JSONdict, JSONitem, MonoTuple, TypeErrorMode
 
+warnings.warn(
+    "this module is deprecated, use `muutils.json_serialize.SerializableDataclass` instead",
+    DeprecationWarning,
+)
+
 # pylint: disable=pointless-string-statement, unreachable, import-outside-toplevel, consider-using-dict-items
 
 
 def dataclass_serializer_factory(
     cls,
     special_serializers: Optional[dict[str, Callable]] = None,
     fields_exclude: Optional[Sequence[str]] = None,
```

### Comparing `muutils-0.4.2/muutils/json_serialize/json_serialize.py` & `muutils-0.4.3/muutils/json_serialize/json_serialize.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.4.3/muutils/json_serialize/serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/json_serialize/util.py` & `muutils-0.4.3/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/jsonlines.py` & `muutils-0.4.3/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/exception_context.py` & `muutils-0.4.3/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/headerfuncs.py` & `muutils-0.4.3/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/log_util.py` & `muutils-0.4.3/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/logger.py` & `muutils-0.4.3/muutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/loggingstream.py` & `muutils-0.4.3/muutils/logger/loggingstream.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/simplelogger.py` & `muutils-0.4.3/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/logger/timing.py` & `muutils-0.4.3/muutils/logger/timing.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/misc.py` & `muutils-0.4.3/muutils/misc.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/mlutils.py` & `muutils-0.4.3/muutils/mlutils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/nbutils/configure_notebook.py` & `muutils-0.4.3/muutils/nbutils/configure_notebook.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/nbutils/convert_ipynb_to_script.py` & `muutils-0.4.3/muutils/nbutils/convert_ipynb_to_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 DISABLE_PLOTS_WARNING: list[str] = [
     """
 # ------------------------------------------------------------
 # WARNING: this script is auto-generated by `convert_ipynb_to_script.py`
 # showing plots has been disabled, so this is presumably in a temp dict for CI or something
 # so don't modify this code, it will be overwritten!
 # ------------------------------------------------------------
-"""
+""".lstrip()
 ]
 
 
 def disable_plots_in_script(script_lines: list[str]) -> list[str]:
     """Disable plots in a script by adding cursed things after the import statements"""
     result_str_TEMP: str = "\n\n".join(script_lines)
     script_lines_new: list[str] = script_lines
```

### Comparing `muutils-0.4.2/muutils/nbutils/run_notebook_tests.py` & `muutils-0.4.3/muutils/nbutils/run_notebook_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from pathlib import Path
 
 
 class NotebookTestError(Exception):
     pass
 
 
-def test_notebooks(
+def run_notebook_tests(
     notebooks_dir: Path,
     converted_notebooks_temp_dir: Path,
     CI_output_suffix: str = ".CI-output.txt",
+    run_python_cmd: str = "poetry run python",
 ):
+    original_cwd: Path = Path.cwd()
     # get paths
     notebooks_dir = Path(notebooks_dir)
     converted_notebooks_temp_dir = Path(converted_notebooks_temp_dir)
     root_relative_to_notebooks: Path = Path(os.path.relpath(".", notebooks_dir))
 
     print(f"testing notebooks in '{notebooks_dir}'")
     print(f"reading converted notebooks from '{converted_notebooks_temp_dir}'")
@@ -60,15 +62,15 @@
 
         for file in converted_notebooks:
             # run the file
             print(f"  Running {file}")
             output_file: Path = file.with_suffix(CI_output_suffix)
             print(f"  Output in {output_file}")
 
-            command: str = f"poetry run python {root_relative_to_notebooks / file} > {root_relative_to_notebooks / output_file} 2>&1"
+            command: str = f"{run_python_cmd} {root_relative_to_notebooks / file} > {root_relative_to_notebooks / output_file} 2>&1"
             process: subprocess.CompletedProcess = subprocess.run(
                 command, shell=True, text=True
             )
 
             print(f"  Run completed with return code {process.returncode}")
 
             # print the output of the file to the console if it failed
@@ -80,14 +82,17 @@
             del process
 
     except NotebookTestError as e:
         print("!" * 50, file=sys.stderr)
         print(e, file=sys.stderr)
         print("!" * 50, file=sys.stderr)
         raise e
+    finally:
+        # return to original cwd
+        os.chdir(original_cwd)
 
 
 if __name__ == "__main__":
     import argparse
 
     parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
@@ -100,11 +105,11 @@
         "--converted-notebooks-temp-dir",
         type=str,
         help="The directory containing the converted notebooks to test",
     )
 
     args: argparse.Namespace = parser.parse_args()
 
-    test_notebooks(
+    run_notebook_tests(
         Path(args.notebooks_dir),
         Path(args.converted_notebooks_temp_dir),
     )
```

### Comparing `muutils-0.4.2/muutils/statcounter.py` & `muutils-0.4.3/muutils/statcounter.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/muutils/sysinfo.py` & `muutils-0.4.3/muutils/sysinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         if git_status["stderr"].startswith("fatal: not a git repository"):
             return {
                 "git version": git_version["stdout"],
                 "git status": git_status,
             }
         else:
             return {
+                "git version": git_version["stdout"],
                 "git status": git_status,
                 "git branch": _popen(["git", "branch"], split_out=True),
                 "git remote -v": _popen(["git", "remote", "-v"], split_out=True),
                 "git log": _popen(["git", "log"]),
             }
 
     @classmethod
```

### Comparing `muutils-0.4.2/muutils/tensor_utils.py` & `muutils-0.4.3/muutils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.2/pyproject.toml` & `muutils-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "muutils"
-version = "0.4.2"
+version = "0.4.3"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 repository = "https://github.com/mivanit/muutils"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,27 +25,33 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 pylint = "^2.16.4"
 pycln = "^2.1.3"
 isort = "^5.12.0"
 mypy = "^1.0.1"
+pytest-cov = "^4.1.0"
+coverage-badge = "^1.1.0"
+matplotlib = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+# TODO: make all of the following ignored across all formatting/linting
+# tests/input_data, tests/junk_data, muutils/_wip 
+
 [tool.pycln]
 all = true
-exclude = "_wip"
+exclude = "tests/input_data"
 
 [tool.isort]
 profile = "black"
 ignore_comments = false
-extend_skip = ["_wip"]
+extend_skip = "tests/input_data"
 
 [tool.black]
-extend-exclude = "_wip"
+extend-exclude = "tests/input_data"
 
 [tool.mypy]
-exclude = ['_wip']
+exclude = ['_wip', "tests/input_data", "tests/junk_data"]
 show_error_codes = true
```

### Comparing `muutils-0.4.2/README.md` & `muutils-0.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-
-
-`muutils`, stylized as "$\mu$utils" or "μutils", is a collection of miscellaneous python utilities, meant to be small and with ~~no~~ minimal dependencies outside of standard python.
-
-
-- [`json_serialize`](https://github.com/mivanit/muutils/tree/main/muutils/json_serialize.py) is a tool for serializing and loading arbitrary python objects into json. plays nicely with [`ZANJ`](https://github.com/mivanit/ZANJ/)
-- [`statcounter`](https://github.com/mivanit/muutils/tree/main/muutils/statcounter.py) is an extension of `collections.Counter` that provides "smart" computation of stats (mean, variance, median, other percentiles) from the counter object without using `Counter.elements()`
-- `misc` contains a few utilities:
-	- `stable_hash()` uses `hashlib.sha256` to compute a hash of an object that is stable across runs of python
-	- `sanitize_fname()` takes any string and makes it only alphanumeric plus `-` and `_`
-	- `shorten_numerical_to_str()` turns numbers like `123456789` into `"123M"`
-	- a couple other things
-- [`nbutils`] (WIP) contains some utilities for working in notebooks (printing latex nicely) and also running notebooks as tests in CI by converting them to python scripts
-- [`tensor_utils`] contains minor utilities for working with pytorch tensors and numpy arrays. This needs to be moved into ZANJ, probably
-- [`group_equiv`](https://github.com/mivanit/muutils/tree/main/muutils/group_equiv.py) groups elements from a sequence according to a given equivalence relation, without assuming that the equivalence relation obeys the transitive property
-- [`logger`](https://github.com/mivanit/muutils/tree/main/muutils/logger.py) implements a logger with "streams" and a timer context manager
-- [`jsonlines`](https://github.com/mivanit/muutils/tree/main/muutils/jsonlines.py) extremely simple utility for reading/writing `jsonl` files
-- [`ZANJ`](https://github.com/mivanit/ZANJ/) is a WIP hdf5 alternative. This ~~will probably be~~ has been spun off into its own repo
-
-There are a couple work-in-progress utilities in [`_wip`](https://github.com/mivanit/muutils/tree/main/muutils/_wip/) that aren't ready for anything, but nothing in this repo is suitable for production. Use at your own risk!
-
-
-# installation
-
-PyPi: [muutils](https://pypi.org/project/muutils/)
-
-```
-pip install muutils
-```
+[![PyPI](https://img.shields.io/pypi/v/muutils)](https://pypi.org/project/muutils/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/muutils)
+
+[![Checks](https://github.com/mivanit/muutils/actions/workflows/checks.yml/badge.svg)](https://github.com/mivanit/muutils/actions/workflows/checks.yml)
+[![Coverage](docs/coverage/coverage.svg)](docs/coverage/coverage.txt)
+
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mivanit/muutils)
+![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/mivanit/muutils)
+![code size, bytes](https://img.shields.io/github/languages/code-size/mivanit/muutils)
+<!-- ![Lines of code](https://img.shields.io/tokei/lines/github.com/mivanit/muutils) -->
+
+`muutils`, stylized as "$\mu$utils" or "μutils", is a collection of miscellaneous python utilities, meant to be small and with ~~no~~ minimal dependencies outside of standard python.
+
+
+- [`json_serialize`](https://github.com/mivanit/muutils/tree/main/muutils/json_serialize.py) is a tool for serializing and loading arbitrary python objects into json. plays nicely with [`ZANJ`](https://github.com/mivanit/ZANJ/)
+- [`statcounter`](https://github.com/mivanit/muutils/tree/main/muutils/statcounter.py) is an extension of `collections.Counter` that provides "smart" computation of stats (mean, variance, median, other percentiles) from the counter object without using `Counter.elements()`
+- `misc` contains a few utilities:
+	- `stable_hash()` uses `hashlib.sha256` to compute a hash of an object that is stable across runs of python
+	- `sanitize_fname()` takes any string and makes it only alphanumeric plus `-` and `_`
+	- `shorten_numerical_to_str()` turns numbers like `123456789` into `"123M"`
+	- a couple other things
+- [`nbutils`] (WIP) contains some utilities for working in notebooks (printing latex nicely) and also running notebooks as tests in CI by converting them to python scripts
+- [`tensor_utils`] contains minor utilities for working with pytorch tensors and numpy arrays. This needs to be moved into ZANJ, probably
+- [`group_equiv`](https://github.com/mivanit/muutils/tree/main/muutils/group_equiv.py) groups elements from a sequence according to a given equivalence relation, without assuming that the equivalence relation obeys the transitive property
+- [`logger`](https://github.com/mivanit/muutils/tree/main/muutils/logger.py) implements a logger with "streams" and a timer context manager
+- [`jsonlines`](https://github.com/mivanit/muutils/tree/main/muutils/jsonlines.py) extremely simple utility for reading/writing `jsonl` files
+- [`ZANJ`](https://github.com/mivanit/ZANJ/) is a WIP hdf5 alternative. This ~~will probably be~~ has been spun off into its own repo
+
+There are a couple work-in-progress utilities in [`_wip`](https://github.com/mivanit/muutils/tree/main/muutils/_wip/) that aren't ready for anything, but nothing in this repo is suitable for production. Use at your own risk!
+
+
+# installation
+
+PyPi: [muutils](https://pypi.org/project/muutils/)
+
+```
+pip install muutils
+```
```

### Comparing `muutils-0.4.2/PKG-INFO` & `muutils-0.4.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.4.2
+Version: 0.4.3
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jaxtyping (>=0.2.12,<0.3.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/muutils
 Description-Content-Type: text/markdown
 
+[![PyPI](https://img.shields.io/pypi/v/muutils)](https://pypi.org/project/muutils/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/muutils)
+
+[![Checks](https://github.com/mivanit/muutils/actions/workflows/checks.yml/badge.svg)](https://github.com/mivanit/muutils/actions/workflows/checks.yml)
+[![Coverage](docs/coverage/coverage.svg)](docs/coverage/coverage.txt)
 
+![GitHub commit activity](https://img.shields.io/github/commit-activity/t/mivanit/muutils)
+![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/mivanit/muutils)
+![code size, bytes](https://img.shields.io/github/languages/code-size/mivanit/muutils)
+<!-- ![Lines of code](https://img.shields.io/tokei/lines/github.com/mivanit/muutils) -->
 
 `muutils`, stylized as "$\mu$utils" or "μutils", is a collection of miscellaneous python utilities, meant to be small and with ~~no~~ minimal dependencies outside of standard python.
 
 
 - [`json_serialize`](https://github.com/mivanit/muutils/tree/main/muutils/json_serialize.py) is a tool for serializing and loading arbitrary python objects into json. plays nicely with [`ZANJ`](https://github.com/mivanit/ZANJ/)
 - [`statcounter`](https://github.com/mivanit/muutils/tree/main/muutils/statcounter.py) is an extension of `collections.Counter` that provides "smart" computation of stats (mean, variance, median, other percentiles) from the counter object without using `Counter.elements()`
 - `misc` contains a few utilities:
```

