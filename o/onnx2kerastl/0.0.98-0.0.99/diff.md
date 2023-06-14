# Comparing `tmp/onnx2kerastl-0.0.98.tar.gz` & `tmp/onnx2kerastl-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.98.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.99.tar", max compression
```

## Comparing `onnx2kerastl-0.0.98.tar` & `onnx2kerastl-0.0.99.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-05-24 12:10:46.678537 onnx2kerastl-0.0.98/LICENSE
--rw-r--r--   0        0        0       66 2022-05-29 07:44:17.204667 onnx2kerastl-0.0.98/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-25 09:04:27.467793 onnx2kerastl-0.0.98/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-08-04 13:51:21.421383 onnx2kerastl-0.0.98/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-03 15:38:22.085235 onnx2kerastl-0.0.98/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    14415 2023-06-12 12:28:45.565375 onnx2kerastl-0.0.98/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-21 12:48:52.329860 onnx2kerastl-0.0.98/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-21 12:48:52.330876 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-23 09:48:40.399903 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 13:34:03.376696 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-05-24 12:10:46.680353 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1585 2023-06-12 13:39:46.673928 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-19 17:39:21.485803 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 13:34:03.376950 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9380 2023-06-12 12:28:45.566760 onnx2kerastl-0.0.98/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-08-04 13:51:21.427113 onnx2kerastl-0.0.98/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3947 2023-06-12 12:28:45.567142 onnx2kerastl-0.0.98/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-01-19 11:41:57.593097 onnx2kerastl-0.0.98/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3664 2023-06-12 13:41:14.046234 onnx2kerastl-0.0.98/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 12:10:46.680940 onnx2kerastl-0.0.98/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-21 12:48:52.333310 onnx2kerastl-0.0.98/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    16027 2023-06-12 12:28:45.567939 onnx2kerastl-0.0.98/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-25 09:04:27.472631 onnx2kerastl-0.0.98/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-01-19 11:41:57.596399 onnx2kerastl-0.0.98/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    18236 2023-06-12 12:28:45.568511 onnx2kerastl-0.0.98/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5006 2023-06-12 12:28:45.569230 onnx2kerastl-0.0.98/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-01-19 11:41:57.597650 onnx2kerastl-0.0.98/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     5822 2023-06-12 12:28:45.570930 onnx2kerastl-0.0.98/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-06-12 13:41:59.160562 onnx2kerastl-0.0.98/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 12:10:46.678537 onnx2kerastl-0.0.99/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-29 07:44:17.204667 onnx2kerastl-0.0.99/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-25 09:04:27.467793 onnx2kerastl-0.0.99/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-08-04 13:51:21.421383 onnx2kerastl-0.0.99/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-03 15:38:22.085235 onnx2kerastl-0.0.99/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    14415 2023-06-12 12:28:45.565375 onnx2kerastl-0.0.99/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-21 12:48:52.329860 onnx2kerastl-0.0.99/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-21 12:48:52.330876 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-23 09:48:40.399903 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 13:34:03.376696 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-05-24 12:10:46.680353 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1585 2023-06-13 09:11:12.408022 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-19 17:39:21.485803 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 13:34:03.376950 onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9380 2023-06-12 12:28:45.566760 onnx2kerastl-0.0.99/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-08-04 13:51:21.427113 onnx2kerastl-0.0.99/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3947 2023-06-12 12:28:45.567142 onnx2kerastl-0.0.99/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-01-19 11:41:57.593097 onnx2kerastl-0.0.99/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3664 2023-06-13 09:12:10.289553 onnx2kerastl-0.0.99/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 12:10:46.680940 onnx2kerastl-0.0.99/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-21 12:48:52.333310 onnx2kerastl-0.0.99/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    16027 2023-06-12 12:28:45.567939 onnx2kerastl-0.0.99/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-25 09:04:27.472631 onnx2kerastl-0.0.99/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-01-19 11:41:57.596399 onnx2kerastl-0.0.99/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    18236 2023-06-12 12:28:45.568511 onnx2kerastl-0.0.99/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5006 2023-06-12 12:28:45.569230 onnx2kerastl-0.0.99/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-01-19 11:41:57.597650 onnx2kerastl-0.0.99/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     5822 2023-06-12 12:28:45.570930 onnx2kerastl-0.0.99/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-06-13 09:12:45.865847 onnx2kerastl-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.99/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.98/LICENSE` & `onnx2kerastl-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.99/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.99/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/ltsm_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
             raise UnsupportedLayer(f"LSTM with {direction} direction")
     should_return_state = len(node.output) == 3
     input_tensor = tf.transpose(ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name[0]), perm=[1, 0, 2])
     weights_w = ensure_numpy_type(layers[node.input[1]])[0]
     weights_r = ensure_numpy_type(layers[node.input[2]])[0]
     weights_b = ensure_numpy_type(layers[node.input[3]])[0]
 
-    initial_h_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[5]]), axis=1), input_tensor.dtype)
-    initial_c_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[6]]), axis=1), input_tensor.dtype)
+    initial_h_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[5]]), axis=0), input_tensor.dtype)
+    initial_c_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[6]]), axis=0), input_tensor.dtype)
 
     tf.keras.backend.set_image_data_format("channels_last")
     hidden_size = params['hidden_size']
     lstm_layer = OnnxLSTM(hidden_size, return_sequences=True, return_lstm_state=should_return_state)
     res = lstm_layer(input_tensor, initial_h_state, initial_c_state)
     # prepare the keras lstm weights from the onnx inputs:
     w1 = np.concatenate([weights_w[0:hidden_size, :], weights_w[2 * hidden_size:3 * hidden_size, :],
```

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.99/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.99/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.98/pyproject.toml` & `onnx2kerastl-0.0.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.98"
+version = "0.0.99"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.98/PKG-INFO` & `onnx2kerastl-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.98
+Version: 0.0.99
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

