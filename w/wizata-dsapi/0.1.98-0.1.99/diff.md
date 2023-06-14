# Comparing `tmp/wizata-dsapi-0.1.98.tar.gz` & `tmp/wizata-dsapi-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.98.tar", last modified: Wed Jun 14 13:12:29 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.99.tar", last modified: Wed Jun 14 14:21:18 2023, max compression
```

## Comparing `wizata-dsapi-0.1.98.tar` & `wizata-dsapi-0.1.99.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.98/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.1.98/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-14 13:12:05.000000 wizata-dsapi-0.1.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.521946 wizata-dsapi-0.1.98/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.98/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.98/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.1.98/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.1.98/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.98/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14658 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.1.98/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-05 13:00:35.000000 wizata-dsapi-0.1.98/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.98/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    12259 2023-06-14 12:59:43.000000 wizata-dsapi-0.1.98/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.98/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     4961 2023-06-14 13:12:05.000000 wizata-dsapi-0.1.98/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-06 12:55:53.000000 wizata-dsapi-0.1.98/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.98/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    57684 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.98/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:12:29.553239 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-14 13:12:29.000000 wizata-dsapi-0.1.98/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 14:21:18.486241 wizata-dsapi-0.1.99/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.1.99/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-14 14:21:18.485233 wizata-dsapi-0.1.99/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.1.99/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-14 14:21:18.486241 wizata-dsapi-0.1.99/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-14 14:21:05.000000 wizata-dsapi-0.1.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:21:18.455482 wizata-dsapi-0.1.99/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.99/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.1.99/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-12 17:31:52.000000 wizata-dsapi-0.1.99/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-12 08:44:45.000000 wizata-dsapi-0.1.99/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.1.99/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.1.99/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14658 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.99/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.1.99/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-05 13:00:35.000000 wizata-dsapi-0.1.99/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-05 19:26:47.000000 wizata-dsapi-0.1.99/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    12259 2023-06-14 14:10:02.000000 wizata-dsapi-0.1.99/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.99/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.99/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.1.99/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     4961 2023-06-14 14:10:02.000000 wizata-dsapi-0.1.99/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-06 12:55:53.000000 wizata-dsapi-0.1.99/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-04-27 15:26:26.000000 wizata-dsapi-0.1.99/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.1.99/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    58180 2023-06-14 14:21:05.000000 wizata-dsapi-0.1.99/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:21:18.483724 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-14 14:21:18.000000 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-14 14:21:18.000000 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:21:18.000000 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-14 14:21:18.000000 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 14:21:18.000000 wizata-dsapi-0.1.99/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.98/LICENSE.txt` & `wizata-dsapi-0.1.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/setup.py` & `wizata-dsapi-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.98',
+    version='0.1.99',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.99/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.99/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.99/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.99/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.99/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.99/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.99/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.99/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.99/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.99/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.99/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.99/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/request.py` & `wizata-dsapi-0.1.99/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/script.py` & `wizata-dsapi-0.1.99/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/template.py` & `wizata-dsapi-0.1.99/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.99/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.99/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.99/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,16 @@
             if response.status_code == 200:
                 obj.model_id = uuid.UUID(response.json()['id'])
                 return obj.model_id
             else:
                 raise self.__raise_error(response)
         if isinstance(obj, Template):
             return self.upsert_template(obj.key, obj.name)
+        if isinstance(obj, Pipeline):
+            return self.upsert_pipeline(pipeline=obj)
         else:
             raise TypeError("Type not supported.")
 
     def delete(self, obj):
         """
         delete an object on the server
 
@@ -1084,14 +1086,27 @@
             found = False
 
         if not found:
             return self.create(template)
         else:
             return self.update(template)
 
+    def upsert_pipeline(self, pipeline: Pipeline):
+        """
+        Upsert a template (ignore ID, use the key)
+        :return: upserted template.
+        """
+
+        get = self.get(pipeline_key=pipeline.key)
+        if get is not None:
+            pipeline.pipeline_id = get.pipeline_id
+            return self.update(pipeline)
+        else:
+            return self.create(pipeline)
+
     def add_template_property(self, template, property_name: str, property_type: str = "datapoint"):
 
         if property_type not in ['datapoint', 'float', 'integer', 'string']:
             raise ValueError('property type must be datapoint, float, integer or string')
 
         if isinstance(template, str):
             template = self.get(template_key=template)
```

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.99/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.98/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.99/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

