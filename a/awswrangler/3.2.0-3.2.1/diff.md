# Comparing `tmp/awswrangler-3.2.0.tar.gz` & `tmp/awswrangler-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.2.0.tar", max compression
+gzip compressed data, was "awswrangler-3.2.1.tar", max compression
```

## Comparing `awswrangler-3.2.0.tar` & `awswrangler-3.2.1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.2.0/NOTICE.txt
--rw-r--r--   0        0        0    19946 2023-06-12 13:30:35.513945 awswrangler-3.2.0/README.md
--rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.2.0/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1445 2023-05-31 14:40:28.389961 awswrangler-3.2.0/awswrangler/__init__.py
--rw-r--r--   0        0        0      276 2023-06-12 13:30:35.514884 awswrangler-3.2.0/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     4351 2023-06-01 19:20:47.696084 awswrangler-3.2.0/awswrangler/_arrow.py
--rw-r--r--   0        0        0    28922 2023-05-31 14:40:28.390662 awswrangler-3.2.0/awswrangler/_config.py
--rw-r--r--   0        0        0    32498 2023-05-30 21:03:56.362052 awswrangler-3.2.0/awswrangler/_data_types.py
--rw-r--r--   0        0        0    13918 2023-05-30 20:11:08.955818 awswrangler-3.2.0/awswrangler/_databases.py
--rw-r--r--   0        0        0     6254 2023-06-01 18:11:15.743108 awswrangler-3.2.0/awswrangler/_distributed.py
--rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.2.0/awswrangler/_executor.py
--rw-r--r--   0        0        0     5780 2023-06-08 17:37:13.335354 awswrangler-3.2.0/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0    29441 2023-06-07 15:18:15.457609 awswrangler-3.2.0/awswrangler/_utils.py
--rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.2.0/awswrangler/annotations.py
--rw-r--r--   0        0        0     1329 2023-06-12 13:31:06.245746 awswrangler-3.2.0/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9602 2023-05-26 14:00:36.361829 awswrangler-3.2.0/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0     9681 2023-06-12 13:31:06.246845 awswrangler-3.2.0/awswrangler/athena/_executions.py
--rw-r--r--   0        0        0     2148 2023-06-12 13:31:06.247439 awswrangler-3.2.0/awswrangler/athena/_executions.pyi
--rw-r--r--   0        0        0    57298 2023-06-12 13:31:06.248210 awswrangler-3.2.0/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    12408 2023-06-12 13:31:06.248740 awswrangler-3.2.0/awswrangler/athena/_read.pyi
--rw-r--r--   0        0        0     8661 2023-06-06 15:33:48.272209 awswrangler-3.2.0/awswrangler/athena/_spark.py
--rw-r--r--   0        0        0    42079 2023-06-12 13:31:06.249301 awswrangler-3.2.0/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     8398 2023-06-05 15:24:55.446413 awswrangler-3.2.0/awswrangler/athena/_write_iceberg.py
--rw-r--r--   0        0        0     2531 2023-06-08 16:04:13.943426 awswrangler-3.2.0/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    17109 2023-06-08 16:04:13.943922 awswrangler-3.2.0/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    60168 2023-06-08 16:04:13.944729 awswrangler-3.2.0/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    14525 2023-06-08 16:04:13.945212 awswrangler-3.2.0/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.2.0/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36053 2023-05-26 15:59:19.165550 awswrangler-3.2.0/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.2.0/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2023-06-07 15:18:15.458044 awswrangler-3.2.0/awswrangler/chime.py
--rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.2.0/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.2.0/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     5367 2023-05-30 20:11:08.961643 awswrangler-3.2.0/awswrangler/data_api/_connector.py
--rw-r--r--   0        0        0    16265 2023-06-08 16:04:13.945849 awswrangler-3.2.0/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0    11152 2023-05-30 20:11:08.962941 awswrangler-3.2.0/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.2.0/awswrangler/data_quality/__init__.py
--rw-r--r--   0        0        0    13403 2023-05-24 14:22:08.634079 awswrangler-3.2.0/awswrangler/data_quality/_create.py
--rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.2.0/awswrangler/data_quality/_get.py
--rw-r--r--   0        0        0     6762 2023-06-02 15:24:52.109779 awswrangler-3.2.0/awswrangler/data_quality/_utils.py
--rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.2.0/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.2.0/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     6334 2023-05-31 17:49:00.586004 awswrangler-3.2.0/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.2.0/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.2.0/awswrangler/distributed/ray/_executor.py
--rw-r--r--   0        0        0     4971 2023-06-08 16:04:13.946455 awswrangler-3.2.0/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.2.0/awswrangler/distributed/ray/_utils.py
--rw-r--r--   0        0        0     1131 2023-06-08 16:04:13.946930 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
--rw-r--r--   0        0        0     1999 2023-06-08 16:04:13.947209 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py
--rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
--rw-r--r--   0        0        0    19699 2023-06-09 14:50:38.346223 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     9016 2023-06-02 15:24:52.110526 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.2.0/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      929 2023-06-12 14:16:31.031863 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     4126 2023-05-24 14:22:08.637288 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1484 2023-06-08 16:04:13.947578 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_orc.py
--rw-r--r--   0        0        0     1871 2023-05-31 17:49:00.586748 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     5507 2023-05-31 17:49:00.587331 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3043 2023-06-08 16:04:13.947746 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_orc.py
--rw-r--r--   0        0        0     3065 2023-06-05 20:19:19.920635 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5479 2023-05-24 14:22:08.637884 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.2.0/awswrangler/distributed/ray/s3/__init__.py
--rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_list.py
--rw-r--r--   0        0        0      850 2023-06-08 16:04:13.947913 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_orc.py
--rw-r--r--   0        0        0     1005 2023-05-24 14:22:08.638085 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_parquet.py
--rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.2.0/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.2.0/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0    25553 2023-05-25 19:44:59.410205 awswrangler-3.2.0/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     9612 2023-05-25 19:44:59.410735 awswrangler-3.2.0/awswrangler/dynamodb/_read.pyi
--rw-r--r--   0        0        0     6918 2023-05-31 14:40:28.392193 awswrangler-3.2.0/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.2.0/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    44390 2023-05-30 21:03:56.363883 awswrangler-3.2.0/awswrangler/emr.py
--rw-r--r--   0        0        0    10247 2023-05-31 14:40:28.392544 awswrangler-3.2.0/awswrangler/emr_serverless.py
--rw-r--r--   0        0        0     2977 2023-06-06 15:33:48.272648 awswrangler-3.2.0/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.2.0/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    12069 2023-06-01 18:11:15.749542 awswrangler-3.2.0/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.2.0/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    21739 2023-06-07 15:18:11.152506 awswrangler-3.2.0/awswrangler/mysql.py
--rw-r--r--   0        0        0      673 2023-05-26 16:02:45.896496 awswrangler-3.2.0/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0    16117 2023-05-30 20:11:08.965837 awswrangler-3.2.0/awswrangler/neptune/_client.py
--rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.2.0/awswrangler/neptune/_gremlin_init.py
--rw-r--r--   0        0        0     2708 2023-05-30 20:11:08.966466 awswrangler-3.2.0/awswrangler/neptune/_gremlin_parser.py
--rw-r--r--   0        0        0    25013 2023-05-30 20:11:08.967071 awswrangler-3.2.0/awswrangler/neptune/_neptune.py
--rw-r--r--   0        0        0     3752 2023-05-26 16:02:45.898491 awswrangler-3.2.0/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.2.0/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     6480 2023-05-25 19:45:07.454333 awswrangler-3.2.0/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0    13764 2023-05-25 19:45:07.455041 awswrangler-3.2.0/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    23823 2023-06-01 18:11:15.750105 awswrangler-3.2.0/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    22400 2023-05-30 20:11:08.968627 awswrangler-3.2.0/awswrangler/oracle.py
--rw-r--r--   0        0        0     1282 2023-05-31 19:28:36.904170 awswrangler-3.2.0/awswrangler/pandas/__init__.py
--rw-r--r--   0        0        0    22222 2023-05-25 19:45:07.457161 awswrangler-3.2.0/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.2.0/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.2.0/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.2.0/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    19228 2023-05-24 14:22:08.643001 awswrangler-3.2.0/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.2.0/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.2.0/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.2.0/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     2096 2023-05-24 14:22:08.643693 awswrangler-3.2.0/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0      440 2023-05-24 14:22:08.643793 awswrangler-3.2.0/awswrangler/redshift/__init__.py
--rw-r--r--   0        0        0     8809 2023-05-25 19:45:07.457727 awswrangler-3.2.0/awswrangler/redshift/_connect.py
--rw-r--r--   0        0        0    20832 2023-05-25 19:45:07.458325 awswrangler-3.2.0/awswrangler/redshift/_read.py
--rw-r--r--   0        0        0     6716 2023-05-25 19:44:59.414763 awswrangler-3.2.0/awswrangler/redshift/_read.pyi
--rw-r--r--   0        0        0    15681 2023-06-08 16:02:36.685888 awswrangler-3.2.0/awswrangler/redshift/_utils.py
--rw-r--r--   0        0        0    28318 2023-05-25 19:45:07.459429 awswrangler-3.2.0/awswrangler/redshift/_write.py
--rw-r--r--   0        0        0     2008 2023-06-08 16:04:13.948537 awswrangler-3.2.0/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0    10594 2023-05-24 14:22:08.646591 awswrangler-3.2.0/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.2.0/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.2.0/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.2.0/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.2.0/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.2.0/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     4158 2023-05-25 19:44:59.415563 awswrangler-3.2.0/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0    15344 2023-06-08 16:04:13.949787 awswrangler-3.2.0/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     4167 2023-06-02 15:24:52.111207 awswrangler-3.2.0/awswrangler/s3/_read_deltalake.py
--rw-r--r--   0        0        0     3277 2023-05-25 19:45:07.459896 awswrangler-3.2.0/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    23253 2023-06-08 16:04:13.950493 awswrangler-3.2.0/awswrangler/s3/_read_orc.py
--rw-r--r--   0        0        0    33869 2023-06-12 13:30:35.516197 awswrangler-3.2.0/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0    10040 2023-06-12 13:30:35.516790 awswrangler-3.2.0/awswrangler/s3/_read_parquet.pyi
--rw-r--r--   0        0        0    27928 2023-06-12 13:30:35.517277 awswrangler-3.2.0/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     7993 2023-05-25 19:44:59.418542 awswrangler-3.2.0/awswrangler/s3/_read_text.pyi
--rw-r--r--   0        0        0     4108 2023-05-22 20:51:56.860472 awswrangler-3.2.0/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    12569 2023-05-25 19:44:59.419017 awswrangler-3.2.0/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.2.0/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.2.0/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0    18407 2023-06-08 16:04:13.952552 awswrangler-3.2.0/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.2.0/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12740 2023-05-30 20:11:08.971499 awswrangler-3.2.0/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     4144 2023-06-02 15:24:52.111757 awswrangler-3.2.0/awswrangler/s3/_write_deltalake.py
--rw-r--r--   0        0        0     3196 2023-05-25 19:45:07.460376 awswrangler-3.2.0/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    26674 2023-06-08 16:04:13.953259 awswrangler-3.2.0/awswrangler/s3/_write_orc.py
--rw-r--r--   0        0        0    39437 2023-06-12 13:30:35.518029 awswrangler-3.2.0/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    48588 2023-06-12 13:30:35.518732 awswrangler-3.2.0/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.2.0/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    19421 2023-05-25 19:45:07.461036 awswrangler-3.2.0/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.2.0/awswrangler/sts.py
--rw-r--r--   0        0        0      727 2023-05-25 19:44:59.420093 awswrangler-3.2.0/awswrangler/timestream/__init__.py
--rw-r--r--   0        0        0     4512 2023-05-24 14:22:08.650822 awswrangler-3.2.0/awswrangler/timestream/_create.py
--rw-r--r--   0        0        0     2491 2023-05-24 14:22:08.651071 awswrangler-3.2.0/awswrangler/timestream/_delete.py
--rw-r--r--   0        0        0     2603 2023-05-24 14:22:08.651315 awswrangler-3.2.0/awswrangler/timestream/_list.py
--rw-r--r--   0        0        0    16998 2023-05-30 21:03:56.364637 awswrangler-3.2.0/awswrangler/timestream/_read.py
--rw-r--r--   0        0        0     1910 2023-05-25 19:44:59.421306 awswrangler-3.2.0/awswrangler/timestream/_read.pyi
--rw-r--r--   0        0        0    26397 2023-05-24 14:22:08.652414 awswrangler-3.2.0/awswrangler/timestream/_write.py
--rw-r--r--   0        0        0     9355 2023-06-08 16:04:13.954640 awswrangler-3.2.0/awswrangler/typing.py
--rw-r--r--   0        0        0     4847 2023-06-12 15:27:53.371623 awswrangler-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.2.1/NOTICE.txt
+-rw-r--r--   0        0        0    19946 2023-06-14 21:39:23.380775 awswrangler-3.2.1/README.md
+-rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.2.1/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1445 2023-06-13 21:15:14.188495 awswrangler-3.2.1/awswrangler/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-14 21:39:23.381455 awswrangler-3.2.1/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     4351 2023-06-13 21:15:14.189071 awswrangler-3.2.1/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    28922 2023-06-13 21:15:14.189395 awswrangler-3.2.1/awswrangler/_config.py
+-rw-r--r--   0        0        0    32498 2023-06-13 21:15:14.189750 awswrangler-3.2.1/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    13918 2023-06-13 21:15:14.190038 awswrangler-3.2.1/awswrangler/_databases.py
+-rw-r--r--   0        0        0     6254 2023-06-13 21:15:14.190280 awswrangler-3.2.1/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.2.1/awswrangler/_executor.py
+-rw-r--r--   0        0        0     5780 2023-06-13 21:15:14.190528 awswrangler-3.2.1/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0    29441 2023-06-13 21:15:14.190851 awswrangler-3.2.1/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.2.1/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1329 2023-06-14 21:39:23.381802 awswrangler-3.2.1/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9602 2023-06-13 21:15:14.191569 awswrangler-3.2.1/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0     9681 2023-06-14 21:39:23.382168 awswrangler-3.2.1/awswrangler/athena/_executions.py
+-rw-r--r--   0        0        0     2148 2023-06-14 21:39:23.382413 awswrangler-3.2.1/awswrangler/athena/_executions.pyi
+-rw-r--r--   0        0        0    57298 2023-06-14 21:39:23.382977 awswrangler-3.2.1/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    12408 2023-06-14 21:39:23.383292 awswrangler-3.2.1/awswrangler/athena/_read.pyi
+-rw-r--r--   0        0        0     8661 2023-06-13 21:15:14.193473 awswrangler-3.2.1/awswrangler/athena/_spark.py
+-rw-r--r--   0        0        0    42079 2023-06-14 21:39:23.383659 awswrangler-3.2.1/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     8398 2023-06-13 21:15:14.194522 awswrangler-3.2.1/awswrangler/athena/_write_iceberg.py
+-rw-r--r--   0        0        0     2531 2023-06-13 21:15:14.194795 awswrangler-3.2.1/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    17109 2023-06-13 21:15:14.195033 awswrangler-3.2.1/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    60168 2023-06-13 21:15:14.195357 awswrangler-3.2.1/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    14525 2023-06-13 21:15:14.195595 awswrangler-3.2.1/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.2.1/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36053 2023-05-26 15:59:19.165550 awswrangler-3.2.1/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.2.1/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2023-06-07 15:18:15.458044 awswrangler-3.2.1/awswrangler/chime.py
+-rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.2.1/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.2.1/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     5367 2023-06-13 21:15:14.196073 awswrangler-3.2.1/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0    16265 2023-06-13 21:15:14.196358 awswrangler-3.2.1/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0    11152 2023-06-13 21:15:14.196599 awswrangler-3.2.1/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.2.1/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13403 2023-05-24 14:22:08.634079 awswrangler-3.2.1/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.2.1/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6762 2023-06-13 21:15:14.196842 awswrangler-3.2.1/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.2.1/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.2.1/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6334 2023-06-13 21:15:14.199735 awswrangler-3.2.1/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.2.1/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0     2151 2023-06-14 18:23:54.169183 awswrangler-3.2.1/awswrangler/distributed/ray/_executor.py
+-rw-r--r--   0        0        0     4971 2023-06-13 21:15:14.200016 awswrangler-3.2.1/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     2503 2023-06-14 18:23:54.170071 awswrangler-3.2.1/awswrangler/distributed/ray/_utils.py
+-rw-r--r--   0        0        0     1131 2023-06-13 21:15:14.200645 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2186 2023-06-14 18:23:54.171486 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     2036 2023-06-14 21:46:19.742499 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py
+-rw-r--r--   0        0        0     3318 2023-06-14 18:23:54.173362 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    19694 2023-06-14 18:23:54.174400 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     8953 2023-06-14 18:23:54.175332 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5891 2023-06-14 18:23:54.175963 awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.2.1/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-06-12 14:16:31.031863 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4068 2023-06-14 18:23:54.177267 awswrangler-3.2.1/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-13 21:15:14.202375 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_orc.py
+-rw-r--r--   0        0        0     1871 2023-06-13 21:15:14.202754 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-06-13 21:15:14.203222 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3043 2023-06-13 21:15:14.203325 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_orc.py
+-rw-r--r--   0        0        0     3065 2023-06-05 20:19:19.920635 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5479 2023-06-13 21:15:14.203788 awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.2.1/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0      850 2023-06-13 21:15:14.203888 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_orc.py
+-rw-r--r--   0        0        0     1005 2023-05-24 14:22:08.638085 awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.2.1/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.2.1/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    25553 2023-06-13 21:15:14.204147 awswrangler-3.2.1/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     9612 2023-06-13 21:15:14.204271 awswrangler-3.2.1/awswrangler/dynamodb/_read.pyi
+-rw-r--r--   0        0        0     6918 2023-06-13 21:15:14.204966 awswrangler-3.2.1/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.2.1/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    44390 2023-06-13 21:15:14.206293 awswrangler-3.2.1/awswrangler/emr.py
+-rw-r--r--   0        0        0    10247 2023-06-13 21:15:14.206475 awswrangler-3.2.1/awswrangler/emr_serverless.py
+-rw-r--r--   0        0        0     2977 2023-06-13 21:15:14.207077 awswrangler-3.2.1/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.2.1/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    12069 2023-06-13 21:15:14.207817 awswrangler-3.2.1/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.2.1/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    21739 2023-06-13 21:15:14.208458 awswrangler-3.2.1/awswrangler/mysql.py
+-rw-r--r--   0        0        0      673 2023-06-13 21:15:14.208796 awswrangler-3.2.1/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0    16117 2023-06-13 21:15:14.210053 awswrangler-3.2.1/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.2.1/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2708 2023-06-13 21:15:14.210311 awswrangler-3.2.1/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    25013 2023-06-13 21:15:14.211352 awswrangler-3.2.1/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3752 2023-06-13 21:15:14.212053 awswrangler-3.2.1/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.2.1/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6480 2023-06-13 21:13:23.797325 awswrangler-3.2.1/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13764 2023-06-13 21:13:23.797629 awswrangler-3.2.1/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    23823 2023-06-13 21:15:14.212648 awswrangler-3.2.1/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    22400 2023-06-13 21:15:14.212930 awswrangler-3.2.1/awswrangler/oracle.py
+-rw-r--r--   0        0        0     1282 2023-06-13 21:15:14.213188 awswrangler-3.2.1/awswrangler/pandas/__init__.py
+-rw-r--r--   0        0        0    22222 2023-06-13 21:15:14.214956 awswrangler-3.2.1/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.2.1/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.2.1/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.2.1/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    19228 2023-06-13 21:15:14.218977 awswrangler-3.2.1/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.2.1/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.2.1/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.2.1/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     2096 2023-06-13 21:15:14.220205 awswrangler-3.2.1/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0      440 2023-06-13 21:15:14.220549 awswrangler-3.2.1/awswrangler/redshift/__init__.py
+-rw-r--r--   0        0        0     8809 2023-06-13 21:15:14.220661 awswrangler-3.2.1/awswrangler/redshift/_connect.py
+-rw-r--r--   0        0        0    20832 2023-06-13 21:15:14.220795 awswrangler-3.2.1/awswrangler/redshift/_read.py
+-rw-r--r--   0        0        0     6716 2023-06-13 21:15:14.220904 awswrangler-3.2.1/awswrangler/redshift/_read.pyi
+-rw-r--r--   0        0        0    15681 2023-06-13 21:15:14.221067 awswrangler-3.2.1/awswrangler/redshift/_utils.py
+-rw-r--r--   0        0        0    28318 2023-06-13 21:15:14.221202 awswrangler-3.2.1/awswrangler/redshift/_write.py
+-rw-r--r--   0        0        0     2008 2023-06-13 21:15:14.221574 awswrangler-3.2.1/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10594 2023-05-24 14:22:08.646591 awswrangler-3.2.1/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.2.1/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.2.1/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.2.1/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.2.1/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.2.1/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     4158 2023-06-13 21:15:14.221765 awswrangler-3.2.1/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0    15344 2023-06-13 21:15:14.222716 awswrangler-3.2.1/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     4167 2023-06-13 21:15:14.222974 awswrangler-3.2.1/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3277 2023-06-13 21:13:23.801300 awswrangler-3.2.1/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    23265 2023-06-14 20:26:54.837101 awswrangler-3.2.1/awswrangler/s3/_read_orc.py
+-rw-r--r--   0        0        0    33869 2023-06-14 21:39:23.384240 awswrangler-3.2.1/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0    10040 2023-06-13 21:15:14.225352 awswrangler-3.2.1/awswrangler/s3/_read_parquet.pyi
+-rw-r--r--   0        0        0    27928 2023-06-14 21:39:23.384699 awswrangler-3.2.1/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     7993 2023-06-13 21:15:14.226169 awswrangler-3.2.1/awswrangler/s3/_read_text.pyi
+-rw-r--r--   0        0        0     4108 2023-05-22 20:51:56.860472 awswrangler-3.2.1/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    12569 2023-06-13 21:15:14.226577 awswrangler-3.2.1/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.2.1/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.2.1/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0    18407 2023-06-13 21:15:14.227190 awswrangler-3.2.1/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.2.1/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12740 2023-06-13 21:15:14.227436 awswrangler-3.2.1/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     4144 2023-06-13 21:15:14.227527 awswrangler-3.2.1/awswrangler/s3/_write_deltalake.py
+-rw-r--r--   0        0        0     3196 2023-06-13 21:13:23.801521 awswrangler-3.2.1/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    26700 2023-06-14 20:26:54.837927 awswrangler-3.2.1/awswrangler/s3/_write_orc.py
+-rw-r--r--   0        0        0    39437 2023-06-14 21:39:23.386060 awswrangler-3.2.1/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48588 2023-06-14 21:39:23.386613 awswrangler-3.2.1/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.2.1/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    19421 2023-06-13 21:15:14.231127 awswrangler-3.2.1/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.2.1/awswrangler/sts.py
+-rw-r--r--   0        0        0      727 2023-06-13 21:15:14.231474 awswrangler-3.2.1/awswrangler/timestream/__init__.py
+-rw-r--r--   0        0        0     4512 2023-06-13 21:15:14.231567 awswrangler-3.2.1/awswrangler/timestream/_create.py
+-rw-r--r--   0        0        0     2491 2023-06-13 21:15:14.231639 awswrangler-3.2.1/awswrangler/timestream/_delete.py
+-rw-r--r--   0        0        0     2603 2023-06-13 21:15:14.231709 awswrangler-3.2.1/awswrangler/timestream/_list.py
+-rw-r--r--   0        0        0    16998 2023-06-13 21:15:14.231817 awswrangler-3.2.1/awswrangler/timestream/_read.py
+-rw-r--r--   0        0        0     1910 2023-06-13 21:15:14.231911 awswrangler-3.2.1/awswrangler/timestream/_read.pyi
+-rw-r--r--   0        0        0    26397 2023-06-13 21:15:14.232051 awswrangler-3.2.1/awswrangler/timestream/_write.py
+-rw-r--r--   0        0        0     9355 2023-06-13 21:15:14.233372 awswrangler-3.2.1/awswrangler/typing.py
+-rw-r--r--   0        0        0     4854 2023-06-14 21:39:23.387816 awswrangler-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.2.1/PKG-INFO
```

### Comparing `awswrangler-3.2.0/LICENSE.txt` & `awswrangler-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/README.md` & `awswrangler-3.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.2.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.2.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -95,33 +95,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -154,39 +154,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

