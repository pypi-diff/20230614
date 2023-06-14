# Comparing `tmp/refractio-2.0.5.tar.gz` & `tmp/refractio-2.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.tar", last modified: Wed May 31 14:07:01 2023, max compression
+gzip compressed data, was "refractio-2.0.5.1.tar", last modified: Tue Jun 13 10:21:37 2023, max compression
```

## Comparing `refractio-2.0.5.tar` & `refractio-2.0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.718990 refractio-2.0.5/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8919 2023-05-31 14:07:01.718990 refractio-2.0.5/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8224 2023-05-31 14:06:39.000000 refractio-2.0.5/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.717990 refractio-2.0.5/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      376 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4717 2023-05-30 09:31:33.000000 refractio-2.0.5/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4250 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    15148 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-30 09:31:19.000000 refractio-2.0.5/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6140 2023-05-31 13:57:21.000000 refractio-2.0.5/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-31 14:07:01.718990 refractio-2.0.5/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8919 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      390 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      526 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-31 14:07:01.000000 refractio-2.0.5/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-31 14:07:01.718990 refractio-2.0.5/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1884 2023-05-31 14:06:39.000000 refractio-2.0.5/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-13 10:21:37.559608 refractio-2.0.5.1/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8921 2023-06-13 10:21:37.558608 refractio-2.0.5.1/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8224 2023-06-13 10:20:37.000000 refractio-2.0.5.1/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-13 10:21:37.557608 refractio-2.0.5.1/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      376 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7652 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    15148 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-13 10:20:37.000000 refractio-2.0.5.1/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-13 10:21:37.558608 refractio-2.0.5.1/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8921 2023-06-13 10:21:37.000000 refractio-2.0.5.1/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      390 2023-06-13 10:21:37.000000 refractio-2.0.5.1/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-13 10:21:37.000000 refractio-2.0.5.1/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      526 2023-06-13 10:21:37.000000 refractio-2.0.5.1/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-13 10:21:37.000000 refractio-2.0.5.1/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-13 10:21:37.559608 refractio-2.0.5.1/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1886 2023-06-13 10:20:37.000000 refractio-2.0.5.1/setup.py
```

### Comparing `refractio-2.0.5/PKG-INFO` & `refractio-2.0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5
+Version: 2.0.5.1
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5/README.md` & `refractio-2.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5/refractio/amazons3.py` & `refractio-2.0.5.1/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5/refractio/azure.py` & `refractio-2.0.5.1/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5/refractio/hive.py` & `refractio-2.0.5.1/refractio/sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,92 @@
 #! -*- coding: utf-8 -*-
-"""Class to get HIVE connection object and related operations"""
+"""Class to get SFTP connection object and related operations"""
 
 import os
 import pandas as pd
 from .manager import (
     get_conn_details_from_conn_name,
     get_conn_details_from_ds_name,
     validate_project_id,
-    default_connection_name,
-    get_dataframe_query
+    default_connection_name
 )
 
 
-class Hive:
+class Sftp:
 
     def __init__(self):
         self.__connection_details = None
         self.con_obj = None
 
-    def _get_connection(self, user_id):
+    def _get_connection(self):
         try:
-            os.environ['USER'] = user_id
-            # Connect to Hive
-            from impala.dbapi import connect
-            self.con_obj = connect(
+            # Connect to SFTP
+            import pysftp
+            cnopts = pysftp.CnOpts()
+            cnopts.hostkeys = None
+            self.con_obj = pysftp.Connection(
                 # todo: To update the keys here, once we have the connection manager API created for refractio.
-                user=self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
-                password=self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword"),
-                host=self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress"),
-                auth_mechanism='PLAIN',
-                port=int(self.__connection_details["params"]["READER"]["port"]),
-                database=self.__connection_details["params"]["READER"].get("database")
+                username=self.__connection_details["params"]["READER_STORAGE"].get("user") if self.__connection_details["params"]["READER_STORAGE"].get("user") else self.__connection_details["params"]["READER_STORAGE"].get("dbUserName"),
+                password=self.__connection_details["params"]["READER_STORAGE"].get("password") if self.__connection_details["params"]["READER_STORAGE"].get("password") else self.__connection_details["params"]["READER_STORAGE"].get("dbPassword"),
+                host=self.__connection_details["params"]["READER_STORAGE"]["host"] if self.__connection_details["params"]["READER_STORAGE"].get("host") else self.__connection_details["params"]["READER_STORAGE"].get("ipAddress"),
+                cnopts=cnopts
             )
         except Exception as ex:
             print(f"Connection details fetched: {self.__connection_details}")
             print(f"Ex: {ex}")
-            raise Exception(f"Exception occurred in creating hive connection: "
+            raise Exception(f"Exception occurred in creating sftp connection: "
                             f"{self.__connection_details.get('detailMessage')}")
 
-    def get_connection(self, connection_name=None, user_id="1001"):
+    def _active_connection(self):
         try:
-            # Getting connection.
-            # connection.close() is not working in hive and there seems to be no attribute to validate whether the
-            # connection is live in hive connection object.
-            if self.con_obj is None:
+            if self.con_obj.listdir():
+                return True
+        except Exception:
+            return False
+
+    def get_connection(self, connection_name=None):
+        try:
+            # Getting connection
+            if self.con_obj is None or not self._active_connection():
                 # Getting default connection name
                 if connection_name is None:
-                    connection_name = default_connection_name("HIVE")
+                    connection_name = default_connection_name("SFTP")
                     if not connection_name:
                         raise Exception("Could not get the default connection name,"
-                                        "please create/pass an active hive connection name.")
+                                        "please create/pass an active sftp connection name.")
                 self.__connection_details = get_conn_details_from_conn_name(
-                    connection_name=connection_name, connection_type="hive")
-                self._get_connection(user_id=user_id)
+                    connection_name=connection_name, connection_type="sftp")
+                self._get_connection()
                 print(f"Connection object created: {self.con_obj}\nPlease close the connection after use!")
             else:
                 print(f"Existing connection object fetched: {self.con_obj}\nPlease close the connection after use!")
 
             return self.con_obj
         except Exception as ex:
-            print(f"Exception occurred in getting hive connection: {ex}")
+            print(f"Exception occurred in getting sftp connection: {ex}")
 
-    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), user_id="1001", row_count=-1):
+    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1):
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
-            # Creating new connection attached to dataset_id for reading the dataset.
-            self._get_connection(user_id=user_id)
 
-            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'], row_count)     # Get query to fetch details
-
-            data_frame = pd.read_sql(query, self.con_obj)   # Read data from hive
+            # Creating new connection attached to dataset_id for reading the dataset.
+            self._get_connection()
 
-            self.con_obj.close()    # Closing the connection used for reading dataset.
-            return data_frame
-        except Exception as ex:
-            print(f"Exception occurred in reading data_frame from hive connection: {ex}")
+            # Getting the file to current working directory
+            self.con_obj.get(self.__connection_details["params"]["READER_STORAGE"]["sftp_file_path"])
 
-    def execute_query(self, query, connection_name=None, user_id="1001"):
-        try:
-            # Getting connection object
-            if self.con_obj is None:
-                self.get_connection(connection_name, user_id=user_id)
+            # Extracting the file name
+            file_name = self.__connection_details["params"]["READER_STORAGE"]["sftp_file_path"].split("/")[-1]
 
-            data_frame = pd.read_sql(query, self.con_obj)   # Fetch all records in pandas dataframe
+            # Reading pandas dataframe
+            data_frame = pd.read_csv(file_name, nrows=int(row_count)) if int(row_count) > 0 else pd.read_csv(file_name)
 
-            self.con_obj.close()    # Closing the connection
+            self.con_obj.close()    # Closing the connection used for reading dataset.
             return data_frame
         except Exception as ex:
-            print(f"Exception occurred in execute_query: {ex}")
+            print(f"Exception occurred in reading data_frame from sftp connection: {ex}")
 
     def close_connection(self):
         self.con_obj.close()
-        print("hive connection closed!")
+        print("sftp connection closed!")
```

### Comparing `refractio-2.0.5/refractio/manager.py` & `refractio-2.0.5.1/refractio/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,33 +86,26 @@
                     (con["createdBy"].lower() if con["createdBy"] else None) == default_user_name.lower()]
         print(f"Connection names fetched {con_name}, created by {default_user_name}")
     else:
         print("Could not get user id from the OS env.")
     return con_name[0] if con_name else None  # first connection name from all the connections created by user_id
 
 
-def get_dataframe_query(table_name, row_count):
+def get_dataframe_query(table_name, row_count, filter_condition, top=None):
     """
     To get the query to fetch dataframe
     :param table_name:
     :param row_count:
+    :param filter_condition:
+    :param top:
     :return: query
     """
-    if int(row_count) > 0:
+    query = f"SELECT * FROM {table_name}"
+    if top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
-        return f"SELECT * FROM {table_name} LIMIT {row_count}"
-    else:
-        return f"SELECT * FROM {table_name}"
-
-
-def get_top_dataframe_query(table_name, row_count):
-    """
-    To get the sqlserver query to fetch dataframe
-    :param table_name:
-    :param row_count:
-    :return: query
-    """
-    if int(row_count) > 0:
+        query = f"SELECT TOP * FROM {table_name}"
+    if filter_condition:
+        query = query + " " + filter_condition
+    if not top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
-        return f"SELECT TOP {row_count} * FROM {table_name}"
-    else:
-        return f"SELECT * FROM {table_name}"
+        query = f"{query} LIMIT {row_count}"
+    return query
```

### Comparing `refractio-2.0.5/refractio/mysql.py` & `refractio-2.0.5.1/refractio/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,24 @@
             else:
                 print(f"Existing connection object fetched: {self.con_obj}\nPlease close the connection after use!")
 
             return self.con_obj
         except Exception as ex:
             print(f"Exception occurred in getting mysql connection: {ex}")
 
-    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1):
+    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1, filter_condition=None):
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
-            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'], row_count)     # Get query to fetch details
+            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'],
+                                        row_count, filter_condition)     # Get query to fetch details
 
             data_frame = pd.read_sql(query, con=self.con_obj)   # Read data from mysql
 
             self.con_obj.close()    # Closing the connection used for reading dataset.
             return data_frame
         except Exception as ex:
             print(f"Exception occurred in reading data_frame from mysql connection: {ex}")
```

### Comparing `refractio-2.0.5/refractio/refractio.py` & `refractio-2.0.5.1/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5/refractio/sftp.py` & `refractio-2.0.5.1/refractio/snowflake.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,110 @@
 #! -*- coding: utf-8 -*-
-"""Class to get SFTP connection object and related operations"""
+"""Class to get SNOWFLAKE connection object and related operations"""
 
 import os
-import pandas as pd
 from .manager import (
     get_conn_details_from_conn_name,
     get_conn_details_from_ds_name,
     validate_project_id,
-    default_connection_name
+    default_connection_name,
+    get_dataframe_query
 )
 
 
-class Sftp:
+class Snowflake:
 
     def __init__(self):
         self.__connection_details = None
         self.con_obj = None
 
     def _get_connection(self):
         try:
-            # Connect to SFTP
-            import pysftp
-            cnopts = pysftp.CnOpts()
-            cnopts.hostkeys = None
-            self.con_obj = pysftp.Connection(
+            # Connect to Snowflake
+            import snowflake.connector
+            self.con_obj = snowflake.connector.connect(
                 # todo: To update the keys here, once we have the connection manager API created for refractio.
-                username=self.__connection_details["params"]["READER_STORAGE"].get("user") if self.__connection_details["params"]["READER_STORAGE"].get("user") else self.__connection_details["params"]["READER_STORAGE"].get("dbUserName"),
-                password=self.__connection_details["params"]["READER_STORAGE"].get("password") if self.__connection_details["params"]["READER_STORAGE"].get("password") else self.__connection_details["params"]["READER_STORAGE"].get("dbPassword"),
-                host=self.__connection_details["params"]["READER_STORAGE"]["host"] if self.__connection_details["params"]["READER_STORAGE"].get("host") else self.__connection_details["params"]["READER_STORAGE"].get("ipAddress"),
-                cnopts=cnopts
+                user=self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
+                password=self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword"),
+                account=self.__connection_details["params"]["READER"].get("accountId") if self.__connection_details["params"]["READER"].get("accountId") else self.__connection_details["params"]["READER"].get("accountName"),
+                database=self.__connection_details["params"]["READER"].get("database"),
+                role=self.__connection_details["params"]["READER"]["role"],
+                cloudPlatform=self.__connection_details["params"]["READER"]["cloudPlatform"],
+                schema=self.__connection_details["params"]["READER"].get("schema"),
+                wareHouse=self.__connection_details["params"]["READER"]["wareHouse"],
+                region=self.__connection_details["params"]["READER"]["region"]
             )
         except Exception as ex:
             print(f"Connection details fetched: {self.__connection_details}")
             print(f"Ex: {ex}")
-            raise Exception(f"Exception occurred in creating sftp connection: "
+            raise Exception(f"Exception occurred in creating snowflake connection: "
                             f"{self.__connection_details.get('detailMessage')}")
 
-    def _active_connection(self):
-        try:
-            if self.con_obj.listdir():
-                return True
-        except Exception:
-            return False
-
     def get_connection(self, connection_name=None):
         try:
             # Getting connection
-            if self.con_obj is None or not self._active_connection():
+            if self.con_obj is None or self.con_obj.is_closed():
                 # Getting default connection name
                 if connection_name is None:
-                    connection_name = default_connection_name("SFTP")
+                    connection_name = default_connection_name("SNOWFLAKE")
                     if not connection_name:
                         raise Exception("Could not get the default connection name,"
-                                        "please create/pass an active sftp connection name.")
+                                        "please create/pass an active snowflake connection name.")
                 self.__connection_details = get_conn_details_from_conn_name(
-                    connection_name=connection_name, connection_type="sftp")
+                    connection_name=connection_name, connection_type="snowflake")
                 self._get_connection()
                 print(f"Connection object created: {self.con_obj}\nPlease close the connection after use!")
             else:
                 print(f"Existing connection object fetched: {self.con_obj}\nPlease close the connection after use!")
 
             return self.con_obj
         except Exception as ex:
-            print(f"Exception occurred in getting sftp connection: {ex}")
+            print(f"Exception occurred in getting snowflake connection: {ex}")
 
-    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1):
+    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1, filter_condition=None):
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
-
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
-            # Getting the file to current working directory
-            self.con_obj.get(self.__connection_details["params"]["READER_STORAGE"]["sftp_file_path"])
+            cur = self.con_obj.cursor()     # Creating cursor for executing query
+
+            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'],
+                                        row_count, filter_condition)     # Get query to fetch details
+
+            cur.execute(query)      # Execute query
+
+            data_frame = cur.fetch_pandas_all()     # Fetch all records in pandas dataframe
+
+            cur.close()
+            # Closing the connection used for reading dataset.
+            self.con_obj.close()
+            return data_frame
+        except Exception as ex:
+            print(f"Exception occurred in reading data_frame from snowflake connection: {ex}")
+
+    def execute_query(self, query, database=None, schema=None, connection_name=None):
+        try:
+            # Getting connection object
+            if self.con_obj is None or self.con_obj.is_closed():
+                self.get_connection(connection_name)
+
+            # Creating cursor for executing query
+            cur = self.con_obj.cursor()
+            if database and schema:
+                cur.execute(f"USE {database}.{schema}")     # To select database and schema
 
