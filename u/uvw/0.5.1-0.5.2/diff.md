# Comparing `tmp/uvw-0.5.1.tar.gz` & `tmp/uvw-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvw-0.5.1.tar", last modified: Thu Apr 13 09:02:03 2023, max compression
+gzip compressed data, was "uvw-0.5.2.tar", last modified: Wed Jun 14 08:16:00 2023, max compression
```

## Comparing `uvw-0.5.1.tar` & `uvw-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 09:01:53.000000 uvw-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 09:01:53.000000 uvw-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-13 09:02:03.407386 uvw-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-13 09:01:53.000000 uvw-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 09:02:03.407386 uvw-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 09:01:53.000000 uvw-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/data_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw/dropin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/dropin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/dropin/hl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/vtk_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-13 09:01:53.000000 uvw-0.5.1/uvw/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:03.407386 uvw-0.5.1/uvw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 09:02:03.000000 uvw-0.5.1/uvw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-13 09:01:53.000000 uvw-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:00.307916 uvw-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-14 08:15:33.000000 uvw-0.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 08:15:33.000000 uvw-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-14 08:16:00.307916 uvw-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-14 08:15:33.000000 uvw-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 08:16:00.311916 uvw-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-14 08:15:33.000000 uvw-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:00.311916 uvw-0.5.2/uvw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 08:16:00.311916 uvw-0.5.2/uvw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/data_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:00.307916 uvw-0.5.2/uvw/dropin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/dropin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/dropin/hl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/vtk_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-14 08:15:33.000000 uvw-0.5.2/uvw/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:16:00.307916 uvw-0.5.2/uvw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-14 08:16:00.000000 uvw-0.5.2/uvw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 08:16:00.000000 uvw-0.5.2/uvw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:16:00.000000 uvw-0.5.2/uvw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 08:16:00.000000 uvw-0.5.2/uvw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 08:16:00.000000 uvw-0.5.2/uvw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-14 08:15:33.000000 uvw-0.5.2/versioneer.py
```

### Comparing `uvw-0.5.1/LICENSE.md` & `uvw-0.5.2/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright © 2018-2022 Lucas Frérot
+Copyright © 2018-2023 Lucas Frérot
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `uvw-0.5.1/PKG-INFO` & `uvw-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvw
-Version: 0.5.1
+Version: 0.5.2
 Summary: Universal VTK Writer for Numpy Arrays
 Home-page: https://github.com/prs513rosewood/uvw
 Author: Lucas Frérot
 Author-email: lucas.frerot@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uvw-0.5.1/README.md` & `uvw-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `uvw-0.5.1/setup.py` & `uvw-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `uvw-0.5.1/uvw/__init__.py` & `uvw-0.5.2/uvw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 For documentation and examples, check out the various classes' docstrings and
 the repository home on GitHub: https://github.com/prs513rosewood/uvw
 """
 
 __author__ = "Lucas Frérot"
 __maintainer__ = __author__
-__copyright__ = "Copyright © 2018-2021 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 # flake8: noqa
 
 from .vtk_files import (
     RectilinearGrid,
     ImageData,
```

### Comparing `uvw-0.5.1/uvw/data_array.py` & `uvw-0.5.2/uvw/data_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Defining class (`DataArray`) used to represent Numpy arrays in XML model."""
 
