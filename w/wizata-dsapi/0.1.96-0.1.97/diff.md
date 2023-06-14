# Comparing `tmp/wizata-dsapi-0.1.96.tar.gz` & `tmp/wizata-dsapi-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.96.tar", last modified: Tue Jun 13 15:13:14 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.97.tar", last modified: Tue Jun 13 18:13:34 2023, max compression
```

## Comparing `wizata-dsapi-0.1.96.tar` & `wizata-dsapi-0.1.97.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.449827 wizata-dsapi-0.1.96/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-13 15:13:14.449334 wizata-dsapi-0.1.96/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.96/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 15:13:14.450321 wizata-dsapi-0.1.96/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-13 15:13:09.000000 wizata-dsapi-0.1.96/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.429986 wizata-dsapi-0.1.96/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.96/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.96/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14658 2023-06-13 14:38:41.000000 wizata-dsapi-0.1.96/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.96/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.96/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56528 2023-06-13 15:13:09.000000 wizata-dsapi-0.1.96/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.447364 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.725855 wizata-dsapi-0.1.97/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-13 18:13:34.724367 wizata-dsapi-0.1.97/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.97/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:13:34.725855 wizata-dsapi-0.1.97/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-13 18:13:10.000000 wizata-dsapi-0.1.97/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.679728 wizata-dsapi-0.1.97/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-13 15:31:21.000000 wizata-dsapi-0.1.97/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.97/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14658 2023-06-13 15:31:21.000000 wizata-dsapi-0.1.97/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.97/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.97/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    57684 2023-06-13 18:13:10.000000 wizata-dsapi-0.1.97/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.721391 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.96/LICENSE.txt` & `wizata-dsapi-0.1.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/setup.py` & `wizata-dsapi-0.1.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.96',
+    version='0.1.97',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.97/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.97/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.97/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.97/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.97/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.97/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.97/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.97/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.97/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.97/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.97/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.97/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/request.py` & `wizata-dsapi-0.1.97/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/script.py` & `wizata-dsapi-0.1.97/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/template.py` & `wizata-dsapi-0.1.97/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.97/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.97/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.97/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -959,35 +959,65 @@
 
     def plot(self, plot_id: str = None, plot: Plot = None, figure=None,):
         """
         Fetch and show plot.
         :param plot: Wizata Plot Object
         :param figure: JSON Figure
         :param plot_id: Plot Id
-        :return:
+        :return: plotly figure
         """
         if plot is not None and plot.figure is not None:
             return plotly.io.from_json(plot.figure)
         elif plot is not None and plot.figure is None:
             plot = self.get(plot)
             if plot.figure is not None:
                 return plotly.io.from_json(plot.figure)
             else:
                 raise ValueError('No plot has been fetch.')
         elif figure is not None:
             return plotly.io.from_json(plot.figure)
-        elif id is not None:
+        elif plot_id is not None:
             plot = self.get(Plot(plot_id=plot_id))
             if plot.figure is not None:
                 return plotly.io.from_json(plot.figure)
             else:
                 raise ValueError('No plot has been fetch.')
         else:
             raise KeyError('No valid arguments.')
 
+    def plots(self, execution):
+        """
+        get all plot for an execution.
+        :param execution: id or Execution.
+        :return: list of plots.
+        """
+
+        if execution is None:
+            raise ValueError("execution cannot be None to retrieve plot")
+        if isinstance(execution, uuid.UUID):
+            execution_id = execution
+        elif isinstance(execution, str):
+            execution_id = uuid.UUID(execution)
+        elif isinstance(execution, Execution):
+            execution_id = execution.execution_id
+        else:
+            raise Exception(f'unsupported type {execution}')
+
+        response = requests.request("GET",
+                                    self.__url() + f"plots/?generatedById={execution_id}",
+                                    headers=self.__header()
+                                    )
+        if response.status_code == 200:
+            plots = []
+            for plot in response.json():
+                plots.append(self.plot(plot_id=str(plot["id"])))
+            return plots
+        else:
+            raise self.__raise_error(response)
+
     def register_model(self,
                        model_key,
                        train_model,
                        df: pandas.DataFrame,
                        scaler=None,
                        has_anomalies: bool = False,
                        has_target_feat: bool = False,
```

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.97/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.96/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.97/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

