# Comparing `tmp/awsdf-0.1.8.tar.gz` & `tmp/awsdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsdf-0.1.8.tar", max compression
+gzip compressed data, was "awsdf-0.1.9.tar", max compression
```

## Comparing `awsdf-0.1.8.tar` & `awsdf-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1754 2022-12-14 07:00:57.989017 awsdf-0.1.8/awsdf.rst
--rw-r--r--   0        0        0      573 2022-12-14 07:15:06.962886 awsdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       29 2022-12-04 01:32:00.013300 awsdf-0.1.8/src/awsdf/__init__.py
--rw-r--r--   0        0        0    25194 2022-12-04 05:54:34.983467 awsdf-0.1.8/src/awsdf/aws.py
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 awsdf-0.1.8/setup.py
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 awsdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1944 2022-12-16 04:52:25.062872 awsdf-0.1.9/awsdf.rst
+-rw-r--r--   0        0        0      573 2022-12-16 04:53:10.513535 awsdf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       29 2022-12-04 01:32:00.013300 awsdf-0.1.9/src/awsdf/__init__.py
+-rw-r--r--   0        0        0    26304 2022-12-15 08:14:13.936999 awsdf-0.1.9/src/awsdf/aws.py
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 awsdf-0.1.9/setup.py
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 awsdf-0.1.9/PKG-INFO
```

### Comparing `awsdf-0.1.8/pyproject.toml` & `awsdf-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsdf"
-version = "0.1.8"
+version = "0.1.9"
 description = "AWS metadata as dataframes"
 authors = ["Allan <allan.dsouza@gmail.com>"]
 readme = "awsdf.rst"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<3.11"
 awswrangler = "^2.14.0"
```

### Comparing `awsdf-0.1.8/src/awsdf/aws.py` & `awsdf-0.1.9/src/awsdf/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-"""Main module."""
+"""
+This module enables connecting to AWS and extracting metadata in pandas dataframes.
+
+**Installing from PyPI:** *pip install -U awsdf*
+
+**USAGE:**
+
+    import awsdf
+
+    aws_account = awsdf.Account(profile_name="<PROFILE_NAME>")
+
+    glue_databases_df = aws_account.glue_get_databases()
+
+"""
 from datetime import timedelta, datetime
 from awswrangler import exceptions
 import boto3
 import botocore
 import botocore.exceptions
 from loguru import logger
 import numpy as np
@@ -35,28 +48,40 @@
     return obj[key] if key in obj else None
 
 
 error_df = pd.DataFrame(columns=["Error"], data=[[-1]])
 
 
 class Account(object):
