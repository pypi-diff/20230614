# Comparing `tmp/apollo-lunar-2023.3.22rc2.tar.gz` & `tmp/apollo_lunar-2023.6.14rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-lunar-2023.3.22rc2.tar", max compression
+gzip compressed data, was "apollo_lunar-2023.6.14rc1.tar", max compression
```

## Comparing `apollo-lunar-2023.3.22rc2.tar` & `apollo_lunar-2023.6.14rc1.tar`

### file list

```diff
@@ -1,46 +1,44 @@
--rw-r--r--   0        0        0     1089 2023-03-22 06:15:07.107435 apollo-lunar-2023.3.22rc2/LICENSE
--rw-r--r--   0        0        0     4618 2023-03-22 06:15:07.107435 apollo-lunar-2023.3.22rc2/README.md
--rw-r--r--   0        0        0       56 2023-03-22 06:15:07.107435 apollo-lunar-2023.3.22rc2/bap/__init__.py
--rw-r--r--   0        0        0     6034 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/__init__.py
--rw-r--r--   0        0        0    12593 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/cli.py
--rw-r--r--   0        0        0     4288 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/config/__init__.py
--rw-r--r--   0        0        0      255 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/__init__.py
--rw-r--r--   0        0        0       58 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/batch/__init__.py
--rw-r--r--   0        0        0     1794 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/batch/batch.py
--rw-r--r--   0        0        0       99 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/batch/models/__init__.py
--rw-r--r--   0        0        0      421 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/batch/models/batch_models.py
--rw-r--r--   0        0        0       55 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/data/__init__.py
--rw-r--r--   0        0        0     8963 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/data/data.py
--rw-r--r--   0        0        0      103 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/__init__.py
--rw-r--r--   0        0        0     9741 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/dataset.py
--rw-r--r--   0        0        0      123 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/__init__.py
--rw-r--r--   0        0        0      856 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/dataset_models.py
--rw-r--r--   0        0        0      226 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/params/__init__.py
--rw-r--r--   0        0        0      175 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/params/docdb.py
--rw-r--r--   0        0        0      845 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/params/dynamodb.py
--rw-r--r--   0        0        0       67 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/dynamodb/__init__.py
--rw-r--r--   0        0        0     2853 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/dynamodb/dynamodb.py
--rw-r--r--   0        0        0       58 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/query/__init__.py
--rw-r--r--   0        0        0     3340 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/data/query/query.py
--rw-r--r--   0        0        0     2768 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/lunar_client.py
--rw-r--r--   0        0        0      224 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/ml/__init__.py
--rw-r--r--   0        0        0     5329 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/ml/aidp_service.py
--rw-r--r--   0        0        0     6821 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/ml/edd_service.py
--rw-r--r--   0        0        0      740 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/ml/lunar_model.py
--rw-r--r--   0        0        0     4075 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/ml/model_registry.py
--rw-r--r--   0        0        0      201 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/__init__.py
--rw-r--r--   0        0        0       64 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/channels/__init__.py
--rw-r--r--   0        0        0     7391 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/channels/channel.py
--rw-r--r--   0        0        0      123 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/channels/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/channels/models/channel_models.py
--rw-r--r--   0        0        0       74 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/experiments/__init__.py
--rw-r--r--   0        0        0     9615 2023-03-22 06:15:07.111435 apollo-lunar-2023.3.22rc2/lunar/rec/experiments/experiment.py
--rw-r--r--   0        0        0      144 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/experiments/models/__init__.py
--rw-r--r--   0        0        0     1768 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/experiments/models/experiment_models.py
--rw-r--r--   0        0        0       85 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/__init__.py
--rw-r--r--   0        0        0      124 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/models/__init__.py
--rw-r--r--   0        0        0      799 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/models/recommendation_models.py
--rw-r--r--   0        0        0     2432 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/recommendation.py
--rw-r--r--   0        0        0     1021 2023-03-22 06:15:07.115435 apollo-lunar-2023.3.22rc2/pyproject.toml
--rw-r--r--   0        0        0     6322 2023-03-22 06:15:18.591943 apollo-lunar-2023.3.22rc2/setup.py
--rw-r--r--   0        0        0     5495 2023-03-22 06:15:18.593182 apollo-lunar-2023.3.22rc2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-14 06:14:35.766079 apollo_lunar-2023.6.14rc1/LICENSE
+-rw-r--r--   0        0        0     4618 2023-06-14 06:14:35.766079 apollo_lunar-2023.6.14rc1/README.md
+-rw-r--r--   0        0        0       56 2023-06-14 06:14:35.766079 apollo_lunar-2023.6.14rc1/bap/__init__.py
+-rw-r--r--   0        0        0     6034 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/__init__.py
+-rw-r--r--   0        0        0    12593 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/cli.py
+-rw-r--r--   0        0        0     4288 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/config/__init__.py
+-rw-r--r--   0        0        0      255 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/batch/__init__.py
+-rw-r--r--   0        0        0     1794 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/batch/batch.py
+-rw-r--r--   0        0        0       99 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/batch/models/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/batch/models/batch_models.py
+-rw-r--r--   0        0        0       55 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/data/__init__.py
+-rw-r--r--   0        0        0     8963 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/data/data.py
+-rw-r--r--   0        0        0      103 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     8959 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/dataset.py
+-rw-r--r--   0        0        0      123 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/__init__.py
+-rw-r--r--   0        0        0      856 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/dataset_models.py
+-rw-r--r--   0        0        0      150 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/params/__init__.py
+-rw-r--r--   0        0        0      845 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/params/dynamodb.py
+-rw-r--r--   0        0        0       67 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/dynamodb/dynamodb.py
+-rw-r--r--   0        0        0       58 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/query/__init__.py
+-rw-r--r--   0        0        0     3340 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/data/query/query.py
+-rw-r--r--   0        0        0     2768 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/lunar_client.py
+-rw-r--r--   0        0        0      224 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/ml/__init__.py
+-rw-r--r--   0        0        0     5039 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/ml/aidp_service.py
+-rw-r--r--   0        0        0     6495 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/ml/edd_service.py
+-rw-r--r--   0        0        0      740 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/ml/lunar_model.py
+-rw-r--r--   0        0        0     4075 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/ml/model_registry.py
+-rw-r--r--   0        0        0      201 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/channels/__init__.py
+-rw-r--r--   0        0        0     7391 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/channels/channel.py
+-rw-r--r--   0        0        0      123 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/channels/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/channels/models/channel_models.py
+-rw-r--r--   0        0        0       74 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/experiments/__init__.py
+-rw-r--r--   0        0        0     9615 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/experiments/experiment.py
+-rw-r--r--   0        0        0      144 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/experiments/models/__init__.py
+-rw-r--r--   0        0        0     1768 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/experiments/models/experiment_models.py
+-rw-r--r--   0        0        0       85 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/models/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/models/recommendation_models.py
+-rw-r--r--   0        0        0     2432 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/recommendation.py
+-rw-r--r--   0        0        0     1021 2023-06-14 06:14:35.770079 apollo_lunar-2023.6.14rc1/pyproject.toml
+-rw-r--r--   0        0        0     5499 1970-01-01 00:00:00.000000 apollo_lunar-2023.6.14rc1/PKG-INFO
```

### Comparing `apollo-lunar-2023.3.22rc2/LICENSE` & `apollo_lunar-2023.6.14rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/README.md` & `apollo_lunar-2023.6.14rc1/README.md`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/__init__.py` & `apollo_lunar-2023.6.14rc1/lunar/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/cli.py` & `apollo_lunar-2023.6.14rc1/lunar/cli.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/config/__init__.py` & `apollo_lunar-2023.6.14rc1/lunar/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/batch/batch.py` & `apollo_lunar-2023.6.14rc1/lunar/data/batch/batch.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/data/data.py` & `apollo_lunar-2023.6.14rc1/lunar/data/data/data.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/datasets/dataset.py` & `apollo_lunar-2023.6.14rc1/lunar/data/datasets/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,23 +46,14 @@
         ```python
         # For dynamodb
         dataset = await client.create_dataset_async(
             id="my_dataset",
             data_type="dynamodb",
             params={"tables": ["first_table", "second_table"], "main_table": "first_table"},
         )
