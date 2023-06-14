# Comparing `tmp/enstools-encoding-2023.4.1.tar.gz` & `tmp/enstools-encoding-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-encoding-2023.4.1.tar", last modified: Mon Apr 17 12:03:16 2023, max compression
+gzip compressed data, was "enstools-encoding-2023.6.tar", last modified: Wed Jun 14 14:50:12 2023, max compression
```

## Comparing `enstools-encoding-2023.4.1.tar` & `enstools-encoding-2023.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-17 11:52:31.000000 enstools-encoding-2023.4.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.559552 enstools-encoding-2023.4.1/enstools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.561552 enstools-encoding-2023.4.1/enstools/encoding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/api.py
--rw-rw-rw-   0 root         (0) root         (0)     9046 2023-04-17 09:53:42.000000 enstools-encoding-2023.4.1/enstools/encoding/dataset_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/enstools/encoding/rules.py
--rw-rw-rw-   0 root         (0) root         (0)    11435 2023-04-17 11:57:40.000000 enstools-encoding-2023.4.1/enstools/encoding/variable_encoding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.561552 enstools-encoding-2023.4.1/enstools_encoding.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 12:03:16.000000 enstools-encoding-2023.4.1/enstools_encoding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      992 2023-01-18 16:25:49.000000 enstools-encoding-2023.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:03:16.562552 enstools-encoding-2023.4.1/test/
--rw-rw-rw-   0 root         (0) root         (0)    15517 2023-01-18 16:11:59.000000 enstools-encoding-2023.4.1/test/test_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:50:12.710336 enstools-encoding-2023.6/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:11:59.000000 enstools-encoding-2023.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:11:59.000000 enstools-encoding-2023.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-06-14 14:50:12.710336 enstools-encoding-2023.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-14 14:46:20.000000 enstools-encoding-2023.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:50:12.708336 enstools-encoding-2023.6/enstools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:50:12.709336 enstools-encoding-2023.6/enstools/encoding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 16:11:59.000000 enstools-encoding-2023.6/enstools/encoding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-11 14:59:43.000000 enstools-encoding-2023.6/enstools/encoding/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-06-14 14:44:32.000000 enstools-encoding-2023.6/enstools/encoding/chunk_size.py
+-rw-rw-rw-   0 root         (0) root         (0)    12947 2023-06-14 14:44:32.000000 enstools-encoding-2023.6/enstools/encoding/dataset_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-05-11 14:59:43.000000 enstools-encoding-2023.6/enstools/encoding/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-05-11 14:59:43.000000 enstools-encoding-2023.6/enstools/encoding/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-01-18 16:11:59.000000 enstools-encoding-2023.6/enstools/encoding/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-06-14 14:44:32.000000 enstools-encoding-2023.6/enstools/encoding/variable_encoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:50:12.710336 enstools-encoding-2023.6/enstools_encoding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 14:50:12.000000 enstools-encoding-2023.6/enstools_encoding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 14:50:12.710336 enstools-encoding-2023.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-01-18 16:25:49.000000 enstools-encoding-2023.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:50:12.710336 enstools-encoding-2023.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2023-01-18 16:11:59.000000 enstools-encoding-2023.6/test/test_classes.py
```

### Comparing `enstools-encoding-2023.4.1/LICENSE` & `enstools-encoding-2023.6/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.4.1/PKG-INFO` & `enstools-encoding-2023.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: enstools-encoding
-Version: 2023.4.1
-Summary: UNKNOWN
+Version: 2023.6
 Home-page: https://github.com/wavestoweather/enstools-encoding
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-encoding [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-encoding.readthedocs.io/en/latest/?badge=latest)
 
 Library to generate the encodings to write compressed files as easily as possible with **xarray** using **hdf5 filters**.
 
