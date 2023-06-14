# Comparing `tmp/larq-0.9.5.tar.gz` & `tmp/larq-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/larq-0.9.5.tar", last modified: Mon May 11 09:48:55 2020, max compression
+gzip compressed data, was "dist/larq-0.9.6.tar", last modified: Mon May 18 16:32:58 2020, max compression
```

## Comparing `larq-0.9.5.tar` & `larq-0.9.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-11 09:48:55.000000 larq-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (116)     6161 2020-05-11 09:48:55.000000 larq-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4445 2020-05-11 09:48:45.000000 larq-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-11 09:48:55.000000 larq-0.9.5/larq/
--rw-r--r--   0 runner    (1001) docker     (116)      548 2020-05-11 09:48:45.000000 larq-0.9.5/larq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-11 09:48:45.000000 larq-0.9.5/larq/activations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1259 2020-05-11 09:48:45.000000 larq-0.9.5/larq/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     4404 2020-05-11 09:48:45.000000 larq-0.9.5/larq/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (116)     5659 2020-05-11 09:48:45.000000 larq-0.9.5/larq/callbacks_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2114 2020-05-11 09:48:45.000000 larq-0.9.5/larq/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)      716 2020-05-11 09:48:45.000000 larq-0.9.5/larq/conftest_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2020-05-11 09:48:45.000000 larq-0.9.5/larq/constraints.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2020-05-11 09:48:45.000000 larq-0.9.5/larq/constraints_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2953 2020-05-11 09:48:45.000000 larq-0.9.5/larq/context.py
--rw-r--r--   0 runner    (1001) docker     (116)      426 2020-05-11 09:48:45.000000 larq-0.9.5/larq/context_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    62865 2020-05-11 09:48:45.000000 larq-0.9.5/larq/layers.py
--rw-r--r--   0 runner    (1001) docker     (116)     8546 2020-05-11 09:48:45.000000 larq-0.9.5/larq/layers_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    11135 2020-05-11 09:48:45.000000 larq-0.9.5/larq/layers_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      885 2020-05-11 09:48:45.000000 larq-0.9.5/larq/math.py
--rw-r--r--   0 runner    (1001) docker     (116)     1299 2020-05-11 09:48:45.000000 larq-0.9.5/larq/math_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3401 2020-05-11 09:48:45.000000 larq-0.9.5/larq/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     2302 2020-05-11 09:48:45.000000 larq-0.9.5/larq/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    15887 2020-05-11 09:48:45.000000 larq-0.9.5/larq/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     5447 2020-05-11 09:48:45.000000 larq-0.9.5/larq/models_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    13701 2020-05-11 09:48:45.000000 larq-0.9.5/larq/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (116)     9961 2020-05-11 09:48:45.000000 larq-0.9.5/larq/optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    14205 2020-05-11 09:48:45.000000 larq-0.9.5/larq/quantized_variable.py
--rw-r--r--   0 runner    (1001) docker     (116)    11318 2020-05-11 09:48:45.000000 larq-0.9.5/larq/quantized_variable_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    18379 2020-05-11 09:48:45.000000 larq-0.9.5/larq/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (116)    15337 2020-05-11 09:48:45.000000 larq-0.9.5/larq/quantizers_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     7930 2020-05-11 09:48:45.000000 larq-0.9.5/larq/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1876 2020-05-11 09:48:45.000000 larq-0.9.5/larq/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2020-05-11 09:48:45.000000 larq-0.9.5/larq/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6161 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      749 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      362 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-05-11 09:48:55.000000 larq-0.9.5/larq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      399 2020-05-11 09:48:55.000000 larq-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2020-05-11 09:48:45.000000 larq-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:32:58.000000 larq-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (116)     6161 2020-05-18 16:32:58.000000 larq-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4445 2020-05-18 16:32:55.000000 larq-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:32:58.000000 larq-0.9.6/larq/
+-rw-r--r--   0 runner    (1001) docker     (116)      548 2020-05-18 16:32:55.000000 larq-0.9.6/larq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-18 16:32:55.000000 larq-0.9.6/larq/activations.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1259 2020-05-18 16:32:55.000000 larq-0.9.6/larq/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4404 2020-05-18 16:32:55.000000 larq-0.9.6/larq/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5659 2020-05-18 16:32:55.000000 larq-0.9.6/larq/callbacks_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2114 2020-05-18 16:32:55.000000 larq-0.9.6/larq/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      716 2020-05-18 16:32:55.000000 larq-0.9.6/larq/conftest_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1392 2020-05-18 16:32:55.000000 larq-0.9.6/larq/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2020-05-18 16:32:55.000000 larq-0.9.6/larq/constraints_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2953 2020-05-18 16:32:55.000000 larq-0.9.6/larq/context.py
+-rw-r--r--   0 runner    (1001) docker     (116)      426 2020-05-18 16:32:55.000000 larq-0.9.6/larq/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    62885 2020-05-18 16:32:55.000000 larq-0.9.6/larq/layers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8981 2020-05-18 16:32:55.000000 larq-0.9.6/larq/layers_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11293 2020-05-18 16:32:55.000000 larq-0.9.6/larq/layers_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      885 2020-05-18 16:32:55.000000 larq-0.9.6/larq/math.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1299 2020-05-18 16:32:55.000000 larq-0.9.6/larq/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3401 2020-05-18 16:32:55.000000 larq-0.9.6/larq/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2302 2020-05-18 16:32:55.000000 larq-0.9.6/larq/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15909 2020-05-18 16:32:55.000000 larq-0.9.6/larq/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5447 2020-05-18 16:32:55.000000 larq-0.9.6/larq/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13701 2020-05-18 16:32:55.000000 larq-0.9.6/larq/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9961 2020-05-18 16:32:55.000000 larq-0.9.6/larq/optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14205 2020-05-18 16:32:55.000000 larq-0.9.6/larq/quantized_variable.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11318 2020-05-18 16:32:55.000000 larq-0.9.6/larq/quantized_variable_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18379 2020-05-18 16:32:55.000000 larq-0.9.6/larq/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15337 2020-05-18 16:32:55.000000 larq-0.9.6/larq/quantizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7930 2020-05-18 16:32:55.000000 larq-0.9.6/larq/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1876 2020-05-18 16:32:55.000000 larq-0.9.6/larq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1140 2020-05-18 16:32:55.000000 larq-0.9.6/larq/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     6161 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      369 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2020-05-18 16:32:58.000000 larq-0.9.6/larq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      399 2020-05-18 16:32:58.000000 larq-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2062 2020-05-18 16:32:55.000000 larq-0.9.6/setup.py
```

### Comparing `larq-0.9.5/PKG-INFO` & `larq-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larq
-Version: 0.9.5
+Version: 0.9.6
 Summary: An Open Source Machine Learning Library for Training Binarized Neural Networks
 Home-page: https://larq.dev/
 Author: Plumerai
 Author-email: lukas@plumerai.co.uk
 License: Apache 2.0
 Description: <img src="https://user-images.githubusercontent.com/13285808/66865479-39c3b600-ef8f-11e9-9bd4-d47b8e432140.gif" alt="logo" height="100px" align="left"/>
         <br/>
