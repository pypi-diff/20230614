# Comparing `tmp/witchcraft-0.2.8.tar.gz` & `tmp/witchcraft-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/witchcraft-0.2.8.tar", last modified: Tue Apr  4 09:58:50 2017, max compression
+gzip compressed data, was "dist/witchcraft-0.2.9.tar", last modified: Wed Apr 12 08:30:50 2017, max compression
```

## Comparing `witchcraft-0.2.8.tar` & `witchcraft-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/
--rw-r--r--   0 qalt      (1000) qalt      (1000)      684 2017-04-04 09:58:50.000000 witchcraft-0.2.8/PKG-INFO
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/
--rw-r--r--   0 qalt      (1000) qalt      (1000)      684 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/PKG-INFO
--rw-r--r--   0 qalt      (1000) qalt      (1000)       62 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/requires.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/dependency_links.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)       11 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/top_level.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2016-03-29 17:15:54.000000 witchcraft-0.2.8/witchcraft.egg-info/not-zip-safe
--rw-r--r--   0 qalt      (1000) qalt      (1000)      918 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft.egg-info/SOURCES.txt
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft/
--rw-r--r--   0 qalt      (1000) qalt      (1000)    10108 2017-03-31 13:19:11.000000 witchcraft-0.2.8/witchcraft/combinators.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)     1512 2016-03-30 19:35:44.000000 witchcraft-0.2.8/witchcraft/reserved_psql.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)     2336 2016-10-05 14:59:13.000000 witchcraft-0.2.8/witchcraft/connection.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)     9508 2017-03-31 12:58:34.000000 witchcraft-0.2.8/witchcraft/utils.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)     5388 2017-03-10 16:27:57.000000 witchcraft-0.2.8/witchcraft/template.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)     1067 2017-03-23 12:48:13.000000 witchcraft-0.2.8/witchcraft/__init__.py
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft/dateutil/
--rw-r--r--   0 qalt      (1000) qalt      (1000)    21509 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/relativedelta.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)       58 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/tzwin.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)       46 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/__init__.py
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft/dateutil/tz/
--rw-r--r--   0 qalt      (1000) qalt      (1000)    11143 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/tz/win.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)    33867 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/tz/tz.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)      145 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/tz/__init__.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)      461 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/tz/_common.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)    61599 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/rrule.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)     2611 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/easter.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)    50334 2017-03-20 07:22:41.000000 witchcraft-0.2.8/witchcraft/dateutil/parser.py
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-04 09:58:50.000000 witchcraft-0.2.8/witchcraft/queries/
--rw-r--r--   0 qalt      (1000) qalt      (1000)     1125 2016-09-30 13:13:39.000000 witchcraft-0.2.8/witchcraft/queries/psql_upsert.sql
--rw-r--r--   0 qalt      (1000) qalt      (1000)     1168 2016-09-12 13:27:58.000000 witchcraft-0.2.8/witchcraft/queries/psql_discover_columns.sql
--rw-r--r--   0 qalt      (1000) qalt      (1000)       75 2016-09-12 13:10:23.000000 witchcraft-0.2.8/witchcraft/queries/psql_add_column.sql
--rw-r--r--   0 qalt      (1000) qalt      (1000)      237 2017-03-07 14:01:51.000000 witchcraft-0.2.8/witchcraft/queries/psql_insert.sql
--rw-r--r--   0 qalt      (1000) qalt      (1000)      188 2016-09-12 14:27:43.000000 witchcraft-0.2.8/witchcraft/queries/psql_create_table.sql
--rw-r--r--   0 qalt      (1000) qalt      (1000)      453 2017-03-20 08:19:11.000000 witchcraft-0.2.8/witchcraft/test.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)    10590 2017-03-31 16:02:54.000000 witchcraft-0.2.8/witchcraft/upsert.py
--rw-r--r--   0 qalt      (1000) qalt      (1000)       59 2017-04-04 09:58:50.000000 witchcraft-0.2.8/setup.cfg
--rw-r--r--   0 qalt      (1000) qalt      (1000)       58 2016-09-30 13:13:39.000000 witchcraft-0.2.8/MANIFEST.in
--rwxr-xr-x   0 qalt      (1000) qalt      (1000)      983 2017-04-04 09:58:42.000000 witchcraft-0.2.8/setup.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      684 2017-04-12 08:30:50.000000 witchcraft-0.2.9/PKG-INFO
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft.egg-info/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      684 2017-04-12 08:30:49.000000 witchcraft-0.2.9/witchcraft.egg-info/PKG-INFO
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       62 2017-04-12 08:30:49.000000 witchcraft-0.2.9/witchcraft.egg-info/requires.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2017-04-12 08:30:49.000000 witchcraft-0.2.9/witchcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       11 2017-04-12 08:30:49.000000 witchcraft-0.2.9/witchcraft.egg-info/top_level.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2016-03-29 17:15:54.000000 witchcraft-0.2.9/witchcraft.egg-info/not-zip-safe
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      993 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft.egg-info/SOURCES.txt
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    10083 2017-04-11 14:53:00.000000 witchcraft-0.2.9/witchcraft/combinators.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     1512 2016-03-30 19:35:44.000000 witchcraft-0.2.9/witchcraft/reserved_psql.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     2336 2016-10-05 14:59:13.000000 witchcraft-0.2.9/witchcraft/connection.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     9508 2017-04-10 13:54:41.000000 witchcraft-0.2.9/witchcraft/utils.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     5388 2017-04-11 13:24:28.000000 witchcraft-0.2.9/witchcraft/template.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     2046 2017-04-11 14:16:32.000000 witchcraft-0.2.9/witchcraft/__init__.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft/dateutil/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    21509 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/relativedelta.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       58 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/tzwin.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       46 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/__init__.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft/dateutil/tz/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    11143 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/tz/win.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    33867 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/tz/tz.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      145 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/tz/__init__.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      461 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/tz/_common.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    61599 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/rrule.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     2611 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/easter.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    50334 2017-03-20 07:22:41.000000 witchcraft-0.2.9/witchcraft/dateutil/parser.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-04-12 08:30:50.000000 witchcraft-0.2.9/witchcraft/queries/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     1125 2016-09-30 13:13:39.000000 witchcraft-0.2.9/witchcraft/queries/psql_upsert.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     1202 2017-04-11 12:08:26.000000 witchcraft-0.2.9/witchcraft/queries/psql_discover_columns.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       75 2016-09-12 13:10:23.000000 witchcraft-0.2.9/witchcraft/queries/psql_add_column.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       62 2017-04-11 09:34:26.000000 witchcraft-0.2.9/witchcraft/queries/psql_max_version.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      237 2017-03-07 14:01:51.000000 witchcraft-0.2.9/witchcraft/queries/psql_insert.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       38 2017-04-10 17:00:09.000000 witchcraft-0.2.9/witchcraft/queries/psql_delete.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      387 2017-04-11 14:29:31.000000 witchcraft-0.2.9/witchcraft/queries/psql_create_table.sql
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      453 2017-03-20 08:19:11.000000 witchcraft-0.2.9/witchcraft/test.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)    12085 2017-04-11 14:49:05.000000 witchcraft-0.2.9/witchcraft/upsert.py
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       59 2017-04-12 08:30:50.000000 witchcraft-0.2.9/setup.cfg
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       58 2016-09-30 13:13:39.000000 witchcraft-0.2.9/MANIFEST.in
+-rwxr-xr-x   0 qalt      (1000) qalt      (1000)      983 2017-04-12 08:03:12.000000 witchcraft-0.2.9/setup.py
```

### Comparing `witchcraft-0.2.8/PKG-INFO` & `witchcraft-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: witchcraft
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/spookyowl/witchcraft
 Author: Peter Facka
 Author-email: pfacka@spookyowl.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -13,8 +13,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: License :: OSI Approved :: MIT License