@@ -48,9 +45,7 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
-
-
```

### Comparing `enstools-encoding-2023.4.1/enstools/encoding/dataset_encoding.py` & `enstools-encoding-2023.6/enstools/encoding/dataset_encoding.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,86 @@
+"""
+This module provides utility functions and a class for handling compression specifications
+and chunking in xarray Datasets.
+
+Functions:
+- convert_size(size_bytes): Converts a given size in bytes to a human-readable format.
+- convert_to_bytes(size_string): Converts a size string (e.g., '5MB') to the number of bytes.
+- compression_dictionary_to_string(compression_dictionary): Converts a dictionary with
+  compression entries to a single-line specification string.
+- parse_full_specification(spec): Parses a full compression specification and returns a
+  dictionary of variable encodings.
+- is_a_valid_dataset_compression_specification(specification): Checks if a compression
+  specification is valid for a dataset.
+- find_chunk_sizes(data_array, chunk_size): Determines chunk sizes for each dimension of a
+  data array based on a desired chunk size.
+
+Class:
+- DatasetEncoding: Encapsulates compression specification parameters for a full dataset.
+  Provides methods to generate encodings and add metadata.
+
+"""
+
 import os
+import re
 from copy import deepcopy
 from pathlib import Path
 from typing import Hashable, Union, Dict
+import math
 
+import numpy as np
 import xarray
 import yaml
-import numpy as np
 
+import enstools.encoding.chunk_size
 from . import rules
 from .errors import InvalidCompressionSpecification
 from .variable_encoding import _Mapping, parse_variable_specification, Encoding, \
     NullEncoding
+from .rules import VARIABLE_SEPARATOR, VARIABLE_NAME_SEPARATOR, \
+    DATA_DEFAULT_LABEL, DATA_DEFAULT_VALUE, COORD_LABEL, COORD_DEFAULT_VALUE
 
 
 def convert_size(size_bytes):
-    import math
+    """
+    Converts a given size in bytes to a human-readable format.
+
+    Args:
+        size_bytes (int): Size in bytes.
+
+    Returns:
+        str: Size in human-readable format (e.g., '5MB').
+    """
     if size_bytes < 0:
         prefix = "-"
         size_bytes = -size_bytes
     else:
         prefix = ""
 
     if size_bytes == 0:
         return "0B"
-    size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
-    i = int(math.floor(math.log(size_bytes, 1024)))
-    p = math.pow(1024, i)
-    s = round(size_bytes / p, 2)
-    return f"{prefix}{s}{size_name[i]}"
+
+    size_units = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
+    magnitude = int(math.floor(math.log(size_bytes, 1024)))
+    factor = math.pow(1024, magnitude)
+    size = round(size_bytes / factor, 2)
+    return f"{prefix}{size}{size_units[magnitude]}"
 
 
 def convert_to_bytes(size_string):
     """
     This function converts a given size string (e.g. '5MB') to the number of bytes.
     
     Args:
     size_string (str): The size string to be converted (e.g. '5MB')
     
     Returns:
     int: The number of bytes.
     """
-    import re
+
     size_string = size_string.upper()
     digits = re.match(r'\d+(?:\.\d+)?', size_string)  # matches digits and optionally a dot followed by more digits
     if digits:
         digits = digits.group()  # get the matched digits
     else:
         raise ValueError(f"Invalid size string: {size_string}")
     unit = size_string.replace(digits, "")