+    """
+    Instantiate class object for connecting to AWS and retriving metadata from AWS
+    """
+
     def __init__(
         self,
         aws_access_key_id=None,
         aws_secret_access_key=None,
         aws_session_token=None,
         region_name=None,
         profile_name=None,
     ):
         """
         Provide access keys OR Profile name to connect to AWS account. Keys take preceedence
-        Parameters:
-            aws_access_key_id (string) -- AWS access key ID
-            aws_secret_access_key (string) -- AWS secret access key
-            aws_session_token (string) -- AWS temporary session token
+
+        **Parameters:**
+
+            *aws_access_key_id (string) -- AWS access key ID*
+
+            *aws_secret_access_key (string) -- AWS secret access key*
+
+            *aws_session_token (string) -- AWS temporary session token*
+
+            *region_name (string) -- AWS region*
+
+            *profile_name (string) -- AWS profile name*
         """
         try:
             self._session = boto3.Session(
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 region_name=region_name,
@@ -99,15 +124,21 @@
             logger.error(error)
             exit(0)
         except botocore.exceptions.BotoCoreError as error:
             print("Exception while getting accountid.")
             logger.error(error)
             exit(0)
 
-    def glue_get_jobs(self):
+    def glue_get_jobs(self) -> pd.DataFrame:
+        """
+        Get AWS Glue jobs
+
+        Returns:
+            dataframe
+        """
         glue_job_df_columns = ["Name", "CreatedOn", "LastModifiedOn"]
 
         # initialize Glue client
         client = self.session.client(AWS_GLUE_CLIENT)
         paginator = client.get_paginator("get_jobs")
 
         page_iterator = paginator.paginate()
@@ -120,15 +151,28 @@
         jobs_df = pd.DataFrame(data, columns=glue_job_df_columns)
         # localize dates to remove timezone; writing to excel with timezone is not supported
         jobs_df["CreatedOn"] = jobs_df["CreatedOn"].dt.tz_localize(None)
         jobs_df["LastModifiedOn"] = jobs_df["LastModifiedOn"].dt.tz_localize(None)
 
         return jobs_df
 
-    def glue_get_job_history(self, job_name, no_of_runs=1):
+    def glue_get_job_history(self, job_name, no_of_runs=1) -> pd.DataFrame:
+        """
+        Retrieve glue job history
+
+        Arguments:
+            job_name -- Name of job to retrive history
+
+        Keyword Arguments:
+            no_of_runs -- No of runs to retrive in descending order (default: {1})
+
+        Returns:
+            dataframe
+        """
+
         glue_run_df_columns = [
             "Id",
             "JobName",
             "JobRunState",
             "StartedOn",
             "stopDate",
             DURATION_COL_NAME,
@@ -226,21 +270,36 @@
 
         if not final_df.empty:
             final_df["startDate"] = final_df["startDate"].dt.tz_localize(None)
             final_df["stopDate"] = final_df["stopDate"].dt.tz_localize(None)
 
         return final_df
 
-    def glue_get_databases(self) -> DataFrame:
+    def glue_get_databases(self) -> pd.DataFrame:
+        """
+        Get AWS Glue jobs
+
+        Returns:
+            dataframe
+        """
         dbs = wr.catalog.get_databases(boto3_session=self.session)
         data = [(db["Name"]) for db in dbs]
         databases_df = pd.DataFrame(data, columns=["DBName"])
         return databases_df
 
-    def glue_get_tables(self, dbname=None):
+    def glue_get_tables(self, dbname=None) -> pd.DataFrame:
+        """
+        Get AWS Glue tables
+
+        Keyword Arguments:
+            dbname -- Database Name for which to retrive tables (default: {None})
+
+        Returns:
+            dataframe
+        """
         tables = wr.catalog.get_tables(database=dbname, boto3_session=self.session)
 
         data = [
             (
                 table["Name"],
                 get_value("CreateTime", table),
                 get_value("UpdateTime", table),
@@ -338,21 +397,14 @@
         self,
         dataframe_to_upload: pd.DataFrame,
         table_name: str,
         s3_path: str,
         database="qdl_temp",
         mode="overwrite",
     ):
-        """
-        create_athena_table
-
-        Arguments:
-            dataframe_to_upload
-        """
-
         try:
             session = self.session
             wr.s3.to_parquet(
                 df=dataframe_to_upload,
                 path=s3_path,
                 dataset=True,
                 mode=mode,
```

### Comparing `awsdf-0.1.8/PKG-INFO` & `awsdf-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsdf
-Version: 0.1.8
+Version: 0.1.9
 Summary: AWS metadata as dataframes
 Author: Allan
 Author-email: allan.dsouza@gmail.com
 Requires-Python: >=3.7.2,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,85 +23,88 @@
 Submodules
 ==========
 
 
 awsdf.aws module
 ================
 
-Main module.
+This module enables connecting to AWS and extracting metadata in
+pandas dataframes.
 
-**class awsdf.aws.Account(aws_access_key_id=None,
-aws_secret_access_key=None, aws_session_token=None, region_name=None,
-profile_name=None)**
+**Installing from PyPI:** *pip install -U awsdf*
 
-   Bases: ``object``
+**USAGE:**
 
-   ``property accountid``
+   import awsdf
 
-   **athena_create_table(dataframe_to_upload: DataFrame, table_name:
-   str, s3_path: str, database='qdl_temp', mode='overwrite')**
-
-      create_athena_table
-
-      Arguments:
-         dataframe_to_upload
+   aws_account = awsdf.Account(profile_name=”<PROFILE_NAME>”)
 
-   **athena_execute_query(database: str, query: str, use_cache: bool =
-   True)**
+   glue_databases_df = aws_account.glue_get_databases()
 
-   **athena_get_view_definition(database: str, viewname: str,
-   query_location: str)**
+**class awsdf.aws.Account(aws_access_key_id=None,
+aws_secret_access_key=None, aws_session_token=None, region_name=None,
+profile_name=None)**
 
-   **ec2_get_instance_id(hostname)**
+   Instantiate class object for connecting to AWS and retriving
+   metadata from AWS
 
-   **ec2_get_instanceip(ec2_instance_id)**
+   **__init__(aws_access_key_id=None, aws_secret_access_key=None,
+   aws_session_token=None, region_name=None, profile_name=None)**
 
-   **ec2_get_instances()**
+      Provide access keys OR Profile name to connect to AWS account.
+      Keys take preceedence
 
-   **ecs_get_allservices() -> DataFrame**
+      **Parameters:**
 
-   **ecs_get_clusters() -> DataFrame**
+         *aws_access_key_id (string) – AWS access key ID*
 
-   **ecs_get_container_ec2_instanceid(cluster_arn,
-   container_instance)**
+         *aws_secret_access_key (string) – AWS secret access key*
 
-   **ecs_get_container_instance(cluster_arn, task_arn)**
+         *aws_session_token (string) – AWS temporary session token*
 
-   **ecs_get_services(cluster_arn) -> DataFrame**
+         *region_name (string) – AWS region*
 
-   **ecs_get_tasks(cluster_arn, service_arn)**
+         *profile_name (string) – AWS profile name*
 
-   **get_available_profiles() -> list[str]**
+   **glue_get_jobs() -> DataFrame**
 
-   **glue_get_databases() -> DataFrame**
+      Get AWS Glue jobs
 
-   **glue_get_job_history(job_name, no_of_runs=1)**
+      Returns:
+         dataframe
 
-   **glue_get_jobs()**
+   **glue_get_job_history(job_name, no_of_runs=1) -> DataFrame**
 
-   **glue_get_tables(dbname=None)**
+      Retrieve glue job history
 
-   **iam_get_accountid() -> str**
+      Arguments:
+         job_name – Name of job to retrive history
 
-   **lambda_get_functions()**
+      Keyword Arguments:
+         no_of_runs – No of runs to retrive in descending order
+         (default: {1})
 
-   **lambda_get_invocations(lambda_name, start_date=None,
-   end_date=None)**
+      Returns:
+         dataframe
 
-   **lambda_get_metrics_list(namespace='AWS/Lambda')**
+   **glue_get_databases() -> DataFrame**
 
-   ``property region``
+      Get AWS Glue jobs
 
-   **s3_wait_check_object_exists(bucket_name, key_name)**
+      Returns:
+         dataframe
 
-   ``property session``
+   **glue_get_tables(dbname=None) -> DataFrame**
 
-   **sfn_get_statemachines()**
+      Get AWS Glue tables
 
-**awsdf.aws.get_value(key, obj)**
+      Keyword Arguments:
+         dbname – Database Name for which to retrive tables (default:
+         {None})
 
-**awsdf.aws.keyexists(key, dictionary)**
+      Returns:
+         dataframe
 
 
 Module contents
 ===============
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

