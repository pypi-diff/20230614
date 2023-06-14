# Comparing `tmp/neptune_tensorboard-1.0.0rc1.tar.gz` & `tmp/neptune_tensorboard-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_tensorboard-1.0.0rc1.tar", max compression
+gzip compressed data, was "neptune_tensorboard-1.0.0rc2.tar", max compression
```

## Comparing `neptune_tensorboard-1.0.0rc1.tar` & `neptune_tensorboard-1.0.0rc2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      589 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/README.md
--rw-r--r--   0        0        0     2736 2023-06-13 10:38:12.895124 neptune_tensorboard-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      820 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/__init__.py
--rw-r--r--   0        0        0     3557 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/__init__.py
--rw-r--r--   0        0        0     5605 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/pytorch_integration.py
--rw-r--r--   0        0        0     3563 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/tensorflow_integration.py
--rw-r--r--   0        0        0      292 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/utils.py
--rw-r--r--   0        0        0      742 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/version.py
--rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      767 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     3420 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     2792 2023-06-14 08:02:10.005843 neptune_tensorboard-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      820 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/__init__.py
+-rw-r--r--   0        0        0     5605 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/pytorch_integration.py
+-rw-r--r--   0        0        0     5662 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorboardx_integration.py
+-rw-r--r--   0        0        0     3563 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorflow_integration.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/utils.py
+-rw-r--r--   0        0        0      742 2023-06-14 08:01:58.653968 neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/version.py
+-rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc2/PKG-INFO
```

### Comparing `neptune_tensorboard-1.0.0rc1/CHANGELOG.md` & `neptune_tensorboard-1.0.0rc2/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune-tensorboard 1.0.0.pre2
+
+### Changes
+- Update integration to work with tensorboardX's SummaryWriter ([#56](https://github.com/neptune-ai/neptune-tensorboard/pull/56))
+
 ## neptune-tensorboard 1.0.0.pre1
 
 ### Changes
 - Update integration to work with PyTorch's SummaryWriter ([#55](https://github.com/neptune-ai/neptune-tensorboard/pull/55))
 
 ## neptune-tensorboard 1.0.0.pre0
```

### Comparing `neptune_tensorboard-1.0.0rc1/LICENSE` & `neptune_tensorboard-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/README.md` & `neptune_tensorboard-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/pyproject.toml` & `neptune_tensorboard-1.0.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Python lack of functionalities from future versions
 importlib-metadata = { version = "*", python = "<3.8" }
 tensorflow = { version = ">=2.0.0", optional = true }
 torch = { version = ">=1.9.0", optional = true }
+tensorboardX = { version = ">=2.2.0", optional = true }
 
 # dev
 pre-commit = { version = "*", optional = true }
 pytest = { version = ">=5.0", optional = true }
 pytest-cov = { version = "2.10.1", optional = true }
 pytest-xdist = { version = "*", optional = true }
 pydot = { version = "*", optional = true }
@@ -40,15 +41,15 @@
 repository = "https://github.com/neptune-ai/neptune-tensorboard"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorboard"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-tensorboard"
 readme = "README.md"
-version = "1.0.0-pre.1"
+version = "1.0.0-pre.2"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/__init__.py` & `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/__init__.py` & `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 __all__ = ["enable_tensorboard_logging", "__version__"]
 
-import contextlib
 import warnings
+from contextlib import (
+    contextmanager,
+    nullcontext,
+)
 from importlib.util import find_spec
 
 from pkg_resources import parse_version
 
 from neptune_tensorboard.integration.version import __version__
 
 # NOTE: We don't use `importlib.find_spec` here as
@@ -30,14 +33,15 @@
 IS_TF_AVAILABLE = True
 try:
     import tensorflow as tf  # noqa
 except ModuleNotFoundError:
     IS_TF_AVAILABLE = False
 
 IS_PYT_AVAILABLE = find_spec("torch")
+IS_TENSORBOARDX_AVAILABLE = find_spec("tensorboardX")
 
 if IS_TF_AVAILABLE:
     MIN_TF_VERSION = "2.0.0-rc0"
     from neptune_tensorboard.integration.tensorflow_integration import (
         NeptuneTensorflowTracker,
         patch_tensorflow,
     )
@@ -47,16 +51,19 @@
         try:
             # noinspection PyUnresolvedReferences
             version = parse_version(tf.version.VERSION)
 
             if version >= parse_version(MIN_TF_VERSION):
                 return
         except AttributeError:
-            message = "Unrecognized tensorflow version: {}. Please make sure " "that the tensorflow version is >=2.0"
-            raise Exception(message.format(version))
+            message = (
+                f"Unrecognized tensorflow version: {version}. Please make sure "
+                "that the tensorflow version is >={MIN_TF_VERSION}"
+            )
+            raise Exception(message)
 
 
 if IS_PYT_AVAILABLE:
     MIN_PT_VERSION = "1.9.0"
     import torch
 
     from neptune_tensorboard.integration.pytorch_integration import (
@@ -69,45 +76,80 @@
         try:
             # noinspection PyUnresolvedReferences
             version = parse_version(torch.__version__)
 
             if version >= parse_version(MIN_PT_VERSION):
                 return
         except AttributeError:
-            message = "Unrecognized PyTorch version: {}. Please make sure " "that the PyTorch version is >=1.9.0"
-            raise Exception(message.format(version))
+            message = (
+                f"Unrecognized PyTorch version: {version}. Please make sure "
+                "that the PyTorch version is >={MIN_PT_VERSION}"
+            )
+            raise Exception(message)
+
+
+if IS_TENSORBOARDX_AVAILABLE:
+    import tensorboardX
+
+    MIN_TBX_VERSION = "2.2.0"
+    from neptune_tensorboard.integration.tensorboardx_integration import (
+        NeptuneTensorboardXTracker,
+        patch_tensorboardx,
+    )
+
+    def check_tensorboardx_version():
+        version = "<unknown>"
+        try:
+            # noinspection PyUnresolvedReferences
+            version = parse_version(tensorboardX.__version__)
+
+            if version >= parse_version(MIN_TBX_VERSION):
+                return
+        except AttributeError:
+            message = (
+                f"Unrecognized tensorboardX version: {version}. Please make sure "
+                "that the tensorboardX version is >={MIN_TBX_VERSION}"
+            )
+            raise Exception(message)
 
 
 FRAMEWORK_NOT_FOUND_WARNING_MSG = (
-    "neptune-tensorboard: Tensorflow or PyTorch was not found, ",
+    "neptune-tensorboard: Tensorflow or PyTorch or tensorboardX was not found, ",
     "please ensure that it is available.",
 )
 
 
 def enable_tensorboard_logging(run, *, base_namespace="tensorboard"):
     if IS_TF_AVAILABLE:
         check_tf_version()
         patch_tensorflow(run, base_namespace)
     if IS_PYT_AVAILABLE:
         check_pytorch_version()
         patch_pytorch(run, base_namespace)
+    if IS_TENSORBOARDX_AVAILABLE:
+        check_tensorboardx_version()
+        patch_tensorboardx(run, base_namespace)
 
-    if not (IS_PYT_AVAILABLE or IS_TF_AVAILABLE):
+    if not (IS_PYT_AVAILABLE or IS_TF_AVAILABLE or IS_TENSORBOARDX_AVAILABLE):
         warnings.warn(FRAMEWORK_NOT_FOUND_WARNING_MSG)
 
 
-@contextlib.contextmanager
+@contextmanager
 def enable_tensorboard_logging_ctx(run, *, base_namespace="tensorboard"):
-    tf_tracker, pt_tracker = contextlib.nullcontext(), contextlib.nullcontext()
+    tf_tracker, pt_tracker, tbx_tracker = nullcontext(), nullcontext(), nullcontext()
     if IS_TF_AVAILABLE:
         check_tf_version()
         tf_tracker = NeptuneTensorflowTracker(run, base_namespace)
 
     if IS_PYT_AVAILABLE:
         check_pytorch_version()
         pt_tracker = NeptunePytorchTracker(run, base_namespace)
 
-    if not (IS_PYT_AVAILABLE or IS_TF_AVAILABLE):
+    if IS_TENSORBOARDX_AVAILABLE:
+        check_tensorboardx_version()
+        tbx_tracker = NeptuneTensorboardXTracker(run, base_namespace)
+
+    if not (IS_PYT_AVAILABLE or IS_TF_AVAILABLE or IS_TENSORBOARDX_AVAILABLE):
         warnings.warn(FRAMEWORK_NOT_FOUND_WARNING_MSG)
 
-    with pt_tracker, tf_tracker:
+    with pt_tracker, tf_tracker, tbx_tracker:
         yield
```

### Comparing `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/pytorch_integration.py` & `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/pytorch_integration.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/tensorflow_integration.py` & `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/tensorflow_integration.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/version.py` & `neptune_tensorboard-1.0.0rc2/src/neptune_tensorboard/integration/version.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc1/PKG-INFO` & `neptune_tensorboard-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-tensorboard
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Neptune.ai Tensorboard integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -32,14 +32,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: neptune (>=1.0.1) ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydot ; extra == "dev"
 Requires-Dist: pytest (>=5.0) ; extra == "dev"
 Requires-Dist: pytest-cov (==2.10.1) ; extra == "dev"
 Requires-Dist: pytest-xdist
+Requires-Dist: tensorboardX (>=2.2.0)
 Requires-Dist: tensorflow (>=2.0.0)
 Requires-Dist: torch (>=1.9.0)
 Project-URL: Documentation, https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorboard
 Project-URL: Repository, https://github.com/neptune-ai/neptune-tensorboard
 Project-URL: Tracker, https://github.com/neptune-ai/neptune-tensorboard/issues
 Description-Content-Type: text/markdown
```

