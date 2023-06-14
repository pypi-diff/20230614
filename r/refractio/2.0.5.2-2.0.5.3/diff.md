# Comparing `tmp/refractio-2.0.5.2.tar.gz` & `tmp/refractio-2.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.2.tar", last modified: Wed Jun 14 13:26:37 2023, max compression
+gzip compressed data, was "refractio-2.0.5.3.tar", last modified: Wed Jun 14 14:54:24 2023, max compression
```

## Comparing `refractio-2.0.5.2.tar` & `refractio-2.0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 13:26:37.843605 refractio-2.0.5.2/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9982 2023-06-14 13:26:37.843605 refractio-2.0.5.2/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9260 2023-06-14 13:25:53.000000 refractio-2.0.5.2/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 13:26:37.842605 refractio-2.0.5.2/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-14 13:25:53.000000 refractio-2.0.5.2/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4555 2023-06-14 13:25:53.000000 refractio-2.0.5.2/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16530 2023-06-14 13:25:53.000000 refractio-2.0.5.2/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.2/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 13:26:37.843605 refractio-2.0.5.2/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9982 2023-06-14 13:26:37.000000 refractio-2.0.5.2/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-14 13:26:37.000000 refractio-2.0.5.2/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-14 13:26:37.000000 refractio-2.0.5.2/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-14 13:26:37.000000 refractio-2.0.5.2/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-14 13:26:37.000000 refractio-2.0.5.2/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-14 13:26:37.843605 refractio-2.0.5.2/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-14 13:25:53.000000 refractio-2.0.5.2/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 14:54:24.442780 refractio-2.0.5.3/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-14 14:54:24.441780 refractio-2.0.5.3/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-14 14:53:40.000000 refractio-2.0.5.3/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 14:54:24.440780 refractio-2.0.5.3/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-14 13:25:53.000000 refractio-2.0.5.3/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4797 2023-06-14 14:53:40.000000 refractio-2.0.5.3/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16530 2023-06-14 13:25:53.000000 refractio-2.0.5.3/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.3/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-14 14:54:24.441780 refractio-2.0.5.3/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-14 14:54:24.000000 refractio-2.0.5.3/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-14 14:54:24.000000 refractio-2.0.5.3/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-14 14:54:24.000000 refractio-2.0.5.3/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-14 14:54:24.000000 refractio-2.0.5.3/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-14 14:54:24.000000 refractio-2.0.5.3/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-14 14:54:24.442780 refractio-2.0.5.3/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-14 14:53:40.000000 refractio-2.0.5.3/setup.py
```

### Comparing `refractio-2.0.5.2/PKG-INFO` & `refractio-2.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.2
+Version: 2.0.5.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -61,14 +61,19 @@
 pip install refractio[hive]
 ```
 ## With sqlserver:
 ```commandline
 pip install refractio[sqlserver]
 ```
 
+## With postgres:
+```commandline
+pip install refractio[postgres]
+```
+
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
```

### Comparing `refractio-2.0.5.2/README.md` & `refractio-2.0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 pip install refractio[hive]
 ```
 ## With sqlserver:
 ```commandline
 pip install refractio[sqlserver]
 ```
 
+## With postgres:
+```commandline
+pip install refractio[postgres]
+```
+
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
```

### Comparing `refractio-2.0.5.2/refractio/amazons3.py` & `refractio-2.0.5.3/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/azure.py` & `refractio-2.0.5.3/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/hive.py` & `refractio-2.0.5.3/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/manager.py` & `refractio-2.0.5.3/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/mysql.py` & `refractio-2.0.5.3/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/postgres.py` & `refractio-2.0.5.3/refractio/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             import psycopg2
             self.con_obj = psycopg2.connect(
                 # todo: To update the keys here, once we have the connection manager API created for refractio.
                 user=self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
                 password=self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword"),
                 host=self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress"),
                 port=int(self.__connection_details["params"]["READER"]["port"]),
-                database=self.__connection_details["params"]["READER"].get("database")
+                database=self.__connection_details["params"]["READER"].get("database") if self.__connection_details["params"]["READER"].get("database") else self.__connection_details["params"]["READER"].get("defaultDb")
             )
         except Exception as ex:
             print(f"Connection details fetched: {self.__connection_details}")
             print(f"Ex: {ex}")
             raise Exception(f"Exception occurred in creating postgres connection: "
                             f"{self.__connection_details.get('detailMessage')}")
 
@@ -61,15 +61,16 @@
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
-            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'],
+            query = get_dataframe_query(f"{self.__connection_details['params']['READER']['database']}."
+                                        f"{self.__connection_details['params']['READER']['tables']}",
                                         row_count, filter_condition)     # Get query to fetch details
 
             data_frame = sqlio.read_sql_query(query, con=self.con_obj)   # Read data from postgres
 
             self.con_obj.close()    # Closing the connection used for reading dataset.
             return data_frame
         except Exception as ex:
```

### Comparing `refractio-2.0.5.2/refractio/refractio.py` & `refractio-2.0.5.3/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/sftp.py` & `refractio-2.0.5.3/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/snowflake.py` & `refractio-2.0.5.3/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio/sqlserver.py` & `refractio-2.0.5.3/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.3/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.2
+Version: 2.0.5.3
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -61,14 +61,19 @@
 pip install refractio[hive]
 ```
 ## With sqlserver:
 ```commandline
 pip install refractio[sqlserver]
 ```
 
+## With postgres:
+```commandline
+pip install refractio[postgres]
+```
+
 #### Source code is available at: https://git.lti-aiq.in/refract-sdk/refract-sdk.git 
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
```

### Comparing `refractio-2.0.5.2/refractio.egg-info/requires.txt` & `refractio-2.0.5.3/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.2/setup.py` & `refractio-2.0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.2'
+VERSION = '2.0.5.3'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