-Provides: witchcraft (0.2.8)
+Provides: witchcraft (0.2.9)
```

### Comparing `witchcraft-0.2.8/witchcraft.egg-info/PKG-INFO` & `witchcraft-0.2.9/witchcraft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: witchcraft
-Version: 0.2.8
+Version: 0.2.9
 Summary: UNKNOWN
 Home-page: https://github.com/spookyowl/witchcraft
 Author: Peter Facka
 Author-email: pfacka@spookyowl.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -13,8 +13,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: License :: OSI Approved :: MIT License
-Provides: witchcraft (0.2.8)
+Provides: witchcraft (0.2.9)
```

### Comparing `witchcraft-0.2.8/witchcraft.egg-info/SOURCES.txt` & `witchcraft-0.2.9/witchcraft.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,10 +22,12 @@
 witchcraft/dateutil/tzwin.py
 witchcraft/dateutil/tz/__init__.py
 witchcraft/dateutil/tz/_common.py
 witchcraft/dateutil/tz/tz.py
 witchcraft/dateutil/tz/win.py
 witchcraft/queries/psql_add_column.sql
 witchcraft/queries/psql_create_table.sql
+witchcraft/queries/psql_delete.sql
 witchcraft/queries/psql_discover_columns.sql
 witchcraft/queries/psql_insert.sql
