# Comparing `tmp/ardupilot_log_reader-0.1.0.tar.gz` & `tmp/ardupilot_log_reader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardupilot_log_reader-0.1.0.tar", last modified: Wed Mar  1 14:09:11 2023, max compression
+gzip compressed data, was "ardupilot_log_reader-0.1.1.tar", last modified: Wed Jun 14 09:39:29 2023, max compression
```

## Comparing `ardupilot_log_reader-0.1.0.tar` & `ardupilot_log_reader-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 14:09:11.712392 ardupilot_log_reader-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1002 2023-03-01 14:09:11.712392 ardupilot_log_reader-0.1.0/PKG-INFO
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 14:09:11.712392 ardupilot_log_reader-0.1.0/ardupilot_log_reader/
--rw-r--r--   0 tom       (1000) tom       (1000)       29 2022-12-20 14:21:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7671 2022-12-20 14:21:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader/reader.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 14:09:11.712392 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1002 2023-03-01 14:09:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      301 2023-03-01 14:09:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-03-01 14:09:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       30 2023-03-01 14:09:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       21 2023-03-01 14:09:11.000000 ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      455 2023-03-01 14:09:11.712392 ardupilot_log_reader-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      666 2023-03-01 14:06:34.000000 ardupilot_log_reader-0.1.0/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1002 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      718 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.1.1/ReadMe.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/ardupilot_log_reader/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       29 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7685 2023-05-18 15:06:39.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader/reader.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1002 2023-06-14 09:39:29.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      335 2023-06-14 09:39:29.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:39:29.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       30 2023-06-14 09:39:29.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       21 2023-06-14 09:39:29.000000 ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      455 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      666 2023-03-28 15:54:18.000000 ardupilot_log_reader-0.1.1/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:39:29.579241 ardupilot_log_reader-0.1.1/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2018 2023-05-18 15:02:58.000000 ardupilot_log_reader-0.1.1/tests/test_ardupilot.py
```

### Comparing `ardupilot_log_reader-0.1.0/PKG-INFO` & `ardupilot_log_reader-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardupilot_log_reader
-Version: 0.1.0
+Version: 0.1.1
 Summary: module to read ardupilot binary logs to memory
 Home-page: https://github.com/PyFlightCoach/ardupilot_log_reader
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 
 # Ardupilot Log Reader
```

### Comparing `ardupilot_log_reader-0.1.0/ardupilot_log_reader/reader.py` & `ardupilot_log_reader-0.1.1/ardupilot_log_reader/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,21 +82,14 @@
         filename = bin_file
         mlog = mavutil.mavlink_connection(filename, planner_format=planner,
                                   notimestamps=no_timestamps,
                                   robust_parsing=robust,
                                   dialect=dialect,
                                   zero_time_base=zero_time_base)
 
-        ext = os.path.splitext(filename)[1]
-        isbin = ext in ['.bin', '.BIN', '.px4log']
-        islog = ext in ['.log', '.LOG'] # NOTE: "islog" does not mean a tlog
-        istlog = ext in ['.tlog', '.TLOG']
-
-        # Track types found
-        available_types = set()
 
         types = list(set(types + ['PARM']))
 
         if nottypes is not None:
             nottypes = nottypes.split(',')
 
         def match_type(mtype, patterns):
@@ -130,65 +123,66 @@
                 continue
             if source_system is not None and source_system != m.get_srcSystem():
                 continue
             if source_component is not None and source_component != m.get_srcComponent():
                 continue
             if link is not None and link != m._link:
                 continue
-
             if types is not None and m.get_type() != 'BAD_DATA' and not match_type(m.get_type(), types):
                 continue
-
             if nottypes is not None and match_type(m.get_type(), nottypes):
                 continue
 
             # Ignore BAD_DATA messages is the user requested or if they're because of a bad prefix. The
             # latter case is normally because of a mismatched MAVLink version.
             if m.get_type() == 'BAD_DATA':
                 continue
+            
+            key = f"{m.get_type()}_{str(m.C)}" if hasattr(m, "C") else m.get_type()
 
