# Comparing `tmp/flytekitplugins-bigquery-1.6.2b1.tar.gz` & `tmp/flytekitplugins-bigquery-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.6.2b1.tar", last modified: Thu Jun  8 23:49:40 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.7.0.tar", last modified: Wed Jun 14 04:33:26 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.6.2b1.tar` & `flytekitplugins-bigquery-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-08 23:49:15.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 23:49:40.000000 flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:49:40.623215 flytekitplugins-bigquery-1.6.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-08 23:49:38.000000 flytekitplugins-bigquery-1.6.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.381290 flytekitplugins-bigquery-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-14 04:33:05.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:33:26.377290 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:33:26.000000 flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:33:26.381290 flytekitplugins-bigquery-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 04:33:24.000000 flytekitplugins-bigquery-1.7.0/setup.py
```

### Comparing `flytekitplugins-bigquery-1.6.2b1/PKG-INFO` & `flytekitplugins-bigquery-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.2b1/README.md` & `flytekitplugins-bigquery-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/agent.py` & `flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.2b1/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.7.0/flytekitplugins/bigquery/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from google.cloud import bigquery
 from google.protobuf import json_format
 from google.protobuf.struct_pb2 import Struct
 
 from flytekit.configuration import SerializationSettings
 from flytekit.extend import SQLTask
+from flytekit.extend.backend.base_agent import AsyncAgentExecutorMixin
 from flytekit.models import task as _task_model
 from flytekit.types.structured import StructuredDataset
 
 
 @dataclass
 class BigQueryConfig(object):
     """
@@ -18,15 +19,15 @@
     """
 
     ProjectID: str
     Location: Optional[str] = None
     QueryJobConfig: Optional[bigquery.QueryJobConfig] = None
 
 
-class BigQueryTask(SQLTask[BigQueryConfig]):
+class BigQueryTask(AsyncAgentExecutorMixin, SQLTask[BigQueryConfig]):
     """
     This is the simplest form of a BigQuery Task, that can be used even for tasks that do not produce any output.
     """
 
     # This task is executed using the BigQuery handler in the backend.
     # https://github.com/flyteorg/flyteplugins/blob/43623826fb189fa64dc4cb53e7025b517d911f22/go/tasks/plugins/webapi/bigquery/plugin.go#L34
     _TASK_TYPE = "bigquery_query_job_task"
@@ -40,16 +41,15 @@
         output_structured_dataset_type: Optional[Type[StructuredDataset]] = None,
         **kwargs,
     ):
         """
         To be used to query BigQuery Tables.
 
         :param name: Name of this task, should be unique in the project
-        :param query_template: The actual query to run. We use Flyte's Golang templating format for Query templating.
-          Refer to the templating documentation
+        :param query_template: The actual query to run. We use Flyte's Golang templating format for Query templating. Refer to the templating documentation
         :param task_config: BigQueryConfig object
         :param inputs: Name and type of inputs specified as an ordered dictionary
         :param output_structured_dataset_type: If some data is produced by this query, then you can specify the output StructuredDataset type
         :param kwargs: All other args required by Parent type - SQLTask
         """
         outputs = None
         if output_structured_dataset_type is not None:
@@ -77,10 +77,7 @@
         s = Struct()
         s.update(config)
         return json_format.MessageToDict(s)
 
     def get_sql(self, settings: SerializationSettings) -> Optional[_task_model.Sql]:
         sql = _task_model.Sql(statement=self.query_template, dialect=_task_model.Sql.Dialect.ANSI)
         return sql
-
-    def execute(self, **kwargs) -> Any:
-        raise Exception("Cannot run a SQL Task natively, please mock.")
```

### Comparing `flytekitplugins-bigquery-1.6.2b1/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.7.0/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.2b1
+Version: 1.7.0
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.2b1/setup.py` & `flytekitplugins-bigquery-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.6.2b1"
+__version__ = "1.7.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

