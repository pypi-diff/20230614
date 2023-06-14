# Comparing `tmp/leap_model_parser-0.1.98.tar.gz` & `tmp/leap_model_parser-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.98.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.99.tar", max compression
```

## Comparing `leap_model_parser-0.1.98.tar` & `leap_model_parser-0.1.99.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1067 2022-03-21 10:18:19.706997 leap_model_parser-0.1.98/LICENSE
--rw-r--r--   0        0        0       68 2022-03-21 10:18:19.707319 leap_model_parser-0.1.98/README.md
--rw-r--r--   0        0        0      132 2022-06-01 08:37:39.139932 leap_model_parser-0.1.98/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-03-21 10:18:19.707654 leap_model_parser-0.1.98/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-03-13 09:16:28.638511 leap_model_parser-0.1.98/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43465 2023-05-17 13:33:35.411332 leap_model_parser-0.1.98/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   417479 2023-05-17 13:33:35.408945 leap_model_parser-0.1.98/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-05-14 16:30:42.392645 leap_model_parser-0.1.98/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-05-14 16:30:42.392981 leap_model_parser-0.1.98/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077038 leap_model_parser-0.1.98/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077489 leap_model_parser-0.1.98/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-05-26 12:03:02.078100 leap_model_parser-0.1.98/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-05-26 12:03:02.078264 leap_model_parser-0.1.98/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-05-14 16:30:36.727364 leap_model_parser-0.1.98/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-05-26 12:03:02.079257 leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-05-26 12:03:02.079831 leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     6775 2023-05-14 16:30:36.728911 leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-05-01 11:24:32.069577 leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1052 2023-05-17 13:34:32.959041 leap_model_parser-0.1.98/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-09 13:47:40.672102 leap_model_parser-0.1.99/LICENSE
+-rw-r--r--   0        0        0       68 2023-02-09 13:47:40.672339 leap_model_parser-0.1.99/README.md
+-rw-r--r--   0        0        0      132 2023-02-09 13:47:40.672539 leap_model_parser-0.1.99/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 13:47:40.672676 leap_model_parser-0.1.99/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0     1132 2023-05-22 11:32:57.336413 leap_model_parser-0.1.99/leap_model_parser/contract/graph.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:31:06.108645 leap_model_parser-0.1.99/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43326 2023-05-17 12:19:56.895805 leap_model_parser-0.1.99/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   416303 2023-05-17 12:19:56.897859 leap_model_parser-0.1.99/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15660 2023-05-22 11:32:57.342581 leap_model_parser-0.1.99/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6738 2023-05-22 11:32:57.342850 leap_model_parser-0.1.99/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2023-02-09 13:47:40.674784 leap_model_parser-0.1.99/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 13:47:40.674908 leap_model_parser-0.1.99/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2023-02-09 13:47:40.675042 leap_model_parser-0.1.99/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2023-02-09 13:47:40.675210 leap_model_parser-0.1.99/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-05-17 12:19:56.900019 leap_model_parser-0.1.99/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2023-02-09 13:47:40.675512 leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2023-02-09 13:47:40.675638 leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     6775 2023-05-17 12:19:56.900565 leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-05-17 12:19:56.900905 leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1052 2023-05-22 11:36:52.843742 leap_model_parser-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.99/PKG-INFO
```

### Comparing `leap_model_parser-0.1.98/LICENSE` & `leap_model_parser-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.99/leap_model_parser/contract/graph.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,65 @@
-from enum import Enum
 from typing import Dict, Any, List, Optional
 
 from dataclasses import dataclass, field
 
 
-class ImportModelTypeEnum(Enum):
-    JSON_TF2 = "JSON_TF2"
-    ONNX = "ONNX"
-    PB_TF2 = "PB_TF2"
-    H5_TF2 = "H5_TF2"
-
-
 @dataclass
 class WrapperData:
     type: str
     data: Dict
 
+
 @dataclass
 class InputInfo:
     name: str
     shape: List[int]
 
+
+@dataclass
+class InputData:
+    node: str
+    output: str
+
+
+@dataclass
+class OutputData:
+    node: str
+    input: str
+
+
 @dataclass
-class NodeResponse:
+class ConnectionInput:
+    connections: List[InputData]
+
+
+@dataclass
+class ConnectionOutput:
+    connections: List[OutputData]
+
+
+@dataclass
+class Node:
     id: str
     name: str
+    position: List[int]
     data: Dict[str, Any] = field(default_factory=dict)