-
-        or
-
-        # For docdb
-        dataset = await client.create_dataset_async(
-            id="my_dataset",
-            data_type="docdb",
-            params={"collection": "my_collection"},
-        )
         ```
         """
         assert data_type in PARAMS, f"`data_type` is only available on {list(PARAMS)}"
         assert isinstance(params, dict), "`params` should be `dict` type"
 
         try:
             dataset = Dataset[PARAMS[data_type]](id=id, data_type=data_type, params=params)
@@ -90,21 +81,14 @@
         ```python
         # For dynamodb
         dataset = client.create_dataset(
             id="my_dataset",
             data_type="dynamodb",
             params={"tables": ["first_table", "second_table"], "main_table": "first_table"},
         )
-
-        # For docdb
-        dataset = client.create_dataset(
-            id="my_dataset",
-            data_type="docdb",
-            params={"collection": "my_collection"},
-        )
         ```
         """
 
         return loop.run_until_complete(self.create_dataset_async(id=id, data_type=data_type, params=params))
 
     async def list_datasets_async(self) -> List[Dataset]:
         """
@@ -199,21 +183,14 @@
         ```python
         # For dynamodb
         experiment = await client.update_dataset_async(
             id="my_dataset",
             data_type="dynamodb",
             params={"tables": ["first_table", "second_table", "third_table"], "main_table": "second_table"}
         )
