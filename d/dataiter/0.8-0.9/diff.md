# Comparing `tmp/dataiter-0.8.tar.gz` & `tmp/dataiter-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataiter-0.8.tar", last modified: Sun May 10 18:09:12 2020, max compression
+gzip compressed data, was "dist/dataiter-0.9.tar", last modified: Mon May 11 19:36:32 2020, max compression
```

## Comparing `dataiter-0.8.tar` & `dataiter-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-10 18:09:12.833070 dataiter-0.8/
--rw-r--r--   0 osmo      (1000) osmo      (1000)     3505 2020-05-10 18:09:12.833070 dataiter-0.8/PKG-INFO
--rw-r--r--   0 osmo      (1000) osmo      (1000)     2575 2020-05-10 17:53:59.000000 dataiter-0.8/README.md
-drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-10 18:09:12.833070 dataiter-0.8/dataiter/
--rw-r--r--   0 osmo      (1000) osmo      (1000)     1666 2020-05-10 18:07:53.000000 dataiter-0.8/dataiter/__init__.py
--rw-r--r--   0 osmo      (1000) osmo      (1000)     6243 2020-05-10 17:55:08.000000 dataiter-0.8/dataiter/array.py
--rw-r--r--   0 osmo      (1000) osmo      (1000)    18055 2020-05-10 18:04:11.000000 dataiter-0.8/dataiter/data_frame.py
--rw-r--r--   0 osmo      (1000) osmo      (1000)     1910 2020-05-10 17:52:17.000000 dataiter-0.8/dataiter/deco.py
--rw-r--r--   0 osmo      (1000) osmo      (1000)    14033 2020-05-10 18:06:40.000000 dataiter-0.8/dataiter/list_of_dicts.py
--rw-r--r--   0 osmo      (1000) osmo      (1000)     2116 2020-05-10 17:53:39.000000 dataiter-0.8/dataiter/util.py
-drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-10 18:09:12.833070 dataiter-0.8/dataiter.egg-info/
--rw-r--r--   0 osmo      (1000) osmo      (1000)     3505 2020-05-10 18:09:12.000000 dataiter-0.8/dataiter.egg-info/PKG-INFO
--rw-r--r--   0 osmo      (1000) osmo      (1000)      299 2020-05-10 18:09:12.000000 dataiter-0.8/dataiter.egg-info/SOURCES.txt
--rw-r--r--   0 osmo      (1000) osmo      (1000)        1 2020-05-10 18:09:12.000000 dataiter-0.8/dataiter.egg-info/dependency_links.txt
--rw-r--r--   0 osmo      (1000) osmo      (1000)       33 2020-05-10 18:09:12.000000 dataiter-0.8/dataiter.egg-info/requires.txt
--rw-r--r--   0 osmo      (1000) osmo      (1000)        9 2020-05-10 18:09:12.000000 dataiter-0.8/dataiter.egg-info/top_level.txt
--rw-r--r--   0 osmo      (1000) osmo      (1000)       38 2020-05-10 18:09:12.833070 dataiter-0.8/setup.cfg
--rwxr-xr-x   0 osmo      (1000) osmo      (1000)      566 2020-05-10 18:07:56.000000 dataiter-0.8/setup.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-11 19:36:31.997802 dataiter-0.9/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3505 2020-05-11 19:36:31.997802 dataiter-0.9/PKG-INFO
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2575 2020-05-11 19:31:58.000000 dataiter-0.9/README.md
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-11 19:36:31.997802 dataiter-0.9/dataiter/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1695 2020-05-11 19:34:58.000000 dataiter-0.9/dataiter/__init__.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    17919 2020-05-11 19:31:31.000000 dataiter-0.9/dataiter/data_frame.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     1910 2020-05-11 19:32:08.000000 dataiter-0.9/dataiter/deco.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)    14033 2020-05-11 19:32:35.000000 dataiter-0.9/dataiter/list_of_dicts.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     2122 2020-05-11 19:33:17.000000 dataiter-0.9/dataiter/util.py
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     7699 2020-05-11 19:33:46.000000 dataiter-0.9/dataiter/vector.py
+drwxr-xr-x   0 osmo      (1000) osmo      (1000)        0 2020-05-11 19:36:31.997802 dataiter-0.9/dataiter.egg-info/
+-rw-r--r--   0 osmo      (1000) osmo      (1000)     3505 2020-05-11 19:36:31.000000 dataiter-0.9/dataiter.egg-info/PKG-INFO
+-rw-r--r--   0 osmo      (1000) osmo      (1000)      300 2020-05-11 19:36:31.000000 dataiter-0.9/dataiter.egg-info/SOURCES.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        1 2020-05-11 19:36:31.000000 dataiter-0.9/dataiter.egg-info/dependency_links.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)       33 2020-05-11 19:36:31.000000 dataiter-0.9/dataiter.egg-info/requires.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)        9 2020-05-11 19:36:31.000000 dataiter-0.9/dataiter.egg-info/top_level.txt
+-rw-r--r--   0 osmo      (1000) osmo      (1000)       38 2020-05-11 19:36:31.997802 dataiter-0.9/setup.cfg
+-rwxr-xr-x   0 osmo      (1000) osmo      (1000)      566 2020-05-11 19:35:07.000000 dataiter-0.9/setup.py
```

### Comparing `dataiter-0.8/PKG-INFO` & `dataiter-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiter
-Version: 0.8
+Version: 0.9
 Summary: Classes for data manipulation
 Home-page: https://github.com/otsaloma/dataiter
 Author: Osmo Salomaa
 Author-email: otsaloma@iki.fi
 License: MIT
 Description: Python Classes for Data Manipulation
         ====================================