+witchcraft/queries/psql_max_version.sql
 witchcraft/queries/psql_upsert.sql
```

### Comparing `witchcraft-0.2.8/witchcraft/combinators.py` & `witchcraft-0.2.9/witchcraft/combinators.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     filename_patterns = [template_name,
                          template_name.replace('-', '_'),
                          template_name.replace('_', '-')]   
 
     path_pattern = itertools.product(__query_paths, filename_patterns)
     for t in path_pattern:
         file_path = os.path.join(t[0], t[1])
-        print(file_path)
         if os.path.isfile(file_path):
 
             with open(file_path) as query_file:
                 query_tpl = query_file.read()
 
             __template_cache[cache_key] = query_tpl
             #TODO: cache template instance
```

### Comparing `witchcraft-0.2.8/witchcraft/reserved_psql.txt` & `witchcraft-0.2.9/witchcraft/reserved_psql.txt`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/connection.py` & `witchcraft-0.2.9/witchcraft/connection.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/utils.py` & `witchcraft-0.2.9/witchcraft/utils.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/template.py` & `witchcraft-0.2.9/witchcraft/template.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/__init__.py` & `witchcraft-0.2.9/witchcraft/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 from witchcraft.utils import seekable
 from witchcraft.upsert import prepare_table, upsert_data, insert_data
+from witchcraft.upsert import delete_data, get_max_version
 from witchcraft.combinators import query, template
 
 #TODO: allow using serial primary key without defining value in data set
+#TODO: combine schema_name + table_name into one argument
 
-def upsert(connection, schema_name, table_name, data_points, primary_keys):
+def upsert(connection, schema_name, table_name, data_points, primary_keys=None):
     #TODO: use seekable from utils and call prepare table (to create new columns) in batches (10000)
     data_points = list(data_points)
 
     if len(data_points) == 0:
         return
 
-    prepare_table(connection, schema_name, table_name, data_points, primary_keys)
+    if primary_keys is None:
+        primary_keys = []
+
+    primary_keys = prepare_table(connection, schema_name, table_name, data_points, primary_keys)
     upsert_data(connection, schema_name, table_name, data_points, primary_keys)
 
 
 def insert(connection, schema_name, table_name, data_points, primary_keys):
     #TODO: use seekable from utils and call prepare table (to create new columns) in batches (10000)
     data_points = list(data_points)
 
     if len(data_points) == 0:
         return
 
     prepare_table(connection, schema_name, table_name, data_points, primary_keys)
     insert_data(connection, schema_name, table_name, data_points)
 
+
+def replace(connection, schema_name, table_name, data_points):
+    data_points = list(data_points)
+    delete_data(connection, schema_name, table_name)
+    prepare_table(connection, schema_name, table_name, data_points, [])
+    insert_data(connection, schema_name, table_name, data_points)
+
+
+def append_history(connection, schema_name, table_name, data_points):
+
+    max_version = get_max_version(connection, schema_name, table_name)
+    
+    def add_history_column(item):
+        item.add_field('version', psql_type='int')
+        item['version'] = max_version
+        return item  
+
+    data_points = list(map(add_history_column, data_points))
+
+    prepare_table(connection, schema_name, table_name, data_points, [])
+    insert_data(connection, schema_name, table_name, data_points)
```

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/relativedelta.py` & `witchcraft-0.2.9/witchcraft/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/tz/win.py` & `witchcraft-0.2.9/witchcraft/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/tz/tz.py` & `witchcraft-0.2.9/witchcraft/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/rrule.py` & `witchcraft-0.2.9/witchcraft/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/easter.py` & `witchcraft-0.2.9/witchcraft/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/dateutil/parser.py` & `witchcraft-0.2.9/witchcraft/dateutil/parser.py`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/queries/psql_upsert.sql` & `witchcraft-0.2.9/witchcraft/queries/psql_upsert.sql`

 * *Files identical despite different names*