-    inputs: Dict[str, Any] = field(default_factory=dict)
-    outputs: Dict[str, Any] = field(default_factory=dict)
-    position: List[int] = field(default_factory=lambda: [0, 0])
+    inputs: Dict[str, ConnectionInput] = field(default_factory=dict)
+    outputs: Dict[str, ConnectionOutput] = field(default_factory=dict)
+    pruning_plan_id: Optional[str] = None
     wrapper: Optional[WrapperData] = None
+
+    def __key(self):
+        return (self.id, self.name)
+
+    def __hash__(self):
+        return hash(self.__key())
+
+    @property
+    def type(self) -> Optional[str]:
+        return self.data.get('type')
+
+
+@dataclass
+class ModelGraph:
+    id: str
+    nodes: Dict[str, Node] = field(default_factory=dict)
```

### Comparing `leap_model_parser-0.1.98/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.99/leap_model_parser/contract/nodedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
-from typing import Union
 from typing import List
+from typing import Union
 from enum import Enum
 
 
 class ActivationsEnum(Enum):
     relu = "relu"
     softmax = "softmax"
     selu = "selu"
@@ -199,15 +199,14 @@
     Adamax = "Adamax"
     Ftrl = "Ftrl"
     Nadam = "Nadam"
     RMSprop = "RMSprop"
     SGD = "SGD"
     OnnxAbs = "OnnxAbs"
     OnnxErf = "OnnxErf"
-    OnnxGridSampler = "OnnxGridSampler"
     OnnxHardSigmoid = "OnnxHardSigmoid"
     OnnxLSTM = "OnnxLSTM"
     OnnxReduceMean = "OnnxReduceMean"
     OnnxSqrt = "OnnxSqrt"
     Dataset = "Dataset"
     Input = "Input"
     RepresentationBlock = "RepresentationBlock"
@@ -1799,20 +1798,14 @@
 
 @dataclass
 class OnnxErf:
     type: NodeType
 
 
 @dataclass
-class OnnxGridSampler:
-    sample_grid: List[int]
-    type: NodeType
-
-
-@dataclass
 class OnnxHardSigmoid:
     alpha: float
     beta: float
     type: NodeType
 
 
 @dataclass
@@ -1934,10 +1927,10 @@
                  SeparableConv1D, SeparableConv2D, SimpleRNN, SimpleRNNCell, Softmax, SpatialDropout1D, 
                  SpatialDropout2D, SpatialDropout3D, StringLookup, Subtract, SyncBatchNormalization, TextVectorization, 
                  ThresholdedReLU, TimeDistributed, UnitNormalization, UpSampling1D, UpSampling2D, UpSampling3D, 
                  ZeroPadding1D, ZeroPadding2D, ZeroPadding3D, BinaryCrossentropy, BinaryFocalCrossentropy, 
                  CategoricalCrossentropy, CategoricalHinge, CosineSimilarity, Hinge, Huber, KLDivergence, LogCosh, 
                  MeanAbsoluteError, MeanAbsolutePercentageError, MeanSquaredError, MeanSquaredLogarithmicError, Poisson, 
                  SquaredHinge, Adadelta, Adagrad, Adam, Adamax, Ftrl, Nadam, RMSprop, SGD, OnnxAbs, OnnxErf, 
-                 OnnxGridSampler, OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, 
-                 RepresentationBlock, GroundTruth, CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, 
-                 SlicingOpLambda, Repeat, Variable, Gather, FixedDropout]
+                 OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
+                 CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, SlicingOpLambda, Repeat, Variable, 
+                 Gather, FixedDropout]
```

### Comparing `leap_model_parser-0.1.98/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.99/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935064935064936%*

 * *Differences: {'delete': '[134]'}*

```diff
@@ -14524,61 +14524,14 @@
                 }
             ]
         },
         "menu_sections": [
             "Layer",
             "Onnx"
         ],
-        "name": "OnnxGridSampler",
-        "options": null,
-        "outputs_data": {
-            "outputs": [
-                {
-                    "name": "feature_map"
-                }
-            ]
-        },
-        "parents": [
-            "onnx2kerastl",
-            "customonnxlayer",
-            "onnxgridsampler"
-        ],
-        "properties": [
-            {
-                "default_val": null,
-                "isdefault": false,
-                "name": "sample_grid",
-                "type": "tuple"
-            }
-        ],
-        "receptive_fields_func": "IdentityReceptiveFieldsFunc",
-        "shape_calc": [
-            "IdentityFunc"
-        ],
-        "type": "Layer"
-    },
-    {
-        "inputs_data": {
-            "add_input_by_drag": false,
-            "inputs": [
-                {
-                    "approval_connection": [
-                        "Input",
-                        "Dataset",
-                        "Layer",
-                        "CustomLayer"
-                    ],
-                    "name": "input"
-                }
-            ]
-        },
-        "menu_sections": [
-            "Layer",
-            "Onnx"
-        ],
         "name": "OnnxHardSigmoid",
         "options": null,
         "outputs_data": {
             "outputs": [
                 {
                     "name": "feature_map"
                 }
```

