# Comparing `tmp/gradio_client-0.2.6.tar.gz` & `tmp/gradio_client-0.2.7.tar.gz`

## Comparing `gradio_client-0.2.6.tar` & `gradio_client-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.6/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.6/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/__init__.py
--rw-r--r--   0        0        0    47504 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/media_data.py
--rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/types.json
--rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.6/gradio_client/version.txt
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 gradio_client-0.2.6/.gitignore
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 gradio_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 gradio_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.7/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.7/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/__init__.py
+-rw-r--r--   0        0        0    48042 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/client.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/types.json
+-rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/version.txt
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 gradio_client-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.7/PKG-INFO
```

### Comparing `gradio_client-0.2.6/README.md` & `gradio_client-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
 
 ## Installation
 
 If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
 
-Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
+Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.8 or higher:
 
 ```bash
 $ pip install gradio_client
 ```
 
 ## Basic Usage
```

### Comparing `gradio_client-0.2.6/gradio_client/client.py` & `gradio_client-0.2.7/gradio_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 """The main Client class for the Python client."""
 from __future__ import annotations
 
 import concurrent.futures
 import json
+import os
 import re
+import tempfile
 import threading
 import time
 import urllib.parse
 import uuid
 import warnings
 from concurrent.futures import Future, TimeoutError
 from datetime import datetime
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable
+from typing import Any, Callable, Literal
 
 import huggingface_hub
 import requests
 import websockets
 from huggingface_hub import SpaceStage
 from huggingface_hub.utils import (
     RepositoryNotFoundError,
     build_hf_headers,
     send_telemetry,
 )
 from packaging import version
-from typing_extensions import Literal
 
 from gradio_client import serializing, utils
 from gradio_client.documentation import document, set_documentation_group
 from gradio_client.serializing import Serializable
 from gradio_client.utils import (
     Communicator,
     JobStatus,
     Status,
     StatusUpdate,
 )
 
 set_documentation_group("py-client")
 
 
+DEFAULT_TEMP_DIR = os.environ.get("GRADIO_TEMP_DIR") or str(
+    Path(tempfile.gettempdir()) / "gradio"
+)
+
+
 @document("predict", "submit", "view_api", "duplicate")
 class Client:
     """
     The main Client class for the Python client. This class is used to connect to a remote Gradio app and call its API endpoints.
 
     Example:
         from gradio_client import Client
@@ -60,33 +66,36 @@
 
     def __init__(
         self,
         src: str,
         hf_token: str | None = None,
         max_workers: int = 40,
         serialize: bool = True,
+        output_dir: str | Path | None = DEFAULT_TEMP_DIR,
         verbose: bool = True,
     ):
         """
         Parameters:
             src: Either the name of the Hugging Face Space to load, (e.g. "abidlabs/whisper-large-v2") or the full URL (including "http" or "https") of the hosted Gradio app to load (e.g. "http://mydomain.com/app" or "https://bec81a83-5b5c-471e.gradio.live/").
             hf_token: The Hugging Face token to use to access private Spaces. Automatically fetched if you are logged in via the Hugging Face Hub CLI. Obtain from: https://huggingface.co/settings/token
             max_workers: The maximum number of thread workers that can be used to make requests to the remote Gradio app simultaneously.
             serialize: Whether the client should serialize the inputs and deserialize the outputs of the remote API. If set to False, the client will pass the inputs and outputs as-is, without serializing/deserializing them. E.g. you if you set this to False, you'd submit an image in base64 format instead of a filepath, and you'd get back an image in base64 format from the remote API instead of a filepath.
