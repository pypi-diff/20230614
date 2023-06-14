# Comparing `tmp/searchkit-0.2.6.post4.tar.gz` & `tmp/searchkit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.6.post4.tar", last modified: Thu May 25 13:52:33 2023, max compression
+gzip compressed data, was "searchkit-0.2.7.tar", last modified: Sat May 27 14:58:08 2023, max compression
```

## Comparing `searchkit-0.2.6.post4.tar` & `searchkit-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6.post4/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.6.post4/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6.post4/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6.post4/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6.post4/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6.post4/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49612 2023-05-25 13:52:19.000000 searchkit-0.2.6.post4/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6.post4/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6.post4/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.7/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4413 2023-05-27 14:58:08.196353 searchkit-0.2.7/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.7/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.7/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.192353 searchkit-0.2.7/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.7/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29362 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.7/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49678 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5773 2023-05-27 14:47:28.000000 searchkit-0.2.7/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4413 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      468 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       21 2023-05-27 14:58:08.000000 searchkit-0.2.7/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       76 2023-05-27 14:58:08.196353 searchkit-0.2.7/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.7/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/tests/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7/tests/__init__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-27 14:58:08.196353 searchkit-0.2.7/tests/unit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.2.7/tests/unit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    39444 2023-05-27 14:47:28.000000 searchkit-0.2.7/tests/unit/test_search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8212 2023-05-24 11:46:12.000000 searchkit-0.2.7/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2526 2023-05-16 10:48:26.000000 searchkit-0.2.7/tests/unit/test_utils.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1331 2023-04-13 19:54:24.000000 searchkit-0.2.7/tests/unit/utils.py
```

### Comparing `searchkit-0.2.6.post4/LICENSE` & `searchkit-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post4/PKG-INFO` & `searchkit-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6.post4
+Version: 0.2.7
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.6.post4/README.md` & `searchkit-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post4/pyproject.toml` & `searchkit-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post4/searchkit/constraints.py` & `searchkit-0.2.7/searchkit/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,19 @@
         property has been defined.
 
         @return: datetime.datetime object
         """
         vals = {}
         for key in ['day', 'month', 'year', 'hours', 'minutes', 'seconds']:
             if hasattr(self, key):
-                vals[key] = getattr(self, key)
+                vals[key.rstrip('s')] = int(getattr(self, key))
             else:
-                vals[key] = self.result.group(key)
+                vals[key.rstrip('s')] = int(self.result.group(key))
 
-        _date = ("{year}-{month}-{day} {hours}:{minutes}:{seconds}".
-                 format(**vals))
-        return datetime.strptime(_date, self.DEFAULT_DATETIME_FORMAT)
+        return datetime(**vals)
 
 
 class ConstraintBase(abc.ABC):
 
     @cached_property
     def id(self):
         """
@@ -385,15 +383,15 @@
 
         mtime = os.path.getmtime(path)
         size = os.path.getsize(path)
         return "{}+{}".format(mtime, size)
 
     def _readchunk(self, fd):
         while True:
-            data = fd.read(self.chunk_size).decode()
+            data = fd.read(self.chunk_size).decode('unicode_escape')
             if data == '':
                 break
 
             yield data
 
     def __getitem__(self, key):
         if not self._primed:
```

### Comparing `searchkit-0.2.6.post4/searchkit/search.py` & `searchkit-0.2.7/searchkit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,19 +655,19 @@
         return int(ret.group(1))
 
 
 class SearchCatalog(object):
 
     def __init__(self, max_logrotate_depth=7):
         self.max_logrotate_depth = max_logrotate_depth
-        self._user_paths = {}
         self._source_ids = {}
         self._search_tags = {}
         self._simple_searches = {}
         self._sequence_searches = {}