### Comparing `leap_model_parser-0.1.98/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.99/leap_model_parser/keras_json_model_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 from pathlib import Path
 from typing import Set, Dict, Any, List, Type, Optional, Tuple
 import tensorflow as tf  # type: ignore
 from keras.engine.keras_tensor import KerasTensor  # type: ignore
 from tensorflow.python.keras.utils.generic_utils import func_load  # type: ignore
 
 from keras.engine.node import Node  # type: ignore
-from leap_model_parser.contract.importmodelresponse import InputInfo, NodeResponse, WrapperData
+from leap_model_parser.contract.graph import InputInfo, Node, WrapperData, ConnectionOutput, OutputData, \
+    ConnectionInput, InputData
 
 layer_attributes_adaptation = {'bias_initializer', 'kernel_initializer'}
 
 nojsonable_arg_serialization_prefix = '*tensorleap-nojsonable*'
 
 
 def deserialize_non_json_arg(arg: str):
     return eval(arg[len(nojsonable_arg_serialization_prefix):])
 
 
 class KerasJsonModelImport:
     def __init__(self, custom_layers: Optional[Dict[str, Type[tf.keras.layers.Layer]]] = None) -> None:
         self.id = 1
-        self.nodes_cache: Dict[str, NodeResponse] = defaultdict()
+        self.nodes_cache: Dict[str, Node] = defaultdict()
         self.layer_name_to_layer: Dict[str, Dict] = defaultdict()
         self.visited_connections: Set[str] = set()
         self.ui_components: Dict[str, Dict] = defaultdict()
         self.connected_inputs: List[InputInfo] = []
 
         if custom_layers is None:
             custom_layers = {}
@@ -46,15 +47,15 @@
 
     @staticmethod
     def is_representation_block(layer: Dict[str, Any]) -> bool:
         return len(layer['inbound_nodes']) > 1
 
     def generate_graph(
             self, model_schema: Dict, layer_name_to_inbound_nodes: Dict[str, List[Node]]) -> Tuple[
-        Dict[str, NodeResponse], List[InputInfo]]:
+        Dict[str, Node], List[InputInfo]]:
         self.prepare_model_to_import(model_schema)
         for graph_output_layer in model_schema['config']['output_layers']:
             current_layer = self.layer_name_to_layer[graph_output_layer[0]]
             self.generate_graph_recursive(
                 current_layer, graph_output_layer[1], layer_name_to_inbound_nodes)
 
         nodes = {node.id: node for node in self.nodes_cache.values()}
@@ -105,26 +106,25 @@
             input_layer, node_input_layer, 'outputs', input_index)
         node_input_key = self.get_connection_key(
             input_layer, node_output_layer, 'inputs', input_index)
         if node_output_key is None or node_input_key is None:
             return
 
         if node_output_key not in node_input_layer.outputs:
-            node_input_layer.outputs[node_output_key] = {'connections': []}
-        node_input_layer.outputs[node_output_key]['connections'].append({
-            "node": node_output_layer.id,
-            "input": node_input_key
-        })
+            node_input_layer.outputs[node_output_key] = ConnectionOutput(connections=[])
+        node_input_layer.outputs[node_output_key].connections.append(OutputData(node=node_output_layer.id,
+                                                                                input=node_input_key
+                                                                                ))
 
         if node_input_key not in node_output_layer.inputs:
-            node_output_layer.inputs[node_input_key] = {'connections': []}
-        node_output_layer.inputs[node_input_key]['connections'].append({
-            "node": node_input_layer.id,
-            "output": node_output_key
-        })
+            node_output_layer.inputs[node_input_key] = ConnectionInput(connections=[])
+        node_output_layer.inputs[node_input_key].connections.append(InputData(
+            node=node_input_layer.id,
+            output=node_output_key
+        ))
 
     def _get_layer_metadata(self, layer_json: Dict) -> Optional[Dict]:
         layer_metadata = self.ui_components.get(layer_json['class_name'])
         if layer_metadata is None:
             if layer_json['class_name'] in self.custom_layers:
                 layer_metadata = {
                     'type': 'CustomLayer',
@@ -201,16 +201,16 @@
             data['call_args'] = self._serialize_call_args(
                 call_args, call_kwargs)
         elif layer['class_name'] == "Lambda":
             lambda_func = func_load(layer['config']['function'])
             data['arg_names'] = list(lambda_func.__code__.co_varnames)
 
         self.layer_data_adjustments(data, layer_metadata)
-        node = NodeResponse(id=str(self.id), name=layer_metadata.get(
-            "class_name", layer["class_name"]), data=data)
+        node = Node(id=str(self.id), name=layer_metadata.get(
+            "class_name", layer["class_name"]), data=data, position=[0, 0])
         if 'wrapper' in layer:
             node.wrapper = layer['wrapper']
         self.nodes_cache[node_key] = node
 
     @classmethod
     def handle_wrapper_layer(cls, layer):
         wrapped_layer = layer['config']['layer']
@@ -242,34 +242,34 @@
                             f" please try to contact Tensorleap support")
 
     def generate_rp_node(self, layer: Dict[str, Any], layer_metadata: Dict[str, Any], node_key: str) -> None:
         if layer['name'] not in self.nodes_cache:
             data = layer['config']
             self.layer_data_adjustments(data, layer_metadata)
             data["output_blocks"] = []
-            node = NodeResponse(id=str(self.id),
-                                name=layer["class_name"], data=data)
+            node = Node(id=str(self.id),
+                        name=layer["class_name"], data=data, position=[0, 0])
             if 'wrapper' in layer:
                 node.wrapper = layer['wrapper']
             self.nodes_cache[layer['name']] = node
 
             self.id += 1
         data = {
             "output_name": "Action",
             "node_id": self.nodes_cache[layer["name"]].id,
             "parent_name": layer["class_name"]
         }
-        self.nodes_cache[node_key] = NodeResponse(
-            id=str(self.id), name='Representation Block', data=data)
+        self.nodes_cache[node_key] = Node(
+            id=str(self.id), name='Representation Block', data=data, position=[0, 0])
         self.nodes_cache[layer["name"]].data["output_blocks"].append({
             "block_node_id": self.nodes_cache[node_key].id,
             "output_name": "Action"
         })
 
-    def get_connection_key(self, node_input_layer, node: NodeResponse, direction: str, index: int) -> Optional[str]:
+    def get_connection_key(self, node_input_layer, node: Node, direction: str, index: int) -> Optional[str]:
         layer_metadata = self.ui_components.get(node.name)
         if _is_represntaion_block_node(node) or layer_metadata is None:
             if direction == 'inputs':
                 connection_format = f"{node.id}-input"
             else:
                 connection_format = f"{node.id}-feature_map"
         elif _is_input_node(node):
@@ -315,26 +315,26 @@
         shape = layer['config']['batch_input_shape']
         input_info = InputInfo(name=input_name, shape=shape[1:])
         self.connected_inputs.append(input_info)
         input_copy = {
             'type': 'Input',
             'output_name': input_name
         }
-        inputNode = NodeResponse(
-            id=str(self.id), name='Input', data=input_copy)
+        inputNode = Node(
+            id=str(self.id), name='Input', data=input_copy, position=[0, 0])
         self.nodes_cache[node_key] = inputNode
         self.id += 1
 
 
-def _add_origin_name_to_nodes(nodes: Dict[str, NodeResponse]):
+def _add_origin_name_to_nodes(nodes: Dict[str, Node]):
     for node in nodes.values():
         if "name" in node.data:
             node.data["origin_name"] = node.data["name"]
             node.data.pop("name")
 
 
-def _is_input_node(node: NodeResponse) -> bool:
+def _is_input_node(node: Node) -> bool:
     return node.name == 'Input'
 
 
-def _is_represntaion_block_node(node: NodeResponse) -> bool:
+def _is_represntaion_block_node(node: Node) -> bool:
     return node.name == 'Representation Block'
```

### Comparing `leap_model_parser-0.1.98/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.99/leap_model_parser/model_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from keras import Model  # type: ignore
 from keras_data_format_converter import convert_channels_first_to_last  # type: ignore
 from leap_model_rebuilder import rebuild_model  # type: ignore
 from onnx2kerastl import onnx_to_keras  # type: ignore
 from onnx2kerastl.exceptions import OnnxUnsupported  # type: ignore
 from tensorflow.keras.models import load_model  # type: ignore
 
-from leap_model_parser.contract.importmodelresponse import InputInfo, NodeResponse, ImportModelTypeEnum
+from leap_model_parser.contract.graph import Node, InputInfo
+from leap_model_parser.contract.importmodelresponse import ImportModelTypeEnum
 from leap_model_parser.keras_json_model_import import KerasJsonModelImport
 
 onnx_imported = False
 package_name = 'onnx'
 spec = find_spec(package_name)
 if spec is not None:
     import onnx  # type: ignore