@@ -61,31 +97,43 @@
     Convert a dictionary containing multiple entries to a single line specification
     """
     return rules.VARIABLE_SEPARATOR.join(
         [f"{key}{rules.VARIABLE_NAME_SEPARATOR}{value}" for key, value in compression_dictionary.items()])
 
 
 def parse_full_specification(spec: Union[str, None]) -> Dict[str, Encoding]:
-    from enstools.encoding.rules import VARIABLE_SEPARATOR, VARIABLE_NAME_SEPARATOR, \
-        DATA_DEFAULT_LABEL, DATA_DEFAULT_VALUE, COORD_LABEL, COORD_DEFAULT_VALUE
+    """
+    Parses a full compression specification and returns a dictionary of variable encodings.
+
+    Args:
+        spec (Union[str, None]): The full compression specification as a string or None.
+
+    Returns:
+        Dict[str, Encoding]: A dictionary mapping variable names to their corresponding encodings.
+
+    Raises:
+        InvalidCompressionSpecification: If a variable has multiple definitions in the specification.
+
+    """
+
     result = {}
 
     if spec is None:
         spec = "None"
 
     parts = spec.split(VARIABLE_SEPARATOR)
-    for p in parts:
+    for part in parts:
         # For each part, check if there's a variable name.
         # If there's a variable name, split the name and the specification
-        if VARIABLE_NAME_SEPARATOR in p:
-            var_name, var_spec = p.split(VARIABLE_NAME_SEPARATOR)
+        if VARIABLE_NAME_SEPARATOR in part:
+            var_name, var_spec = part.split(VARIABLE_NAME_SEPARATOR)
         # Otherwise, it corresponds to the default.
         else:
             var_name = DATA_DEFAULT_LABEL
-            var_spec = p
+            var_spec = part
 
         # If the variable name was already in the dictionary, raise an error.
         if var_name in result:
             raise InvalidCompressionSpecification(f"Variable {var_name} has multiple definitions."
                                                   f"")
         # Parse the variable specification
         result[var_name] = parse_variable_specification(var_spec)
@@ -121,40 +169,61 @@
         compression = self.get_a_single_compression_string(compression)
 
         # Save it
         self.variable_encodings = parse_full_specification(compression)
 
     @staticmethod
     def get_a_single_compression_string(compression: Union[str, Dict[str, str], Path, None]) -> Union[str, None]:
+        """
+        Converts the compression parameter into a single compression specification string.
+
+        Args:
+            compression (Union[str, Dict[str, str], Path, None]): The compression parameter,
+            which can be a string, a dictionary, a file path, or None.
+
+        Returns:
+            Union[str, None]: The single compression specification string or None.
+
+        Raises:
+            InvalidCompressionSpecification: If the compression argument is not a valid type.
+
+        """
         # The compression parameter can be a string or a dictionary.
 
         # In case it is a string, it can be directly a compression specification or a yaml file.
         # If it is a file, convert it to a Path
         if isinstance(compression, str) and os.path.exists(compression):
             compression = Path(compression)
 
         if isinstance(compression, dict):
             # Just to make sure that we have all the mandatory fields (default, coordinates), we will convert
             # the input dictionary to a single specification string and convert it back.
             return compression_dictionary_to_string(compression)
-        elif isinstance(compression, Path):
-            with compression.open("r") as stream:
+        if isinstance(compression, Path):
+            with compression.open("r", encoding="utf-8") as stream:
                 dict_of_strings = yaml.safe_load(stream)
             return compression_dictionary_to_string(dict_of_strings)
-        elif isinstance(compression, str):
+        if isinstance(compression, str):
             # Convert the single string in a dictionary with an entry for each specified variable plus the defaults
             # for data and coordinates
             return compression
-        elif compression is None:
+        if compression is None:
             return None
-        else:
-            raise InvalidCompressionSpecification(
+
+        raise InvalidCompressionSpecification(
                 f"The argument 'compression' should be a string, a dictionary or a Path. It is {type(compression)!r}-")
 
     def encoding(self):
+        """
+        Generate the encoding dictionary for all variables in the dataset.
+
+        Returns:
+            dict: A dictionary mapping variable names to their corresponding encodings.
+
+        """
         # Get the defaults
         data_default = self.variable_encodings[rules.DATA_DEFAULT_LABEL]
         coordinates_default = self.variable_encodings[rules.COORD_LABEL]
 
         # Set encoding for coordinates
         coordinate_encodings = {coord: deepcopy(coordinates_default) for coord in self.dataset.coords}
         # Set encoding for data variables
@@ -164,15 +233,18 @@
             var
             in self.dataset.data_vars}
 
         # Merge
         all_encodings = {**coordinate_encodings, **data_variable_encodings}
 
         # Need to specify chunk size, otherwise it breaks down.
-        self.chunk(encodings=all_encodings)
+        self.chunk(
+            encodings=all_encodings,
+            chunk_memory_size=enstools.encoding.chunk_size.chunk_size,
+        )
 
         return all_encodings
 
     def chunk(self, encodings: Dict[Union[Hashable, str], Encoding], chunk_memory_size="10MB"):
         """
         Add a variable "chunksizes" to each variable encoding with the corresponding 
 
