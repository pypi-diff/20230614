# Comparing `tmp/zxt-0.20230428.1624.tar.gz` & `tmp/zxt-0.20230614.1615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zxt-0.20230428.1624.tar", last modified: Fri Apr 28 08:58:20 2023, max compression
+gzip compressed data, was "zxt-0.20230614.1615.tar", last modified: Wed Jun 14 08:23:57 2023, max compression
```

## Comparing `zxt-0.20230428.1624.tar` & `zxt-0.20230614.1615.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.076342 zxt-0.20230428.1624/
--rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20230428.1624/LICENSE
--rw-rw-rw-   0        0        0    42858 2023-04-28 08:58:20.077432 zxt-0.20230428.1624/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-04-28 08:58:03.000000 zxt-0.20230428.1624/README.md
--rw-rw-rw-   0        0        0      815 2023-04-28 08:24:59.000000 zxt-0.20230428.1624/pyproject.toml
--rw-rw-rw-   0        0        0      555 2023-04-28 08:58:20.081964 zxt-0.20230428.1624/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20230428.1624/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.061621 zxt-0.20230428.1624/zxt/
--rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20230428.1624/zxt/__init__.py
--rw-rw-rw-   0        0        0     4302 2023-02-14 08:03:45.000000 zxt-0.20230428.1624/zxt/log_helper.py
--rw-rw-rw-   0        0        0     6720 2023-04-28 08:14:21.000000 zxt-0.20230428.1624/zxt/pth.py
--rw-rw-rw-   0        0        0    12100 2023-02-14 08:08:11.000000 zxt-0.20230428.1624/zxt/redis_helper.py
--rw-rw-rw-   0        0        0     8390 2023-04-28 08:40:56.000000 zxt-0.20230428.1624/zxt/sql_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:58:20.075336 zxt-0.20230428.1624/zxt.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 08:58:20.000000 zxt-0.20230428.1624/zxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:23:57.862823 zxt-0.20230614.1615/
+-rw-rw-rw-   0        0        0    35821 2022-12-30 03:02:11.000000 zxt-0.20230614.1615/LICENSE
+-rw-rw-rw-   0        0        0    42858 2023-06-14 08:23:57.863952 zxt-0.20230614.1615/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-04-28 08:58:03.000000 zxt-0.20230614.1615/README.md
+-rw-rw-rw-   0        0        0      815 2023-06-14 08:17:06.000000 zxt-0.20230614.1615/pyproject.toml
+-rw-rw-rw-   0        0        0      555 2023-06-14 08:23:57.865618 zxt-0.20230614.1615/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-06 17:11:18.000000 zxt-0.20230614.1615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:23:57.848196 zxt-0.20230614.1615/zxt/
+-rw-rw-rw-   0        0        0        0 2023-02-06 07:46:40.000000 zxt-0.20230614.1615/zxt/__init__.py
+-rw-rw-rw-   0        0        0     4302 2023-02-14 08:03:45.000000 zxt-0.20230614.1615/zxt/log_helper.py
+-rw-rw-rw-   0        0        0     6720 2023-04-28 08:14:21.000000 zxt-0.20230614.1615/zxt/pth.py
+-rw-rw-rw-   0        0        0    12100 2023-02-14 08:08:11.000000 zxt-0.20230614.1615/zxt/redis_helper.py
+-rw-rw-rw-   0        0        0    10344 2023-06-14 08:10:41.000000 zxt-0.20230614.1615/zxt/sql_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:23:57.860458 zxt-0.20230614.1615/zxt.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-14 08:23:57.000000 zxt-0.20230614.1615/zxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-14 08:23:57.000000 zxt-0.20230614.1615/zxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:23:57.000000 zxt-0.20230614.1615/zxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 08:23:57.000000 zxt-0.20230614.1615/zxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-14 08:23:57.000000 zxt-0.20230614.1615/zxt.egg-info/top_level.txt
```

### Comparing `zxt-0.20230428.1624/LICENSE` & `zxt-0.20230614.1615/LICENSE`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/PKG-INFO` & `zxt-0.20230614.1615/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20230428.1624
+Version: 0.20230614.1615
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `zxt-0.20230428.1624/README.md` & `zxt-0.20230614.1615/README.md`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/pyproject.toml` & `zxt-0.20230614.1615/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#creating-pyproject-toml
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "zxt"
-version = "0.20230428.1624"
+version = "0.20230614.1615"
 description = "A handy toolkit"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["tool", "toolkit"]
 # https://pypi.org/pypi?:action=list_classifiers
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `zxt-0.20230428.1624/setup.cfg` & `zxt-0.20230614.1615/setup.cfg`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/zxt/log_helper.py` & `zxt-0.20230614.1615/zxt/log_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/zxt/pth.py` & `zxt-0.20230614.1615/zxt/pth.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/zxt/redis_helper.py` & `zxt-0.20230614.1615/zxt/redis_helper.py`

 * *Files identical despite different names*

