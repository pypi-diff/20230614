# Comparing `tmp/ctidb-0.0.4.tar.gz` & `tmp/ctidb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ctidb-0.0.4.tar", last modified: Tue Jun 13 05:33:43 2023, max compression
+gzip compressed data, was "dist\ctidb-0.0.5.tar", last modified: Wed Jun 14 02:07:17 2023, max compression
```

## Comparing `ctidb-0.0.4.tar` & `ctidb-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:33:43.000000 ctidb-0.0.4/
--rw-rw-rw-   0        0        0     3202 2023-06-13 05:33:43.000000 ctidb-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1766 2023-06-12 09:19:34.000000 ctidb-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb/
--rw-rw-rw-   0        0        0      229 2023-06-13 05:26:20.000000 ctidb-0.0.4/ctidb/__init__.py
--rw-rw-rw-   0        0        0      565 2023-06-12 03:30:39.000000 ctidb-0.0.4/ctidb/custom.py
--rw-rw-rw-   0        0        0     6920 2023-06-13 02:53:41.000000 ctidb-0.0.4/ctidb/decoder.py
--rw-rw-rw-   0        0        0    10017 2023-06-13 05:25:36.000000 ctidb-0.0.4/ctidb/reader.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb.egg-info/
--rw-rw-rw-   0        0        0     3202 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-12 09:11:31.000000 ctidb-0.0.4/ctidb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-13 05:33:43.000000 ctidb-0.0.4/ctidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 05:33:43.000000 ctidb-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1762 2023-06-12 09:07:31.000000 ctidb-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:07:17.000000 ctidb-0.0.5/
+-rw-rw-rw-   0        0        0     3202 2023-06-14 02:07:17.000000 ctidb-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1766 2023-06-12 09:19:34.000000 ctidb-0.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb/
+-rw-rw-rw-   0        0        0      229 2023-06-14 02:06:51.000000 ctidb-0.0.5/ctidb/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-06-13 05:58:52.000000 ctidb-0.0.5/ctidb/custom.py
+-rw-rw-rw-   0        0        0     6920 2023-06-13 05:58:52.000000 ctidb-0.0.5/ctidb/decoder.py
+-rw-rw-rw-   0        0        0    10140 2023-06-14 02:00:56.000000 ctidb-0.0.5/ctidb/reader.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb.egg-info/
+-rw-rw-rw-   0        0        0     3202 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 09:11:31.000000 ctidb-0.0.5/ctidb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-14 02:07:17.000000 ctidb-0.0.5/ctidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 02:07:17.000000 ctidb-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1762 2023-06-12 09:07:31.000000 ctidb-0.0.5/setup.py
```

### Comparing `ctidb-0.0.4/PKG-INFO` & `ctidb-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ctidb
-Version: 0.0.4
+Version: 0.0.5
 Summary: criminalip.ctidb reader
 Home-page: https://github.com/aispera/ctidb
 Author: aispera
 Author-email: infra@aispera.com
 License: Apache License, Version 2.0
 Description: ========================
         CTI DB Python Module
```

### Comparing `ctidb-0.0.4/README.rst` & `ctidb-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `ctidb-0.0.4/ctidb/custom.py` & `ctidb-0.0.5/ctidb/custom.py`

 * *Files identical despite different names*

### Comparing `ctidb-0.0.4/ctidb/decoder.py` & `ctidb-0.0.5/ctidb/decoder.py`

 * *Files identical despite different names*

### Comparing `ctidb-0.0.4/ctidb/reader.py` & `ctidb-0.0.5/ctidb/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,16 @@
     def _resolve_data_pointer(self, pointer: int) -> Record:
         resolved = pointer - self._metadata.node_count + self._metadata.search_tree_size
 
         if resolved >= self._buffer_size:
             raise InvalidDatabaseError("The cti DB file's search tree is corrupt")
 
         (data, _) = self._decoder.decode(resolved)
+        if isinstance(data.get('products'), list):
+            data['products'] = list(filter(None, data.get('products')))
         return data
 
     def close(self) -> None:
         """Closes the cti DB file and returns the resources to the system"""
         try:
             self._buffer.close()  # type: ignore
         except AttributeError:
```

### Comparing `ctidb-0.0.4/ctidb.egg-info/PKG-INFO` & `ctidb-0.0.5/ctidb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ctidb
-Version: 0.0.4
+Version: 0.0.5
 Summary: criminalip.ctidb reader
 Home-page: https://github.com/aispera/ctidb
 Author: aispera
 Author-email: infra@aispera.com
 License: Apache License, Version 2.0
 Description: ========================
         CTI DB Python Module
```

### Comparing `ctidb-0.0.4/setup.py` & `ctidb-0.0.5/setup.py`

 * *Files identical despite different names*

