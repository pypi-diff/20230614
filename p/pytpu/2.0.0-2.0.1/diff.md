# Comparing `tmp/pytpu-2.0.0.tar.gz` & `tmp/pytpu-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytpu-2.0.0.tar", last modified: Wed Apr 26 11:03:38 2023, max compression
+gzip compressed data, was "dist/pytpu-2.0.1.tar", last modified: Thu Apr 27 12:00:44 2023, max compression
```

## Comparing `pytpu-2.0.0.tar` & `pytpu-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.272816 pytpu-2.0.0/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-26 11:02:53.000000 pytpu-2.0.0/MANIFEST.in
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-26 11:03:38.272816 pytpu-2.0.0/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3137 2023-04-26 11:02:53.000000 pytpu-2.0.0/README.md
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      255 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/__init__.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      306 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5047 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/converter_to_raw.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    14101 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/libtpu_bindings.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/scripts/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2352 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/pyrun_tpu_cli.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      834 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/run_get_fps.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.272816 pytpu-2.0.0/pytpu/tools/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      123 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3919 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/get_fps.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6073 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/helpers.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2896 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/lenet5_processing.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3758 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/resnet50_processing.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7094 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/tpu_runner.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu.egg-info/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      589 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/entry_points.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/not-zip-safe
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       84 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/top_level.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-26 11:03:38.272816 pytpu-2.0.0/setup.cfg
--rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)      970 2023-04-26 11:03:38.000000 pytpu-2.0.0/setup.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 12:00:44.770956 pytpu-2.0.1/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-27 11:59:59.000000 pytpu-2.0.1/MANIFEST.in
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-27 12:00:44.770956 pytpu-2.0.1/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3137 2023-04-27 11:59:59.000000 pytpu-2.0.1/README.md
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 12:00:44.766956 pytpu-2.0.1/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      328 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    16772 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu/_bindings.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5657 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu/_converter_to_raw.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 12:00:44.770956 pytpu-2.0.1/pytpu.egg-info/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      627 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/entry_points.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/not-zip-safe
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      144 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       18 2023-04-27 12:00:44.000000 pytpu-2.0.1/pytpu.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 12:00:44.770956 pytpu-2.0.1/pytpu_tests/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/__init__.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 12:00:44.770956 pytpu-2.0.1/pytpu_tests/unit/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      786 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/_helpres.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2933 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/_lenet5.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3796 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/_resnet50.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5566 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/test_lenet5.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      773 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/test_program_lut_parameters.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3833 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/test_resnet50.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      443 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/test_total_mem.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     1175 2023-04-27 11:59:59.000000 pytpu-2.0.1/pytpu_tests/unit/test_watchdog_error.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-27 12:00:44.770956 pytpu-2.0.1/setup.cfg
+-rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1291 2023-04-27 12:00:44.000000 pytpu-2.0.1/setup.py
```

### Comparing `pytpu-2.0.0/PKG-INFO` & `pytpu-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 2.0.0
+Version: 2.0.1
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: IVA-Tech
 Author-email: info@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

### Comparing `pytpu-2.0.0/README.md` & `pytpu-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytpu-2.0.0/pytpu/pytpu/converter_to_raw.py` & `pytpu-2.0.1/pytpu/_converter_to_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-import os
+# type: ignore
+
+from __future__ import annotations
+
+# TODO: fix type ignore
+
+__all__ = [
+    'convert_to_raw'
+]
+
 import copy
-import shutil
-import numpy as np
 import json
+import os
+import shutil
 import tempfile
 import zipfile
 from math import ceil
-
-from typing import Dict
 from typing import Any
+from typing import Dict
+from typing import TYPE_CHECKING
 
-try:
-    from tpu_tlm_is.models.iotools import tpu_encode, tpu_decode
+import numpy as np
+
+if TYPE_CHECKING:
     from tpu_tlm_is.base import TensorDescription
     from tpu_tlm_is.base import TpuParameters
-    from tpu_tlm_is.base import get_hw_params
-    from tpu_tlm_is.base.number_types import STR_TO_USER_NUMBER_TYPE
-    from tpu_tlm_is.base.number_types import STR_TO_TPU_NUMBER_TYPE
-    from tpu_tlm_is.base.number_types import UserNumberType
-    from tpu_tlm_is.base.number_types import TpuNumberType
-except ImportError:
-    pass
 
 
 class Codec:
-    def __init__(self, tpu_par, tensor_descriptions):
+    def __init__(self, tpu_par: TpuParameters, tensor_descriptions: Dict[str, TensorDescription]) -> None:
         self._tpu_par = tpu_par
         self._tensor_descriptions = tensor_descriptions
 
