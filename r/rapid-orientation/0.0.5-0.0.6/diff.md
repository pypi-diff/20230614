# Comparing `tmp/rapid_orientation-0.0.5-py3-none-any.whl.zip` & `tmp/rapid_orientation-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6289346 bytes, number of entries: 10
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-19 02:02 rapid_orientation/__init__.py
--rw-r--r--  2.0 unx      350 b- defN 23-Apr-19 02:02 rapid_orientation/config.yaml
--rw-r--r--  2.0 unx     2644 b- defN 23-Apr-19 02:02 rapid_orientation/rapid_orientation.py
--rw-r--r--  2.0 unx     5730 b- defN 23-Apr-19 02:02 rapid_orientation/utils.py
+Zip file size: 6289942 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-14 14:37 rapid_orientation/__init__.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-14 14:37 rapid_orientation/config.yaml
+-rw-r--r--  2.0 unx     2804 b- defN 23-Jun-14 14:37 rapid_orientation/rapid_orientation.py
+-rw-r--r--  2.0 unx     7735 b- defN 23-Jun-14 14:37 rapid_orientation/utils.py
 -rw-rw-r--  2.0 unx  6792721 b- defN 23-Jan-20 13:53 rapid_orientation/models/rapid_orientation.onnx
--rw-r--r--  2.0 unx     2725 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      898 b- defN 23-Apr-19 02:02 rapid_orientation-0.0.5.dist-info/RECORD
-10 files, 6805379 bytes uncompressed, 6287790 bytes compressed:  7.6%
+-rw-r--r--  2.0 unx     2759 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-14 14:38 rapid_orientation-0.0.6.dist-info/RECORD
+10 files, 6807578 bytes uncompressed, 6288386 bytes compressed:  7.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_orientation/utils.py
 Comment: 
 
 Filename: rapid_orientation/models/rapid_orientation.onnx
 Comment: 
 
-Filename: rapid_orientation-0.0.5.dist-info/METADATA
+Filename: rapid_orientation-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_orientation-0.0.5.dist-info/WHEEL
+Filename: rapid_orientation-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_orientation-0.0.5.dist-info/entry_points.txt
+Filename: rapid_orientation-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.5.dist-info/top_level.txt
+Filename: rapid_orientation-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_orientation-0.0.5.dist-info/RECORD
+Filename: rapid_orientation-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_orientation/rapid_orientation.py

```diff
@@ -13,20 +13,21 @@
 # limitations under the License.
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 import time
 from pathlib import Path
-import cv2
+from typing import Union
 
+import cv2
 import numpy as np
 import yaml
 
-from .utils import OrtInferSession, create_operators
+from .utils import LoadImage, OrtInferSession, create_operators
 
 root_dir = Path(__file__).resolve().parent
 
 
 class RapidOrientation():
     def __init__(self, model_path: str = None):
         config_path = str(root_dir / 'config.yaml')
@@ -36,15 +37,19 @@
         config['model_path'] = model_path
 
         self.session = OrtInferSession(config)
         self.labels = self.session.get_metadata()['character'].splitlines()
 
         self.preprocess_ops = create_operators(config["PreProcess"])
 
-    def __call__(self, images):
+        self.load_img = LoadImage()
+
+    def __call__(self, img_content: Union[str, np.ndarray, bytes, Path]):
+        images = self.load_img(img_content)
+
         s = time.time()
         for ops in self.preprocess_ops:
             images = ops(images)
         image = np.array(images)[None, ...]
 
         pred_output = self.session(image)[0]
```

## rapid_orientation/utils.py

```diff
@@ -1,18 +1,23 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import importlib
-from pathlib import Path
 import warnings
+from io import BytesIO
+from pathlib import Path
+from typing import Union
 
 import cv2
 import numpy as np
 from onnxruntime import (GraphOptimizationLevel, InferenceSession,
                          SessionOptions, get_available_providers, get_device)
+from PIL import Image, UnidentifiedImageError
+
+InputType = Union[str, np.ndarray, bytes, Path]
 
 
 class OrtInferSession():
     def __init__(self, config):
         sess_opt = SessionOptions()
         sess_opt.log_severity_level = 4
         sess_opt.enable_cpu_mem_arena = False
@@ -70,14 +75,78 @@
             raise FileExistsError(f'{model_path} is not a file.')
 
 
 class ONNXRuntimeError(Exception):
     pass
 
 
+class LoadImage():
+    def __init__(self, ):
+        pass
+
+    def __call__(self, img: InputType) -> np.ndarray:
+        if not isinstance(img, InputType.__args__):
+            raise LoadImageError(
+                f'The img type {type(img)} does not in {InputType.__args__}')
+
+        img = self.load_img(img)
+
+        if img.ndim == 2:
+            return cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+
+        if img.ndim == 3 and img.shape[2] == 4:
+            return self.cvt_four_to_three(img)
+
+        return img
+
+    def load_img(self, img: InputType) -> np.ndarray:
+        if isinstance(img, (str, Path)):
+            self.verify_exist(img)
+            try:
+                img = np.array(Image.open(img))
+                img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+            except UnidentifiedImageError as e:
+                raise LoadImageError(
+                    f'cannot identify image file {img}') from e
+            return img
+
+        if isinstance(img, bytes):
+            img = np.array(Image.open(BytesIO(img)))
+            img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+            return img
+
+        if isinstance(img, np.ndarray):
+            return img
+
+        raise LoadImageError(f'{type(img)} is not supported!')
+
+    @staticmethod
+    def cvt_four_to_three(img: np.ndarray) -> np.ndarray:
+        '''RGBA → RGB
+        '''
+        r, g, b, a = cv2.split(img)
+        new_img = cv2.merge((b, g, r))
+
+        not_a = cv2.bitwise_not(a)
+        not_a = cv2.cvtColor(not_a, cv2.COLOR_GRAY2BGR)
+
+        new_img = cv2.bitwise_and(new_img, new_img, mask=a)
+        new_img = cv2.add(new_img, not_a)
+        return new_img
+
+    @staticmethod
+    def verify_exist(file_path: Union[str, Path]):
+        if not Path(file_path).exists():
+            raise LoadImageError(f'{file_path} does not exist.')
+
+
+class LoadImageError(Exception):
+    pass
+
+
 def create_operators(params):
     """
     create operators based on the config
 
     Args:
         params(list): a dict list, used to create some operators
     """
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `rapid_orientation-0.0.5.dist-info/METADATA` & `rapid_orientation-0.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-orientation
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools for classifying the direction of images containing text based ONNXRuntime.
 Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,layout,rapidocr,rapid_orientation
 Platform: Any
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6,<=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: onnxruntime (>=1.7.0)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: opencv-python (>=4.5.1.48)
 Requires-Dist: numpy (>=1.21.6)