-            # Grab the timestamp.
-            timestamp = getattr(m, '_timestamp', 0.0)
-
-            try:
-                dfs_dicts[m.get_type()]
-            except KeyError:
-                dfs_dicts[m.get_type()] = {}
-                dfs_dicts[m.get_type()]['timestamp'] = []
+            if not key in dfs_dicts:
+                dfs_dicts[key] = {}
+                dfs_dicts[key]['timestamp'] = []
                 for field in m.get_fieldnames():
-                    dfs_dicts[m.get_type()][field] = []
+                    dfs_dicts[key][field] = []
             
-            dfs_dicts[m.get_type()]['timestamp'].append( getattr(m,'_timestamp', 0.0) )
+            dfs_dicts[key]['timestamp'].append( getattr(m,'_timestamp', 0.0) )
             for field in m.get_fieldnames():
-                dfs_dicts[m.get_type()][field].append( getattr(m,field) )
-
-        self._dfs = {}
-        for msgType in dfs_dicts.keys():
-            self._dfs[msgType] = pd.DataFrame(data=dfs_dicts[msgType])
-
-            new_cols = []
-            for val in self._dfs[msgType].columns:
-                if val == 'timestamp':
-                    new_cols.append(val)
-                else:
-                    new_cols.append(msgType + val)
-
-            self._dfs[msgType].columns = new_cols
-
+                dfs_dicts[key][field].append( getattr(m,field) )
+        
         mlog.filehandle.close()
 
-    @property
-    def dfs(self):
-        return self._dfs
-    
-    @property
-    def parms(self):
-        if not self._parms:
-            self._parms = self.dfs['PARM'].set_index('PARMName')['PARMValue'].to_dict()
-        return self._parms
+        self._dfs = {}
+        self.dfs = {}
+        for k, v in dfs_dicts.items():
+            self._dfs[k] = pd.DataFrame(v)
+            core, name = Ardupilot._get_core(k)
+            self._dfs[k].columns =[val if val == "timestamp" else name + val for val in v.keys()]
+            #for back compatibility
+            if not core:
+                self.dfs[k.split("_")[0]] = self._dfs[k]
+        
+        self.parms = self.dfs['PARM'].set_index('PARMName')['PARMValue'].to_dict()
+
+
+    @staticmethod
+    def _get_core(k):
+        """returns the core if it exists, otherwise None"""
+        try:
+            spl = k.split("_")
+            assert len(spl) == 2
+            return int(spl[1]), spl[0]
+        except Exception as e:
+            return None, k
+
+    def __getattr__(self, name):
+        if name in self.dfs:
+            return self.dfs[name]
+        elif name in self._dfs:
+            return self._dfs[name]
 
     def join_logs(self, titles):
         """Merge logs on timestamp 
         """
         available_titles = [title for title in titles if title in self.dfs.keys()]
         joined_log = self.dfs[available_titles[0]]
         for title in available_titles[1:]:
@@ -203,8 +197,11 @@
             )
             l1 = len(joined_log)
             if l1 < l0:
                 pass
         return joined_log
 
     def full_df(self):
-        return self.join_logs(list(self.dfs.keys())) # TODO remove PARA from here.
+        dfnames = list(self.dfs.keys())
+        dfnames.remove("PARM")
+        dfnames = [dfn for dfn in dfnames if Ardupilot._get_core(dfn) is None]
+        return self.join_logs(dfnames)
```

### Comparing `ardupilot_log_reader-0.1.0/ardupilot_log_reader.egg-info/PKG-INFO` & `ardupilot_log_reader-0.1.1/ardupilot_log_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardupilot-log-reader
-Version: 0.1.0
+Version: 0.1.1
 Summary: module to read ardupilot binary logs to memory
 Home-page: https://github.com/PyFlightCoach/ardupilot_log_reader
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 
 # Ardupilot Log Reader
```

### Comparing `ardupilot_log_reader-0.1.0/setup.py` & `ardupilot_log_reader-0.1.1/setup.py`

 * *Files identical despite different names*