```

### Comparing `dataiter-0.8/README.md` & `dataiter-0.9/README.md`

 * *Files identical despite different names*

### Comparing `dataiter-0.8/dataiter/__init__.py` & `dataiter-0.9/dataiter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from dataiter.array import Array # noqa
+from dataiter.vector import Vector # noqa
 from dataiter.data_frame import DataFrame # noqa
 from dataiter.data_frame import DataFrameColumn # noqa
 from dataiter.list_of_dicts import ListOfDicts # noqa
 from dataiter.list_of_dicts import ObsoleteError # noqa
 from dataiter.list_of_dicts import ObsoleteListOfDicts # noqa
 
-__version__ = "0.8"
+__version__ = "0.9"
 
+DEFAULT_PEEK_ELEMENTS = 10
 DEFAULT_PEEK_ITEMS = 3
 DEFAULT_PEEK_ROWS = 10
 PRINT_FLOAT_PRECISION = 6
 PRINT_MAX_ITEMS = 10
 PRINT_MAX_ROWS = 100
 PRINT_MAX_WIDTH = 80
```

### Comparing `dataiter-0.8/dataiter/array.py` & `dataiter-0.9/dataiter/vector.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,38 +16,42 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
+import dataiter
 import datetime
 import numpy as np
 
 from dataiter import util
 
 TYPE_CONVERSIONS = {
     datetime.date: "datetime64[D]",
     datetime.datetime: "datetime64[us]",
 }
 
 
-class Array(np.ndarray):
+class Vector(np.ndarray):
 
     def __new__(cls, object, dtype=None):
         # If given a NumPy array, we can do a fast initialization.
         if isinstance(object, np.ndarray):
             dtype = dtype or object.dtype
             return np.array(object, dtype).view(cls)
         # If given a Python list, or something else generic, we need
         # to convert certain types and special values. This is really
-        # slow, see Array.fast for faster initialization.
+        # slow, see Vector.fast for faster initialization.
         object = [object] if np.isscalar(object) else object
         return cls._std_to_np(object, dtype).view(cls)
 
+    def __init__(self, object, dtype=None):
+        self._check_dimensions()
+
     def __array_wrap__(self, array, context=None):
         # Avoid returning 0-dimensional arrays.
         # https://github.com/numpy/numpy/issues/7403
         return array[()] if array.shape == () else array
 
     def __repr__(self):
         return self.__str__()
@@ -69,14 +73,18 @@
 
     def as_integer(self):
         return self.astype(int)
 
     def as_string(self):
         return self.astype(str)
 
+    def _check_dimensions(self):
+        if self.ndim == 1: return
+        raise ValueError(f"Bad dimensions: {self.ndim!r}")
+
     def equal(self, other):
         if self.is_datetime and other.is_datetime:
             return self._equal_missing(other, np.isnat)
         if self.is_float and other.is_float:
             return self._equal_missing(other, np.isnan)
         return np.array_equal(self, other)
 
@@ -85,14 +93,20 @@
         return (np.all(ii == jj) and
                 np.all(self[~ii] == other[~jj]))
 
     @classmethod
     def fast(cls, object, dtype=None):
         return np.array(object, dtype).view(cls)
 
+    def head(self, n=None):
+        if n is None:
+            n = dataiter.DEFAULT_PEEK_ELEMENTS
+        n = min(self.length, n)
+        return self[np.arange(n)].copy()
+
     @property
     def is_boolean(self):
         return np.issubdtype(self.dtype, np.bool_)
 
     @property
     def is_datetime(self):
         return np.issubdtype(self.dtype, np.datetime64)
@@ -101,27 +115,41 @@
     def is_float(self):
         return np.issubdtype(self.dtype, np.floating)
 
     @property
     def is_integer(self):
         return np.issubdtype(self.dtype, np.integer)
 