+Requires-Dist: Pillow
 
 ## rapid-orientation
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-orientation/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-orientation"></a>
     <a href="https://pepy.tech/project/rapid-orientation"><img src="https://static.pepy.tech/personalized-badge/rapid-orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
@@ -35,21 +36,20 @@
 
 ### 2. Run by script.
 - RapidOrientation has the default `model_path` value, you can set the different value of `model_path` to use different models, e.g. `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')`
 - See details, for [README_Layout](https://github.com/RapidAI/RapidStructure/blob/main/docs/README_Orientation.md) .
 - 📌 `layout.png` source: [link](https://github.com/RapidAI/RapidStructure/blob/main/test_images/layout.png)
 
 ```python
-import cv2
 from rapid_orientation import RapidOrientation
 
 orientation_engine = RapidOrientation()
 
-img = cv2.imread('test_images/layout.png')
-
+with open('test_images/layout.png', 'rb') as f:
+    img = f.read()
 orientation_res, elapse = orientation_engine(img)
 print(orientation_res)
 ```
 
 ### 3. Run by command line.
 - Usage:
     ```bash
```

### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.5 Summary: Tools for
+Metadata-Version: 2.1 Name: rapid-orientation Version: 0.0.6 Summary: Tools for
 classifying the direction of images containing text based ONNXRuntime. Home-
 page: https://github.com/RapidAI/RapidStructure Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Keywords:
 ppstructure,layout,rapidocr,rapid_orientation Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.6,<=3.10 Description-Content-Type: text/
 markdown Requires-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0)
-Requires-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) ##
-rapid-orientation
+Requires-Dist: opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6)
+Requires-Dist: Pillow ## rapid-orientation
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/rapid-
 orientation?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### 1. Install package by pypi. ```bash $ pip install rapid-orientation ``` ###
 2. Run by script. - RapidOrientation has the default `model_path` value, you
 can set the different value of `model_path` to use different models, e.g.
 `orientation_engine = RapidOrientation(model_path='rapid_orientation.onnx')` -
 See details, for [README_Layout](https://github.com/RapidAI/RapidStructure/
 blob/main/docs/README_Orientation.md) . - ð `layout.png` source: [link]
 (https://github.com/RapidAI/RapidStructure/blob/main/test_images/layout.png)
-```python import cv2 from rapid_orientation import RapidOrientation
-orientation_engine = RapidOrientation() img = cv2.imread('test_images/
-layout.png') orientation_res, elapse = orientation_engine(img) print
-(orientation_res) ``` ### 3. Run by command line. - Usage: ```bash $
-rapid_orientation -h usage: rapid_orientation [-h] -img IMG_PATH [-
-m MODEL_PATH] optional arguments: -h, --help show this help message and exit -
-img IMG_PATH, --img_path IMG_PATH Path to image for layout. -m MODEL_PATH, --
-model_path MODEL_PATH The model path used for inference ``` - Example: ```bash
-$ rapid_orientation -img layout.png ``` ### 4. Result. ```python # Return str,
-four types:ï¼0 | 90 | 180 | 270 ```
+```python from rapid_orientation import RapidOrientation orientation_engine =
+RapidOrientation() with open('test_images/layout.png', 'rb') as f: img = f.read
+() orientation_res, elapse = orientation_engine(img) print(orientation_res) ```
+### 3. Run by command line. - Usage: ```bash $ rapid_orientation -h usage:
+rapid_orientation [-h] -img IMG_PATH [-m MODEL_PATH] optional arguments: -h, --
+help show this help message and exit -img IMG_PATH, --img_path IMG_PATH Path to
+image for layout. -m MODEL_PATH, --model_path MODEL_PATH The model path used
+for inference ``` - Example: ```bash $ rapid_orientation -img layout.png ```
+### 4. Result. ```python # Return str, four types:ï¼0 | 90 | 180 | 270 ```
```