### Comparing `awswrangler-3.2.0/THIRD_PARTY.txt` & `awswrangler-3.2.1/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/__init__.py` & `awswrangler-3.2.1/awswrangler/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_arrow.py` & `awswrangler-3.2.1/awswrangler/_arrow.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_config.py` & `awswrangler-3.2.1/awswrangler/_config.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_data_types.py` & `awswrangler-3.2.1/awswrangler/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_databases.py` & `awswrangler-3.2.1/awswrangler/_databases.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_distributed.py` & `awswrangler-3.2.1/awswrangler/_distributed.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_executor.py` & `awswrangler-3.2.1/awswrangler/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_sql_formatter.py` & `awswrangler-3.2.1/awswrangler/_sql_formatter.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/_utils.py` & `awswrangler-3.2.1/awswrangler/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/annotations.py` & `awswrangler-3.2.1/awswrangler/annotations.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/__init__.py` & `awswrangler-3.2.1/awswrangler/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_cache.py` & `awswrangler-3.2.1/awswrangler/athena/_cache.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_executions.py` & `awswrangler-3.2.1/awswrangler/athena/_executions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_executions.pyi` & `awswrangler-3.2.1/awswrangler/athena/_executions.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_read.py` & `awswrangler-3.2.1/awswrangler/athena/_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,19 +740,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -808,15 +808,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1062,19 +1062,19 @@
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -1130,15 +1130,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.1/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
```

### Comparing `awswrangler-3.2.0/awswrangler/athena/_read.pyi` & `awswrangler-3.2.1/awswrangler/athena/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_spark.py` & `awswrangler-3.2.1/awswrangler/athena/_spark.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_utils.py` & `awswrangler-3.2.1/awswrangler/athena/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/athena/_write_iceberg.py` & `awswrangler-3.2.1/awswrangler/athena/_write_iceberg.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/__init__.py` & `awswrangler-3.2.1/awswrangler/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_add.py` & `awswrangler-3.2.1/awswrangler/catalog/_add.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_create.py` & `awswrangler-3.2.1/awswrangler/catalog/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_definitions.py` & `awswrangler-3.2.1/awswrangler/catalog/_definitions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_delete.py` & `awswrangler-3.2.1/awswrangler/catalog/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_get.py` & `awswrangler-3.2.1/awswrangler/catalog/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/catalog/_utils.py` & `awswrangler-3.2.1/awswrangler/catalog/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/chime.py` & `awswrangler-3.2.1/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/cloudwatch.py` & `awswrangler-3.2.1/awswrangler/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_api/_connector.py` & `awswrangler-3.2.1/awswrangler/data_api/_connector.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_api/rds.py` & `awswrangler-3.2.1/awswrangler/data_api/rds.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_api/redshift.py` & `awswrangler-3.2.1/awswrangler/data_api/redshift.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_quality/_create.py` & `awswrangler-3.2.1/awswrangler/data_quality/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_quality/_get.py` & `awswrangler-3.2.1/awswrangler/data_quality/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/data_quality/_utils.py` & `awswrangler-3.2.1/awswrangler/data_quality/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/_core.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.2.1/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/_executor.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def map(self, func: Callable[..., MapOutputType], _: Optional["BaseClient"], *args: Any) -> List[MapOutputType]:
         """Map func and return ray futures."""
         _logger.debug("Ray map: %s", func)
         # Discard boto3 client
         return list(func(*arg) for arg in zip(itertools.repeat(None), *args))
 
 
