# Comparing `tmp/bs_orm-0.8.tar.gz` & `tmp/bs_orm-0.8.1.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.tar", last modified: Mon Apr 24 22:06:59 2023, max compression
+gzip compressed data, was "bs_orm-0.8.1.post20230615.tar", last modified: Wed Jun 14 21:56:31 2023, max compression
```

## Comparing `bs_orm-0.8.tar` & `bs_orm-0.8.1.post20230615.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 22:06:59.461548 bs_orm-0.8/
--rw-rw-rw-   0        0        0      154 2023-04-24 22:06:59.461548 bs_orm-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-04-23 10:46:02.000000 bs_orm-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 22:06:59.447560 bs_orm-0.8/bs_orm/
--rw-rw-rw-   0        0        0     9148 2023-04-24 21:58:22.000000 bs_orm-0.8/bs_orm/Better_orm.py
--rw-rw-rw-   0        0        0     3069 2023-04-24 21:58:22.000000 bs_orm-0.8/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0        0 2023-04-24 21:57:55.000000 bs_orm-0.8/bs_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:06:59.458529 bs_orm-0.8/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      154 2023-04-24 22:06:59.000000 bs_orm-0.8/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-24 22:06:59.000000 bs_orm-0.8/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 22:06:59.000000 bs_orm-0.8/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 22:06:59.000000 bs_orm-0.8/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-04-24 22:06:59.000000 bs_orm-0.8/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 22:06:59.463548 bs_orm-0.8/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-04-24 22:06:43.000000 bs_orm-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:56:31.723312 bs_orm-0.8.1.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-14 21:56:31.723312 bs_orm-0.8.1.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.1.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 21:56:31.659449 bs_orm-0.8.1.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     3281 2023-06-14 21:33:52.000000 bs_orm-0.8.1.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0     9281 2023-06-14 21:35:48.000000 bs_orm-0.8.1.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.1.post20230615/bs_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 21:56:31.721309 bs_orm-0.8.1.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-14 21:56:31.000000 bs_orm-0.8.1.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 21:56:31.000000 bs_orm-0.8.1.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 21:56:31.000000 bs_orm-0.8.1.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 21:56:31.000000 bs_orm-0.8.1.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 21:56:31.000000 bs_orm-0.8.1.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-14 21:56:31.725306 bs_orm-0.8.1.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-14 21:56:19.000000 bs_orm-0.8.1.post20230615/setup.py
```

### Comparing `bs_orm-0.8/README.md` & `bs_orm-0.8.1.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8/bs_orm/Better_orm.py` & `bs_orm-0.8.1.post20230615/bs_orm/Requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import models
 from .DataTypes import *
 import sqlite3
 import os
 import datetime
 
 
 class empty:
     pass
 
 
 class db_settings:
     path = 'database.db'
+    models = 0
 
 
 def for_size(content, request):
     try:
         if content.size:
             request += f'({content.size})'
         return ['ok', request]
@@ -113,41 +113,43 @@
         returned += f'"id" INTEGER PRIMARY KEY  '
     returned = returned[:-2]+')'
     return returned
 
 
 def create_execute():
     request = ''
-    for mod_name, value in models.__dict__.items():
+    for mod_name, value in db_settings.models.__dict__.items():
         if hasattr(value, '__module__') and value.__module__ == 'models':
             table_name = mod_name
             mod = dict(value.__dict__)
             for i in empty.__dict__:
                 if i in mod:
                     mod.pop(i)
             request += get_table(table_name, mod)+';\n'
-    # print(request)
     return request
 
 
-def create_tables():
+def create_tables(models):
+    db_settings.models = models
     conn = sqlite3.connect(db_settings.path)
     cur = conn.cursor()
     cur.executescript(create_execute() +
                       'CREATE TABLE IF NOT EXISTS "migrations"(filename TEXT)')
     conn.commit()
     conn.close()
 
 
 def write(table, **qwargs):
     conn = sqlite3.connect(db_settings.path)
     cur = conn.cursor()
     try:
         request = 'INSERT INTO '
-        for mod_name, value in models.__dict__.items():
+        if db_settings.models == 0:
+            raise  Exception("You haven`t models file. Please create it!")
+        for mod_name, value in db_settings.models.__dict__.items():
             if table == value:
                 request += f'{mod_name}('
                 req_val = 'VALUES('
                 for k, v in qwargs.items():
                     request += k+', '
                     if v.__class__ == str:
                         req_val += f'\'{v}\','
@@ -270,15 +272,13 @@
     except:
         pass
 
     fileName = str(datetime.datetime.now().timestamp())
     with open(f'./migrations/{fileName}.py', 'w') as f:
         f.write(textFromPattern)
 
-    print(upgrade)
-
     cur.execute(f'INSERT INTO migrations (filename) VALUES({fileName})')
     cur.executescript(upgrade)
     conn.commit()
     conn.close()
 
     # debugging
```

### Comparing `bs_orm-0.8/bs_orm/DataTypes.py` & `bs_orm-0.8.1.post20230615/bs_orm/DataTypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,11 +82,19 @@
             raise Exception(f'well congratulations your father goes fucking you with a chair on the head with these words: {ex}')
 
     @classmethod
     def create(cls, **qwargs):
         obj = qwargs
         new_cls = type(cls.__name__, (Table_Engine,), obj)
         return new_cls
+    
+    @classmethod
+    def execute(cls, execut: str):
+        conn = sqlite3.connect(db_settings.path)
+        cur = conn.cursor()
+        cur.execute(execut)
+        conn.commit()
+        return True
 
 class db_settings:
     path = 'database.db'
     debug = False # добавить возможность с дебагом
```

