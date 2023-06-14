# Comparing `tmp/sparksnake-0.1.8.tar.gz` & `tmp/sparksnake-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparksnake-0.1.8.tar", last modified: Fri Mar 24 00:05:20 2023, max compression
+gzip compressed data, was "sparksnake-0.1.9.tar", last modified: Mon Mar 27 02:19:15 2023, max compression
```

## Comparing `sparksnake-0.1.8.tar` & `sparksnake-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:20.200172 sparksnake-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-24 00:05:08.000000 sparksnake-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-03-24 00:05:20.200172 sparksnake-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-24 00:05:08.000000 sparksnake-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 00:05:20.200172 sparksnake-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-24 00:05:09.000000 sparksnake-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:20.200172 sparksnake-0.1.8/sparksnake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:09.000000 sparksnake-0.1.8/sparksnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25985 2023-03-24 00:05:09.000000 sparksnake-0.1.8/sparksnake/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26047 2023-03-24 00:05:09.000000 sparksnake-0.1.8/sparksnake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:20.200172 sparksnake-0.1.8/sparksnake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:09.000000 sparksnake-0.1.8/sparksnake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-24 00:05:09.000000 sparksnake-0.1.8/sparksnake/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:20.200172 sparksnake-0.1.8/sparksnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 00:05:20.000000 sparksnake-0.1.8/sparksnake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:20.200172 sparksnake-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 00:05:09.000000 sparksnake-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-24 00:05:09.000000 sparksnake-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-24 00:05:09.000000 sparksnake-0.1.8/tests/test_01_job_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.406170 sparksnake-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-27 02:19:03.000000 sparksnake-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-27 02:19:15.402170 sparksnake-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-27 02:19:03.000000 sparksnake-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 02:19:15.406170 sparksnake-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-27 02:19:03.000000 sparksnake-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.398170 sparksnake-0.1.9/sparksnake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25976 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/sparksnake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-27 02:19:03.000000 sparksnake-0.1.9/sparksnake/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/sparksnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 02:19:15.000000 sparksnake-0.1.9/sparksnake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:15.402170 sparksnake-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/test_glue_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-03-27 02:19:03.000000 sparksnake-0.1.9/tests/test_manager_module.py
```

### Comparing `sparksnake-0.1.8/LICENSE` & `sparksnake-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksnake-0.1.8/PKG-INFO` & `sparksnake-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.1.8
+Version: 0.1.9
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
   ![PyPI - Downloads](https://img.shields.io/pypi/dm/sparksnake?color=purple)
   ![PyPI - Status](https://img.shields.io/pypi/status/sparksnake?color=purple)
   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ThiagoPanini/sparksnake?color=purple)
   ![GitHub Last Commit](https://img.shields.io/github/last-commit/ThiagoPanini/sparksnake?color=purple)
   <br>
 
   ![CI workflow](https://img.shields.io/github/actions/workflow/status/ThiagoPanini/sparksnake/ci-main.yml?label=ci)
-  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/pt/latest/?badge=latest)
+  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/en/latest/?badge=latest)
   [![codecov](https://codecov.io/gh/ThiagoPanini/sparksnake/branch/main/graph/badge.svg?token=zSdFO9jkD8)](https://codecov.io/gh/ThiagoPanini/sparksnake)
 
 </div>
 
 ## Table of content
 
 - [Table of content](#table-of-content)
@@ -54,24 +54,24 @@
 ## What is the sparksnake library?
 
 The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications along all the particularities found in AWS services, such as Glue and EMR, for example.
 
 Do you want to take your job Glue or your EMR cluster to the next level? Take a look at *sparksnake*!
 
 > **Note**
->  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/pt/latest/) and check out usability technical details, practical examples and more!
+>  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, practical examples and more!
 
 
 ## Features
 
-- 🤖 Simplification of building Spark applications with already coded classes and methods
-- 🌟 Consolidation of most common functionalities involving ETL processes in pyspark
-- ⚙️ Abstraction of the whole process of setting up a Job Glue with one line of code
+- 🤖 Enhanced development experience of Spark Applications to be deployed as jobs in AWS services like Glue and EMR
+- 🌟 Possibility to use common Spark operations for improving ETL steps using custom classes and methods
+- ⚙️ No need to think too much into the hard and complex service setup (e.g. with *sparksnake* you can have all elements for a Glue Job on AWS with a single line of code)
 - 👁️‍🗨️ Application observability improvement with detailed log messages in CloudWatch
-- 🛠️ Exception handling processes already embedded in library methods
+- 🛠️ Exception handling already embedded in library methods
 
 ___
 
 ## Contacts
 
 - [Thiago Panini - LinkedIn](https://www.linkedin.com/in/thiago-panini/)
 - [paninitechlab @ hashnode](https://panini.hashnode.dev/)
```

### Comparing `sparksnake-0.1.8/README.md` & `sparksnake-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   ![PyPI - Downloads](https://img.shields.io/pypi/dm/sparksnake?color=purple)
   ![PyPI - Status](https://img.shields.io/pypi/status/sparksnake?color=purple)
   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ThiagoPanini/sparksnake?color=purple)
   ![GitHub Last Commit](https://img.shields.io/github/last-commit/ThiagoPanini/sparksnake?color=purple)
   <br>
 
   ![CI workflow](https://img.shields.io/github/actions/workflow/status/ThiagoPanini/sparksnake/ci-main.yml?label=ci)
-  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/pt/latest/?badge=latest)
+  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/en/latest/?badge=latest)
   [![codecov](https://codecov.io/gh/ThiagoPanini/sparksnake/branch/main/graph/badge.svg?token=zSdFO9jkD8)](https://codecov.io/gh/ThiagoPanini/sparksnake)
 
 </div>
 
 ## Table of content
 
 - [Table of content](#table-of-content)
@@ -30,24 +30,24 @@
 ## What is the sparksnake library?
 
 The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications along all the particularities found in AWS services, such as Glue and EMR, for example.
 
 Do you want to take your job Glue or your EMR cluster to the next level? Take a look at *sparksnake*!
 
 > **Note**
->  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/pt/latest/) and check out usability technical details, practical examples and more!
+>  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, practical examples and more!
 
 
 ## Features
 
-- 🤖 Simplification of building Spark applications with already coded classes and methods
-- 🌟 Consolidation of most common functionalities involving ETL processes in pyspark
-- ⚙️ Abstraction of the whole process of setting up a Job Glue with one line of code
+- 🤖 Enhanced development experience of Spark Applications to be deployed as jobs in AWS services like Glue and EMR
+- 🌟 Possibility to use common Spark operations for improving ETL steps using custom classes and methods
+- ⚙️ No need to think too much into the hard and complex service setup (e.g. with *sparksnake* you can have all elements for a Glue Job on AWS with a single line of code)
 - 👁️‍🗨️ Application observability improvement with detailed log messages in CloudWatch
-- 🛠️ Exception handling processes already embedded in library methods
+- 🛠️ Exception handling already embedded in library methods
 
 ___
 
 ## Contacts
 
 - [Thiago Panini - LinkedIn](https://www.linkedin.com/in/thiago-panini/)
 - [paninitechlab @ hashnode](https://panini.hashnode.dev/)
```

### Comparing `sparksnake-0.1.8/setup.py` & `sparksnake-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Reading README.md for project description
 with open("README.md", "r", encoding='utf-8') as f:
     __long_description__ = f.read()
 
 # Setting up package information
 setup(
     name='sparksnake',
-    version='0.1.8',
+    version='0.1.9',
     author='Thiago Panini',
     author_email='panini.development@gmail.com',
     packages=find_packages(),
     install_requires=[
         "pyspark"
     ],
     license='MIT',
```

### Comparing `sparksnake-0.1.8/sparksnake/glue.py` & `sparksnake-0.1.9/sparksnake/glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             }
             ```
 
             where the tags <DynamicFrame> means objects of DynamicFrame type
             read for each data source.
         """
 
-        logger.info("Looping for the data_dict dictionary for reading data "
+        logger.info("Iterating over data_dict dictionary for reading data "
                     "sources as Glue DynamicFrame objects")
         try:
             dynamic_frames = []
             for t in self.data_dict.keys():
                 # Getting some required args: database, table_name, ctx
                 database = self.data_dict[t]["database"]
                 table_name = self.data_dict[t]["table_name"]
@@ -310,16 +310,16 @@
 
         logger.info("Mapping DynamicFrames objects to a dictionary key")
         sleep(0.01)
 
         # Creating a DynamicFrames dictionary
         dynamic_dict = {k: dyf for k, dyf
                         in zip(self.data_dict.keys(), dynamic_frames)}
-        logger.info("Success on creating data. There are a number of "
-                    f"{len(dynamic_dict.values())} DynamicFrames read.")
+        logger.info("Success on reading data. There are "
+                    f"{len(dynamic_dict.values())} DynamicFrames available.")
 
         # Returning the dictionary
         sleep(0.01)
         return dynamic_dict
 
     def generate_dataframes_dict(self) -> dict:
         """Getting a dictionary of DataFrames objects read from the catalog.
```

### Comparing `sparksnake-0.1.8/sparksnake/manager.py` & `sparksnake-0.1.9/sparksnake/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Managing Spark operations in AWS services that uses it in ETL jobs.
 
-This module aims to provide a central point for users to have a series of
-useful features for developing their own Spark applications in AWS in services
-like Glue and EMR.
+This module provides Spark features do be applied in Spark applications to
+be deployed locally or using AWS services like Glue and EMR.
 
 ___
 """
 
 # Importing libraries
 from time import sleep
 
@@ -176,30 +175,31 @@
 
         # Looking out for local mode
         elif self.mode == "local":
             # Checking if user wants to pass its own SparkSession object
             if "spark" in kwargs and type(kwargs["spark"]) is SparkSession:
                 self.spark = kwargs["spark"]
             else:
-                # Creating a SparkSession object
+                logger.info("Creating a SparkSession object to be used in a "
+                            "local environment")
                 self.spark = SparkSession.builder\
                     .appName("sparksnake-app")\
                     .getOrCreate()
 
             # Logging initialization message
             logger.info("The class was succesfully initialized with 'local' "
                         "operation mode")
 
     @staticmethod
-    def extract_date_attributes(df: DataFrame,
-                                date_col: str,
-                                date_col_type: str = "date",
-                                date_format: str = "yyyy-MM-dd",
-                                convert_string_to_date: bool = True,
-                                **kwargs) -> DataFrame:
+    def date_transform(df: DataFrame,
+                       date_col: str,
+                       date_col_type: str = "date",
+                       date_format: str = "yyyy-MM-dd",
+                       convert_string_to_date: bool = True,
+                       **kwargs) -> DataFrame:
         """Extracting date attributes from a Spark DataFrame date column.
 
         This method makes it possible to extract multiple date attributes from
         a column in a Spark DataFrame that represents a date or timestamp
         information. To do that, the given date column in the DataFrame should
         be of types DATE, TIMESTAMP. There is a special case where the target
         date column is of STRING data type. In that situtation, the column
@@ -311,21 +311,22 @@
             return df
 
         except Exception as e:
             logger.error("Error on adding new date columns into the "
                          f"DataFrame. Exception: {e}")
             raise e
 
-    def extract_aggregate_statistics(self,
-                                     df: DataFrame,
-                                     numeric_col: str,
-                                     group_by: str or list,
-                                     round_result: bool = False,
-                                     n_round: int = 2,
-                                     **kwargs) -> DataFrame:
+    @staticmethod
+    def aggregate_data(df: DataFrame,
+                       spark_session: SparkSession,
+                       numeric_col: str,
+                       group_by: str or list,
+                       round_result: bool = False,
+                       n_round: int = 2,
+                       **kwargs) -> DataFrame:
         """Extracts statistical attributes based on a group by opreation.
 
         This method makes it possible to extract multiple statistical
         aggregations based in a numerical column and a set of columns to be
         grouped by. With this feature, users can configure complex aggregations
         in a single method call in order to enhance their analysis.
 
@@ -438,15 +439,15 @@
                     {group_by},
                     {agg_query}
                 FROM tmp_extract_aggregate_statistics
                 GROUP BY
                     {group_by}
             """
 
-            return self.spark.sql(final_query)
+            return spark_session.sql(final_query)
 
         except Exception as e:
             logger.error("Error on extracting statistical attributes from "
                          f"DataFrame. Exception: {e}")
             raise e
 
     @staticmethod
```

### Comparing `sparksnake-0.1.8/sparksnake/utils/log.py` & `sparksnake-0.1.9/sparksnake/utils/log.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.1.8/sparksnake.egg-info/PKG-INFO` & `sparksnake-0.1.9/sparksnake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.1.8
+Version: 0.1.9
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
   ![PyPI - Downloads](https://img.shields.io/pypi/dm/sparksnake?color=purple)
   ![PyPI - Status](https://img.shields.io/pypi/status/sparksnake?color=purple)
   ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ThiagoPanini/sparksnake?color=purple)
   ![GitHub Last Commit](https://img.shields.io/github/last-commit/ThiagoPanini/sparksnake?color=purple)
   <br>
 
   ![CI workflow](https://img.shields.io/github/actions/workflow/status/ThiagoPanini/sparksnake/ci-main.yml?label=ci)
-  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/pt/latest/?badge=latest)
+  [![Documentation Status](https://readthedocs.org/projects/sparksnake/badge/?version=latest)](https://sparksnake.readthedocs.io/en/latest/?badge=latest)
   [![codecov](https://codecov.io/gh/ThiagoPanini/sparksnake/branch/main/graph/badge.svg?token=zSdFO9jkD8)](https://codecov.io/gh/ThiagoPanini/sparksnake)
 
 </div>
 
 ## Table of content
 
 - [Table of content](#table-of-content)
@@ -54,24 +54,24 @@
 ## What is the sparksnake library?
 
 The *sparksnake* library provides an easy, fast, and efficient way to use Spark features inside analytics services on AWS. With *sparksnake*, it is possible to use classes, methods and functions developed in pyspark to simplify, as much as possible, the journey of building Spark applications along all the particularities found in AWS services, such as Glue and EMR, for example.
 
 Do you want to take your job Glue or your EMR cluster to the next level? Take a look at *sparksnake*!
 
 > **Note**
->  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/pt/latest/) and check out usability technical details, practical examples and more!
+>  Now the *sparksnake* library has an official documentation in readthedocs! Visit the [following link](https://sparksnake.readthedocs.io/en/latest/) and check out usability technical details, practical examples and more!
 
 
 ## Features
 
-- 🤖 Simplification of building Spark applications with already coded classes and methods
-- 🌟 Consolidation of most common functionalities involving ETL processes in pyspark
-- ⚙️ Abstraction of the whole process of setting up a Job Glue with one line of code
+- 🤖 Enhanced development experience of Spark Applications to be deployed as jobs in AWS services like Glue and EMR
+- 🌟 Possibility to use common Spark operations for improving ETL steps using custom classes and methods
+- ⚙️ No need to think too much into the hard and complex service setup (e.g. with *sparksnake* you can have all elements for a Glue Job on AWS with a single line of code)
 - 👁️‍🗨️ Application observability improvement with detailed log messages in CloudWatch
-- 🛠️ Exception handling processes already embedded in library methods
+- 🛠️ Exception handling already embedded in library methods
 
 ___
 
 ## Contacts
 
 - [Thiago Panini - LinkedIn](https://www.linkedin.com/in/thiago-panini/)
 - [paninitechlab @ hashnode](https://panini.hashnode.dev/)
```

### Comparing `sparksnake-0.1.8/tests/conftest.py` & `sparksnake-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.1.8/tests/test_01_job_manager.py` & `sparksnake-0.1.9/tests/test_glue_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Test cases for GlueJobManager class features.
 
-This file will handle all test cases for testing GlueJobManager class and its
-features.
+This file handles the definition of all test cases for testing GlueJobManager
+class and its features. The idea is to isolate a test script for testing
+sparksnake features delivered for users who want to develop Spark applications
+using AWS Glue service.
 
 ___
 """
 
 # Importing libraries
 import pytest
 import logging
```