+    def is_missing(self):
+        if self.is_datetime:
+            return np.isnat(self)
+        if self.is_float:
+            return np.isnan(self)
+        if self.is_string:
+            return self == ""
+        return np.isin(self, [None])
+
     @property
     def is_number(self):
         return np.issubdtype(self.dtype, np.number)
 
     @property
     def is_object(self):
         return np.issubdtype(self.dtype, np.object_)
 
     @property
     def is_string(self):
         return np.issubdtype(self.dtype, np.character)
 
     @property
+    def length(self):
+        self._check_dimensions()
+        return self.size
+
+    @property
     def missing_dtype(self):
         # Return corresponding dtype that can handle missing data.
         # Needed for upcasting when missing data is first introduced.
         if self.is_datetime:
             return self.dtype
         if self.is_float:
             return self.dtype
@@ -138,22 +166,43 @@
             return np.datetime64("NaT")
         if self.is_float:
             return np.nan
         if self.is_integer:
             return np.nan
         if self.is_string:
             return ""
-        # Note that using None, e.g. for a boolean array,
+        # Note that using None, e.g. for a boolean vector,
         # might not work directly as it requires upcasting to object.
         return None
 
+    def range(self):
+        rng = [np.nanmin(self), np.nanmax(self)]
+        return self.__class__(rng, self.dtype)
+
     def rank(self):
         rank = np.unique(self, return_inverse=True)[1]
         return rank.view(self.__class__)
 
+    def sample(self, n=None):
+        if n is None:
+            n = dataiter.DEFAULT_PEEK_ELEMENTS
+        n = min(self.length, n)
+        indices = np.random.choice(self.length, n, replace=False)
+        return self[np.sort(indices)].copy()
+
+    def sort(self, dir=1):
+        vector = self.copy()
+        np.ndarray.sort(vector)
+        if dir < 0:
+            # Flip order, but keep missing last.
+            na = vector.is_missing()
+            ok = np.nonzero(~na)
+            np.put(vector, ok, vector[ok][::-1])
+        return vector
+
     @classmethod
     def _std_to_np(cls, seq, dtype=None):
         # Convert missing values in seq to NumPy equivalents.
         types = util.unique_types(seq)
         missing = cls._std_to_np_missing_value(types)
         seq = [missing if x is None else x for x in seq]
         if dtype is not None:
@@ -174,17 +223,19 @@
             return np.nan
         datetimes = [datetime.date, datetime.datetime, np.datetime64]
         if all(x in datetimes for x in types):
             return np.datetime64("NaT")
         # Usually causes dtype to be object!
         return None
 
+    def tail(self, n=None):
+        if n is None:
+            n = dataiter.DEFAULT_PEEK_ELEMENTS
+        n = min(self.length, n)
+        return self[np.arange(self.length - n, self.length)].copy()
+
     def tolist(self):
-        def replace(isna):
-            return np.where(isna(self), None, self).tolist()
-        if self.is_datetime:
-            return replace(np.isnat)
-        if self.is_float:
-            return replace(np.isnan)
-        if self.is_string:
-            return replace(lambda x: x == "")
-        return super().tolist()
+        return np.where(self.is_missing(), None, self).tolist()
+
+    def unique(self):
+        u, indices = np.unique(self, return_index=True)
+        return self[indices.sort()].copy()
```

### Comparing `dataiter-0.8/dataiter/data_frame.py` & `dataiter-0.9/dataiter/data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,41 +22,36 @@
 
 import dataiter
 import itertools
 import json
 import numpy as np
 import pickle
 
-from dataiter import Array
 from dataiter import deco
 from dataiter import util
+from dataiter import Vector
 
 
-class DataFrameColumn(Array):
+class DataFrameColumn(Vector):
 
     def __new__(cls, object, dtype=None, nrow=None):
         object = [object] if np.isscalar(object) else object
-        column = Array(object, dtype)
-        if nrow is not None and nrow != column.size:
-            if column.size != 1 or nrow < 1:
+        column = Vector(object, dtype)
+        if nrow is not None and nrow != column.length:
+            if column.length != 1 or nrow < 1:
                 raise ValueError("Bad arguments for broadcast")
             column = column.repeat(nrow)
         return column.view(cls)
 
     def __init__(self, object, dtype=None, nrow=None):
-        self._check_dimensions()
-
-    def _check_dimensions(self):
-        if self.ndim == 1: return
-        raise ValueError(f"Bad dimensions: {self.ndim!r}")
+        super().__init__(object, dtype)
 
     @property
     def nrow(self):
-        self._check_dimensions()
-        return self.size
+        return self.length
 
 
 class DataFrame(dict):
 
     # List of names that are actual attributes, not columns
     ATTRIBUTES = ["colnames", "_group_colnames"]
 
