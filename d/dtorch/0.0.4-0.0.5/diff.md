# Comparing `tmp/dtorch-0.0.4.tar.gz` & `tmp/dtorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtorch-0.0.4.tar", last modified: Mon Jun 12 12:10:01 2023, max compression
+gzip compressed data, was "dtorch-0.0.5.tar", last modified: Wed Jun 14 14:58:47 2023, max compression
```

## Comparing `dtorch-0.0.4.tar` & `dtorch-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.4/LICENSE
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-12 12:10:01.642850 dtorch-0.0.4/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2134 2023-06-07 09:47:40.000000 dtorch-0.0.4/README.md
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/dtorch/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      203 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/__init__.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.4/dtorch/dataset.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    16603 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/derivatives.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2096 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/einops.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17143 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/functionnal.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    12424 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/jtensors.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2679 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/loss.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    13038 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/nn.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-08 10:17:42.000000 dtorch-0.0.4/dtorch/operation_class.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.4/dtorch/operations.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     7914 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/optim.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1606 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/typing.py
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/dtorch.egg-info/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      377 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/SOURCES.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/dependency_links.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        7 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/top_level.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      616 2023-06-12 11:58:25.000000 dtorch-0.0.4/pyproject.toml
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-12 12:10:01.642850 dtorch-0.0.4/setup.cfg
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.5/LICENSE
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-14 14:58:47.026172 dtorch-0.0.5/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2134 2023-06-07 09:47:40.000000 dtorch-0.0.5/README.md
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorch/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      225 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/__init__.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.5/dtorch/dataset.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17758 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/derivatives.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2096 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/einops.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17143 2023-06-13 17:43:40.000000 dtorch-0.0.5/dtorch/functionnal.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    12424 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/jtensors.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2679 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/loss.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    16153 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/nn.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-08 10:17:42.000000 dtorch-0.0.5/dtorch/operation_class.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.5/dtorch/operations.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     7914 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/optim.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1606 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/typing.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorch.egg-info/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      498 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       15 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/requires.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       31 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/top_level.txt
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorchtext/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchtext/datasets.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchtext/models.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorchvision/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     4690 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchvision/datasets.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2994 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchvision/models.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      689 2023-06-14 14:57:56.000000 dtorch-0.0.5/pyproject.toml
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-14 14:58:47.026172 dtorch-0.0.5/setup.cfg
```

### Comparing `dtorch-0.0.4/LICENSE` & `dtorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/PKG-INFO` & `dtorch-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dtorch-0.0.4/README.md` & `dtorch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/dataset.py` & `dtorch-0.0.5/dtorch/dataset.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/derivatives.py` & `dtorch-0.0.5/dtorch/derivatives.py`

 * *Files 6% similar despite different names*

```diff
@@ -308,42 +308,64 @@
             if (tensors[i].isLeaf()):
                 tensors[i].grad += dtorch.jtensors.JTensors(base_tensor()[i])
             else:
                 tensors[i].grad = dtorch.jtensors.JTensors(base_tensor()[i])
             tensors[i].backward(tensors[i].grad, forced=True)
 
 
+# def add_deriv(base_tensor, *tensors):
+
+#     unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
+#     is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
+#     left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape)))
+#     right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape)))
+
+#     if (unpacked_tensors[0].require_grads):
+#         grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape, unpacked_tensors[0].shape)).reshape(*unpacked_tensors[0].shape)
+#                                                                 if left_size < right_size
+#                                                                 else base_tensor.numpy().reshape(*unpacked_tensors[0].shape))
+#         if (unpacked_tensors[0].isLeaf()):
+#             unpacked_tensors[0].grad += grad
+#         else:
+#             unpacked_tensors[0].grad = grad
+#         unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
+
+#     if (is_tensor and unpacked_tensors[1].require_grads):
+#         grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape)
+#                                                                if right_size < left_size
+#                                                                else base_tensor.numpy().reshape(*unpacked_tensors[1].shape))
+#         if (unpacked_tensors[1].isLeaf()):
+#             unpacked_tensors[1].grad += grad
+#         else:
+#             unpacked_tensors[1].grad = grad
+#         unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
 def add_deriv(base_tensor, *tensors):
 
     unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
     is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
-    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape)))
-    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape)))
-
+    
     if (unpacked_tensors[0].require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape, unpacked_tensors[0].shape)).reshape(*unpacked_tensors[0].shape)
-                                                                if left_size < right_size
-                                                                else base_tensor.numpy().reshape(*unpacked_tensors[0].shape))
+        axis = dimensionToSum(base_tensor().shape, unpacked_tensors[0].shape)
+        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=axis).reshape(*unpacked_tensors[0].shape))
         if (unpacked_tensors[0].isLeaf()):
             unpacked_tensors[0].grad += grad
         else:
             unpacked_tensors[0].grad = grad
         unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
 
     if (is_tensor and unpacked_tensors[1].require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape)
-                                                               if right_size < left_size
-                                                               else base_tensor.numpy().reshape(*unpacked_tensors[1].shape))
+        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape))
         if (unpacked_tensors[1].isLeaf()):
             unpacked_tensors[1].grad += grad
         else:
             unpacked_tensors[1].grad = grad
         unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
 
 
+
 def div_deriv(base_tensor, *tensors):
 
     unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
 
     zis_tensor : bool = isinstance(unpacked_tensors[0], dtorch.jtensors.JTensors)
     is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
```

### Comparing `dtorch-0.0.4/dtorch/einops.py` & `dtorch-0.0.5/dtorch/einops.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/functionnal.py` & `dtorch-0.0.5/dtorch/functionnal.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/jtensors.py` & `dtorch-0.0.5/dtorch/jtensors.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/loss.py` & `dtorch-0.0.5/dtorch/loss.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/operations.py` & `dtorch-0.0.5/dtorch/operations.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/optim.py` & `dtorch-0.0.5/dtorch/optim.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch/typing.py` & `dtorch-0.0.5/dtorch/typing.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.4/dtorch.egg-info/PKG-INFO` & `dtorch-0.0.5/dtorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

