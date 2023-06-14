# Comparing `tmp/bisnet-1.0.0-py3-none-any.whl.zip` & `tmp/bisnet-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5790 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      283 b- defN 23-Jun-14 14:30 bisnet/__init__.py
--rw-rw-r--  2.0 unx    11124 b- defN 23-Jun-14 14:27 bisnet/model.py
+Zip file size: 5791 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      282 b- defN 23-Jun-14 15:48 bisnet/__init__.py
+-rw-rw-r--  2.0 unx    11124 b- defN 23-Jun-14 15:32 bisnet/model.py
 -rw-rw-r--  2.0 unx     3879 b- defN 23-Jun-14 14:26 bisnet/resnet.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-14 15:22 bisnet-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-14 15:22 bisnet-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 15:22 bisnet-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-14 15:22 bisnet-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      599 b- defN 23-Jun-14 15:22 bisnet-1.0.0.dist-info/RECORD
-8 files, 17982 bytes uncompressed, 4754 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-14 15:48 bisnet-1.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-14 15:48 bisnet-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 15:48 bisnet-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-14 15:48 bisnet-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      599 b- defN 23-Jun-14 15:48 bisnet-1.0.1.dist-info/RECORD
+8 files, 17981 bytes uncompressed, 4755 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: bisnet/model.py
 Comment: 
 
 Filename: bisnet/resnet.py
 Comment: 
 
-Filename: bisnet-1.0.0.dist-info/LICENSE
+Filename: bisnet-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: bisnet-1.0.0.dist-info/METADATA
+Filename: bisnet-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: bisnet-1.0.0.dist-info/WHEEL
+Filename: bisnet-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: bisnet-1.0.0.dist-info/top_level.txt
+Filename: bisnet-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bisnet-1.0.0.dist-info/RECORD
+Filename: bisnet-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bisnet/__init__.py

```diff
@@ -1,10 +1,11 @@
 #############################################################################
 #
 #   Source from:
 #   https://github.com/leonelhs/face-makeup.PyTorch
 #
 ##############################################################################
 
-from .resnet import Resnet18
+from .model import BiSeNet
+
+__version__ = "1.0.1"
 
-__version__ = "1.0.0"
```

## bisnet/model.py

```diff
@@ -7,16 +7,15 @@
 #
 ##############################################################################
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from bisnet import Resnet18
-
+from .resnet import Resnet18
 
 # from modules.bn import InPlaceABNSync as BatchNorm2d
 
 
 class ConvBNReLU(nn.Module):
     def __init__(self, in_chan, out_chan, ks=3, stride=1, padding=1, *args, **kwargs):
         super(ConvBNReLU, self).__init__()
```

## Comparing `bisnet-1.0.0.dist-info/LICENSE` & `bisnet-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bisnet-1.0.0.dist-info/METADATA` & `bisnet-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisnet
-Version: 1.0.0
+Version: 1.0.1
 Summary: Face parser model
 Home-page: https://github.com/leonelhs/bisnet
 Author: leonel hernandez
 Author-email: leonelhs@gmail.com
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