-
-        # For docdb
-        experiment = await client.update_dataset_async(
-            id="my_dataset",
-            data_type="docdb",
-            params={"collections": "new_collections"}
-        )
         ```
         """
         assert data_type in PARAMS, f"`data_type` is only available on {list(PARAMS)}"
         assert isinstance(params, dict), "`params` should be `dict` type"
 
         try:
             updated_dataset = DatasetPutIn[PARAMS[data_type]](
@@ -244,21 +221,14 @@
         ```python
         # For dynamodb
         experiment = client.update_dataset(
             id="my_dataset",
             data_type="dynamodb",
             params={"tables": ["first_table", "second_table", "third_table"], "main_table": "second_table"}
         )
-
-        # For docdb
-        experiment = client.update_dataset(
-            id="my_dataset",
-            data_type="docdb",
-            params={"collections": "new_collections"}
-        )
         ```
         """
 
         return loop.run_until_complete(self.update_dataset_async(id=id, data_type=data_type, params=params))
 
     async def update_dataset_partial_async(self, id: str, data_type: str, params: Dict[str, Any] = None) -> Dataset:
         """
```

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/dataset_models.py` & `apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/datasets/models/params/dynamodb.py` & `apollo_lunar-2023.6.14rc1/lunar/data/datasets/models/params/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/dynamodb/dynamodb.py` & `apollo_lunar-2023.6.14rc1/lunar/data/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/data/query/query.py` & `apollo_lunar-2023.6.14rc1/lunar/data/query/query.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/lunar_client.py` & `apollo_lunar-2023.6.14rc1/lunar/lunar_client.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/ml/aidp_service.py` & `apollo_lunar-2023.6.14rc1/lunar/ml/aidp_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,17 @@
         """
         Copy a table from AIDP BigQuery to BAP S3 and Database.
 
         ## Args
 
         - database_name: (str) Database name of Bigquery
         - table_name: (str) Name of a table on Bigquery
-        - db_type: (str) Type of database to be loaded on BAP ('dynamodb' | 'docdb' | 'es' | 's3')
+        - db_type: (str) Type of database to be loaded on BAP ('dynamodb' | 'es' | 's3')
         - operation: (str) Type of operation ('put' (db_type 's3' is only available on 'put') | 'update' | 'upsert' (only for db_type 'dynamodb') | 'delete')
         - target_name: (optional) (str) Target name on database to be loaded (Default: Value of `table_name`)
-        - s3_dt: (optional) (str) Set a dt partition on BAP S3. If db_type is `docdb`, it is necessary
         - bq_table_partition: (optional) (str) Partition value of table on BigQuery
         - write_type: (optional) Write type ((default) 'json' | 'parquet')
         - max_num_files: (optional) (int) Maximum number of files to be saved on AWS S3 (default: 10)
 
         ## Returns
         dict
 
@@ -71,32 +70,29 @@
 
         spark = get_spark()
         # spark dataframe을 fs로 write 시 _SUCCESS 파일을 자동으로 생성하는 것을 방지
         spark.conf.set("mapreduce.fileoutputcommitter.marksuccessfuljobs", "false")
 
         assert db_type in [
             "dynamodb",
-            "docdb",
             "es",
             "s3",
-        ], "`db_type` must be one of `dynamodb` / `docdb` / `es` / `s3`"
+        ], "`db_type` must be one of `dynamodb` / `es` / `s3`"
         assert operation in [
             "put",
             "update",
             "upsert",
             "delete",
         ], "`operation` must be one of `put` / `update` / `upsert` / `delete`"
         assert write_type in ["json", "parquet"], "`write_type` must be one of `json`, `parquet`"
 
         if db_type != "dynamodb" and operation == "upsert":
             raise LunarError(code=400, msg="Operation 'upsert' is only available for db_type 'dynamodb'")
         if db_type == "s3" and operation != "put":
             raise LunarError(code=400, msg="db_type 's3' is only available on operation 'put'")
-        if db_type == "docdb" and not s3_dt:
-            raise LunarError(code=400, msg="Parameter 's3_dt' is necessary when db_type is 'docdb'")
 
         target_name = target_name if target_name else table_name
 
         job_name = f"{target_name}-{operation}"
         job_list = self.batch_client.get_batch_list(job_status_list=BATCH_JOB_CHECK_STATUS_LIST)
 
         if job_name in job_list:
```

### Comparing `apollo-lunar-2023.3.22rc2/lunar/ml/edd_service.py` & `apollo_lunar-2023.6.14rc1/lunar/ml/edd_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,65 +89,60 @@
         db_type: str,
         operation: str,
         target_name: str = None,
         s3_dt: str = None,
         edd_table_partition: str = None,
     ) -> Dict[str, Any]:
         """