### Comparing `witchcraft-0.2.8/witchcraft/queries/psql_discover_columns.sql` & `witchcraft-0.2.9/witchcraft/queries/psql_discover_columns.sql`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 SELECT
   columns.column_name AS column_name,
+  columns.data_type AS data_type,
   columns.character_maximum_length,
   columns.numeric_precision,
   columns.numeric_scale,
   columns.ordinal_position,
   (constraints.constraint_type IS NOT NULL) AS is_pkey
 
 FROM information_schema.columns
```

### Comparing `witchcraft-0.2.8/witchcraft/upsert.py` & `witchcraft-0.2.9/witchcraft/upsert.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import string
 from decimal import Decimal
 import csv
 
 from witchcraft.combinators import execute, query, template
 from witchcraft.dateutil.parser import parse as dateutil_parse
 
+
 prefix_dict = {                                                                    
     'pgsql': 'psql',                                                            
     'mysql': 'mysql',                                                              
     'oracle': 'oracle',                                                            
     'mssql': 'mssql',                                                              
 }
      
@@ -55,31 +56,36 @@
 
         result = query(connection, template('%s_discover_columns' % prefix,
                                      dict(schema_name=schema_name,
                                           table_name=discovery_table_name)))
 
         discovered_columns = set(map(lambda r: r.column_name.lower(), result))
 
-
     else:
         discovered_pkeys = filter(lambda r: r.is_pkey, result)
-        discovered_pkeys = map(lambda r: r.column_name.lower(), discovered_pkeys)
-        if set(primary_keys) != set(discovered_pkeys):
-            raise ValueError('Primary keys in destination table are not matching')
+        discovered_pkeys = list(map(lambda r: r.column_name.lower(), discovered_pkeys))
+
+        if len(primary_keys) != 0:
+
+            if set(primary_keys) != set(discovered_pkeys):
+                raise ValueError('Primary keys in destination table are not matching')
+
+            primary_keys = discovered_pkeys
 
     missing_columns = required_columns - discovered_columns
 
     for column_name in missing_columns:
         column_type = fields.get(column_name)['%s_type' % prefix]
 
         execute(connection, template('%s_add_column' % prefix,
                                 dict(schema_name=schema_name,
                                      table_name=table_name,
                                      column_name=column_name,
                                      column_type=column_type)))