-            # Extracting the file name
-            file_name = self.__connection_details["params"]["READER_STORAGE"]["sftp_file_path"].split("/")[-1]
+            cur.execute(query)  # Execute user query
 
-            # Reading pandas dataframe
-            data_frame = pd.read_csv(file_name, nrows=int(row_count)) if int(row_count) > 0 else pd.read_csv(file_name)
+            data_frame = cur.fetch_pandas_all()     # Fetch all records in pandas dataframe
 
-            self.con_obj.close()    # Closing the connection used for reading dataset.
+            cur.close()     # Closing the cursor
+            self.con_obj.close()    # Closing the connection
             return data_frame
         except Exception as ex:
-            print(f"Exception occurred in reading data_frame from sftp connection: {ex}")
+            print(f"Exception occurred in execute_query: {ex}")
 
     def close_connection(self):
         self.con_obj.close()
-        print("sftp connection closed!")
+        print("Snowflake connection closed!")
```

### Comparing `refractio-2.0.5/refractio/snowflake.py` & `refractio-2.0.5.1/refractio/sqlserver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,114 @@
 #! -*- coding: utf-8 -*-
-"""Class to get SNOWFLAKE connection object and related operations"""
+"""
+Class to get SQLSERVER connection object and related operations.
+Requirements: This will need sqlserver driver library to work.
+To do so,
+Create a custom template with the following commands added in init_script section,
+sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
+sudo ACCEPT_EULA=Y yum install -y msodbcsql18
+"""
 
 import os
+import pandas as pd
 from .manager import (
     get_conn_details_from_conn_name,
     get_conn_details_from_ds_name,
     validate_project_id,
     default_connection_name,
     get_dataframe_query
 )
 
 
-class Snowflake:
+class Sqlserver:
 
     def __init__(self):
         self.__connection_details = None
         self.con_obj = None
 
     def _get_connection(self):
         try:
-            # Connect to Snowflake
-            import snowflake.connector
-            self.con_obj = snowflake.connector.connect(
-                # todo: To update the keys here, once we have the connection manager API created for refractio.
-                user=self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName"),
-                password=self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword"),
-                account=self.__connection_details["params"]["READER"].get("accountId") if self.__connection_details["params"]["READER"].get("accountId") else self.__connection_details["params"]["READER"].get("accountName"),
-                database=self.__connection_details["params"]["READER"].get("database"),
-                role=self.__connection_details["params"]["READER"]["role"],
-                cloudPlatform=self.__connection_details["params"]["READER"]["cloudPlatform"],
-                schema=self.__connection_details["params"]["READER"].get("schema"),
-                wareHouse=self.__connection_details["params"]["READER"]["wareHouse"],
-                region=self.__connection_details["params"]["READER"]["region"]
-            )
+            # Connect to Sqlserver
+            import pyodbc
+            # This need the OS should have sql server driver installed. Like,
+            # sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
+            # sudo ACCEPT_EULA=Y yum install -y msodbcsql18
+            driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+            # todo: To update the keys here, once we have the connection manager API created for refractio.
+            if self.__connection_details["params"]["READER"].get("database"):
+                connection_string = f'''DRIVER={driver_lib};
+                SERVER={self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress")};
+                UID={self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName")};
+                PWD={self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword")};
+                DATABASE={self.__connection_details["params"]["READER"].get("database")};
+                TrustServerCertificate=yes;'''
+            else:
+                connection_string = f'''DRIVER={driver_lib};
+                SERVER={self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress")};
+                UID={self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName")};
+                PWD={self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword")};
+                TrustServerCertificate=yes;'''
+            self.con_obj = pyodbc.connect(connection_string)
         except Exception as ex:
             print(f"Connection details fetched: {self.__connection_details}")
             print(f"Ex: {ex}")