-@ray.remote
+@ray.remote  # type: ignore[attr-defined]
 class AsyncActor:
     async def run_concurrent(self, func: Callable[..., MapOutputType], *args: Any) -> MapOutputType:
         return func(*args)
 
 
 class _RayMaxConcurrencyExecutor(_BaseExecutor):
     def __init__(self, max_concurrency: int) -> None:
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/_register.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/_register.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/_utils.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     If we aren't in a placement group, this is trivially the number of CPUs in the
     cluster. Otherwise, we try to calculate how large the placement group is relative
     to the size of the cluster.
 
     Args:
         cur_pg: The current placement group, if any.
     """
-    cluster_cpus = int(ray.cluster_resources().get("CPU", 1))
-    cluster_gpus = int(ray.cluster_resources().get("GPU", 0))
+    cluster_cpus = int(ray.cluster_resources().get("CPU", 1))  # type: ignore[attr-defined]
+    cluster_gpus = int(ray.cluster_resources().get("GPU", 0))  # type: ignore[attr-defined]
 
     # If we're in a placement group, we shouldn't assume the entire cluster's
     # resources are available for us to use. Estimate an upper bound on what's
     # reasonable to assume is available for datasets to use.
     if cur_pg:
         pg_cpus = 0
         for bundle in cur_pg.bundle_specs:
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,14 @@
 
             except StopIteration:
                 return
 
     def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ
         self,
         f: pa.NativeFile,
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         **writer_args: Any,
     ) -> None:
         write_options_dict = writer_args.get("write_options", {})
         write_options = csv.WriteOptions(**write_options_dict)
 
         csv.write_csv(block.to_arrow(), f, write_options)
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Ray ArrowCSVDatasource Module."""
 from typing import Any, Dict, List, Optional
 
 import pyarrow as pa
