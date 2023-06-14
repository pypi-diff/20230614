# Comparing `tmp/wizata-dsapi-0.1.97.tar.gz` & `tmp/wizata-dsapi-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.97.tar", last modified: Tue Jun 13 18:13:34 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.98.tar", last modified: Wed Jun 14 13:12:29 2023, max compression
```

## Comparing `wizata-dsapi-0.1.97.tar` & `wizata-dsapi-0.1.98.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.725855 wizata-dsapi-0.1.97/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-13 18:13:34.724367 wizata-dsapi-0.1.97/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.97/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 18:13:34.725855 wizata-dsapi-0.1.97/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-13 18:13:10.000000 wizata-dsapi-0.1.97/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.679728 wizata-dsapi-0.1.97/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-13 15:31:21.000000 wizata-dsapi-0.1.97/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.97/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14658 2023-06-13 15:31:21.000000 wizata-dsapi-0.1.97/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.97/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.97/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.97/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.97/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    57684 2023-06-13 18:13:10.000000 wizata-dsapi-0.1.97/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:13:34.721391 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 18:13:34.000000 wizata-dsapi-0.1.97/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.98/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.1.98/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-14 13:12:05.000000 wizata-dsapi-0.1.98/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.521946 wizata-dsapi-0.1.98/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.98/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.98/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.1.98/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.1.98/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.98/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14658 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.1.98/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-05 13:00:35.000000 wizata-dsapi-0.1.98/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.98/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    12259 2023-06-14 12:59:43.000000 wizata-dsapi-0.1.98/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.98/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     4961 2023-06-14 13:12:05.000000 wizata-dsapi-0.1.98/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-06 12:55:53.000000 wizata-dsapi-0.1.98/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.98/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    57684 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.97/LICENSE.txt` & `wizata-dsapi-0.1.98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/setup.py` & `wizata-dsapi-0.1.98/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.97',
+    version='0.1.98',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.98/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.98/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.98/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.98/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.98/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.98/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.98/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.98/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.98/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.98/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.98/wizata_dsapi/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -165,14 +165,18 @@
         if pipeline_id is None:
             pipeline_id = uuid.uuid4()
         self.pipeline_id = pipeline_id
         self.key = key
         self.variables = variables
         self.template_id = template_id
         self.experiment_id = experiment_id
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
         self.plots = plots
         if plots is None:
             self.plots = []
         if steps is not None:
             for step in steps:
                 if not isinstance(step, PipelineStep):
                     raise TypeError(f'step expected PipelineStep but received {step.__class__.__name__}')
@@ -277,14 +281,22 @@
                 step.from_json(obj_step)
                 self.steps.append(step)
         if "plots" in obj.keys():
             if isinstance(obj["plots"], str):
                 self.plots = json.loads(obj["plots"])
             else:
                 self.plots = obj["plots"]
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
 
     def to_json(self):
         """
         Convert to a json version of Execution definition.
         By default, use DS API format.
         """
         obj = {
@@ -302,12 +314,20 @@
             obj["plots"] = json.dumps(self.plots)
         if self.variables is not None:
             obj["variables"] = json.dumps(self.variables)
         if self.template_id is not None:
             obj["templateId"] = str(self.template_id)
         if self.experiment_id is not None:
             obj["experimentKey"] = str(self.experiment_id)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
         return obj
```

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.98/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/request.py` & `wizata-dsapi-0.1.98/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/script.py` & `wizata-dsapi-0.1.98/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/template.py` & `wizata-dsapi-0.1.98/wizata_dsapi/template.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         if template_id is None:
             self.template_id = uuid.uuid4()
         else:
             self.template_id = template_id
         self.key = key
         self.name = name
         self.properties = properties
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
 
     def api_id(self) -> str:
         """
         Id of the Template (template_id)
 
         :return: string formatted UUID of the template.
         """
@@ -55,14 +59,22 @@
             if isinstance(obj["properties"], str):
                 properties = json.loads(obj["properties"])
             else:
                 properties = obj["properties"]
             # add properties to add method to ensure unicity of name and validity of type
             for to_add in properties:
                 self.add_property(to_add)
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
 
     def to_json(self):
         """
         Convert the template to a dictionary compatible to JSON format.
 
         :return: dictionary representation of the Template object.
         """
@@ -71,14 +83,22 @@
         }
         if self.key is not None:
             obj["key"] = str(self.key)
         if self.name is not None:
             obj["name"] = str(self.name)
         if self.properties is not None:
             obj["properties"] = json.dumps(self.properties)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
         return obj
 
     def add_property(self, property_value):
         """
         add a property in list of properties
         :param property_value: property { type , name }
         """
```

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.98/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.98/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.98/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.98/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.97/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.98/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