-    def encode(self, input_dict):
+    def encode(self, input_dict: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
+        from tpu_tlm_is.models.iotools import tpu_encode
         return tpu_encode(self._tpu_par, input_dict, self._tensor_descriptions)
 
-    def decode(self, output_raw_dict):
+    def decode(self, output_raw_dict: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
+        from tpu_tlm_is.models.iotools import tpu_decode
         return tpu_decode(self._tpu_par, output_raw_dict, self._tensor_descriptions)
 
 
 def _to_raw_old(io_: Dict[str, Any], name: str) -> Dict[str, Any]:
+    # TODO: this is fake raw mode, need to clarify that
+
     size = io_['size']
     io_out = {
         'address': io_['address'],
         'size': size,
         'user_shape': [1, size, ],
         'user_order': ['N', 'C', ],
         'user_dtype': 'int8',
@@ -50,14 +57,16 @@
         'scales': [1.0, ],
         'anchor': io_.get('anchor', name),
     }
     return io_out
 
 
 def _get_tpu_parameters(hw_par: Dict[str, Any]) -> TpuParameters:
+    from tpu_tlm_is.base import get_hw_params
+
     if hw_par['cache_word_len'] == 128 and hw_par['ddr_word_len'] == 32:
         return get_hw_params('128x128').tpu_parameters
     if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 16:
         return get_hw_params('64x64').tpu_parameters
     if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 64:
         return get_hw_params('64x64_fpga').tpu_parameters
 
@@ -74,43 +83,50 @@
         for name, _ in region.items():
             raw_metadata['outputs'][idx][name] = _to_raw_old(metadata['outputs'][idx][name], name)
 
     return raw_metadata
 
 
 def _get_tensor_description(io_: Dict[str, Any], cwl: int) -> TensorDescription:
+    from tpu_tlm_is.base import TensorDescription
+    from tpu_tlm_is.base.number_types import STR_TO_USER_NUMBER_TYPE
+    from tpu_tlm_is.base.number_types import STR_TO_TPU_NUMBER_TYPE
+    from tpu_tlm_is.base.number_types import UserNumberType
+    from tpu_tlm_is.base.number_types import TpuNumberType
+
     if 'user_shape' in io_.keys():
         return TensorDescription(
             user_shape_mask=tuple(tuple([True, ] * abs(p[0]) + [False, ] * s + [True, ] * abs(p[1])
-                                  for p, s in zip(io_['padding'], io_['user_shape']))),
+                                        for p, s in zip(io_['padding'], io_['user_shape']))),
             user_order=io_['user_order'],
             user_dtype=STR_TO_USER_NUMBER_TYPE[io_['user_dtype']],
             tpu_shape=io_['tpu_shape'],
             tpu_order=io_['tpu_order'],
             tpu_dtype=STR_TO_TPU_NUMBER_TYPE[io_['tpu_dtype']],
             scales=tuple([float(s) for s in io_['scales']]),
             anchor=io_['anchor'],
         )
     else:
         return TensorDescription(
-            user_shape_mask=((False, ), tuple([False, ] * int(io_['size'])), ),
-            user_order=('N', 'C', ),
+            user_shape_mask=((False,), tuple([False, ] * int(io_['size'])),),
+            user_order=('N', 'C',),
             user_dtype=UserNumberType.INT8,
             tpu_shape=(1, ceil(int(io_['size']) / cwl), np.minimum(cwl, int(io_['size']))),
             tpu_order=('N', 'C', 'B'),
             tpu_dtype=TpuNumberType.INT8,
-            scales=(1.0, ),
+            scales=(1.0,),
         )
 
 
 def convert_to_raw(program_path: str, raw_program_path: str) -> Codec:
     try:
         from tpu_tlm_is.base import TensorDescription
     except ImportError:
-        raise BaseException('no tpu_tlm_is package found')
+        raise ImportError('Raw conversion is a debug feature that requires internal'
+                          ' library tpu_tlm_is to be installed.')
 
     with zipfile.ZipFile(program_path, 'r') as program:
         data = program.read('metadata.json')
 
     metadata = json.loads(data)
     tpu_par = _get_tpu_parameters(metadata['hardware_parameters'])
     tensor_descriptions: Dict[str, TensorDescription] = dict()
@@ -119,14 +135,16 @@
         for name, io_ in region.items():
             tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
 
     for _, region in metadata['outputs'].items():
         for name, io_ in region.items():
             tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
 
+    # TODO: rewrite later without extracting all zip file to a temp directory
+
     with tempfile.TemporaryDirectory() as tempdir:
         with zipfile.ZipFile(program_path, 'r') as zip_obj:
             zip_obj.extractall(tempdir)
 
         with open(os.path.join(tempdir, 'metadata.json'), 'w') as metadata_file:
             json.dump(_to_raw(metadata), metadata_file, indent=4)
