# Comparing `tmp/litesqlite-2.6.8.tar.gz` & `tmp/litesqlite-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.8.tar", last modified: Wed Jun 14 15:08:40 2023, max compression
+gzip compressed data, was "litesqlite-2.6.9.tar", last modified: Wed Jun 14 15:18:46 2023, max compression
```

## Comparing `litesqlite-2.6.8.tar` & `litesqlite-2.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.962481 litesqlite-2.6.8/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.8/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:08:40.962481 litesqlite-2.6.8/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3248 2023-06-13 17:37:30.000000 litesqlite-2.6.8/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.958481 litesqlite-2.6.8/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.8/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.8/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8472 2023-06-14 15:06:12.000000 litesqlite-2.6.8/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:08:40.962481 litesqlite-2.6.8/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 15:08:40.000000 litesqlite-2.6.8/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 15:08:40.962481 litesqlite-2.6.8/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 13:45:59.000000 litesqlite-2.6.8/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.515923 litesqlite-2.6.9/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.9/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:18:46.511923 litesqlite-2.6.9/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3248 2023-06-13 17:37:30.000000 litesqlite-2.6.9/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.511923 litesqlite-2.6.9/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.9/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.9/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8544 2023-06-14 15:18:42.000000 litesqlite-2.6.9/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 15:18:46.511923 litesqlite-2.6.9/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 15:18:46.000000 litesqlite-2.6.9/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 15:18:46.515923 litesqlite-2.6.9/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 15:18:42.000000 litesqlite-2.6.9/setup.py
```

### Comparing `litesqlite-2.6.8/LICENSE` & `litesqlite-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.8/PKG-INFO` & `litesqlite-2.6.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.8
+Version: 2.6.9
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.8/README.md` & `litesqlite-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.8/litesqlite/datatypes.py` & `litesqlite-2.6.9/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.8/litesqlite/lite_sqlite.py` & `litesqlite-2.6.9/litesqlite/lite_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,23 +68,23 @@
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = self.__cursor.fetchall()
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
-                    where: Union[Dict[str, Union[str, int, float]], None] = None,
+                    where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
                     sign: Union[str, None] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
-            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(set_data.values()) + tuple(where.values())
+            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
@@ -173,23 +173,23 @@
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
         return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
-                          where: Union[Dict[str, Union[str, int, float]], None] = None,
+                          where: Union[List[Dict[str, Union[str, int, float]]], None] = None,
                           sign: Union[str, None] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
-            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(set_data.values()) + tuple(where.values())
+            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
```

### Comparing `litesqlite-2.6.8/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.9/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.8
+Version: 2.6.9
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.8/setup.py` & `litesqlite-2.6.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.8',
+    version='2.6.9',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

