# Comparing `tmp/litesqlite-2.6.9.tar.gz` & `tmp/litesqlite-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.9.tar", last modified: Wed Jun 14 15:18:46 2023, max compression
+gzip compressed data, was "litesqlite-2.7.tar", last modified: Wed Jun 14 17:30:07 2023, max compression
```

## Comparing `litesqlite-2.6.9.tar` & `litesqlite-2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.515923 litesqlite-2.6.9/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.9/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:18:46.511923 litesqlite-2.6.9/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3248 2023-06-13 17:37:30.000000 litesqlite-2.6.9/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.511923 litesqlite-2.6.9/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.9/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.9/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8544 2023-06-14 15:18:42.000000 litesqlite-2.6.9/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.511923 litesqlite-2.6.9/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 15:18:46.515923 litesqlite-2.6.9/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 15:18:42.000000 litesqlite-2.6.9/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.731193 litesqlite-2.7/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.7/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      626 2023-06-14 17:30:07.731193 litesqlite-2.7/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1735 2023-06-14 17:26:48.000000 litesqlite-2.7/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.727193 litesqlite-2.7/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.7/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.7/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8905 2023-06-14 17:06:04.000000 litesqlite-2.7/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.731193 litesqlite-2.7/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      626 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 17:30:07.731193 litesqlite-2.7/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 17:29:45.000000 litesqlite-2.7/setup.py
```

### Comparing `litesqlite-2.6.9/LICENSE` & `litesqlite-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.9/PKG-INFO` & `litesqlite-2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.9
+Version: 2.7
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.9/litesqlite/datatypes.py` & `litesqlite-2.7/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.9/litesqlite/lite_sqlite.py` & `litesqlite-2.7/litesqlite/lite_sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiosqlite
 import sqlite3
-from typing import Dict, Union, Tuple, List
+from typing import Dict, Union, Tuple, List, Optional
 from .datatypes import DataTypes
 
 
 class Sqlite:
 
     def __init__(self,
                  db_name: str) -> None:
@@ -37,47 +37,52 @@
         query = f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], str] = '*',
-                    where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
-                    limit: Union[int, None] = None,
-                    offset: Union[int, None] = None,
+                    where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
+                    order_by: Optional[str] = None,
+                    limit: Optional[int] = None,
+                    offset: Optional[int] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns != '*':
             columns = ', '.join(columns)
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
+        if order_by:
+            order_by_clause = f"ORDER BY {order_by}"
+        else:
+            order_by_clause = ''
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
-        query = f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}"
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause} {offset_clause}"
         self.__cursor.execute(query, values)
         if fetch == DataTypes.Fetch.FETCHONE:
             result = self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = self.__cursor.fetchall()
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
-                    where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
-                    sign: Union[str, None] = None) -> None:
+                    where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
+                    sign: Optional[str] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
@@ -86,15 +91,15 @@
             values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
-                    where: Union[Dict[str, Union[str, int, float]], None] = None) -> None:
+                    where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if where:
             where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
             values = tuple(where.values())
         else:
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
@@ -141,48 +146,52 @@
         query = f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], str] = '*',
-                          where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
-                          limit: Union[int, None] = None,
-                          offset: Union[int, None] = None,
+                          where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
+                          order_by: Optional[str] = None,
+                          limit: Optional[int] = None,
+                          offset: Optional[int] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns != '*':
             columns = ', '.join(columns)
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
+        if order_by:
+            order_by_clause = f"ORDER BY {order_by}"
+        else:
+            order_by_clause = ''
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
-        query = f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}"
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause} {offset_clause}"
         await self.__cursor.execute(query, values)
-
         if fetch == DataTypes.Fetch.FETCHONE:
             result = await self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
         return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
-                          where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
-                          sign: Union[str, None] = None) -> None:
+                          where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
+                          sign: Optional[str] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
@@ -191,15 +200,15 @@
             values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
-                          where: Union[Dict[str, Union[str, int, float]], None] = None) -> None:
+                          where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if where:
             where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
             values = tuple(where.values())
         else:
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
```

### Comparing `litesqlite-2.6.9/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.7/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.9
+Version: 2.7
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.9/setup.py` & `litesqlite-2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.9',
+    version='2.7',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
@@ -18,8 +18,8 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ]
-)
+)
```