+    return primary_keys
 
 
 def upsert_data(connection, schema_name, table_name, data_points, primary_keys):
 
     prefix = prefix_dict.get(connection.database_type)
     column_names = list(find_keys(data_points))
 
@@ -88,28 +94,68 @@
                                  table_name=table_name,
                                  column_names=column_names,
                                  columns=data_points[0].fields.items(),
                                  data_points=data_points,
                                  primary_keys=primary_keys),
                             connection.database_type))
 
-
 def insert_data(connection, schema_name, table_name, data_points):
     prefix = prefix_dict.get(connection.database_type)
     column_names = list(find_keys(data_points))
 
+    #TODO: use SqlSession insert directly
     execute(connection, template('%s_insert' % prefix,
                             dict(schema_name=schema_name,
                                  table_name=table_name,
                                  column_names=column_names,
                                  columns=data_points[0].fields.items(),
                                  data_points=data_points),
                             connection.database_type))
 
 
+def delete_data(connection, schema_name, table_name):
+    prefix = prefix_dict.get(connection.database_type)
+
+    #TODO: use SqlSession delete directly
+    execute(connection, template('%s_delete' % prefix,
+                            dict(schema_name=schema_name,
+                                 table_name=table_name),
+                            connection.database_type))
+
+
+def discover_columns(connection):
+    prefix = prefix_dict.get(connection.database_type)
+    result = query(connection, template('%s_discover_columns' % prefix,
+                                 dict(schema_name=schema_name,
+                                      table_name=discovery_table_name)))
+
+
+def get_max_version(connection, schema_name, table_name):
+    prefix = prefix_dict.get(connection.database_type)
+
+    result = query(connection, template('%s_discover_columns' % prefix,
+                                        dict(schema_name=schema_name,
+                                             table_name=table_name)))
+
+    if len(result) == 0:
+        return 1
+
+    tpl = template('%s_max_version' % prefix,
+                     dict(schema_name=schema_name,
+                          table_name=table_name),
+                     connection.database_type)
+
+    result = query(connection, tpl)
+
+    if len(result) > 0:
+        return result[0].version+1
+    else:
+        return 1
+
+
 class InputType(object):
     
     def __init__(self, name, params=None):
         if params is None:
             params = {}
   
         self.name = name
@@ -195,15 +241,14 @@
          None
 
 
 def parse_csv(input_data):
     sniffer = csv.Sniffer()
     try:
         dialect = sniffer.sniff(input_data)
-        dialect.delimiter = '\t'
     except:
         csv.register_dialect('dlb_excel', delimiter=';', quotechar='"')
         dialect = csv.get_dialect('dlb_excel')
 
     data = input_data
     data = data.splitlines()
     data = csv.reader(data, dialect=dialect)
@@ -338,8 +383,7 @@
             v, current_types[header[i]] = detect_type(value, current_types.get(header[i]))
 
             result_row.append(v)
             
         result_data.append(result_row)
 
     return result_data, current_types
-
```

### Comparing `witchcraft-0.2.8/setup.py` & `witchcraft-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="witchcraft",
-    version="0.2.8",
+    version="0.2.9",
     description='',
     author='Peter Facka',
     author_email='pfacka@spookyowl.com',
     url='https://github.com/spookyowl/witchcraft',
     packages=[
         'witchcraft',
         'witchcraft.dateutil',
@@ -16,15 +16,15 @@
     zip_safe=False,	
     install_requires=[
 	'psycopg2>=2.6.1',
 	'SQLAlchemy>=1.0.6',
         'hy>=0.11.1',
         'pyparsing>=2.1.1'
     ],
-    provides=['witchcraft (0.2.8)'],
+    provides=['witchcraft (0.2.9)'],
     include_package_data=True,
     classifiers=[
       'Development Status :: 3 - Alpha',
       'Environment :: Web Environment',
       'Intended Audience :: Developers',
       'Operating System :: Microsoft :: Windows',
       'Operating System :: MacOS :: MacOS X',
```

