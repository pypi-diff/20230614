# Comparing `tmp/biglist-0.8.2b2.tar.gz` & `tmp/biglist-0.8.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.8.2b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "biglist-0.8.2b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `biglist-0.8.2b2.tar` & `biglist-0.8.2b3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.2b2/LICENSE
--rw-r--r--   0        0        0      844 2023-06-13 03:31:25.325512 biglist-0.8.2b2/README.rst
--rw-r--r--   0        0        0     1558 2023-06-13 05:25:39.353267 biglist-0.8.2b2/pyproject.toml
--rw-r--r--   0        0        0     2193 2023-06-13 04:52:58.072799 biglist-0.8.2b2/src/biglist/__init__.py
--rw-r--r--   0        0        0    17850 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_base.py
--rw-r--r--   0        0        0    44494 2023-06-13 03:31:28.205526 biglist-0.8.2b2/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34699 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_parquet.py
--rw-r--r--   0        0        0    13137 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.2b2/src/biglist/py.typed
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 biglist-0.8.2b2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.2b3/LICENSE
+-rw-r--r--   0        0        0      844 2023-06-13 03:31:25.325512 biglist-0.8.2b3/README.rst
+-rw-r--r--   0        0        0     1558 2023-06-13 05:25:39.353267 biglist-0.8.2b3/pyproject.toml
+-rw-r--r--   0        0        0     2193 2023-06-13 07:07:19.727496 biglist-0.8.2b3/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17850 2023-06-13 05:25:39.353267 biglist-0.8.2b3/src/biglist/_base.py
+-rw-r--r--   0        0        0    44494 2023-06-13 03:31:28.205526 biglist-0.8.2b3/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    33357 2023-06-13 07:07:47.458706 biglist-0.8.2b3/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    13137 2023-06-13 05:25:39.353267 biglist-0.8.2b3/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.2b3/src/biglist/py.typed
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 biglist-0.8.2b3/PKG-INFO
```

### Comparing `biglist-0.8.2b2/LICENSE` & `biglist-0.8.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/README.rst` & `biglist-0.8.2b3/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/pyproject.toml` & `biglist-0.8.2b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/src/biglist/__init__.py` & `biglist-0.8.2b3/src/biglist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.8.2b2"
+__version__ = "0.8.2b3"
```

### Comparing `biglist-0.8.2b2/src/biglist/_base.py` & `biglist-0.8.2b3/src/biglist/_base.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/src/biglist/_biglist.py` & `biglist-0.8.2b3/src/biglist/_biglist.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/src/biglist/_parquet.py` & `biglist-0.8.2b3/src/biglist/_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import io
 import itertools
 import logging
 from collections.abc import Iterable, Iterator, Sequence
 from multiprocessing.util import Finalize
 from pathlib import Path
 
 import pyarrow
@@ -66,68 +65,45 @@
                 access_token=cls._GCP_CREDENTIALS.token,
                 credential_token_expiration=cls._GCP_CREDENTIALS.expiry,
             )
             cls._GCSFS = fs
         return cls._GCSFS
 
     @classmethod
-    def load_file(cls, path: Upath, *, lazy: bool = True) -> ParquetFile:
+    def load_file(cls, path: Upath) -> ParquetFile:
         '''
         Depending on the implementation, this may read *meta* info only, or
         load in the entire file eagerly.
 
         Parameters
         ----------
         path
             Path of the file.
-        lazy
-            If ``True`` (the default), only *meta* info is loaded to construct
-            a ``ParquetFile`` object.
-            If ``False``, ``path.read_bytes()`` is called to read in the entire file into memory,
-            and the bytes are then used to construct a ``ParquetFile`` object.
-            The second route is provided to work around an issue encountered when
-            ``path`` is in Google Cloud Storage.
         '''
-        # References for the issue:
-        # https://stackoverflow.com/q/76012391/6178706
-        # https://github.com/apache/arrow/issues/35318
-        if lazy:
-            ff, pp = FileSystem.from_uri(str(path))
-            if isinstance(ff, GcsFileSystem):
-                ff = cls.get_gcsfs()
-            file = ParquetFile(pp, filesystem=ff)
-        else:
-            data = io.BytesIO(path.read_bytes())
-            file = ParquetFile(data)
+        ff, pp = FileSystem.from_uri(str(path))
+        if isinstance(ff, GcsFileSystem):
+            ff = cls.get_gcsfs()
+        file = ParquetFile(pp, filesystem=ff)
         Finalize(file, file.reader.close)
         # NOTE: can not use
         #
         #   Finalize(file, file.close, kwargs={'force': True})
         #
         # because the instance method `file.close` can't be used as the callback---the
         # object `file` is no long available at that time.
-
         return file
 
     def __init__(self, path: PathType):
         """
         Parameters
         ----------
         path
             Path of a Parquet file.
         """
         self.path: Upath = resolve_path(path)
-        self.lazy = True
-        # ``self.lazy`` is used in ``self.file`` when it calls ``self.load_file``.
-        # If you change ``self.lazy`` after ``self.file`` has been called, then
-        # the change has no effect.
-        # This attribute is not controlled by a parameter conveniently because
-        # this may be removed later once the issue it is working around is resolved.
-        # To use this, just set its value directly on the ``ParquetFileReader`` object
-        # before the object has been used (hence its ``file`` may have been called).
         self._reset()
 
     def _reset(self):
         self._file: ParquetFile | None = None
         self._data: ParquetBatchData | None = None
 
         self._row_groups_num_rows = None
@@ -138,18 +114,18 @@
         self._columns = {}
         self._getitem_last_row_group = None
 
         self._scalar_as_py = None
         self.scalar_as_py = True
 
     def __getstate__(self):
-        return self.path, self.lazy
+        return (self.path,)
 
     def __setstate__(self, data):
-        self.path, self.lazy = data
+        self.path = data[0]
         self._reset()
 
     @property
     def scalar_as_py(self) -> bool:
         """
         ``scalar_as_py`` controls whether the values returned by :meth:`__getitem__`
         (or indirectly by :meth:`__iter__`) are converted from a `pyarrow.Scalar`_ type
@@ -194,15 +170,15 @@
 
         Upon initiation of a :class:`ParquetFileReader` object,
         the file is not read at all. When this property is requested,
         the file is accessed to construct a `pyarrow.parquet.ParquetFile`_ object.
 
         """
         if self._file is None:
-            self._file = self.load_file(self.path, lazy=self.lazy)
+            self._file = self.load_file(self.path)
         return self._file
 
     @property
     def metadata(self) -> FileMetaData:
         return self.file.metadata
 
     @property
```

### Comparing `biglist-0.8.2b2/src/biglist/_util.py` & `biglist-0.8.2b3/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b2/PKG-INFO` & `biglist-0.8.2b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.8.2b2
+Version: 0.8.2b3
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