+            output_dir: The directory to save files that are downloaded from the remote API. If None, reads from the GRADIO_TEMP_DIR environment variable. Defaults to a temporary directory on your machine.
             verbose: Whether the client should print statements to the console.
         """
         self.verbose = verbose
         self.hf_token = hf_token
         self.serialize = serialize
         self.headers = build_hf_headers(
             token=hf_token,
             library_name="gradio_client",
             library_version=utils.__version__,
         )
         self.space_id = None
+        self.output_dir = output_dir
 
         if src.startswith("http://") or src.startswith("https://"):
             _src = src if src.endswith("/") else src + "/"
         else:
             _src = self._space_name_to_src(src)
             if _src is None:
                 raise ValueError(
@@ -792,15 +801,20 @@
 
     def deserialize(self, *data) -> tuple:
         assert len(data) == len(
             self.deserializers
         ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
         outputs = tuple(
             [
-                s.deserialize(d, hf_token=self.client.hf_token, root_url=self.root_url)
+                s.deserialize(
+                    d,
+                    save_dir=self.client.output_dir,
+                    hf_token=self.client.hf_token,
+                    root_url=self.root_url,
+                )
                 for s, d in zip(self.deserializers, data)
             ]
         )
         return outputs
 
     def process_predictions(self, *predictions):
         if self.client.serialize:
```

### Comparing `gradio_client-0.2.6/gradio_client/documentation.py` & `gradio_client-0.2.7/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.6/gradio_client/media_data.py` & `gradio_client-0.2.7/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.6/gradio_client/serializing.py` & `gradio_client-0.2.7/gradio_client/serializing.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.6/gradio_client/types.json` & `gradio_client-0.2.7/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.6/gradio_client/utils.py` & `gradio_client-0.2.7/gradio_client/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -379,35 +379,37 @@
 
 def decode_base64_to_file(
     encoding: str,
     file_path: str | None = None,
     dir: str | Path | None = None,
     prefix: str | None = None,
 ):
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
+    directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
+    directory.mkdir(exist_ok=True, parents=True)
     data, extension = decode_base64_to_binary(encoding)
     if file_path is not None and prefix is None:
         filename = Path(file_path).name
         prefix = filename
         if "." in filename:
             prefix = filename[0 : filename.index(".")]
             extension = filename[filename.index(".") + 1 :]
 
     if prefix is not None:
         prefix = strip_invalid_filename_characters(prefix)
 
     if extension is None:
-        file_obj = tempfile.NamedTemporaryFile(delete=False, prefix=prefix, dir=dir)
+        file_obj = tempfile.NamedTemporaryFile(
+            delete=False, prefix=prefix, dir=directory
+        )
     else:
         file_obj = tempfile.NamedTemporaryFile(
             delete=False,
             prefix=prefix,
             suffix="." + extension,
-            dir=dir,
+            dir=directory,
         )
     file_obj.write(data)
     file_obj.flush()
     return file_obj
 
 
 def dict_or_str_to_json_file(jsn: str | dict | list, dir: str | Path | None = None):
```

### Comparing `gradio_client-0.2.6/.gitignore` & `gradio_client-0.2.7/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 .idea/*
 .vscode/*
 .DS_Store
 *.bak
 workspace.code-workspace
 *.h5
 
+# dev containers
+.pnpm-store/
+
 # log files
 .pnpm-debug.log
 
 # Local virtualenv for devs
 .venv*
 
 # FRP
```

### Comparing `gradio_client-0.2.6/pyproject.toml` & `gradio_client-0.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_client"
 dynamic = ["version", "dependencies", "readme"]
 description = "Python library for easily interacting with trained machine learning models"
 license = "Apache-2.0"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   { name = "Abubakar Abid", email = "team@gradio.app" },
   { name = "Ali Abid", email = "team@gradio.app" },
   { name = "Ali Abdalla", email = "team@gradio.app" },
   { name = "Dawood Khan", email = "team@gradio.app" },
   { name = "Ahsen Khaliq", email = "team@gradio.app" },
   { name = "Pete Allen", email = "team@gradio.app" },
@@ -21,15 +21,14 @@
 
 classifiers = [
   'Development Status :: 4 - Beta',
   'License :: OSI Approved :: Apache Software License',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
-  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Topic :: Scientific/Engineering',
   'Topic :: Scientific/Engineering :: Artificial Intelligence',
   'Topic :: Software Development :: User Interfaces',
```

### Comparing `gradio_client-0.2.6/PKG-INFO` & `gradio_client-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: fsspec
 Requires-Dist: httpx
 Requires-Dist: huggingface-hub>=0.13.0
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: typing-extensions
 Requires-Dist: websockets
@@ -52,15 +51,15 @@
 
 The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
 
 ## Installation
 
 If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
 
-Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
+Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.8 or higher:
 
 ```bash
 $ pip install gradio_client
 ```
 
 ## Basic Usage
```