@@ -39,16 +40,16 @@
             ImportModelTypeEnum.JSON_TF2.value: self.convert_json_model,
             ImportModelTypeEnum.H5_TF2.value: self.convert_h5_model,
             ImportModelTypeEnum.ONNX.value: self.convert_onnx_model,
             ImportModelTypeEnum.PB_TF2.value: self.convert_pb_model,
         }
 
     def get_keras_model_and_model_graph(
-            self, model_path: Path, model_type: ImportModelTypeEnum) -> Tuple[Dict[str, NodeResponse], List[InputInfo], Optional[Model]]:
-        model_to_keras_converter: Optional[Callable[[str], Tuple[Dict[str, NodeResponse], Model]]] = \
+            self, model_path: Path, model_type: ImportModelTypeEnum) -> Tuple[Dict[str, Node], List[InputInfo], Optional[Model]]:
+        model_to_keras_converter: Optional[Callable[[str], Tuple[Dict[str, Node], Model]]] = \
             self._model_types_converter.get(model_type.value)
         if model_to_keras_converter is None:
             raise Exception(
                 f"Unable to import external version, {str(model_path)} file format isn't supported")
 
         file_path = str(model_path)
         try:
@@ -99,30 +100,30 @@
 
             pb_file_path = next(iter(pb_files))
             pb_folder_path = next(iter(ntpath.split(pb_file_path)))
 
             k_model = self._load_keras_model_with_custom_layers(pb_folder_path)
         return k_model
 
-    def generate_model_graph(self, model_path: Path, model_type: ImportModelTypeEnum) -> Tuple[Dict[str, NodeResponse], List[InputInfo]]:
+    def generate_model_graph(self, model_path: Path, model_type: ImportModelTypeEnum) -> Tuple[Dict[str, Node], List[InputInfo]]:
         model_graph, connected_inputs, _ = self.get_keras_model_and_model_graph(
             model_path, model_type)
         return model_graph, connected_inputs
 
     @classmethod
-    def convert_json_model(cls, file_path: str) -> Tuple[Dict[str, NodeResponse], None]:
+    def convert_json_model(cls, file_path: str) -> Tuple[Dict[str, Node], None]:
         with open(file_path, 'r') as f:
             model_schema = json.load(f)
         return model_schema, None
 
-    def convert_pb_model(self, file_path: str) -> Tuple[Dict[str, NodeResponse], Model]:
+    def convert_pb_model(self, file_path: str) -> Tuple[Dict[str, Node], Model]:
         k_model = self._get_k_model_from_pb_path(file_path)
         return self.convert_to_keras_model(k_model)
 
-    def convert_onnx_model(self, file_path: str) -> Tuple[Dict[str, NodeResponse], Model]:
+    def convert_onnx_model(self, file_path: str) -> Tuple[Dict[str, Node], Model]:
         if not onnx_imported:
             raise OnnxUnsupported()
 
         onnx_model = onnx.load_model(file_path)
         input_all = [_input.name for _input in onnx_model.graph.input]
         input_initializer = [
             node.name for node in onnx_model.graph.initializer]
@@ -133,18 +134,18 @@
 
     def _load_keras_model_with_custom_layers(self, file_path: str):
         custom_objects = {}
         if self.custom_layers is not None:
             custom_objects = self.custom_layers
         return load_model(file_path, custom_objects=custom_objects, compile=False)
 
-    def convert_h5_model(self, file_path: str) -> Tuple[Dict[str, NodeResponse], Model]:
+    def convert_h5_model(self, file_path: str) -> Tuple[Dict[str, Node], Model]:
         imported_model = self._load_keras_model_with_custom_layers(file_path)
         return self.convert_to_keras_model(imported_model)
 
-    def convert_to_keras_model(self, k_model) -> Tuple[Dict[str, NodeResponse], Model]:
+    def convert_to_keras_model(self, k_model) -> Tuple[Dict[str, Node], Model]:
         converted_k_model = convert_channels_first_to_last(
             k_model, self._should_transform_inputs_and_outputs, self.custom_layers)
 
         model_schema = json.loads(converted_k_model.to_json())
 
         return model_schema, converted_k_model
```

### Comparing `leap_model_parser-0.1.98/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.99/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.99/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.99/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.98/pyproject.toml` & `leap_model_parser-0.1.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.98"
+version = "0.1.99"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.93"
+onnx2kerastl = "0.0.86"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.98/PKG-INFO` & `leap_model_parser-0.1.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.98
+Version: 0.1.99
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.93)
+Requires-Dist: onnx2kerastl (==0.0.86)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

