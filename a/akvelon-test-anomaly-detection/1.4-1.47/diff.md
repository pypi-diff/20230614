# Comparing `tmp/akvelon-test-anomaly-detection-1.4.tar.gz` & `tmp/akvelon-test-anomaly-detection-1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akvelon-test-anomaly-detection-1.4.tar", last modified: Thu Mar 30 00:31:47 2023, max compression
+gzip compressed data, was "akvelon-test-anomaly-detection-1.47.tar", last modified: Wed Jun 14 16:49:01 2023, max compression
```

## Comparing `akvelon-test-anomaly-detection-1.4.tar` & `akvelon-test-anomaly-detection-1.47.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 00:31:47.483267 akvelon-test-anomaly-detection-1.4/
--rw-rw-rw-   0        0        0       75 2023-03-30 00:31:47.483267 akvelon-test-anomaly-detection-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-30 00:31:47.481260 akvelon-test-anomaly-detection-1.4/akvelon_test_anomaly_detection.egg-info/
--rw-rw-rw-   0        0        0       75 2023-03-30 00:31:47.000000 akvelon-test-anomaly-detection-1.4/akvelon_test_anomaly_detection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-03-30 00:31:47.000000 akvelon-test-anomaly-detection-1.4/akvelon_test_anomaly_detection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 00:31:47.000000 akvelon-test-anomaly-detection-1.4/akvelon_test_anomaly_detection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-30 00:31:47.000000 akvelon-test-anomaly-detection-1.4/akvelon_test_anomaly_detection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 00:31:47.482264 akvelon-test-anomaly-detection-1.4/anomaly_detection/
--rw-rw-rw-   0        0        0      884 2023-03-24 11:56:19.000000 akvelon-test-anomaly-detection-1.4/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0     5116 2023-03-30 00:24:44.000000 akvelon-test-anomaly-detection-1.4/anomaly_detection/anomaly_detection.py
--rw-rw-rw-   0        0        0       86 2023-03-02 11:12:35.000000 akvelon-test-anomaly-detection-1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 00:31:47.483267 akvelon-test-anomaly-detection-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-03-30 00:28:07.000000 akvelon-test-anomaly-detection-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 16:49:01.854574 akvelon-test-anomaly-detection-1.47/
+-rw-rw-rw-   0        0        0       76 2023-06-14 16:49:01.854574 akvelon-test-anomaly-detection-1.47/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 16:49:01.852058 akvelon-test-anomaly-detection-1.47/akvelon_test_anomaly_detection.egg-info/
+-rw-rw-rw-   0        0        0       76 2023-06-14 16:49:01.000000 akvelon-test-anomaly-detection-1.47/akvelon_test_anomaly_detection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-14 16:49:01.000000 akvelon-test-anomaly-detection-1.47/akvelon_test_anomaly_detection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 16:49:01.000000 akvelon-test-anomaly-detection-1.47/akvelon_test_anomaly_detection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-14 16:49:01.000000 akvelon-test-anomaly-detection-1.47/akvelon_test_anomaly_detection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 16:49:01.853574 akvelon-test-anomaly-detection-1.47/anomaly_detection/
+-rw-rw-rw-   0        0        0      884 2023-05-08 12:47:10.000000 akvelon-test-anomaly-detection-1.47/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0     5120 2023-05-08 17:57:52.000000 akvelon-test-anomaly-detection-1.47/anomaly_detection/anomaly_detection.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 16:49:01.854574 akvelon-test-anomaly-detection-1.47/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-14 16:48:52.000000 akvelon-test-anomaly-detection-1.47/setup.py
```

### Comparing `akvelon-test-anomaly-detection-1.4/anomaly_detection/__init__.py` & `akvelon-test-anomaly-detection-1.47/anomaly_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `akvelon-test-anomaly-detection-1.4/anomaly_detection/anomaly_detection.py` & `akvelon-test-anomaly-detection-1.47/anomaly_detection/anomaly_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 import sys
 import joblib
 import hdbscan
 from autoembedder import Autoembedder
 from apache_beam.io.filesystems import FileSystems
 from apache_beam.ml.inference.base import RunInference, PredictionResult, KeyedModelHandler
 from apache_beam.ml.inference.sklearn_inference import SklearnModelHandlerNumpy, ModelFileType
-from apache_beam.ml.inference.pytorch_inference import PytorchModelHandlerTensor, _convert_to_result
+from apache_beam.ml.inference.pytorch_inference import PytorchModelHandlerTensor
+from apache_beam.ml.inference.utils import _convert_to_result
 
 
 class CustomSklearnModelHandlerNumpy(SklearnModelHandlerNumpy):
     def run_inference(self, batch, model, inference_args=None):
         predictions = hdbscan.approximate_predict(model, batch)
         return [PredictionResult(x, y) for x, y in zip(batch[0], predictions[0])]
 
 
 class CustomPytorchModelHandlerTensor(PytorchModelHandlerTensor):
-
     def run_inference(self, batch, model, inference_args=None):
         with torch.no_grad():
             list_of_cont_tensors = []
             list_of_cat_tensors = []
             for item in batch:
                 list_of_cont_tensors.append(item['cont_cols'])
                 list_of_cat_tensors.append(item['cat_cols'])
@@ -70,15 +70,14 @@
         self.anomaly_detection_model_handler = CustomSklearnModelHandlerNumpy(model_uri=self._model_uri,
                                                                               model_file_type=ModelFileType.JOBLIB)
         self.encoder_handler = CustomPytorchModelHandlerTensor(state_dict_path=self._encoder_uri,
                                                                model_class=Autoembedder,
                                                                model_params={'config': self.params['params'],
                                                                              'num_cont_features': self.params['num_cont_features'],
                                                                              'embedding_sizes': self.params['list_cat']})
-        print(self.encoder_handler)
 
     def encode_and_normalize(self, bq_row, num_fields=None, id_field='Id'):
         if num_fields is None:
             num_fields = ['Amount']
 
         # This is mean and deviation calculated on a training data set
         # These parameters are unique for each set of data
```

### Comparing `akvelon-test-anomaly-detection-1.4/setup.py` & `akvelon-test-anomaly-detection-1.47/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 setuptools.setup(
     name='akvelon-test-anomaly-detection',
-    version='1.4',
+    version='1.47',
     install_requires=[],
     packages=setuptools.find_packages(),
 )
```