@@ -181,20 +253,20 @@
             chunk_memory_size (str): Desired chunk size in memory.
         """
 
         chunk_memory_size = convert_to_bytes(chunk_memory_size)
 
         # Loop over all the variables
         for variable in self.dataset.data_vars:
-            da = self.dataset[variable]
-            type_size = da.dtype.itemsize
+            data_array = self.dataset[variable]
+            type_size = data_array.dtype.itemsize
 
             optimal_chunk_size = chunk_memory_size / type_size
-            chunk_sizes = find_chunk_sizes(data_array=da, chunk_size=optimal_chunk_size)
-            chunk_sizes = tuple(chunk_sizes[d] for d in da.dims)
+            chunk_sizes = find_chunk_sizes(data_array=data_array, chunk_size=optimal_chunk_size)
+            chunk_sizes = tuple(chunk_sizes[d] for d in data_array.dims)
             encodings[variable].set_chunk_sizes(chunk_sizes)
 
     @property
     def _kwargs(self):
         return self.encoding()
 
     def add_metadata(self):
@@ -205,30 +277,61 @@
             # If its a case without compression, don't write the metadata.
             if isinstance(encoding, NullEncoding):
                 continue
             self.dataset[variable].attrs["compression"] = encoding.description()
 
 
 def is_a_valid_dataset_compression_specification(specification):
+    """
+        Checks if a compression specification is valid for a dataset.
+
+        Args:
+            specification: The compression specification to be validated.
+
+        Returns:
+            bool: True if the specification is valid, False otherwise.
+
+        Note:
+            - The function attempts to parse the specification using the `parse_full_specification` function.
+            - If the specification is successfully parsed without raising an exception, it is considered valid.
+            - If an `InvalidCompressionSpecification` exception is raised during parsing,
+            the specification is considered invalid.
+    """
     try:
         _ = parse_full_specification(specification)
         return True
     except InvalidCompressionSpecification:
         return False
 
 
 def find_chunk_sizes(data_array, chunk_size):
-    import math
+    """
+    Determines the chunk sizes for each dimension of a data array based on a desired chunk size.
+
+    Args:
+        data_array: The data array for which chunk sizes are determined.
+        chunk_size: The desired chunk size in terms of the number of elements.
+
+    Returns:
+        dict: A dictionary mapping each dimension to its corresponding chunk size.
+    """
     total_points = np.prod(data_array.shape)
     num_chunks = max(1, int(total_points // chunk_size))
     chunk_sizes = {}
     chunk_number = {}
 
-    # Sort dimensions by size
-    dims = sorted(data_array.dims, key=lambda x: data_array[x].shape)
+    # Sort dimensions such that 'time' is always first and rest by size
+    dims = sorted(data_array.dims, key=lambda x: (x != 'time', data_array[x].shape))
+
     pending_num_chunks = num_chunks
     for dim in dims:
-        chunk_sizes[dim] = max(1, int(data_array[dim].size // pending_num_chunks))
-        chunk_number[dim] = data_array[dim].size // chunk_sizes[dim]
+        if dim == 'time' or pending_num_chunks > 1:
+            chunk_sizes[dim] = max(1, int(data_array[dim].size // pending_num_chunks))
+            chunk_number[dim] = data_array[dim].size // chunk_sizes[dim]
 
-        pending_num_chunks = math.ceil(pending_num_chunks / chunk_number[dim])
+            pending_num_chunks = math.ceil(pending_num_chunks / chunk_number[dim])
+        else:
+            # If we have already chunked in the 'time' dimension and pending_num_chunks <= 1,
+            # then keep the whole dimension together in one chunk
+            chunk_sizes[dim] = data_array[dim].size
     return chunk_sizes
+
```

### Comparing `enstools-encoding-2023.4.1/enstools/encoding/definitions.py` & `enstools-encoding-2023.6/enstools/encoding/definitions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""
+This module provides configurations and mappings related to lossy and lossless compressors.
+"""
+import hdf5plugin
 
 # Dictionary of implemented lossy compressors and their respective modes and ranges.
-# TODO: Would that be better to keep the definition of the available compressors and methods in a configuration file?
 lossy_compressors_and_modes = {
     "sz": {
         "abs": {"range": [0, float('inf')], "type": float},
         "rel": {"range": [0, 1], "type": float},
         "pw_rel": {"range": [0, 1], "type": float},
     },
     "sz3": {
@@ -17,32 +20,31 @@
         "rate": {"range": [0, 32], "type": float},
         "precision": {"range": [1, 32], "type": int},
         "accuracy": {"range": [0, float('inf')], "type": float},
     }
 }
 
 # Create a list with the lossy compressors
-lossy_compressors = [c for c in lossy_compressors_and_modes]
+lossy_compressors = list(lossy_compressors_and_modes)
 
 # Create a dictionary containing the available compression modes for each lossy compressor
