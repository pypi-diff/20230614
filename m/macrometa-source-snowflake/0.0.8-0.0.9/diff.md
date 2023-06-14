# Comparing `tmp/macrometa-source-snowflake-0.0.8.tar.gz` & `tmp/macrometa-source-snowflake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-snowflake-0.0.8.tar", last modified: Tue Mar 28 17:11:34 2023, max compression
+gzip compressed data, was "macrometa-source-snowflake-0.0.9.tar", last modified: Tue Mar 28 17:20:08 2023, max compression
```

## Comparing `macrometa-source-snowflake-0.0.8.tar` & `macrometa-source-snowflake-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:11:34.843558 macrometa-source-snowflake-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:11:34.839558 macrometa-source-snowflake-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:11:34.835558 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:11:34.839558 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:11:34.839558 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 17:11:34.000000 macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 17:11:34.843558 macrometa-source-snowflake-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-28 17:11:14.000000 macrometa-source-snowflake-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.942757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 17:20:08.000000 macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 17:20:08.946757 macrometa-source-snowflake-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-28 17:19:53.000000 macrometa-source-snowflake-0.0.9/setup.py
```

### Comparing `macrometa-source-snowflake-0.0.8/LICENSE` & `macrometa-source-snowflake-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/PKG-INFO` & `macrometa-source-snowflake-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa Source for extracting data from Macrometa
 Home-page: https://github.com/Macrometacorp/macrometa-source-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-source-snowflake-0.0.8/README.md` & `macrometa-source-snowflake-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/__init__.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -560,48 +560,59 @@
 
     # TODO: Need to add handling of reserved keys
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the provided configurations."""
         config = self.get_config(integration)
         try:
             snowflake_conn = SnowflakeConnection(config)
+            LOGGER.info('DEBUG SAMPLE 1: %s', config)
             catalog = do_discover(snowflake_conn, config)
+            LOGGER.info('DEBUG SAMPLE 2: %s', catalog)
             results = []
+            
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
+                LOGGER.info('DEBUG SAMPLE 3: %s', s_schema)
                 data = fetch_samples(config, stream)[:10]
+                LOGGER.info('DEBUG SAMPLE 4: %s', data)
                 for k, v in s_schema.properties.items():
                     t = v['type'][-1]
                     s_attribs.append(SchemaAttribute(
                         k, self.get_attribute_type(t)))
                 schema = C8Schema(stream.stream, s_attribs)
+                LOGGER.info('DEBUG SAMPLE 5: %s', schema)
+                LOGGER.info('DEBUG SAMPLE 6: %s', s_attribs)
                 results.append(Sample(
                     schema=schema,
                     data=data)
                 )
         except Exception as e:
             raise e
         return results
 
     # TODO: Need to add handling of reserved keys
     def schemas(self, integration: dict) -> list[C8Schema]:
         """Get supported schemas using the given configurations."""
         config = self.get_config(integration)
         try:
             snowflake_conn = SnowflakeConnection(config)
+            LOGGER.info('DEBUG 1: %s', config)
             catalog = do_discover(snowflake_conn, config)
+            LOGGER.info('DEBUG 2: %s', catalog)
             results = []
             for stream in catalog.streams:
                 s_attribs = []
                 s_schema = stream.schema
+                LOGGER.info('DEBUG 3: %s', s_schema)
                 for k, v in s_schema.properties.items():
                     t = v['type'][-1]
                     s_attribs.append(SchemaAttribute(
                         k, self.get_attribute_type(t)))
+                LOGGER.info('DEBUG 4: %s', s_attribs)
                 results.append(C8Schema(stream.stream, s_attribs))
         except Exception as e:
             raise e
         return results
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
```

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/connection.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/common.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/full_table.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/incremental.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/incremental.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake/sync_strategies/sample_data.py` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/PKG-INFO` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Macrometa Source for extracting data from Macrometa
 Home-page: https://github.com/Macrometacorp/macrometa-source-snowflake
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-source-snowflake-0.0.8/macrometa_source_snowflake.egg-info/SOURCES.txt` & `macrometa-source-snowflake-0.0.9/macrometa_source_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-source-snowflake-0.0.8/setup.py` & `macrometa-source-snowflake-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='macrometa-source-snowflake',
-      version='0.0.8',
+      version='0.0.9',
       description='Macrometa Source for extracting data from Macrometa',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-source-snowflake',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
```