-from pyarrow import orc
 from ray.data.block import BlockAccessor
 
 from awswrangler._arrow import _add_table_partitions, _df_to_table
 from awswrangler.distributed.ray.datasources.pandas_file_based_datasource import PandasFileBasedDatasource
 
 
 class ArrowORCDatasource(PandasFileBasedDatasource):
@@ -17,14 +16,16 @@
     def _read_file(  # type: ignore[override]
         self,
         f: pa.NativeFile,
         path: str,
         path_root: str,
         **reader_args: Any,
     ) -> pa.Table:
+        from pyarrow import orc
+
         columns: Optional[List[str]] = reader_args.get("columns", None)
 
         table: pa.Table = orc.read_table(f, columns=columns)
 
         table = _add_table_partitions(
             table=table,
             path=f"s3://{path}",
@@ -40,18 +41,20 @@
         **open_args: Any,
     ) -> pa.NativeFile:
         return filesystem.open_input_file(path, **open_args)
 
     def _write_block(  # type: ignore[override]
         self,
         f: pa.NativeFile,
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         pandas_kwargs: Optional[Dict[str, Any]],
         **writer_args: Any,
     ) -> None:
+        from pyarrow import orc
+
         schema: Optional[pa.schema] = writer_args.get("schema", None)
         dtype: Optional[Dict[str, str]] = writer_args.get("dtype", None)
         index: bool = writer_args.get("index", False)
         compression: str = writer_args.get("compression", None) or "UNCOMPRESSED"
         pyarrow_additional_kwargs: Dict[str, Any] = writer_args.get("pyarrow_additional_kwargs", {})
 
         orc.write_table(
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     ) -> pa.NativeFile:
         # Parquet requires `open_input_file` due to random access reads
         return filesystem.open_input_file(path, **open_args)
 
     def _write_block(  # type: ignore[override]
         self,
         f: pa.NativeFile,
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         **writer_args: Any,
     ) -> None:
         schema: Optional[pa.schema] = writer_args.get("schema", None)
         dtype: Optional[Dict[str, str]] = writer_args.get("dtype", None)
         index: bool = writer_args.get("index", False)
         compression: Optional[str] = writer_args.get("compression", None)
         pyarrow_additional_kwargs: Dict[str, Any] = writer_args.get("pyarrow_additional_kwargs", {})
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,22 @@
     The following are the changes to the original Ray implementation:
     1. Added handling of additional parameters `dtype`, `index`, `compression` and added the ability
        to pass through additional `pyarrow_additional_kwargs` and `s3_additional_kwargs` for writes.
     3. Added `dataset` and `path_root` parameters to allow user to control loading partitions
        relative to the root S3 prefix.
     """
 
-    def create_reader(self, **kwargs: Dict[str, Any]) -> Reader[Any]:
+    def create_reader(self, **kwargs: Dict[str, Any]) -> Reader:
         """Return a Reader for the given read arguments."""
         return _ArrowParquetDatasourceReader(**kwargs)  # type: ignore[arg-type]
 
     def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ, arguments-renamed, unused-argument
         self,
         f: "pyarrow.NativeFile",
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         pandas_kwargs: Optional[Dict[str, Any]],
         **writer_args: Any,
     ) -> None:
         """Write a block to S3."""
         import pyarrow as pa  # pylint: disable=import-outside-toplevel,reimported
 
         schema: pa.Schema = writer_args.get("schema", None)
@@ -181,39 +181,39 @@
             # 1, 2, 4, 8, 16, 32, 64
             time.sleep(min_interval)
             min_interval = min_interval * 2
             final_exception = e
     raise final_exception  # type: ignore[misc]
 
 
-class _ArrowParquetDatasourceReader(Reader[Any]):  # pylint: disable=too-many-instance-attributes
+class _ArrowParquetDatasourceReader(Reader):  # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
         paths: Union[str, List[str]],
         local_uri: bool = False,
         filesystem: Optional["pyarrow.fs.FileSystem"] = None,
         columns: Optional[List[str]] = None,
         schema: Optional[Schema] = None,
         meta_provider: ParquetMetadataProvider = DefaultParquetMetadataProvider(),
-        _block_udf: Optional[Callable[[Block[Any]], Block[Any]]] = None,
+        _block_udf: Optional[Callable[[Block], Block]] = None,
         **reader_args: Any,
     ):
         import pyarrow as pa
         import pyarrow.parquet as pq
 
         paths, filesystem = _resolve_paths_and_filesystem(paths, filesystem)
         if len(paths) == 1:
             paths = paths[0]
 
         self._local_scheduling = None
         if local_uri:
             import ray
             from ray.util.scheduling_strategies import NodeAffinitySchedulingStrategy
 
-            self._local_scheduling = NodeAffinitySchedulingStrategy(ray.get_runtime_context().get_node_id(), soft=False)
+            self._local_scheduling = NodeAffinitySchedulingStrategy(ray.get_runtime_context().get_node_id(), soft=False)  # type: ignore[attr-defined]
 
         dataset_kwargs = reader_args.pop("dataset_kwargs", {})
         try:
             pq_ds = pq.ParquetDataset(paths, **dataset_kwargs, filesystem=filesystem, use_legacy_dataset=False)
         except OSError as e:
             _handle_read_os_error(e, paths)
         if schema is None:
@@ -357,15 +357,15 @@
         return max(ratio, PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND)  # type: ignore[no-any-return]
 
 
 # (AWS SDK for pandas) The following are the changes to the original ray implementation:
 # 1. Use _add_table_partitions to add partition columns. The behavior is controlled by Pandas SDK
 #    native `dataset` parameter. The partitions are loaded relative to the `path_root` prefix.
 def _read_pieces(
-    block_udf: Optional[Callable[[Block[Any]], Block[Any]]],
+    block_udf: Optional[Callable[[Block], Block]],
     reader_args: Any,
     columns: Optional[List[str]],
     schema: Optional[Union[type, "pyarrow.lib.Schema"]],
     serialized_pieces: List[_SerializedPiece],
 ) -> Iterator["pyarrow.Table"]:
     # Deserialize after loading the filesystem class.
     pieces: List[ParquetFileFragment] = _deserialize_pieces_with_retry(serialized_pieces)
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def _get_write_path_for_block(
         self,
         base_path: str,
         *,
         filesystem: Optional["pyarrow.fs.FileSystem"] = None,
         dataset_uuid: Optional[str] = None,
-        block: Optional[Block[Any]] = None,
+        block: Optional[Block] = None,
         block_index: Optional[int] = None,
         file_format: Optional[str] = None,
     ) -> str:
         return base_path
 
 
 @dataclass
@@ -60,15 +60,15 @@
         super().__init__()
 
         self._write_paths: List[str] = []
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def do_write(  # type: ignore[override] # pylint: disable=arguments-differ
+    def do_write(  # pylint: disable=arguments-differ
         self,
         blocks: List[ObjectRef[pd.DataFrame]],
         metadata: List[BlockMetadata],
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         try_create_dir: bool = True,
@@ -137,17 +137,17 @@
                 file_format=file_suffix,
             )
             write_task = write_block_fn(write_path, block)
             write_tasks.append(write_task)
 
         return write_tasks
 
-    def write(
+    def write(  # type: ignore[override]
         self,
-        blocks: Iterable[Union[Block[pd.DataFrame], ObjectRef[pd.DataFrame]]],
+        blocks: Iterable[Union[Block, ObjectRef[pd.DataFrame]]],
         ctx: TaskContext,
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         block_path_provider: BlockWritePathProvider = DefaultBlockWritePathProvider(),
         _block_udf: Optional[Callable[[pd.DataFrame], pd.DataFrame]] = None,
         s3_additional_kwargs: Optional[Dict[str, str]] = None,
@@ -184,38 +184,38 @@
                     compression=compression,
                     **write_args,
                 )
                 return write_path
 
         file_suffix = self._get_file_suffix(self._FILE_EXTENSION, compression)
 
-        builder = DelegatingBlockBuilder()  # type: ignore[no-untyped-call,var-annotated]
+        builder = DelegatingBlockBuilder()  # type: ignore[no-untyped-call]
         for block in blocks:
             # Dereference the block if ObjectRef is passed
             builder.add_block(ray_get(block) if isinstance(block, ray.ObjectRef) else block)  # type: ignore[arg-type]
         block = builder.build()
 
         write_path = block_path_provider(
             path,
             filesystem=filesystem,
             dataset_uuid=dataset_uuid,
-            block=block,  # type: ignore[arg-type]
+            block=block,
             block_index=ctx.task_idx,
             file_format=file_suffix,
         )
 
         return write_block(write_path, block)
 
     def _get_file_suffix(self, file_format: str, compression: Optional[str]) -> str:
         return f"{file_format}{_COMPRESSION_2_EXT.get(compression)}"
 
     def _write_block(
         self,
         f: "pyarrow.NativeFile",
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         writer_args_fn: Callable[[], Dict[str, Any]] = lambda: {},
         **writer_args: Any,
     ) -> None:
         raise NotImplementedError("Subclasses of PandasFileBasedDatasource must implement _write_block().")
 
     # Note: this callback function is called once by the main thread after
     # [all write tasks complete](https://github.com/ray-project/ray/blob/ray-2.3.0/python/ray/data/dataset.py#L2716)
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
     def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ, arguments-renamed
         self,
         f: io.TextIOWrapper,
-        block: BlockAccessor[Any],
+        block: BlockAccessor,
         pandas_kwargs: Optional[Dict[str, Any]],
         **writer_args: Any,
     ) -> None:
         write_text_func = self.write_text_func
 
         if not pandas_kwargs:
             pandas_kwargs = {}
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_utils.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     if isinstance(block, pd.DataFrame):
         return block
 
     block = BlockAccessor.for_block(block)
     return _table_to_df(table=block._table, kwargs=to_pandas_kwargs)  # pylint: disable=protected-access
 
 
-def _ray_dataset_from_df(df: Union[pd.DataFrame, modin_pd.DataFrame]) -> Dataset[Any]:
+def _ray_dataset_from_df(df: Union[pd.DataFrame, modin_pd.DataFrame]) -> Dataset:
     """Create Ray dataset from supported types of data frames."""
     if isinstance(df, modin_pd.DataFrame):
         return from_modin(df)  # type: ignore[no-any-return]
     if isinstance(df, pd.DataFrame):
         return from_pandas(df)  # type: ignore[no-any-return]
     raise ValueError(f"Unknown DataFrame type: {type(df)}")
 
 
 def _to_modin(
-    dataset: Union[ray.data.Dataset[Any], ray.data.Dataset[pd.DataFrame]],
+    dataset: Dataset,
     to_pandas_kwargs: Optional[Dict[str, Any]] = None,
     ignore_index: Optional[bool] = True,
 ) -> modin_pd.DataFrame:
     index = modin_pd.RangeIndex(start=0, stop=dataset.count()) if ignore_index else None
     _to_pandas_kwargs = {} if to_pandas_kwargs is None else to_pandas_kwargs
 
     return from_partitions(
```

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_orc.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_read_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_orc.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/s3/_list.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_orc.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_orc.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_parquet.py` & `awswrangler-3.2.1/awswrangler/distributed/ray/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/dynamodb/_delete.py` & `awswrangler-3.2.1/awswrangler/dynamodb/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/dynamodb/_read.py` & `awswrangler-3.2.1/awswrangler/dynamodb/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/dynamodb/_read.pyi` & `awswrangler-3.2.1/awswrangler/dynamodb/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/dynamodb/_utils.py` & `awswrangler-3.2.1/awswrangler/dynamodb/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/dynamodb/_write.py` & `awswrangler-3.2.1/awswrangler/dynamodb/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/emr.py` & `awswrangler-3.2.1/awswrangler/emr.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/emr_serverless.py` & `awswrangler-3.2.1/awswrangler/emr_serverless.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/exceptions.py` & `awswrangler-3.2.1/awswrangler/exceptions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/lakeformation/__init__.py` & `awswrangler-3.2.1/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/lakeformation/_read.py` & `awswrangler-3.2.1/awswrangler/lakeformation/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/lakeformation/_utils.py` & `awswrangler-3.2.1/awswrangler/lakeformation/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/mysql.py` & `awswrangler-3.2.1/awswrangler/mysql.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/__init__.py` & `awswrangler-3.2.1/awswrangler/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/_client.py` & `awswrangler-3.2.1/awswrangler/neptune/_client.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/_gremlin_init.py` & `awswrangler-3.2.1/awswrangler/neptune/_gremlin_init.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/_gremlin_parser.py` & `awswrangler-3.2.1/awswrangler/neptune/_gremlin_parser.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/_neptune.py` & `awswrangler-3.2.1/awswrangler/neptune/_neptune.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/neptune/_utils.py` & `awswrangler-3.2.1/awswrangler/neptune/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/opensearch/_read.py` & `awswrangler-3.2.1/awswrangler/opensearch/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/opensearch/_utils.py` & `awswrangler-3.2.1/awswrangler/opensearch/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/opensearch/_write.py` & `awswrangler-3.2.1/awswrangler/opensearch/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/oracle.py` & `awswrangler-3.2.1/awswrangler/oracle.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/pandas/__init__.py` & `awswrangler-3.2.1/awswrangler/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/postgresql.py` & `awswrangler-3.2.1/awswrangler/postgresql.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/__init__.py` & `awswrangler-3.2.1/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_cancel.py` & `awswrangler-3.2.1/awswrangler/quicksight/_cancel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_create.py` & `awswrangler-3.2.1/awswrangler/quicksight/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_delete.py` & `awswrangler-3.2.1/awswrangler/quicksight/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_describe.py` & `awswrangler-3.2.1/awswrangler/quicksight/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_get_list.py` & `awswrangler-3.2.1/awswrangler/quicksight/_get_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/quicksight/_utils.py` & `awswrangler-3.2.1/awswrangler/quicksight/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/redshift/_connect.py` & `awswrangler-3.2.1/awswrangler/redshift/_connect.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/redshift/_read.py` & `awswrangler-3.2.1/awswrangler/redshift/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/redshift/_read.pyi` & `awswrangler-3.2.1/awswrangler/redshift/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/redshift/_utils.py` & `awswrangler-3.2.1/awswrangler/redshift/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/redshift/_write.py` & `awswrangler-3.2.1/awswrangler/redshift/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/__init__.py` & `awswrangler-3.2.1/awswrangler/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_copy.py` & `awswrangler-3.2.1/awswrangler/s3/_copy.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_delete.py` & `awswrangler-3.2.1/awswrangler/s3/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_describe.py` & `awswrangler-3.2.1/awswrangler/s3/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_download.py` & `awswrangler-3.2.1/awswrangler/s3/_download.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_fs.py` & `awswrangler-3.2.1/awswrangler/s3/_fs.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_list.py` & `awswrangler-3.2.1/awswrangler/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_list.pyi` & `awswrangler-3.2.1/awswrangler/s3/_list.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read.py` & `awswrangler-3.2.1/awswrangler/s3/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_deltalake.py` & `awswrangler-3.2.1/awswrangler/s3/_read_deltalake.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_excel.py` & `awswrangler-3.2.1/awswrangler/s3/_read_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_orc.py` & `awswrangler-3.2.1/awswrangler/s3/_read_orc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Union,
 )
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.dataset
-import pyarrow.orc
 from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._arrow import _add_table_partitions
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
@@ -36,24 +35,27 @@
     _get_paths_for_glue_table,
     _TableMetadataReader,
 )
 from awswrangler.typing import RaySettings, _ReadTableMetadataReturnValue
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
+    from pyarrow.orc import ORCFile
 
 FULL_READ_S3_BLOCK_SIZE = 20_971_520  # 20 MB (20 * 2**20)
 METADATA_READ_S3_BLOCK_SIZE = 131_072  # 128 KB (128 * 2**10)
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _pyarrow_orc_file_wrapper(source: Any) -> pyarrow.orc.ORCFile:
+def _pyarrow_orc_file_wrapper(source: Any) -> "ORCFile":
+    from pyarrow.orc import ORCFile
+
     try:
-        return pyarrow.orc.ORCFile(source=source)
+        return ORCFile(source=source)
     except pyarrow.ArrowInvalid as ex:
         if str(ex) == "ORC file size is 0 bytes":
             _logger.warning("Ignoring empty file...")
             return None
         raise
 
 
@@ -70,15 +72,15 @@
         mode="rb",
         version_id=version_id,
         use_threads=use_threads,
         s3_client=s3_client,
         s3_block_size=METADATA_READ_S3_BLOCK_SIZE,
         s3_additional_kwargs=s3_additional_kwargs,
     ) as f:
-        orc_file: Optional[pyarrow.orc.ORCFile] = _pyarrow_orc_file_wrapper(source=f)
+        orc_file: Optional["ORCFile"] = _pyarrow_orc_file_wrapper(source=f)
         if orc_file:
             return orc_file.schema
         return None
 
 
 class _ORCTableMetadataReader(_TableMetadataReader):
     def _read_metadata_file(
@@ -114,15 +116,15 @@
         mode="rb",
         version_id=version_id,
         use_threads=use_threads,
         s3_block_size=s3_block_size,
         s3_additional_kwargs=s3_additional_kwargs,
         s3_client=s3_client,
     ) as f:
-        orc_file: Optional[pyarrow.orc.ORCFile] = _pyarrow_orc_file_wrapper(
+        orc_file: Optional["ORCFile"] = _pyarrow_orc_file_wrapper(
             source=f,
         )
         if orc_file is None:
             raise exceptions.InvalidFile(f"Invalid ORC file: {path}")
         return _add_table_partitions(
             table=orc_file.read(columns=columns),
             path=path,
```

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_parquet.py` & `awswrangler-3.2.1/awswrangler/s3/_read_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     partition_filter : Callable[[Dict[str, str]], bool], optional
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-data-wrangler.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
@@ -601,15 +601,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
```

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_parquet.pyi` & `awswrangler-3.2.1/awswrangler/s3/_read_parquet.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_text.py` & `awswrangler-3.2.1/awswrangler/s3/_read_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
         KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
@@ -389,15 +389,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
@@ -556,15 +556,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
```

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_text.pyi` & `awswrangler-3.2.1/awswrangler/s3/_read_text.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_read_text_core.py` & `awswrangler-3.2.1/awswrangler/s3/_read_text_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_select.py` & `awswrangler-3.2.1/awswrangler/s3/_select.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_upload.py` & `awswrangler-3.2.1/awswrangler/s3/_upload.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_wait.py` & `awswrangler-3.2.1/awswrangler/s3/_wait.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write.py` & `awswrangler-3.2.1/awswrangler/s3/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_concurrent.py` & `awswrangler-3.2.1/awswrangler/s3/_write_concurrent.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_dataset.py` & `awswrangler-3.2.1/awswrangler/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_deltalake.py` & `awswrangler-3.2.1/awswrangler/s3/_write_deltalake.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_excel.py` & `awswrangler-3.2.1/awswrangler/s3/_write_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_orc.py` & `awswrangler-3.2.1/awswrangler/s3/_write_orc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import math
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Literal, Optional, Union, cast
 
 import boto3
 import pandas as pd
 import pyarrow as pa
-import pyarrow.orc
 
 from awswrangler import _utils, catalog, exceptions, typing
 from awswrangler._arrow import _df_to_table
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
 from awswrangler.catalog._create import _create_orc_table
 from awswrangler.s3._fs import open_s3_object
@@ -29,14 +28,15 @@
     BucketingInfoTuple,
     GlueTableSettings,
     _S3WriteDataReturnValue,
 )
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
+    from pyarrow.orc import ORCWriter
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 _COMPRESSION_2_EXT: Dict[Optional[str], str] = {
     None: "",
     "snappy": ".snappy",
@@ -50,28 +50,30 @@
 def _new_writer(
     file_path: str,
     compression: Optional[str],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]],
     s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
-) -> Iterator[pyarrow.orc.ORCWriter]:
-    writer: Optional[pyarrow.orc.ORCWriter] = None
+) -> Iterator["ORCWriter"]:
+    from pyarrow.orc import ORCWriter
+
+    writer: Optional["ORCWriter"] = None
     if not pyarrow_additional_kwargs:
         pyarrow_additional_kwargs = {}
 
     with open_s3_object(
         path=file_path,
         mode="wb",
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         s3_client=s3_client,
     ) as f:
         try:
-            writer = pyarrow.orc.ORCWriter(
+            writer = ORCWriter(
                 where=f,
                 compression="uncompressed" if compression is None else compression,
                 **pyarrow_additional_kwargs,
             )
             yield writer
         finally:
             if writer is not None and writer.is_open is True:
```

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_parquet.py` & `awswrangler-3.2.1/awswrangler/s3/_write_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,26 +405,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode: str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/004%20-%20Parquet%20Datasets.html
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.2.0/awswrangler/s3/_write_text.py` & `awswrangler-3.2.1/awswrangler/s3/_write_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,26 +165,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
@@ -769,26 +769,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.1/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.2.0/awswrangler/secretsmanager.py` & `awswrangler-3.2.1/awswrangler/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/sqlserver.py` & `awswrangler-3.2.1/awswrangler/sqlserver.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/sts.py` & `awswrangler-3.2.1/awswrangler/sts.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/__init__.py` & `awswrangler-3.2.1/awswrangler/timestream/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_create.py` & `awswrangler-3.2.1/awswrangler/timestream/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_delete.py` & `awswrangler-3.2.1/awswrangler/timestream/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_list.py` & `awswrangler-3.2.1/awswrangler/timestream/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_read.py` & `awswrangler-3.2.1/awswrangler/timestream/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_read.pyi` & `awswrangler-3.2.1/awswrangler/timestream/_read.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/timestream/_write.py` & `awswrangler-3.2.1/awswrangler/timestream/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/awswrangler/typing.py` & `awswrangler-3.2.1/awswrangler/typing.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.2.0/pyproject.toml` & `awswrangler-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awswrangler"
-version = "3.2.0"
+version = "3.2.1"
 description = "Pandas on AWS."
 authors = ["Amazon Web Services"]
 license = "Apache License 2.0"
 
 readme = "README.md"
 
 include = ["README.md", "LICENSE.txt", "NOTICE.txt", "THIRD_PARTY.txt", "awswrangler/py.typed"]
@@ -30,15 +30,15 @@
 # Required
 boto3 = "^1.20.32"
 botocore = "^1.23.32"
 pandas = ">=1.2.0,!=1.5.0,<3.0.0" # Exclusion per: https://github.com/aws/aws-sdk-pandas/issues/1678
 numpy = "^1.18"
 pyarrow = ">=7.0.0"
 typing-extensions = "^4.4.0"
-packaging = "^23.1"
+packaging = ">=21.1,<24.0"
 
 # Databases
 redshift-connector = { version = "^2.0.0", optional = true }
 pymysql = { version = "^1.0.0", optional = true }
 pg8000 = { version = "^1.29.0", optional = true }
 pyodbc = { version = "^4.0.0", optional = true }
 oracledb = { version = "^1.0.0", optional = true }
@@ -56,15 +56,15 @@
 # Other
 openpyxl = { version = "^3.0.0", optional = true }
 progressbar2 = { version = "^4.0.0", optional = true }
 deltalake = { version = ">=0.6.4,<0.10.0", optional = true }
 
 # Distributed
 modin = { version = "^0.20.1", optional = true }
-ray = { version = ">=2.0.0,<2.5.0", extras = ["default", "data"], optional = true }
+ray = { version = ">=2.0.0,<2.6.0", extras = ["default", "data"], optional = true }
 
 [tool.poetry.extras]
 redshift = ["redshift-connector"]
 mysql = ["pymysql"]
 postgres = ["pg8000"]
 sqlserver = ["pyodbc"]
 oracle = ["oracledb"]
@@ -100,15 +100,15 @@
 pyparsing = "^3.0.7"
 pytest = "^7.1.2"
 pytest-cov = "^4.0"
 pytest-rerunfailures = "^11.1"
 pytest-timeout = "^2.1.0"
 pytest-xdist = "^3.0.2"
 s3fs = "0.4.2"  # Must be pinned to 0.4.2
-tox = "^4.6.0"
+tox = "^4.5.0"
 
 # Docs
 bump2version = "^1.0.1"
 IPython = "^8.10.0"
 jupyterlab = "^3.0"
 nbsphinx = "^0.8.8"
 nbsphinx-link = "^1.3.0"
```

### Comparing `awswrangler-3.2.0/PKG-INFO` & `awswrangler-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awswrangler
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pandas on AWS.
 Home-page: https://aws-sdk-pandas.readthedocs.io/
 License: Apache-2.0
 Keywords: pandas,aws
 Author: Amazon Web Services
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -38,22 +38,22 @@
 Requires-Dist: gremlinpython (>=3.6.2,<4.0.0) ; extra == "gremlin"
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0) ; extra == "opensearch"
 Requires-Dist: modin (>=0.20.1,<0.21.0) ; extra == "modin"
 Requires-Dist: numpy (>=1.18,<2.0)
 Requires-Dist: openpyxl (>=3.0.0,<4.0.0) ; extra == "openpyxl"
 Requires-Dist: opensearch-py (>=2.0.0,<3.0.0) ; extra == "opensearch"
 Requires-Dist: oracledb (>=1.0.0,<2.0.0) ; extra == "oracle"
-Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: packaging (>=21.1,<24.0)
 Requires-Dist: pandas (>=1.2.0,!=1.5.0,<3.0.0)
 Requires-Dist: pg8000 (>=1.29.0,<2.0.0) ; extra == "postgres"
 Requires-Dist: progressbar2 (>=4.0.0,<5.0.0) ; extra == "progressbar"
 Requires-Dist: pyarrow (>=7.0.0)
 Requires-Dist: pymysql (>=1.0.0,<2.0.0) ; extra == "mysql"
 Requires-Dist: pyodbc (>=4.0.0,<5.0.0) ; extra == "sqlserver"
-Requires-Dist: ray[data,default] (>=2.0.0,<2.5.0) ; extra == "ray"
+Requires-Dist: ray[data,default] (>=2.0.0,<2.6.0) ; extra == "ray"
 Requires-Dist: redshift-connector (>=2.0.0,<3.0.0) ; extra == "redshift"
 Requires-Dist: requests (>=2.0.0,<3.0.0) ; extra == "gremlin" or extra == "sparql" or extra == "opencypher"
 Requires-Dist: requests-aws4auth (>=1.1.1,<2.0.0) ; extra == "opensearch"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://aws-sdk-pandas.readthedocs.io/
 Project-URL: Repository, https://github.com/aws/aws-sdk-pandas
 Description-Content-Type: text/markdown
@@ -67,15 +67,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.2.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.2.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -155,33 +155,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -214,39 +214,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.1/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