-        Copy a table from EDD S3 to BAP S3 and Database(dynamodb or docdb).
+        Copy a table from EDD S3 to BAP S3 and Database(dynamodb).
 
         ## Args
 
         - database_name: (str) Database name of EDD S3 ('Datalake' is not available)
         - table_name: (str) Name of a table on EDD S3
-        - db_type: (str) Type of database to be loaded on BAP ('dynamodb' | 'docdb' | 'es' | 's3')
+        - db_type: (str) Type of database to be loaded on BAP ('dynamodb' | 'es' | 's3')
         - operation: (str) Type of operation ('put' (db_type 's3' is only available on 'put') | 'update' | 'upsert' (only for db_type 'dynamodb') | 'delete')
         - target_name: (optional) (str) Target name on database to be loaded (Default: Value of `table_name`)
-        - s3_dt: (optional) (str) Set a dt partition on BAP S3. If db_type is `docdb`, it is necessary
         - edd_table_partition: (optional) (str) Partition value of table on EDD S3
 
         ## Returns
         dict
 
         ## Example
 
         ```python
         response = copy_table_to_s3(
             database_name="apollo",
             table_name="test_table",
-            db_type="docdb",
+            db_type="dynamodb",
             operation="put",
             target_name="test_data",
-            s3_dt="20211101",
             edd_table_partition="dt=202109/type=put",
         )
 
 
         ```
         """
 
         assert db_type in [
             "dynamodb",
-            "docdb",
             "es",
             "s3",
-        ], "`db_type` must be one of `dynamodb` / `docdb` / `es` / `s3`"
+        ], "`db_type` must be one of `dynamodb` / `es` / `s3`"
         assert operation in [
             "put",
             "update",
             "upsert",
             "delete",
         ], "`operation` must be one of `put` / `update` / `upsert` / `delete`"
 
         if db_type != "dynamodb" and operation == "upsert":
             raise LunarError(code=400, msg="Operation 'upsert' is only available for db_type 'dynamodb'")
         if db_type == "s3" and operation != "put":
             raise LunarError(code=400, msg="db_type 's3' is only available on operation 'put'")
-        if db_type == "docdb" and not s3_dt:
-            raise LunarError(code=400, msg="Parameter 's3_dt' is necessary when db_type is 'docdb'")
 
         target_name = target_name if target_name else table_name
 
         job_name = f"{target_name}-{operation}"
         job_list = self.batch_client.get_batch_list(job_status_list=BATCH_JOB_CHECK_STATUS_LIST)
 
         if job_name in job_list:
```

### Comparing `apollo-lunar-2023.3.22rc2/lunar/ml/lunar_model.py` & `apollo_lunar-2023.6.14rc1/lunar/ml/lunar_model.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/ml/model_registry.py` & `apollo_lunar-2023.6.14rc1/lunar/ml/model_registry.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/rec/channels/channel.py` & `apollo_lunar-2023.6.14rc1/lunar/rec/channels/channel.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/rec/experiments/experiment.py` & `apollo_lunar-2023.6.14rc1/lunar/rec/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/rec/experiments/models/experiment_models.py` & `apollo_lunar-2023.6.14rc1/lunar/rec/experiments/models/experiment_models.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/models/recommendation_models.py` & `apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/models/recommendation_models.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/lunar/rec/recommendations/recommendation.py` & `apollo_lunar-2023.6.14rc1/lunar/rec/recommendations/recommendation.py`

 * *Files identical despite different names*

### Comparing `apollo-lunar-2023.3.22rc2/pyproject.toml` & `apollo_lunar-2023.6.14rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apollo-lunar"
-version = "2023.3.22rc2"
+version = "2023.6.14rc1"
 description = "A Python SDK/CLI for Lunar API"
 authors = ["Lunar module <lunar@sktio.io>"]
 readme = "README.md"
 license = "MIT"
 include = [
     "LICENSE",
 ]
```

### Comparing `apollo-lunar-2023.3.22rc2/PKG-INFO` & `apollo_lunar-2023.6.14rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: apollo-lunar
-Version: 2023.3.22rc2
+Version: 2023.6.14rc1
 Summary: A Python SDK/CLI for Lunar API
 License: MIT
 Author: Lunar module
 Author-email: lunar@sktio.io
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: ml
 Provides-Extra: skt
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: boto3
-Requires-Dist: catboost (>=1.0.6,<1.1.0); extra == "ml"
+Requires-Dist: catboost (>=1.0.6,<1.1.0) ; extra == "ml"
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: cloudpickle (>=2.1.0,<3.0.0)
-Requires-Dist: lightgbm (>=3.3.2,<3.4.0); extra == "ml"
+Requires-Dist: lightgbm (>=3.3.2,<3.4.0) ; extra == "ml"
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<1.2.0); extra == "ml"
-Requires-Dist: xgboost (>=1.6.1,<1.7.0); extra == "ml"
+Requires-Dist: scikit-learn (>=1.1.1,<1.2.0) ; extra == "ml"
+Requires-Dist: xgboost (>=1.6.1,<1.7.0) ; extra == "ml"
 Description-Content-Type: text/markdown
 
 # lunar-sdk
 
 ## Contents 
 - [Description](#description)
 - [Installation](#installation)
```