-lossy_compression_modes = {c: [k for k in lossy_compressors_and_modes[c]] for c in lossy_compressors}
-
+lossy_compression_modes = {c: list(lossy_compressors_and_modes) for c in lossy_compressors}
 
 # List of available BLOSC backends for lossless compression
 lossless_backends = ['blosclz', 'lz4', 'lz4hc', 'snappy', 'zlib', 'zstd']
 
 # Mappings between SZ modes and the keywords used in hdf5plugin
 sz_mode_map = {
     "abs": "absolute",
     "rel": "relative",
     "pw_rel": "pointwise_relative",
     "psnr": "peak_signal_to_noise_ratio",
     "norm2": "norm2",
 }
 
 # Mapping between compressor names and hdf5plugin classes
-import hdf5plugin
+
 compressor_map = {
     "zfp": hdf5plugin.Zfp,
     "sz": hdf5plugin.SZ,
     "sz3": hdf5plugin.SZ3,
 }
```

### Comparing `enstools-encoding-2023.4.1/enstools/encoding/rules.py` & `enstools-encoding-2023.6/enstools/encoding/rules.py`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.4.1/enstools/encoding/variable_encoding.py` & `enstools-encoding-2023.6/enstools/encoding/variable_encoding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""
+This module provides utility classes and functions for compression in Enstools.
 
-from .definitions import lossy_compressors_and_modes
-import logging
 
+This module defines various encodings and exceptions for compression, as well as utility functions.
+
+"""
+
+
+import logging
 from typing import Mapping, Union
 
 import hdf5plugin
 
 from enstools.encoding import rules, definitions
 from enstools.encoding.errors import InvalidCompressionSpecification
-from .rules import LOSSLESS_DEFAULT_BACKEND, LOSSLESS_DEFAULT_COMPRESSION_LEVEL
+from .definitions import lossy_compressors_and_modes
+from .rules import LOSSLESS_DEFAULT_BACKEND, LOSSLESS_DEFAULT_COMPRESSION_LEVEL, COMPRESSION_SPECIFICATION_SEPARATOR
 
 # Change logging level for the hdf5plugin to avoid unnecessary warnings
 loggers = {name: logging.getLogger(name) for name in logging.root.manager.loggerDict}
 hdf5plugin_loggers = [key for key in loggers.keys() if key.count("hdf5plugin")]
 for key in hdf5plugin_loggers:
     loggers[key].setLevel(logging.WARNING)
 
@@ -36,42 +43,61 @@
         return iter(self._kwargs)
 
     def __len__(self):
         return len(self._kwargs)
 
 
 class Encoding(_Mapping):
+    """
+    Base case for encoding representation.
+    """
     def check_validity(self) -> bool:
-        ...
+        """
+        Checks the validity of the encoding.
+
+        Returns:
+        - bool: True if the encoding is valid.
+
+        """
 
     def to_string(self) -> str:
-        ...
+        """
+        Returns the encoding specification as a string.
 
+        Returns:
+        - str: The encoding specification as a string.
+
+        """
     def encoding(self) -> Mapping:
-        ...
+        """
+        Returns the mapping of encoding parameters.
 
-    def description(self) -> str:
-        ...
+        Returns:
+        - Mapping: The mapping of encoding parameters.
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}({self.to_string()})"
-    
-    def set_chunk_sizes(self, chunk_sizes: tuple) -> None:
         """
-        Method to add chunksizes into the encoding dictionary.
-        Parameters
-        ----------
-        chunk_sizes
+    def description(self) -> str:
+        """
+        Returns a description of the encoding.
 
-        Returns
-        -------
+        Returns:
+        - str: A description of the encoding.
 
         """
-        self._kwargs["chunksizes"] = chunk_sizes
 
+    def __repr__(self):
+        """
+         Returns a string representation of the Encoding object.
+
+         Returns:
+         - str: A string representation of the Encoding object.
+
+         """
+        return f"{self.__class__.__name__}({self.to_string()})"
+    
     def set_chunk_sizes(self, chunk_sizes: tuple) -> None:
         """
         Method to add chunksizes into the encoding dictionary.
         Parameters
         ----------
         chunk_sizes
 
@@ -152,18 +178,19 @@
         self.check_validity()
         # Trying to convert it to a dictionary already here.
         self._kwargs = dict(self.encoding())
 
     def check_validity(self) -> bool:
         if self.backend not in definitions.lossless_backends:
             raise InvalidCompressionSpecification(f"Backend {self.backend!r} is not a valid backend.")
-        elif not (1 <= self.compression_level <= 9):
+
+        if not 1 <= self.compression_level <= 9:
             raise InvalidCompressionSpecification(f"Compression level {self.compression_level} must be within 1 and 9.")
-        else:
-            return True
+
+        return True
 
     def to_string(self) -> str:
         return rules.COMPRESSION_SPECIFICATION_SEPARATOR.join(["lossless", self.backend, str(self.compression_level)])
 
     def encoding(self) -> Mapping:
         return hdf5plugin.Blosc(cname=self.backend, clevel=self.compression_level)
 
@@ -172,63 +199,103 @@
                f"(Using {self.backend!r} with compression level {self.compression_level})"
 
     def __repr__(self):
         return f"{self.__class__.__name__}(backend={self.backend}, compression_level={self.compression_level})"
 
 
 class LossyEncoding(Encoding):
+    """
+        Encoding subclass for lossy compression.
+        """
     def __init__(self, compressor: str, mode: str, parameter: Union[float, int]):
         super().__init__()
         self.compressor = compressor
         self.mode = mode
 
         self.parameter = parameter
 
         self.check_validity()
 
         # Trying to convert it to a dictionary already here.
         self._kwargs = dict(self.encoding())
 
     def check_validity(self):
+        """
+        Checks the validity of the compressor, mode, and parameter.
+
+        Raises:
+        - InvalidCompressionSpecification: If the compressor, mode, or parameter is invalid or out of range.
+
+        Returns:
+        - bool: True if the compressor, mode, and parameter are valid.
+
+        """
         # Check compressor validity
         if self.compressor not in definitions.lossy_compressors_and_modes:
             raise InvalidCompressionSpecification(f"Invalid compressor {self.compressor}")
         # Check compression mode validity
         if self.mode not in definitions.lossy_compressors_and_modes[self.compressor]:
             raise InvalidCompressionSpecification(f"Invalid mode {self.mode!r} for compressor {self.compressor!r}")
 
         # Get parameter range and type
         mode_range = definitions.lossy_compressors_and_modes[self.compressor][self.mode]["range"]
         mode_type = definitions.lossy_compressors_and_modes[self.compressor][self.mode]["type"]
         # Check type
         if not isinstance(self.parameter, mode_type):
             try:
                 self.parameter = mode_type(self.parameter)
-            except TypeError:
+            except TypeError as err:
                 raise InvalidCompressionSpecification(f"Invalid parameter type {self.parameter!r}")
         # Check range
         if self.parameter <= mode_range[0] or self.parameter >= mode_range[1]:
             raise InvalidCompressionSpecification(f"Parameter out of range {self.parameter!r}")
         return True
 
     def to_string(self) -> str:
+        """
+        Returns the encoding specification as a string.
+
+        Returns:
+        - str: The encoding specification as a string.
+
+        """
         return rules.COMPRESSION_SPECIFICATION_SEPARATOR.join(
             ["lossy", self.compressor, self.mode, str(self.parameter)])
 
     def encoding(self) -> Mapping:
+        """
+        Returns the mapping of encoding parameters.
 
+        Returns:
+        - Mapping: The mapping of encoding parameters.
+
+        """
         mode = definitions.sz_mode_map[self.mode] if self.mode in definitions.sz_mode_map else self.mode
         arguments = {mode: self.parameter}
         return definitions.compressor_map[self.compressor](**arguments)
 
     def description(self) -> str:
+        """
+        Returns a description of the lossy encoding.
+
+        Returns:
+        - str: A description of the lossy encoding.
+
+        """
         return f"Lossy compressed using the HDF5 filters with specification: {self.to_string()} " \
                f"(Using {self.compressor!r} with mode {self.mode!r} and parameter {self.parameter})"
 
     def __repr__(self):
+        """
+        Returns a string representation of the LossyEncoding object.
+
+        Returns:
+        - str: A string representation of the LossyEncoding object.
+
+        """
         return f"{self.__class__.__name__}(compressor={self.compressor}, mode={self.mode}, parameter={self.parameter})"
 
 
 def parse_variable_specification(var_spec: str) -> Encoding:
     """
     Parse a string following the compression specification format for a single variable
      and return a Specification object.
@@ -239,24 +306,23 @@
     Returns
     -------
 
     """
     if var_spec in (None, "None", "none"):
         return NullEncoding()
 
-    from enstools.encoding.rules import COMPRESSION_SPECIFICATION_SEPARATOR
     # Split the specification in the different parts.
     var_spec_parts = var_spec.split(COMPRESSION_SPECIFICATION_SEPARATOR)
     # Treatment for lossless
     if var_spec_parts[0] == "lossless":
         backend = var_spec_parts[1] if len(var_spec_parts) > 1 else None
         compression_level = int(var_spec_parts[2]) if len(var_spec_parts) > 2 else None
         return LosslessEncoding(backend, compression_level)
     # Treatment for lossy
-    elif var_spec_parts[0] == "lossy":
+    if var_spec_parts[0] == "lossy":
         # Lossy specifications must have 4 elements (lossy,compressor,mode,parameter)
         if len(var_spec_parts) != 4:
             raise InvalidCompressionSpecification(f"Invalid specification {var_spec!r}")
 
         # Get the different components.
         compressor, mode, specification = var_spec_parts[1:]
         # Check that the compressor is a valid option.
@@ -269,17 +335,17 @@
         # Cast the specification to the proper type.
         specification_type = lossy_compressors_and_modes[compressor][mode]["type"]
         try:
             specification = specification_type(specification)
         except ValueError:
             raise InvalidCompressionSpecification(f"Could not cast {specification!r} to type {specification_type!r}")
         return LossyEncoding(compressor, mode, specification)
-    else:
-        # In case its not lossy nor lossless, raise an exception.
-        raise InvalidCompressionSpecification(f"Invalid specification {var_spec!r}")
+
+    # In case its not lossy nor lossless, raise an exception.
+    raise InvalidCompressionSpecification(f"Invalid specification {var_spec!r}")
 
 
 def get_variable_encoding(
         specification: str = None,
         compressor: str = None,
         mode: str = None,
         parameter: Union[str, float, int] = None,
@@ -297,17 +363,17 @@
     if (specification is None) and (compressor is None) and (backend is None):
         return LosslessEncoding(backend=LOSSLESS_DEFAULT_BACKEND, compression_level=LOSSLESS_DEFAULT_COMPRESSION_LEVEL)
 
     assert (specification is None) + (compressor is None) + (backend is None) == 2, \
         "Only one of the options can be used to create an Encoding"
     if specification:
         return parse_variable_specification(specification)
-    elif compressor:
+    if compressor:
         return LossyEncoding(compressor=compressor, mode=mode, parameter=parameter)
-    elif backend:
+    if backend:
         if compression_level is None:
             compression_level = LOSSLESS_DEFAULT_COMPRESSION_LEVEL
         return LosslessEncoding(backend=backend, compression_level=compression_level)
 
 
 def is_valid_variable_compression_specification(specification):
     try:
```