```

### Comparing `larq-0.9.5/README.md` & `larq-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/__init__.py` & `larq-0.9.6/larq/__init__.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/activations.py` & `larq-0.9.6/larq/activations.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/activations_test.py` & `larq-0.9.6/larq/activations_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/callbacks.py` & `larq-0.9.6/larq/callbacks.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/callbacks_test.py` & `larq-0.9.6/larq/callbacks_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/conftest.py` & `larq-0.9.6/larq/conftest.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/conftest_test.py` & `larq-0.9.6/larq/conftest_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/constraints.py` & `larq-0.9.6/larq/constraints.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/constraints_test.py` & `larq-0.9.6/larq/constraints_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/context.py` & `larq-0.9.6/larq/context.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/layers.py` & `larq-0.9.6/larq/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1012,18 +1012,18 @@
         5D tensor with shape:
         `(batch, filters, new_depth, new_rows, new_cols)` if data_format='channels_first'
         or 5D tensor with shape:
         `(batch, new_depth, new_rows, new_cols, filters)` if data_format='channels_last'.
         `depth` and `rows` and `cols` values might have changed due to padding.
 
     # References
-    - [A guide to convolution arithmetic for deep
-      learning](https://arxiv.org/abs/1603.07285v1)
-    - [Deconvolutional
-      Networks](https://www.matthewzeiler.com/mattzeiler/deconvolutionalnetworks.pdf)
+        - [A guide to convolution arithmetic for deep
+            learning](https://arxiv.org/abs/1603.07285v1)
+        - [Deconvolutional
+            Networks](https://www.matthewzeiler.com/mattzeiler/deconvolutionalnetworks.pdf)
     """
 
     def __init__(
         self,
         filters,
         kernel_size,
         strides=(1, 1, 1),
```

### Comparing `larq-0.9.5/larq/layers_base.py` & `larq-0.9.6/larq/layers_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,28 @@
 from larq import context, quantizers, utils
 from larq.quantized_variable import QuantizedVariable
 from larq.quantizers import Quantizer
 
 log = logging.getLogger(__name__)
 
 
-def _compute_padding(stride, dilation_rate, input_size, filter_size):
+def _compute_padded_size(stride, dilation_rate, input_size, filter_size):
+    if input_size is None:
+        return None
     effective_filter_size = (filter_size - 1) * dilation_rate + 1
     output_size = (input_size + stride - 1) // stride
-    total_padding = (output_size - 1) * stride + effective_filter_size - input_size
-    total_padding = tf.math.maximum(total_padding, 0)
+    padded_size = (output_size - 1) * stride + effective_filter_size
+    if tf.is_tensor(input_size):
+        return tf.math.maximum(padded_size, input_size)
+    return max(padded_size, input_size)
+
+
+def _compute_padding(stride, dilation_rate, input_size, filter_size):
+    padded_size = _compute_padded_size(stride, dilation_rate, input_size, filter_size)
+    total_padding = padded_size - input_size
     padding = total_padding // 2
     return padding, padding + (total_padding % 2)
 
 
 class BaseLayer(tf.keras.layers.Layer):
     """Base class for defining quantized layers.
 
@@ -90,17 +99,15 @@
 
 class QuantizerBaseConv(tf.keras.layers.Layer):
     """Base class for defining quantized conv layers"""
 
     def __init__(self, *args, pad_values=0.0, **kwargs):
         self.pad_values = pad_values
         super().__init__(*args, **kwargs)
-
-    def _is_native_padding(self):
-        return self.padding != "same" or (
+        self._is_native_padding = self.padding != "same" or (
             not tf.is_tensor(self.pad_values) and self.pad_values == 0.0
         )
 
     def _get_spatial_padding_same(self, shape):
         return [
             _compute_padding(stride, dilation_rate, shape[i], filter_size)
             for i, (stride, dilation_rate, filter_size) in enumerate(
@@ -123,31 +130,34 @@
         return (
             [[0, 0], *padding, [0, 0]]
             if self.data_format == "channels_last"
             else [[0, 0], [0, 0], *padding]
         )
 
     def _get_padding_same_shape(self, input_shape):
+        spatial_input_shape = self._get_spatial_shape(input_shape)
         spatial_shape = [
-            (size + stride - 1) // stride if size is not None else None
-            for size, stride in zip(self._get_spatial_shape(input_shape), self.strides)
+            _compute_padded_size(stride, dilation, size, filter_size)
+            for size, stride, dilation, filter_size in zip(
+                spatial_input_shape, self.strides, self.dilation_rate, self.kernel_size,
+            )
         ]
         if self.data_format == "channels_last":
             return tf.TensorShape([input_shape[0], *spatial_shape, input_shape[-1]])
         return tf.TensorShape([*input_shape[:2], *spatial_shape])
 
     def build(self, input_shape):
-        if self._is_native_padding():
+        if self._is_native_padding:
             super().build(input_shape)
         else:
             with utils.patch_object(self, "padding", "valid"):
                 super().build(self._get_padding_same_shape(input_shape))
 
     def call(self, inputs):
-        if self._is_native_padding():
+        if self._is_native_padding:
             return super().call(inputs)
 
         inputs = tf.pad(
             inputs, self._get_padding_same(inputs), constant_values=self.pad_values
         )
         with utils.patch_object(self, "padding", "valid"):
             return super().call(inputs)
```

### Comparing `larq-0.9.5/larq/layers_test.py` & `larq-0.9.6/larq/layers_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,16 +199,19 @@
             rand_tuple = int(rand_tuple[0])
         kwargs = {"dilation_rate": rand_tuple} if dilation else {"strides": rand_tuple}
 
         args = (kernel,) if layer_cls == lq.layers.QuantDepthwiseConv2D else (2, kernel)
         ref_layer = layer_cls(*args, padding="same", **kwargs)
         spy = mocker.spy(tf, "pad")
         layer = layer_cls(*args, padding="same", pad_values=1.0, **kwargs)
+        layer.build(inputs.shape)
+        conv_op = getattr(layer, "_convolution_op", None)
         assert layer(inputs).shape == ref_layer(inputs).shape
         spy.assert_called_once_with(mocker.ANY, mocker.ANY, constant_values=1.0)
+        assert conv_op == getattr(layer, "_convolution_op", None)
 
     @pytest.mark.parametrize(
         "layer_cls",
         [
             lq.layers.QuantConv1D,
             lq.layers.QuantConv2D,
             lq.layers.QuantConv3D,
```

### Comparing `larq-0.9.5/larq/math.py` & `larq-0.9.6/larq/math.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/math_test.py` & `larq-0.9.6/larq/math_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/metrics.py` & `larq-0.9.6/larq/metrics.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/metrics_test.py` & `larq-0.9.6/larq/metrics_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/models.py` & `larq-0.9.6/larq/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,48 +258,48 @@
             row.append(n)
 
         return row
 
 
 class ModelProfile(LayerProfile):
     def __init__(self, model: tf.keras.models.Model):
-        self.layer_profiles = [LayerProfile(l) for l in model.layers]
+        self.layer_profiles = [LayerProfile(layer) for layer in model.layers]
 
     @property
     def memory(self) -> int:
-        return sum(l.memory for l in self.layer_profiles)
+        return sum(lp.memory for lp in self.layer_profiles)
 
     @property
     def int8_fp_weights_memory(self) -> int:
-        return sum(l.int8_fp_weights_memory for l in self.layer_profiles)
+        return sum(lp.int8_fp_weights_memory for lp in self.layer_profiles)
 
     @property
     def fp_equivalent_memory(self) -> int:
-        return sum(l.fp_equivalent_memory for l in self.layer_profiles)
+        return sum(lp.fp_equivalent_memory for lp in self.layer_profiles)
 
     def weight_count(
         self, bitwidth: Optional[int] = None, trainable: Optional[bool] = None
     ) -> int:
-        return sum(l.weight_count(bitwidth, trainable) for l in self.layer_profiles)
+        return sum(lp.weight_count(bitwidth, trainable) for lp in self.layer_profiles)
 
     def op_count(
         self, op_type: Optional[str] = None, bitwidth: Optional[int] = None
     ) -> int:
-        return sum(l.op_count(op_type, bitwidth) or 0 for l in self.layer_profiles)
+        return sum(lp.op_count(op_type, bitwidth) or 0 for lp in self.layer_profiles)
 
     @property
     def unique_param_bidtwidths(self) -> Sequence[int]:
         return sorted(
-            set(_flatten(l.unique_param_bidtwidths for l in self.layer_profiles))
+            set(_flatten(lp.unique_param_bidtwidths for lp in self.layer_profiles))
         )
 
     @property
     def unique_op_precisions(self) -> Sequence[int]:
         return sorted(
-            set(_flatten(l.unique_op_precisions for l in self.layer_profiles))
+            set(_flatten(lp.unique_op_precisions for lp in self.layer_profiles))
         )
 
     def _generate_table_header(self, table_config: Mapping[str, Any]) -> Sequence[str]:
         return [
             "Layer",
             "Input prec.\n(bit)",
             "Outputs",
```

### Comparing `larq-0.9.5/larq/models_test.py` & `larq-0.9.6/larq/models_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/optimizers.py` & `larq-0.9.6/larq/optimizers.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/optimizers_test.py` & `larq-0.9.6/larq/optimizers_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/quantized_variable.py` & `larq-0.9.6/larq/quantized_variable.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/quantized_variable_test.py` & `larq-0.9.6/larq/quantized_variable_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/quantizers.py` & `larq-0.9.6/larq/quantizers.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/quantizers_test.py` & `larq-0.9.6/larq/quantizers_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/testing_utils.py` & `larq-0.9.6/larq/testing_utils.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/utils.py` & `larq-0.9.6/larq/utils.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq/utils_test.py` & `larq-0.9.6/larq/utils_test.py`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/larq.egg-info/PKG-INFO` & `larq-0.9.6/larq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larq
-Version: 0.9.5
+Version: 0.9.6
 Summary: An Open Source Machine Learning Library for Training Binarized Neural Networks
 Home-page: https://larq.dev/
 Author: Plumerai
 Author-email: lukas@plumerai.co.uk
 License: Apache 2.0
 Description: <img src="https://user-images.githubusercontent.com/13285808/66865479-39c3b600-ef8f-11e9-9bd4-d47b8e432140.gif" alt="logo" height="100px" align="left"/>
         <br/>
```

### Comparing `larq-0.9.5/larq.egg-info/SOURCES.txt` & `larq-0.9.6/larq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `larq-0.9.5/setup.py` & `larq-0.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="larq",
-    version="0.9.5",
+    version="0.9.6",
     python_requires=">=3.6",
     author="Plumerai",
     author_email="lukas@plumerai.co.uk",
     description="An Open Source Machine Learning Library for Training Binarized Neural Networks",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://larq.dev/",
@@ -24,15 +24,15 @@
         "dataclasses ; python_version<'3.7'",
     ],
     extras_require={
         "tensorflow": ["tensorflow>=1.14.0"],
         "tensorflow_gpu": ["tensorflow-gpu>=1.14.0"],
         "test": [
             "black==19.10b0",
-            "flake8~=3.7.9",
+            "flake8>=3.7.9,<3.9.0",
             "isort~=4.3.21",
             "packaging>=19.2,<21.0",
             "pytest>=5.2.4,<5.5.0",
             "pytest-cov~=2.8.1",
             "pytest-xdist>=1.30,<1.33",
             "pytest-mock>=2.0,<3.2",
             "pytype>=2020.01.07,<2020.3.0",
```