@@ -258,30 +253,30 @@
     @property
     def nrow(self):
         if not self: return 0
         self._check_dimensions()
         return self[next(iter(self))].nrow
 
     def _parse_cols_from_boolean(self, cols):
-        cols = Array.fast(cols, bool)
+        cols = Vector.fast(cols, bool)
         if len(cols) != self.ncol:
             raise ValueError("Bad length for boolean cols")
-        return Array.fast(np.nonzero(cols)[0], int)
+        return Vector.fast(np.nonzero(cols)[0], int)
 
     def _parse_cols_from_integer(self, cols):
-        return Array.fast(cols, int)
+        return Vector.fast(cols, int)
 
     def _parse_rows_from_boolean(self, rows):
-        rows = Array.fast(rows, bool)
+        rows = Vector.fast(rows, bool)
         if len(rows) != self.nrow:
             raise ValueError("Bad length for boolean rows")
-        return Array.fast(np.nonzero(rows)[0], int)
+        return Vector.fast(np.nonzero(rows)[0], int)
 
     def _parse_rows_from_integer(self, rows):
-        return Array.fast(rows, int)
+        return Vector.fast(rows, int)
 
     def print_(self, max_rows=None, max_width=None):
         print(self.to_string(max_rows, max_width))
 
     @deco.new_from_generator
     def rbind(self, *others):
         data_frames = [self] + list(others)
@@ -289,15 +284,15 @@
         def get_part(data, colname):
             if colname in data:
                 return data[colname]
             for ref in data_frames:
                 if colname not in ref: continue
                 value = ref[colname].missing_value
                 dtype = ref[colname].missing_dtype
-                return Array.fast([value], dtype).repeat(data.nrow)
+                return Vector.fast([value], dtype).repeat(data.nrow)
         for colname in colnames:
             parts = [get_part(x, colname) for x in data_frames]
             total = DataFrameColumn(np.concatenate(parts))
             yield colname, total
 
     @classmethod
     def read_csv(cls, fname, encoding="utf_8", header=True, sep=","):
@@ -399,15 +394,15 @@
         return ListOfDicts(data)
 
     def to_pandas(self):
         import pandas as pd
         return pd.DataFrame({x: self[x].tolist() for x in self.colnames})
 
     def to_string(self, max_rows=None, max_width=None):
-        # TODO: Rewrite this mess. Move formatting logic to Array?
+        # TODO: Rewrite this mess. Move formatting logic to Vector?
         max_rows = dataiter.PRINT_MAX_ROWS if max_rows is None else max_rows
         max_width = dataiter.PRINT_MAX_WIDTH if max_width is None else max_width
         rows = [self.colnames]
         rows.append([str(x.dtype) for x in self.columns])
         format = lambda x: util.np_to_string(x, quote=False)
         for i in range(min(self.nrow, max_rows)):
             rows.append([format(x[i]) for x in self.columns])
```

### Comparing `dataiter-0.8/dataiter/deco.py` & `dataiter-0.9/dataiter/deco.py`

 * *Files identical despite different names*

### Comparing `dataiter-0.8/dataiter/list_of_dicts.py` & `dataiter-0.9/dataiter/list_of_dicts.py`

 * *Files identical despite different names*

### Comparing `dataiter-0.8/dataiter/util.py` & `dataiter-0.9/dataiter/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import dataiter as di
+import dataiter
 import itertools
 import numpy as np
 import string
 
 
 def generate_colnames(n):
     return list(itertools.islice(yield_colnames(), n))
@@ -32,16 +32,16 @@
 def length(value):
     return 1 if np.isscalar(value) else len(value)
 
 def np_to_string(value, quote=True):
     str_ = format_quoted if quote else str
     return np.array2string(
         np.array(value),
-        max_line_width=di.PRINT_MAX_WIDTH,
-        precision=di.PRINT_FLOAT_PRECISION,
+        max_line_width=dataiter.PRINT_MAX_WIDTH,
+        precision=dataiter.PRINT_FLOAT_PRECISION,
         formatter={
             "datetime": str_,
             "numpystr": str_,
             "str": str_,
         },
     )
```

### Comparing `dataiter-0.8/dataiter.egg-info/PKG-INFO` & `dataiter-0.9/dataiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiter
-Version: 0.8
+Version: 0.9
 Summary: Classes for data manipulation
 Home-page: https://github.com/otsaloma/dataiter
 Author: Osmo Salomaa
 Author-email: otsaloma@iki.fi
 License: MIT
 Description: Python Classes for Data Manipulation
         ====================================
```

### Comparing `dataiter-0.8/setup.py` & `dataiter-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="dataiter",
-    version="0.8",
+    version="0.9",
     author="Osmo Salomaa",
     author_email="otsaloma@iki.fi",
     description="Classes for data manipulation",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/otsaloma/dataiter",
     license="MIT",
```