### Comparing `enstools-encoding-2023.4.1/enstools_encoding.egg-info/PKG-INFO` & `enstools-encoding-2023.6/enstools_encoding.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: enstools-encoding
-Version: 2023.4.1
-Summary: UNKNOWN
+Version: 2023.6
 Home-page: https://github.com/wavestoweather/enstools-encoding
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-encoding [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-encoding.readthedocs.io/en/latest/?badge=latest)
 
 Library to generate the encodings to write compressed files as easily as possible with **xarray** using **hdf5 filters**.
 
@@ -48,9 +45,7 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
-
-
```

### Comparing `enstools-encoding-2023.4.1/enstools_encoding.egg-info/SOURCES.txt` & `enstools-encoding-2023.6/enstools_encoding.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 VERSION
 setup.py
 enstools/encoding/__init__.py
 enstools/encoding/api.py
+enstools/encoding/chunk_size.py
 enstools/encoding/dataset_encoding.py
 enstools/encoding/definitions.py
 enstools/encoding/errors.py
 enstools/encoding/rules.py
 enstools/encoding/variable_encoding.py
 enstools_encoding.egg-info/PKG-INFO
 enstools_encoding.egg-info/SOURCES.txt
```

### Comparing `enstools-encoding-2023.4.1/setup.py` & `enstools-encoding-2023.6/setup.py`

 * *Files identical despite different names*

### Comparing `enstools-encoding-2023.4.1/test/test_classes.py` & `enstools-encoding-2023.6/test/test_classes.py`

 * *Files identical despite different names*

