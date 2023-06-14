# Comparing `tmp/searchkit-0.2.7.tar.gz` & `tmp/searchkit-0.2.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.7.tar", last modified: Sat May 27 14:58:08 2023, max compression
+gzip compressed data, was "searchkit-0.2.7.post1.tar", last modified: Wed Jun 14 12:03:48 2023, max compression
```

## Comparing `searchkit-0.2.7.tar` & `searchkit-0.2.7.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.7/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     4413 2023-05-27 14:58:08.196353 searchkit-0.2.7/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.7/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.7/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.192353 searchkit-0.2.7/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.7/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    29362 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.7/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49678 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5773 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     4413 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-05-27 14:58:08.196353 searchkit-0.2.7/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.7/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/tests/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7/tests/__init__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/tests/unit/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7/tests/unit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    39444 2023-05-27 14:47:28.000000 searchkit-0.2.7/tests/unit/test_search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8212 2023-05-24 11:46:12.000000 searchkit-0.2.7/tests/unit/test_search_constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2526 2023-05-16 10:48:26.000000 searchkit-0.2.7/tests/unit/test_utils.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1331 2023-04-13 19:54:24.000000 searchkit-0.2.7/tests/unit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.7.post1/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.7.post1/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29362 2023-05-27 14:47:28.000000 searchkit-0.2.7.post1/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.7.post1/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49764 2023-06-14 08:31:14.000000 searchkit-0.2.7.post1/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5773 2023-05-27 14:47:28.000000 searchkit-0.2.7.post1/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-06-14 12:03:48.000000 searchkit-0.2.7.post1/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.7.post1/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post1/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-06-14 12:03:48.205274 searchkit-0.2.7.post1/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7.post1/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    39444 2023-05-31 12:54:07.000000 searchkit-0.2.7.post1/tests/unit/test_search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8212 2023-05-24 11:46:12.000000 searchkit-0.2.7.post1/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2526 2023-05-16 10:48:26.000000 searchkit-0.2.7.post1/tests/unit/test_utils.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1331 2023-04-13 19:54:24.000000 searchkit-0.2.7.post1/tests/unit/utils.py
```

### Comparing `searchkit-0.2.7/LICENSE` & `searchkit-0.2.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/PKG-INFO` & `searchkit-0.2.7.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.7
+Version: 0.2.7.post1
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.7/README.md` & `searchkit-0.2.7.post1/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/pyproject.toml` & `searchkit-0.2.7.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/searchkit/constraints.py` & `searchkit-0.2.7.post1/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/searchkit/search.py` & `searchkit-0.2.7.post1/searchkit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,16 +455,17 @@
         # NOTE: this does not include group(0)
         if num_groups:
             # To reduce memory footprint, don't store group(0) i.e. the whole
             # line, if there are actual groups in the result.
             for i in range(1, num_groups + 1):
                 self._save_part(i, result.group(i))
         else:
-            log.debug("saving full search result which can lead to high "
-                      "memory usage")
+            log.debug("Saving full search result is inefficient and can lead "
+                      "to high memory usage. Use sub groups if possible. "
+                      "(tag=%s)", self.tag)
             self._save_part(0, result.group(0))
 
     @cached_property
     def id(self):
         """ Unique Result ID """
         id_string = "{}-{}-{}".format(uuid.uuid4(), self.source_id,
                                       self.linenumber)
```

### Comparing `searchkit-0.2.7/searchkit/utils.py` & `searchkit-0.2.7.post1/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.7.post1/searchkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.7
+Version: 0.2.7.post1
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.7/tests/unit/test_search.py` & `searchkit-0.2.7.post1/tests/unit/test_search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/tests/unit/test_search_constraints.py` & `searchkit-0.2.7.post1/tests/unit/test_search_constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/tests/unit/test_utils.py` & `searchkit-0.2.7.post1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.7/tests/unit/utils.py` & `searchkit-0.2.7.post1/tests/unit/utils.py`

 * *Files identical despite different names*