### Comparing `zxt-0.20230428.1624/zxt/sql_helper.py` & `zxt-0.20230614.1615/zxt/sql_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 定义编码【# coding=<encoding name>】参见: http://www.python.org/peps/pep-0263.html
 
 对 SQL 的简单封装，支持 MySQL 和 SQLite
 """
 
 
 import json
+import pathlib
 import peewee
 import playhouse.db_url
 import pymysql
 import pymysql.cursors
 import sqlite3
 import threading
 from typing import Dict, List, Tuple, Optional, Union
@@ -94,54 +95,83 @@
                 self.connection.close()
                 self.connection = None
 
     def __del__(self) -> None:
         """"""
         self.terminate()
 
-    def select(self, sql: str, isDictNotList: bool = False) -> List[Union[tuple, dict]]:
-        """"""
+    def select(self, sql: str, params: Union[list, tuple, dict, None] = None, isDictNotList: bool = False) -> List[Union[tuple, dict]]:
+        """
+        sqlite: 不具名占位符{?} 具名占位符{:name}
+        mysql : 不具名占位符{%s}具名占位符{%(name)s}
+        sqlhelper.select("SELECT 'sqlite'AS tag, ?        * ?       AS total", (3, 7), True)
+        sqlhelper.select("SELECT 'sqlite'AS tag, :unit    * :num    AS total", {"unit": 3, "num": 7}, True)
+        sqlhelper.select("SELECT 'mysql' AS tag, %s       * %s      AS total", (3, 7), True)
+        sqlhelper.select("SELECT 'mysql' AS tag, %(unit)s * %(num)s AS total", {"unit": 3, "num": 7}, True)
+        """
         self._lazy_initialize_db()
 
-        self.cursor.execute(sql)
+        if params is None:
+            self.cursor.execute(sql)
+        else:
+            self.cursor.execute(sql, params)
+
         results = self.fetchall(cursor=self.cursor, isDictNotList=isDictNotList)
 
         return results
 
     def commit(self) -> None:
         """"""
+        self._lazy_initialize_db()
+
         self.connection.commit()
 
     def rollback(self) -> None:
         """"""
+        self._lazy_initialize_db()
+
         self.connection.rollback()
 
-    def execute(self, sql: str, commit: bool = True) -> None:
-        """"""
+    def execute(self, sql: str, params: Union[list, tuple, dict, None] = None, commit: bool = True) -> None:
+        """
+        * sqlite: question marks (qmark style) or named placeholders (named style)
+        https://docs.python.org/3/library/sqlite3.html#sqlite3.Cursor.execute
+        https://docs.python.org/3/library/sqlite3.html#sqlite3-placeholders
+        An SQL statement may use one of two kinds of placeholders:
+        question marks (qmark style) or named placeholders (named style).
+        * mysql : variables using %s or %(name)s parameter style
+        https://dev.mysql.com/doc/connector-python/en/connector-python-api-mysqlcursor-execute.html
+        The parameters found in the tuple or dictionary params are bound to the variables in the operation.
+        Specify variables using %s or %(name)s parameter style (that is, using format or pyformat style).
+        """
         self._lazy_initialize_db()
 
-        self.cursor.execute(sql)
+        if params is None:
+            self.cursor.execute(sql)
+        else:
+            self.cursor.execute(sql, params)
+
         if commit:
             self.commit()
 
     @classmethod
     def fetchall(cls, cursor: Union[pymysql.cursors.Cursor, sqlite3.Cursor], isDictNotList: bool = False) -> List[Union[tuple, dict]]:
-        '''如果结果是空,且(isDictNotList=True),那么结果为空,不利于保存到文件'''
+        """如果结果是空,且(isDictNotList=True),那么结果为空,不利于保存到文件"""
         if isDictNotList:
             head = [col[0] for col in cursor.description]
             results = [dict(zip(head, data)) for data in cursor.fetchall()]
         else:
             head = [col[0] for col in cursor.description]
             results = [data for data in cursor.fetchall()]
             results.insert(0, head)
         return results
 
     @classmethod
     def fetchone(cls, cursor: Union[pymysql.cursors.Cursor, sqlite3.Cursor], isDictNotList: bool = False) -> List[Union[tuple, dict]]:
-        '''如果结果是空,且(isDictNotList=True),那么结果为空,不利于保存到文件'''
+        """如果结果是空,且(isDictNotList=True),那么结果为空,不利于保存到文件"""
         if isDictNotList:
             head = [col[0] for col in cursor.description]
             results = [dict(zip(head, data)) for data in (cursor.fetchone(),)]
         else:
             head = [col[0] for col in cursor.description]
             results = [data for data in (cursor.fetchone(),)]
             results.insert(0, head)
@@ -153,15 +183,15 @@
 
     def __init__(self, *args, **kwargs):
         """"""
         self._connections: Dict[str, SqlHelper] = {}
 
     def initialize(self, conf: Union[str, dict], *args, **kwargs):
         """"""
-        if isinstance(conf, str):  # 文件路径,
+        if isinstance(conf, (str, pathlib.Path)):  # 文件路径,
             with open(file=conf, mode="r", encoding="utf8") as fp:
                 conf_obj = json.load(fp=fp)
         else:
             conf_obj = conf  # 文件内容,
 
         for name, params in conf_obj.items():
             assert isinstance(name, str) and (name != '')  # name 不可为空
@@ -195,18 +225,18 @@
         if not name and isinstance(self._connections, dict) and len(self._connections) == 1:
             connection = self._connections.values().__iter__().__next__()
         else:
             connection = self._connections.get(name, None)
 
         return connection
 
-    def select(self, sql: str, isDictNotList: bool = False, name: str = None) -> list:
+    def select(self, sql: str, params: Union[list, tuple, dict, None] = None, isDictNotList: bool = False, name: str = None) -> list:
         """"""
         connection: Optional[SqlHelper] = self._get_connection(name)
-        return connection.select(sql=sql, isDictNotList=isDictNotList)
+        return connection.select(sql=sql, params=params, isDictNotList=isDictNotList)
 
 
 if __name__ == '__main__':
     conf_obj = {
         "testdb": {
             "url": "mysql://root:toor@localhost:13306/mysql?charset=utf8",
             "lazy_init": True,
@@ -216,12 +246,18 @@
             "url": "sqlite:///:memory:",
             "lazy_init": True,
             "__note": "内存模式的SQLite",
         }
     }
     shs = SqlHelperSet()
     shs.initialize(conf=conf_obj)
+
     sql_statement = 'SELECT 3*7 AS number;'
     results = shs.select(sql_statement, isDictNotList=True, name="memory")
+    print(results)
+
+    sqlhelper = shs._get_connection(name="memory")
+    results = sqlhelper.select("SELECT 'sqlite'AS tag, :unit    * :num    AS total", {"unit": 3, "num": 7}, True)
+    print(results)
+    del sqlhelper
+
     shs.terminate()
-    for result in results:
-        print(result)
```

### Comparing `zxt-0.20230428.1624/zxt.egg-info/PKG-INFO` & `zxt-0.20230614.1615/zxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zxt
-Version: 0.20230428.1624
+Version: 0.20230614.1615
 Summary: A handy toolkit
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