```

### Comparing `pytpu-2.0.0/pytpu/pytpu/libtpu_bindings.py` & `pytpu-2.0.1/pytpu/_bindings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,316 @@
+from __future__ import annotations
+
+__all__ = [
+    'Device',
+    'Program',
+    'Inference',
+    'InferenceError',
+]
+
+import collections.abc
+import contextlib
 import json
+import os
+import re
 from ctypes import (CDLL, c_char, c_char_p, c_int, c_void_p, c_uint8, c_size_t, c_bool, cast,
                     POINTER, CFUNCTYPE, Structure)
 from enum import Enum
+from typing import Any
+from typing import Dict
+from typing import Generator
+from typing import List
+from typing import Mapping
+from typing import Optional
 
 import numpy as np
-import contextlib
-from typing import Mapping
-from typing import Dict
-from typing import Any
-import collections.abc
-from ..tools.helpers import get_tpu_devices
 
-libtpu = CDLL('/usr/lib/libtpu.2.so')
+_LIB_TPU_SO_PATH = '/usr/lib/libtpu.2.so'
+
+
 # libtpu = CDLL('libtpu-experimental/build/libtpu.so')
 # libtpu = CDLL('/home/d.baburin/iva_tpu_sdk/libtpu.2/build/libtpu.2.so')
 
-__all__ = [
-    'Device',  # TODO: consider remove TPU prefix? recommended user will be "import pytpu as tpu; tpu.Device(...)"?
-    'Program',
-    'Inference',
-    'ProcessingMode',
-]
+
+class _LibTPUBinder:
+    """This class lazy binds to libtpu *.so file thus allowing module to be imported without *.so file"""
+
+    def __init__(self):
+        self._libtpu: Optional[CDLL] = None
+
+    @property
+    def libtpu(self) -> CDLL:
+        if self._libtpu is None:
+            self._bind()
+
+        assert self._libtpu is not None
+
+        return self._libtpu
+
+    def _bind(self) -> None:
+        libtpu = CDLL(_LIB_TPU_SO_PATH)
+
+        _cb_pointer = CFUNCTYPE(None, POINTER(Inference), c_int, c_void_p)
+
+        # Device
+        libtpu.tpu_create_device.restype = POINTER(Device)
+        # libtpu.tpu_create_device.argtypes = [c_int]
+        libtpu.tpu_create_device.argtypes = [c_char_p]
+
+        libtpu.tpu_destroy_device.restype = c_void_p
+        libtpu.tpu_destroy_device.argtypes = [POINTER(Device)]
+
+        libtpu.tpu_is_device_valid.restype = c_int
+        libtpu.tpu_is_device_valid.argtypes = [POINTER(Device)]
+
+        libtpu.tpu_init_device.restype = c_int
+        libtpu.tpu_init_device.argtypes = [POINTER(Device)]
+
+        libtpu.tpu_get_device_error_message.restype = c_char_p
+        libtpu.tpu_get_device_error_message.argtypes = [POINTER(Device)]
+
+        libtpu.tpu_get_device_info.restype = c_char_p
+        libtpu.tpu_get_device_info.argtypes = [POINTER(Device)]
+
+        libtpu.tpu_load_program.restype = c_int
+        libtpu.tpu_load_program.argtypes = [POINTER(Device), POINTER(Program)]
+
+        libtpu.tpu_run_inference.restype = c_int
+        libtpu.tpu_run_inference.argtypes = [POINTER(Device), POINTER(Inference), c_int]
+
+        libtpu.tpu_submit_inference.restype = c_int
+        libtpu.tpu_submit_inference.argtypes = [POINTER(Device), POINTER(Inference), c_int, _cb_pointer, c_void_p]
+
+        # Program
+        libtpu.tpu_create_program.restype = POINTER(Program)
+        libtpu.tpu_create_program.argtypes = [POINTER(c_char), c_int]
+
+        libtpu.tpu_destroy_program.restype = c_void_p
+        libtpu.tpu_destroy_program.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_is_program_valid.restype = c_int
+        libtpu.tpu_is_program_valid.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_program_info.restype = c_char_p
+        libtpu.tpu_get_program_info.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_program_error_message.restype = c_char_p
+        libtpu.tpu_get_program_error_message.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_batch_size.restype = c_size_t
+        libtpu.tpu_get_batch_size.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_input_count.restype = c_size_t
+        libtpu.tpu_get_input_count.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_input_size.restype = c_size_t
+        libtpu.tpu_get_input_size.argtypes = [POINTER(Program), c_size_t, c_bool]
+
+        libtpu.tpu_get_output_count.restype = c_size_t
+        libtpu.tpu_get_output_count.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_get_output_size.restype = c_size_t
+        libtpu.tpu_get_output_size.argtypes = [POINTER(Program), c_size_t, c_bool]
+
+        # _TensorBufferObject
+        libtpu.tpu_create_tensor_buffer_object.restype = POINTER(_TensorBufferObject)
+        libtpu.tpu_create_tensor_buffer_object.argtypes = [POINTER(Program), c_int]
+
+        libtpu.tpu_destroy_tensor_buffer_object.restype = c_void_p
+        libtpu.tpu_destroy_tensor_buffer_object.argtypes = [POINTER(_TensorBufferObject)]
+
+        libtpu.tpu_process_tensor_buffers.restype = c_void_p
+        libtpu.tpu_process_tensor_buffers.argtypes = [POINTER(_TensorBufferObject)]
+
+        libtpu.tpu_get_tensor_buffer_ptr.restype = POINTER(c_uint8)
+        libtpu.tpu_get_tensor_buffer_ptr.argtypes = [POINTER(_TensorBufferObject), c_size_t, c_bool]
+
+        libtpu.tpu_set_user_tensor_buffer_ptr.restype = POINTER(c_uint8)
+        libtpu.tpu_set_user_tensor_buffer_ptr.argtypes = [POINTER(_TensorBufferObject), c_size_t, POINTER(c_uint8)]
+
+        # Inference
+        libtpu.tpu_create_inference.restype = POINTER(Inference)
+        libtpu.tpu_create_inference.argtypes = [POINTER(Program)]
+
+        libtpu.tpu_destroy_inference.restype = c_void_p
+        libtpu.tpu_destroy_inference.argtypes = [POINTER(Inference)]
+
+        libtpu.tpu_get_inference_program.restype = POINTER(Program)
+        libtpu.tpu_get_inference_program.argtypes = [POINTER(Inference)]
+
+        libtpu.tpu_get_inference_inputs.restype = POINTER(_TensorBufferObject)
+        libtpu.tpu_get_inference_inputs.argtypes = [POINTER(Inference)]
+
+        libtpu.tpu_set_inference_inputs.restype = POINTER(_TensorBufferObject)
+        libtpu.tpu_set_inference_inputs.argtypes = [POINTER(Inference), POINTER(_TensorBufferObject)]
+
+        libtpu.tpu_get_inference_outputs.restype = POINTER(_TensorBufferObject)
+        libtpu.tpu_get_inference_outputs.argtypes = [POINTER(Inference)]
+
+        libtpu.tpu_set_inference_outputs.restype = POINTER(_TensorBufferObject)
+        libtpu.tpu_set_inference_outputs.argtypes = [POINTER(Inference), POINTER(_TensorBufferObject)]
+
+        libtpu.tpu_get_inference_status.restype = c_int
+        libtpu.tpu_get_inference_status.argtypes = [POINTER(Inference)]
+
+        libtpu.tpu_get_inference_error_message.restype = c_char_p
+        libtpu.tpu_get_inference_error_message.argtypes = [POINTER(Inference)]
+
+        self._libtpu = libtpu
+
+
+_LIB_TPU_BINDER = _LibTPUBinder()
 
 
 class ProcessingMode(Enum):
     RAW = 0
     PRE_PROCESS = 1
     POST_PROCESS = 2
     FULL = 3
 
 
 class _TensorBufferType(Enum):
     INPUTS = 0
     OUTPUTS = 1
 
 