+        self._entries = {}
 
     def register(self, search, user_path):
         """
         Register a search against a path.
 
         The same search can be registered against more than one path.
 
@@ -685,18 +685,22 @@
                 self._search_tags[search.tag] = [search.id]
 
         if isinstance(search, SequenceSearchDef):
             self._sequence_searches[search.id] = search
         else:
             self._simple_searches[search.id] = search
 
-        if user_path in self._user_paths:
-            self._user_paths[user_path].append(search.id)
-        else:
-            self._user_paths[user_path] = [search.id]
+        for path in self._expand_path(user_path):
+            if path in self._entries:
+                entry = self._entries[path]
+                entry['searches'].append(search)
+            else:
+                self._entries[path] = {'source_id': self._get_source_id(path),
+                                       'path': path,
+                                       'searches': [search]}
 
     def resolve_from_id(self, id):
         """ Resolve search definition from unique id. """
         if id in self._simple_searches:
             return self._simple_searches[id]
 
         return self._sequence_searches[id]
@@ -772,28 +776,19 @@
             s_id = str(uuid.uuid4())
 
         log.debug("path=%s source_id=%s", path, s_id)
         self._source_ids[s_id] = path
         return s_id
 
     def __len__(self):
-        items = 0
-        for user_path in self._user_paths:
-            items += len(self._expand_path(user_path))
-
-        return items
+        return len(self._entries)
 
     def __iter__(self):
-        for user_path, searches in self._user_paths.items():
-            for path in self._expand_path(user_path):
-                yield {'user_path': user_path,
-                       'path': path,
-                       'source_id': self._get_source_id(path),
-                       'searches': [self.resolve_from_id(id)
-                                    for id in searches]}
+        for entry in self._entries.values():
+            yield entry
 
 
 class SearchTask(object):
 
     def __init__(self, info, constraints_manager, results_queue,
                  results_store):
         self.info = info
@@ -972,23 +967,27 @@
 
     def _run_search(self, fd):
         """
         @param fd: open file descriptor
         """
         self.stats.reset()
         sequence_results = SequenceSearchResults()
-        offset = self.constraints_manager.apply_global(self.info['user_path'],
-                                                       fd)
+        search_ids = set([s.id for s in self.search_defs])
+        offset = self.constraints_manager.apply_global(search_ids, fd)
         log.debug("starting search of %s (offset=%s, pos=%s)", fd.name, offset,
                   fd.tell())
         runnable = {s.id: _runnable
                     for s, _runnable in self.search_defs.items()}
         ln = 0
         # NOTE: line numbers start at 1 hence offset + 1
         for ln, line in enumerate(fd, start=offset + 1):
+            # This could be helpful to show progress for large files
+            if ln % 100000 == 0:
+                log.debug("%s lines searched in %s", ln, fd.name)
+
             self.stats['lines_searched'] += 1
             if type(line) == bytes:
                 line = line.decode("utf-8")
 
             for s_def in self.search_defs:
                 if not runnable[s_def.id]:
                     if not self.constraints_manager.apply_single(s_def, line):
@@ -1119,22 +1118,22 @@
 class SearchConstraintsManager(object):
 
     def __init__(self, search_catalog):
         self.search_catalog = search_catalog
         self.global_constraints = []
         self.global_restrictions = set()
 
-    def apply_global(self, user_path, fd):
+    def apply_global(self, search_ids, fd):
         """ Apply any global constraints to the entire file. """
         offset = 0
         if not self.global_constraints:
             log.debug("no global constraint to apply to %s", fd.name)
             return offset
 
-        if user_path in self.global_restrictions:
+        if self.global_restrictions.intersection(search_ids):
             log.debug("skipping global constraint for %s", fd.name)
             return offset
 
         for c in self.global_constraints:
             log.debug("applying task global constraint %s to %s", c.id,
                       fd.name)
             _offset = c.apply_to_file(fd)
@@ -1194,15 +1193,15 @@
         @param searchdef: a SearchDef or SequenceSearchDef object.
         @param path: path we want to search. this can be a file, dir or glob.
         @param allow_global_constraints: boolean determining whether we want
                                          any global constraints available to be
                                          applied to this path.
         """
         if not allow_global_constraints:
-            self.constraints_manager.global_restrictions.add(path)
+            self.constraints_manager.global_restrictions.add(searchdef.id)
 
         self.catalog.register(searchdef, path)
 
     @property
     def num_parallel_tasks(self):
         if self.max_parallel_tasks == 0:
             cpus = 1  # i.e. no parallelism
@@ -1329,14 +1328,16 @@
         for info in self.catalog:
             task = SearchTask(info,
                               constraints_manager=self.constraints_manager,
                               results_queue=queue,
                               results_store=results_store)
             self.stats.update(task.execute())
 
+        self.stats['jobs_completed'] = 1
+        self.stats['total_jobs'] = 1
         self._purge_results(results, queue, self.stats['results'])
 
     def _run_mp(self, mgr, results, results_store):
         """ Run searches in parallel.
 
         @param mgr: multiprocessing.Manager object
         @param results: SearchResultsCollection object
```

### Comparing `searchkit-0.2.6.post4/searchkit/utils.py` & `searchkit-0.2.7/searchkit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 import fasteners
 import os
 import shelve
+import time
 import _gdbm
 
 from contextlib import ContextDecorator
 from functools import cached_property
 
 from searchkit.log import log
 
@@ -156,14 +157,15 @@
                 try:
                     self._dbs[idx] = shelve.open(path)
                     break
                 except _gdbm.error:
                     log.debug("error opening cache %s - sleeping 10s then "
                               "retrying (attempt %s/%s)", path, attempt,
                               self.max_open_retry)
+                    time.sleep(10)
                     attempt += 1
                     if attempt > self.max_open_retry:
                         raise
 
         return self._dbs[idx]
 
     def get(self, key):
```

### Comparing `searchkit-0.2.6.post4/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.7/searchkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6.post4
+Version: 0.2.7
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

