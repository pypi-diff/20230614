# Comparing `tmp/litesqlite-2.6.7.tar.gz` & `tmp/litesqlite-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.7.tar", last modified: Tue Jun 13 17:29:24 2023, max compression
+gzip compressed data, was "litesqlite-2.6.8.tar", last modified: Wed Jun 14 15:08:40 2023, max compression
```

## Comparing `litesqlite-2.6.7.tar` & `litesqlite-2.6.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.802501 litesqlite-2.6.7/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.7/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:29:24.802501 litesqlite-2.6.7/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3242 2023-06-13 17:29:21.000000 litesqlite-2.6.7/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.798501 litesqlite-2.6.7/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.7/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.7/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7645 2023-06-13 17:18:30.000000 litesqlite-2.6.7/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.802501 litesqlite-2.6.7/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-13 17:29:24.802501 litesqlite-2.6.7/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-13 17:24:45.000000 litesqlite-2.6.7/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.962481 litesqlite-2.6.8/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.8/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:08:40.962481 litesqlite-2.6.8/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3248 2023-06-13 17:37:30.000000 litesqlite-2.6.8/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.958481 litesqlite-2.6.8/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.8/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.8/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8472 2023-06-14 15:06:12.000000 litesqlite-2.6.8/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.962481 litesqlite-2.6.8/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 15:08:40.962481 litesqlite-2.6.8/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 13:45:59.000000 litesqlite-2.6.8/setup.py
```

### Comparing `litesqlite-2.6.7/LICENSE` & `litesqlite-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.7/PKG-INFO` & `litesqlite-2.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.7
+Version: 2.6.8
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.7/README.md` & `litesqlite-2.6.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```python
 
 from litesqlite import Sqlite, DataTypes
 
   
 # Используем контекстный менеджер для правильного открытия и закрытия соединения, передаём в класс имя бд
-with Sqlite('database.db'):
+with Sqlite('database.db') as db:
     
     # Создаём таблицу users с столбцами id, name, age и sex
     
     # В качестве альтернативы DataTypes вы можете просто передать тип текстом
     
     db.create_table('users', {'id': DataTypes.INTEGER(autoincrement=True, primary_key=True), 'name': DataTypes.TEXT(not_null=True), 'age': DataTypes.INTEGER(), 'sex': DataTypes.TEXT(default='М')})
```

### Comparing `litesqlite-2.6.7/litesqlite/datatypes.py` & `litesqlite-2.6.8/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.7/litesqlite/lite_sqlite.py` & `litesqlite-2.6.8/litesqlite/lite_sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,177 +8,206 @@
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    def __enter__(self) -> 'Sqlite':
+    def open_conn(self) -> None:
         self.__conn = sqlite3.connect(self.__db_name)
         self.__cursor = self.__conn.cursor()
+
+    def __enter__(self) -> 'Sqlite':
+        self.open_conn()
         return self
 
     def create_table(self,
                      table_name: str,
                      columns: Dict[str, Union[DataTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-        self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+        query = f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})"
+        self.__cursor.execute(query)
         self.__conn.commit()
 
     def insert_data(self,
                     table_name: str,
                     data: Dict[str, Union[str, int, float]]) -> None:
         columns = ', '.join(data.keys())
         placeholders = ', '.join(['?' for _ in range(len(data))])
         values = tuple(data.values())
-        self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+        query = f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})"
+        self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
-                    columns: Union[List[str], str, None] = None,
-                    where: Union[str, Dict[str, Union[str, int, float]], None] = None,
+                    columns: Union[List[str], str] = '*',
+                    where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
                     limit: Union[int, None] = None,
                     offset: Union[int, None] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
-        if columns:
+        if columns != '*':
             columns = ', '.join(columns)
-        else:
-            columns = '*'
         if where:
-            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
+            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
-        self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                              values)
-
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}"
+        self.__cursor.execute(query, values)
         if fetch == DataTypes.Fetch.FETCHONE:
             result = self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = self.__cursor.fetchall()
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
-                    where: Dict[str, Union[str, int, float]],
+                    where: Union[Dict[str, Union[str, int, float]], None] = None,
                     sign: Union[str, None] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(set_data.values()) + tuple(where.values())
-        self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+        if where:
+            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(set_data.values()) + tuple(where.values())
+        else:
+            where_clause = ''
+            values = tuple(set_data.values())
+        query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
+        self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
-                    where: Dict[str, Union[str, int, float]]) -> None:
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(where.values())
-        self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+                    where: Union[Dict[str, Union[str, int, float]], None] = None) -> None:
+        if where:
+            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+        else:
+            where_clause = ''
+            values = ()
+        query = f"DELETE FROM {table_name} {where_clause}"
+        self.__cursor.execute(query, values)
         self.__conn.commit()
 
+    def close_conn(self) -> None:
+        self.__conn.close()
+
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        if not self.__conn:
-            self.__conn.close()
+        self.open_conn()
 
 
 class AioSqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    async def __aenter__(self) -> 'AioSqlite':
+    async def open_conn(self) -> None:
         self.__conn = await aiosqlite.connect(self.__db_name)
         self.__cursor = await self.__conn.cursor()
+
+    async def __aenter__(self) -> 'AioSqlite':
+        await self.open_conn()
         return self
 
     async def create_table(self,
                            table_name: str,
                            columns: Dict[str, Union[DataTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-        await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+        query = f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})"
+        await self.__cursor.execute(query)
         await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
                           data: Dict[str, Union[str, int, float]]) -> None:
         columns = ', '.join(data.keys())
         placeholders = ', '.join(['?' for _ in range(len(data))])
         values = tuple(data.values())
-        await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+        query = f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})"
+        await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
-                          columns: Union[List[str], str, None] = None,
-                          where: Union[str, Dict[str, Union[str, int, float]], None] = None,
+                          columns: Union[List[str], str] = '*',
+                          where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
                           limit: Union[int, None] = None,
                           offset: Union[int, None] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
-        if columns:
+        if columns != '*':
             columns = ', '.join(columns)
-        else:
-            columns = '*'
         if where:
-            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
+            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
-        await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                                    values)
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}"
+        await self.__cursor.execute(query, values)
 
         if fetch == DataTypes.Fetch.FETCHONE:
             result = await self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
         return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
-                          where: Dict[str, Union[str, int, float]],
+                          where: Union[Dict[str, Union[str, int, float]], None] = None,
                           sign: Union[str, None] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(set_data.values()) + tuple(where.values())
-        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+        if where:
+            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(set_data.values()) + tuple(where.values())
+        else:
+            where_clause = ''
+            values = tuple(set_data.values())
+        query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
+        await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
-                          where: Dict[str, Union[str, int, float]]) -> None:
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(where.values())
-        await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+                          where: Union[Dict[str, Union[str, int, float]], None] = None) -> None:
+        if where:
+            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+        else:
+            where_clause = ''
+            values = ()
+        query = f"DELETE FROM {table_name} {where_clause}"
+        await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
+    async def close_conn(self) -> None:
         await self.__conn.close()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.close_conn()
```

### Comparing `litesqlite-2.6.7/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.8/litesqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.7
+Version: 2.6.8
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.7/setup.py` & `litesqlite-2.6.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.7',
+    version='2.6.8',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