+_Pointer = Any
+
+
 class Device(Structure):
     _fields_ = []
 
     @staticmethod
     @contextlib.contextmanager
-    def open(dev_name):
-        if not isinstance(dev_name, bytes):
-            dev_name = dev_name.encode('utf-8')
+    def open(dev_name: str) -> Generator[Device, None, None]:
+        if not isinstance(dev_name, str):
+            raise ValueError(f'Device name must be a string: {type(dev_name)}')
 
-        pointer = libtpu.tpu_create_device(c_char_p(dev_name))
+        pointer = _LIB_TPU_BINDER.libtpu.tpu_create_device(c_char_p(dev_name.encode('utf-8')))
         device = Device(pointer)
 
         yield device
-        libtpu.tpu_destroy_device(pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_device(pointer)
 
     @staticmethod
-    def list_devices():
-        list_devices = get_tpu_devices()
-        if len(list_devices) < 1:
-            raise EnvironmentError('No TPU devices found')
-
-        return list_devices
+    def list_devices() -> List[str]:
+        # TODO: check why len(f) == 4?
+        return [os.path.join('/dev', f) for f in os.listdir('/dev') if re.match(r'tpu.', f) and len(f) == 4]
 
-    def __init__(self, pointer):
+    def __init__(self, pointer: _Pointer) -> None:
 
         super().__init__()
 
         self._pointer = pointer
 
-        init_code = libtpu.tpu_init_device(pointer)
+        init_code = _LIB_TPU_BINDER.libtpu.tpu_init_device(pointer)
         if init_code != 0:
             raise ValueError(f'Invalid init code {init_code}: {self._get_error_message()}')
 
-        if not libtpu.tpu_is_device_valid(self._pointer):
+        if not _LIB_TPU_BINDER.libtpu.tpu_is_device_valid(self._pointer):
             raise ValueError(f'Invalid device: {self._get_error_message()}')
 
     def _get_error_message(self) -> str:
-        msg = libtpu.tpu_get_device_error_message(self._pointer)
+        msg = _LIB_TPU_BINDER.libtpu.tpu_get_device_error_message(self._pointer)
         return msg.decode('utf-8')
 
-    def info(self):
-        return libtpu.tpu_get_device_info(self._pointer)
+    # TODO: user https://mypy.readthedocs.io/en/latest/more_types.html#typeddict ?
+    def info(self) -> Dict:
+        return json.loads(_LIB_TPU_BINDER.libtpu.tpu_get_device_info(self._pointer).decode('utf-8'))
 
-    def close(self):
-        libtpu.tpu_destroy_device(self._pointer)
+    def close(self) -> None:
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_device(self._pointer)
 
     @contextlib.contextmanager
-    def load(self, program_path, raw=False):
-        if not isinstance(program_path, bytes):
-            program_path = program_path.encode('utf-8')
+    def load(self, program_path: str, raw: bool = False) -> Generator[Program, None, None]:
+
+        # TODO: replace raw with .zip file inspection?
+
+        if not isinstance(program_path, str):
+            raise ValueError(f'Program path must be a string: {type(program_path)}')
 
-        program_pointer = libtpu.tpu_create_program(c_char_p(program_path), raw)
+        program_pointer = _LIB_TPU_BINDER.libtpu.tpu_create_program(c_char_p(program_path.encode('utf-8')), raw)
         program = Program(self, program_pointer)
-        libtpu.tpu_load_program(self._pointer, program_pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_load_program(self._pointer, program_pointer)
 
         yield program
-        libtpu.tpu_destroy_program(program_pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_program(program_pointer)
 
 
 class _TensorBufferObject(Structure):
     _fields_ = []
 
-    def __init__(self, pointer):
+    def __init__(self, pointer: _Pointer) -> None:
         super().__init__()
         self._pointer = pointer
 
-    def set_user_tensor_buffer_ptr(self, n, ptr):
-        return libtpu.tpu_set_user_tensor_buffer_ptr(self._pointer, c_size_t(n), ptr)
+    def set_user_tensor_buffer_ptr(self, n: int, ptr: _Pointer) -> _Pointer:
+        return _LIB_TPU_BINDER.libtpu.tpu_set_user_tensor_buffer_ptr(self._pointer, c_size_t(n), ptr)
 
 
 class Program(Structure):
     _fields_ = []
 
-    def __init__(self, device: Device, pointer):
+    def __init__(self, device: Device, pointer: _Pointer) -> None:
         super().__init__()
 
         self._device = device
         self._pointer = pointer
 
         # Check status
-        if not libtpu.tpu_is_program_valid(self._pointer):
-            msg = libtpu.tpu_get_program_error_message(self._pointer)
+        if not _LIB_TPU_BINDER.libtpu.tpu_is_program_valid(self._pointer):
+            msg = _LIB_TPU_BINDER.libtpu.tpu_get_program_error_message(self._pointer)
             raise ValueError('Invalid program: ' + str(msg.decode('utf-8')))
 
         # Preload metadata
-        metadata = json.loads(self.info())
+        metadata = self.info()
         self._input_metadata = metadata['inputs']['1']
         self._output_metadata = metadata['outputs']['2']
 
-    def info(self):
-        return libtpu.tpu_get_program_info(self._pointer)
+    # TODO: Use https://mypy.readthedocs.io/en/latest/more_types.html#typeddict here?
+    def info(self) -> Dict:
+        return json.loads(_LIB_TPU_BINDER.libtpu.tpu_get_program_info(self._pointer).decode('utf-8'))
 
-    def get_input_size(self, n, raw):
-        return libtpu.tpu_get_input_size(self._pointer, c_size_t(n), c_bool(raw))
+    def get_input_size(self, n: int, raw: bool) -> int:
+        return _LIB_TPU_BINDER.libtpu.tpu_get_input_size(self._pointer, c_size_t(n), c_bool(raw))
 
-    def get_output_size(self, n, raw):
-        return libtpu.tpu_get_output_size(self._pointer, c_size_t(n), c_bool(raw))
+    def get_output_size(self, n: int, raw: bool) -> int:
+        return _LIB_TPU_BINDER.libtpu.tpu_get_output_size(self._pointer, c_size_t(n), c_bool(raw))
 
-    def close(self):
-        libtpu.tpu_destroy_program(self._pointer)
+    def close(self) -> None:
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_program(self._pointer)
 
     @contextlib.contextmanager
-    def inference(self):
+    def inference(self) -> Generator[Inference, None, None]:
         inference = Inference(self)
         yield inference
         inference.close()
 
     @contextlib.contextmanager
-    def buffer(self, type_: _TensorBufferType):
-        buffer_pointer = libtpu.tpu_create_tensor_buffer_object(self._pointer, type_.value)  # make pointer
+    def buffer(self, type_: _TensorBufferType) -> Generator[_TensorBufferObject, None, None]:
+        buffer_pointer = _LIB_TPU_BINDER.libtpu.tpu_create_tensor_buffer_object(self._pointer,
+                                                                                type_.value)  # make pointer
         yield _TensorBufferObject(buffer_pointer)
-        libtpu.tpu_destroy_tensor_buffer_object(buffer_pointer)  # destroy pointer
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_tensor_buffer_object(buffer_pointer)  # destroy pointer
 
 
 CTX = Any
 
 
+class InferenceError(ValueError):
+    """Exception raised if libtpu reports inference as invalid"""
+
+
 class Inference(Structure):
     _fields_ = []
 
     def __init__(self, program: Program, raw: bool = False):
         super().__init__()
         self._program = program
-        self._pointer = libtpu.tpu_create_inference(program._pointer)
+        self._pointer = _LIB_TPU_BINDER.libtpu.tpu_create_inference(program._pointer)
         self._raw = raw
 
         # Explicitly order inputs and outputs:
         _input_tensor_name_to_input_tensor_index = {
             tensor_name: i
             for i, tensor_name in enumerate(program._input_metadata)
         }
@@ -187,22 +335,29 @@
             for tensor_name in program._output_metadata
         }
 
         self._tensor_name_to_tensor_size: Dict[str, int] = dict()
         self._tensor_name_to_tensor_size.update(_input_sizes)
         self._tensor_name_to_tensor_size.update(_output_sizes)
 
-    def _run(self, mode: ProcessingMode):
-        libtpu.tpu_run_inference(
+    def _run(self, mode: ProcessingMode) -> None:
+        status_code = _LIB_TPU_BINDER.libtpu.tpu_run_inference(
             self._program._device._pointer,  # device pointer
             self._pointer,  # inference pointer
             mode.value,  # pass numerical value of processing mode
         )
 
-    def sync(self, inputs, mode: ProcessingMode = ProcessingMode.FULL):
+        if status_code != 0:
+            msg = self._get_error_message()
+            raise InferenceError(f'Invalid tpu_run_inference return code {status_code}: {msg}')
+
+    def _get_error_message(self) -> str:
+        return _LIB_TPU_BINDER.libtpu.tpu_get_inference_error_message(self._pointer).decode('utf-8')
+
+    def sync(self, inputs, mode: ProcessingMode = ProcessingMode.FULL) -> Dict[str, np.ndarray]:
 
         with contextlib.ExitStack() as buffer_exit_stack:
             # Reserve pointers for input and output buffers:
             tpu_input_buf = buffer_exit_stack.enter_context(self._program.buffer(_TensorBufferType.INPUTS))
             tpu_output_buf = buffer_exit_stack.enter_context(self._program.buffer(_TensorBufferType.OUTPUTS))
 
             # Load
@@ -217,22 +372,22 @@
             # NOTE: only after we have a copy of results in memory as numpy arrays -
             #       we can exit from buffer_exit_stack thus releasing IO pointers!
 
         self._check_status()
 
         return result
 
-    def _check_status(self):
-        status_code = libtpu.tpu_get_inference_status(self._pointer)
+    def _check_status(self) -> None:
+        status_code = _LIB_TPU_BINDER.libtpu.tpu_get_inference_status(self._pointer)
         if status_code != 0:
-            msg = libtpu.tpu_get_inference_error_message(self._pointer).decode('utf-8')
-            raise ValueError(f'Invalid inference status code {status_code}: {msg}')
+            msg = self._get_error_message()
+            raise InferenceError(f'Invalid inference status code {status_code}: {msg}')
 
     def close(self):
-        libtpu.tpu_destroy_inference(self._pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_destroy_inference(self._pointer)
 
     def _load_inference(self, tpu_input: _TensorBufferObject, tpu_output: _TensorBufferObject,
                         input_data: Mapping[str, np.ndarray]) -> Dict[str, CTX]:
 
         if not isinstance(input_data, collections.abc.Mapping):
             raise ValueError('Input data must be a mapping, got:' + str(type(input_data)))
 
@@ -241,15 +396,15 @@
             tensor_idx = self._tensor_name_to_tensor_index[tensor_name]
             tensor_size = self._tensor_name_to_tensor_size[tensor_name]
 
             in_tensor = bytearray(tensor_data)
             p_in_tensor = (c_uint8 * tensor_size).from_buffer(in_tensor)
             tpu_input.set_user_tensor_buffer_ptr(tensor_idx, cast(p_in_tensor, POINTER(c_uint8)))
 
-        libtpu.tpu_set_inference_inputs(self._pointer, tpu_input._pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_set_inference_inputs(self._pointer, tpu_input._pointer)
 
         # Outputs:
         out_ctx = dict()
 
         for tensor_name in self._program._output_metadata:
             tensor_idx = self._tensor_name_to_tensor_index[tensor_name]
             tensor_size = self._tensor_name_to_tensor_size[tensor_name]
@@ -257,15 +412,15 @@
             out_tensor = bytearray(np.empty((tensor_size,), dtype=np.uint8))
             p_out_tensor = (c_uint8 * tensor_size).from_buffer(out_tensor)
             c_out_ptr = cast(p_out_tensor, POINTER(c_uint8))
             tpu_output.set_user_tensor_buffer_ptr(tensor_idx, c_out_ptr)
 
             out_ctx[tensor_name] = c_out_ptr
 
-        libtpu.tpu_set_inference_outputs(self._pointer, tpu_output._pointer)
+        _LIB_TPU_BINDER.libtpu.tpu_set_inference_outputs(self._pointer, tpu_output._pointer)
 
         return out_ctx
 
     def _get_inference(self, ctx: Dict[str, CTX]) -> Dict[str, np.ndarray]:
         out_meta = self._program._output_metadata
         collected_data = dict()
 
@@ -277,121 +432,14 @@
             data = data.reshape(out_meta[tensor_name]['user_shape'])
 
             collected_data[tensor_name] = data
 
         return collected_data
 
 
-CB_POINTER = CFUNCTYPE(None, POINTER(Inference), c_int, c_void_p)
-
-# TPUDevice
-libtpu.tpu_create_device.restype = POINTER(Device)
-# libtpu.tpu_create_device.argtypes = [c_int]
-libtpu.tpu_create_device.argtypes = [c_char_p]
-
-libtpu.tpu_destroy_device.restype = c_void_p
-libtpu.tpu_destroy_device.argtypes = [POINTER(Device)]
-
-libtpu.tpu_is_device_valid.restype = c_int
-libtpu.tpu_is_device_valid.argtypes = [POINTER(Device)]
-
-libtpu.tpu_init_device.restype = c_int
-libtpu.tpu_init_device.argtypes = [POINTER(Device)]
-
-libtpu.tpu_get_device_error_message.restype = c_char_p
-libtpu.tpu_get_device_error_message.argtypes = [POINTER(Device)]
-
-libtpu.tpu_get_device_info.restype = c_char_p
-libtpu.tpu_get_device_info.argtypes = [POINTER(Device)]
-
-libtpu.tpu_load_program.restype = c_int
-libtpu.tpu_load_program.argtypes = [POINTER(Device), POINTER(Program)]
-
-libtpu.tpu_run_inference.restype = c_int
-libtpu.tpu_run_inference.argtypes = [POINTER(Device), POINTER(Inference), c_int]
-
-libtpu.tpu_submit_inference.restype = c_int
-libtpu.tpu_submit_inference.argtypes = [POINTER(Device), POINTER(Inference), c_int, CB_POINTER, c_void_p]
-
-# TPUProgram
-libtpu.tpu_create_program.restype = POINTER(Program)
-libtpu.tpu_create_program.argtypes = [POINTER(c_char), c_int]
-
-libtpu.tpu_destroy_program.restype = c_void_p
-libtpu.tpu_destroy_program.argtypes = [POINTER(Program)]
-
-libtpu.tpu_is_program_valid.restype = c_int
-libtpu.tpu_is_program_valid.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_program_info.restype = c_char_p
-libtpu.tpu_get_program_info.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_program_error_message.restype = c_char_p
-libtpu.tpu_get_program_error_message.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_batch_size.restype = c_size_t
-libtpu.tpu_get_batch_size.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_input_count.restype = c_size_t
-libtpu.tpu_get_input_count.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_input_size.restype = c_size_t
-libtpu.tpu_get_input_size.argtypes = [POINTER(Program), c_size_t, c_bool]
-
-libtpu.tpu_get_output_count.restype = c_size_t
-libtpu.tpu_get_output_count.argtypes = [POINTER(Program)]
-
-libtpu.tpu_get_output_size.restype = c_size_t
-libtpu.tpu_get_output_size.argtypes = [POINTER(Program), c_size_t, c_bool]
-
-# TPUTensorBufferObject
-libtpu.tpu_create_tensor_buffer_object.restype = POINTER(_TensorBufferObject)
-libtpu.tpu_create_tensor_buffer_object.argtypes = [POINTER(Program), c_int]
-
-libtpu.tpu_destroy_tensor_buffer_object.restype = c_void_p
-libtpu.tpu_destroy_tensor_buffer_object.argtypes = [POINTER(_TensorBufferObject)]
-
-libtpu.tpu_process_tensor_buffers.restype = c_void_p
-libtpu.tpu_process_tensor_buffers.argtypes = [POINTER(_TensorBufferObject)]
-
-libtpu.tpu_get_tensor_buffer_ptr.restype = POINTER(c_uint8)
-libtpu.tpu_get_tensor_buffer_ptr.argtypes = [POINTER(_TensorBufferObject), c_size_t, c_bool]
-
-libtpu.tpu_set_user_tensor_buffer_ptr.restype = POINTER(c_uint8)
-libtpu.tpu_set_user_tensor_buffer_ptr.argtypes = [POINTER(_TensorBufferObject), c_size_t, POINTER(c_uint8)]
-
-# TPUInference
-libtpu.tpu_create_inference.restype = POINTER(Inference)
-libtpu.tpu_create_inference.argtypes = [POINTER(Program)]
-
-libtpu.tpu_destroy_inference.restype = c_void_p
-libtpu.tpu_destroy_inference.argtypes = [POINTER(Inference)]
-
-libtpu.tpu_get_inference_program.restype = POINTER(Program)
-libtpu.tpu_get_inference_program.argtypes = [POINTER(Inference)]
-
-libtpu.tpu_get_inference_inputs.restype = POINTER(_TensorBufferObject)
-libtpu.tpu_get_inference_inputs.argtypes = [POINTER(Inference)]
-
-libtpu.tpu_set_inference_inputs.restype = POINTER(_TensorBufferObject)
-libtpu.tpu_set_inference_inputs.argtypes = [POINTER(Inference), POINTER(_TensorBufferObject)]
-
-libtpu.tpu_get_inference_outputs.restype = POINTER(_TensorBufferObject)
-libtpu.tpu_get_inference_outputs.argtypes = [POINTER(Inference)]
-
-libtpu.tpu_set_inference_outputs.restype = POINTER(_TensorBufferObject)
-libtpu.tpu_set_inference_outputs.argtypes = [POINTER(Inference), POINTER(_TensorBufferObject)]
-
-libtpu.tpu_get_inference_status.restype = c_int
-libtpu.tpu_get_inference_status.argtypes = [POINTER(Inference)]
-
-libtpu.tpu_get_inference_error_message.restype = c_char_p
-libtpu.tpu_get_inference_error_message.argtypes = [POINTER(Inference)]
-
-
 def _convert_from_uint8_to_user_dtype(data, user_dtype):
     if 'int' in user_dtype:
         return data.view(user_dtype)
     elif 'float16' == user_dtype:
         return data.view(np.uint16).view(user_dtype)
     elif 'float32' == user_dtype:
         return data.view(np.uint32).view(user_dtype)
```

### Comparing `pytpu-2.0.0/pytpu/tools/lenet5_processing.py` & `pytpu-2.0.1/pytpu_tests/unit/_lenet5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# FIXME: refactor according to wiki?
+
 import numpy as np
 from PIL import Image
 
 
 def get_img_sizes(input_data):
     sizes = []
     for inp in input_data:
@@ -44,15 +46,15 @@
 
     _, dim0, dim1, _ = None, 28, 28, 1
     input_hw_size = dim0, dim1
 
     result_array = preprocess_mnist(images, input_hw_size)
 
     result_dict = {}
-    input_tensor_names = ('input_input', )
+    input_tensor_names = ('input_input',)
 
     for input_tensor_name in input_tensor_names:
         result_dict[input_tensor_name] = result_array
 
     return result_dict, sizes
```

### Comparing `pytpu-2.0.0/pytpu/tools/resnet50_processing.py` & `pytpu-2.0.1/pytpu_tests/unit/_resnet50.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# FIXME: refactor according to wiki?
+
+from typing import Tuple, Any
+
 import numpy as np
 from PIL import Image
-from typing import Tuple, Any
 
 
 def get_img_sizes(input_data):
     sizes = []
     for inp in input_data:
         if len(inp) == 1:
             for image in inp:
@@ -64,15 +67,15 @@
     input_hw_size = dim0, dim1
 
     result_array = preprocess_imagenet(images, input_hw_size)
     result_array = _sub_mean_rgb(result_array)
 
     result_dict = {}
 
-    input_tensor_names = ('Placeholder', )
+    input_tensor_names = ('Placeholder',)
 
     for input_tensor_name in input_tensor_names:
         result_dict[input_tensor_name] = result_array
     return result_dict, sizes
 
 
 # Postprocessing
```

### Comparing `pytpu-2.0.0/pytpu.egg-info/PKG-INFO` & `pytpu-2.0.1/pytpu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 2.0.0
+Version: 2.0.1
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: IVA-Tech
 Author-email: info@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