-            raise Exception(f"Exception occurred in creating snowflake connection: "
+            raise Exception(f"Exception occurred in creating sql server connection: "
                             f"{self.__connection_details.get('detailMessage')}")
 
     def get_connection(self, connection_name=None):
         try:
             # Getting connection
-            if self.con_obj is None or self.con_obj.is_closed():
+            if self.con_obj is None or self.con_obj.closed:
                 # Getting default connection name
                 if connection_name is None:
-                    connection_name = default_connection_name("SNOWFLAKE")
+                    connection_name = default_connection_name("SQLSERVER")
                     if not connection_name:
                         raise Exception("Could not get the default connection name,"
-                                        "please create/pass an active snowflake connection name.")
+                                        "please create/pass an active sqlserver connection name.")
                 self.__connection_details = get_conn_details_from_conn_name(
-                    connection_name=connection_name, connection_type="snowflake")
+                    connection_name=connection_name, connection_type="sqlserver")
                 self._get_connection()
                 print(f"Connection object created: {self.con_obj}\nPlease close the connection after use!")
             else:
                 print(f"Existing connection object fetched: {self.con_obj}\nPlease close the connection after use!")
 
             return self.con_obj
         except Exception as ex:
-            print(f"Exception occurred in getting snowflake connection: {ex}")
+            print(f"Exception occurred in getting sqlserver connection: {ex}")
 
-    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1):
+    def get_dataframe(self, dataset_name, project_id=os.getenv("project_id"), row_count=-1, filter_condition=None):
         try:
             project_id = validate_project_id(project_id)
 
             self.__connection_details = get_conn_details_from_ds_name(dataset_name=dataset_name, project_id=project_id)
             # Creating new connection attached to dataset_id for reading the dataset.
             self._get_connection()
 
-            cur = self.con_obj.cursor()     # Creating cursor for executing query
-
-            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'], row_count)     # Get query to fetch details
+            query = get_dataframe_query(self.__connection_details['params']['READER']['tables'],
+                                        row_count, filter_condition, top=True)     # Get query to fetch details
 
-            cur.execute(query)      # Execute query
+            data_frame = pd.read_sql(query, con=self.con_obj)   # Read data from sqlserver
 
-            data_frame = cur.fetch_pandas_all()     # Fetch all records in pandas dataframe
-
-            cur.close()
-            # Closing the connection used for reading dataset.
-            self.con_obj.close()
+            self.con_obj.close()    # Closing the connection used for reading dataset.
             return data_frame
         except Exception as ex:
-            print(f"Exception occurred in reading data_frame from snowflake connection: {ex}")
+            print(f"Exception occurred in reading data_frame from sqlserver connection: {ex}")
 
-    def execute_query(self, query, database=None, schema=None, connection_name=None):
+    def execute_query(self, query, database, connection_name=None):
         try:
             # Getting connection object
-            if self.con_obj is None or self.con_obj.is_closed():
+            if self.con_obj is None or self.con_obj.closed:
                 self.get_connection(connection_name)
 
-            # Creating cursor for executing query
-            cur = self.con_obj.cursor()
-            if database and schema:
-                cur.execute(f"USE {database}.{schema}")     # To select database and schema
-
-            cur.execute(query)  # Execute user query
+            if database:
+                self.con_obj.execute(f"USE {database}")      # To select database
 
-            data_frame = cur.fetch_pandas_all()     # Fetch all records in pandas dataframe
+            data_frame = pd.read_sql(query, con=self.con_obj)   # Fetch all records in pandas dataframe
 
-            cur.close()     # Closing the cursor
             self.con_obj.close()    # Closing the connection
             return data_frame
         except Exception as ex:
             print(f"Exception occurred in execute_query: {ex}")
 
     def close_connection(self):
         self.con_obj.close()
-        print("Snowflake connection closed!")
+        print("sqlserver connection closed!")
```

### Comparing `refractio-2.0.5/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.1/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5
+Version: 2.0.5.1
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5/refractio.egg-info/requires.txt` & `refractio-2.0.5.1/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5/setup.py` & `refractio-2.0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5'
+VERSION = '2.0.5.1'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