-__copyright__ = "Copyright © 2018-2022 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 import functools
 import typing as ts
 import numpy as np
 
 DTYPE_TO_VTK = {
```

### Comparing `uvw-0.5.1/uvw/dropin/hl.py` & `uvw-0.5.2/uvw/dropin/hl.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
 
-__copyright__ = "Copyright © 2018-2021 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 from .. import vtk_files as vtk
 from ..data_array import DataArray
 
 import typing as ts
 import numpy as np
```

### Comparing `uvw-0.5.1/uvw/parallel.py` & `uvw-0.5.2/uvw/parallel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module with MPI-empowered classes for parallel VTK file types."""
 
-__copyright__ = "Copyright © 2018-2022 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 import functools
 
 from os import PathLike
 from os.path import splitext, basename
 from mpi4py import MPI
@@ -40,27 +40,28 @@
         ""
     )
 
 
 class PVTKFile(vtk_files.VTKFile):
     """Generic parallel VTK file."""
 
-    def __init__(self, filename, pfiletype, **kwargs):
+    def __init__(self, filename, pfiletype, comm=None, **kwargs):
         """
         Create a generic VTK file.
 
         :param filename: name of file (cannot be file handle)
-        :param filetype: VTK format of file
+        :param pfiletype: VTK format of file
+        :param comm: MPI communicator (default: MPI.COMM_WORLD)
         :param **kwargs: parameters forwarded to Writer
         """
         _check_file_descriptor(filename)
         filename = str(filename)  # Ensure we have a string
         self.pfilename = filename
         self.pfiletype = pfiletype
-        self.comm = MPI.COMM_WORLD
+        self.comm = MPI.COMM_WORLD if comm is None else comm
         self.rank = self.comm.Get_rank()
 
         # Construct name of piece file
         extension = splitext(filename)[1]
         piece_extension = extension.replace('p', '')
         self.piece_name_template = (
             filename.replace(extension, '.rank{rank}') + piece_extension
@@ -100,23 +101,24 @@
 
 
 class PImageData(PVTKFile, vtk_files.ImageData):
     """Image data parallel writer."""
 
     parent = vtk_files.ImageData
 
-    def __init__(self, filename, ranges, points, offsets, **kwargs):
+    def __init__(self, filename, ranges, points, offsets, comm=None, **kwargs):
         """
         Init an ImageData file (regular orthogonal grid).
 
         :param filename: name of file or file handle
         :param ranges: list of pairs for coordinate ranges
         :param points: list of number of points
+        :param comm: MPI communicator (default: MPI.COMM_WORLD)
         """
-        PVTKFile.__init__(self, filename, 'PImageData', **kwargs)
+        PVTKFile.__init__(self, filename, 'PImageData', comm=comm, **kwargs)
         self.parent.__init__(
             self,
             self.piece_name_template.format(rank=self.rank),
             ranges,
             points,
             offsets,
             **kwargs
@@ -159,23 +161,25 @@
 
 
 class PRectilinearGrid(PVTKFile, vtk_files.RectilinearGrid):
     """Rectilinear grid parallel writer."""
 
     parent = vtk_files.RectilinearGrid
 
-    def __init__(self, filename, coordinates, offsets, **kwargs):
+    def __init__(self, filename, coordinates, offsets, comm=None, **kwargs):
         """
         Init the parallel counterpart of a RectilinearGrid file.
 
         :param filename: name of file or file handle
         :param coordinates: list of coordinate arrays for this rank
         :param offset: offset in global dataset for this rank
+        :param comm: MPI communicator (default: MPI.COMM_WORLD)
         """
-        PVTKFile.__init__(self, filename, 'PRectilinearGrid', **kwargs)
+        PVTKFile.__init__(self, filename, 'PRectilinearGrid',
+                          comm=comm, **kwargs)
 
         # Name of piece file associated to rank
         self.parent.__init__(
             self,
             self.piece_name_template.format(rank=self.rank),
             coordinates,
             offsets,
```

### Comparing `uvw-0.5.1/uvw/unstructured.py` & `uvw-0.5.2/uvw/unstructured.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module with class for cell types in vtkUnstructuredGrid."""
 
-__copyright__ = "Copyright © 2018-2022 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 from enum import Enum, unique
 
 import numpy as np
 
 from .data_array import DTYPE_TO_VTK
```

### Comparing `uvw-0.5.1/uvw/vtk_files.py` & `uvw-0.5.2/uvw/vtk_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 the idiomatic:
 
   with RectilinearGrid(...) as file:
       file.addPointData(...)
 
 """
 
-__copyright__ = "Copyright © 2018-2021 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 import functools
 import typing as ts
 import numpy as np
 
 from . import writer
```

### Comparing `uvw-0.5.1/uvw/writer.py` & `uvw-0.5.2/uvw/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module with classes for interacting with the XML model underlying VTK files.
 
 See https://kitware.github.io/vtk-examples/site/VTKFileFormats/ for format
 description.
 """
 
-__copyright__ = "Copyright © 2018-2021 Lucas Frérot"
+__copyright__ = "Copyright © 2018-2023 Lucas Frérot"
 __license__ = "SPDX-License-Identifier: MIT"
 
 from .data_array import DataArray
 
 import xml.dom.minidom as dom
 import io
 import zlib
```

### Comparing `uvw-0.5.1/uvw.egg-info/PKG-INFO` & `uvw-0.5.2/uvw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvw
-Version: 0.5.1
+Version: 0.5.2
 Summary: Universal VTK Writer for Numpy Arrays
 Home-page: https://github.com/prs513rosewood/uvw
 Author: Lucas Frérot
 Author-email: lucas.frerot@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uvw-0.5.1/versioneer.py` & `uvw-0.5.2/versioneer.py`

 * *Files identical despite different names*

