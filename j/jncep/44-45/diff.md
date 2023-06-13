# Comparing `tmp/jncep-44.tar.gz` & `tmp/jncep-45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jncep-44.tar", last modified: Tue Jun 13 15:14:05 2023, max compression
+gzip compressed data, was "dist/jncep-45.tar", last modified: Tue Jun 13 22:33:02 2023, max compression
```

## Comparing `jncep-44.tar` & `jncep-45.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/
--rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 15:14:05.000000 jncep-44/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep/
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-13 15:13:39.000000 jncep-44/jncep/jnclabs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-06-13 15:13:39.000000 jncep-44/jncep/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-06-13 15:13:39.000000 jncep-44/jncep/jncweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     6552 2023-06-13 15:13:39.000000 jncep-44/jncep/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    20298 2023-06-13 15:13:39.000000 jncep-44/jncep/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-06-13 15:13:39.000000 jncep-44/jncep/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-13 15:13:39.000000 jncep-44/jncep/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-06-13 15:13:39.000000 jncep-44/jncep/trio_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-06-13 15:13:39.000000 jncep-44/jncep/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-06-13 15:13:39.000000 jncep-44/jncep/spec.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-13 15:13:39.000000 jncep-44/jncep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     7765 2023-06-13 15:13:39.000000 jncep-44/jncep/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-13 15:13:39.000000 jncep-44/jncep/jncep.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-13 15:14:05.000000 jncep-44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-13 15:13:39.000000 jncep-44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)    31100 2023-06-13 15:13:39.000000 jncep-44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/
+-rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 22:33:02.000000 jncep-45/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep/
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-13 22:32:43.000000 jncep-45/jncep/jnclabs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-06-13 22:32:43.000000 jncep-45/jncep/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-06-13 22:32:43.000000 jncep-45/jncep/jncweb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6552 2023-06-13 22:32:43.000000 jncep-45/jncep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20298 2023-06-13 22:32:43.000000 jncep-45/jncep/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-06-13 22:32:43.000000 jncep-45/jncep/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-13 22:32:43.000000 jncep-45/jncep/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-06-13 22:32:43.000000 jncep-45/jncep/trio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-06-13 22:32:43.000000 jncep-45/jncep/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-06-13 22:32:43.000000 jncep-45/jncep/spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-13 22:32:43.000000 jncep-45/jncep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-06-13 22:32:43.000000 jncep-45/jncep/cli/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7771 2023-06-13 22:32:43.000000 jncep-45/jncep/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-13 22:32:43.000000 jncep-45/jncep/jncep.py
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-13 22:33:02.000000 jncep-45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-13 22:32:43.000000 jncep-45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 22:33:02.000000 jncep-45/jncep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    31100 2023-06-13 22:32:43.000000 jncep-45/README.md
```

### Comparing `jncep-44/PKG-INFO` & `jncep-45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 44
+Version: 45
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
```

### Comparing `jncep-44/jncep/jnclabs.py` & `jncep-45/jncep/jnclabs.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/epub.py` & `jncep-45/jncep/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/jncweb.py` & `jncep-45/jncep/jncweb.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/utils.py` & `jncep-45/jncep/utils.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/update.py` & `jncep-45/jncep/update.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/core.py` & `jncep-45/jncep/core.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/model.py` & `jncep-45/jncep/model.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/trio_utils.py` & `jncep-45/jncep/trio_utils.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/config.py` & `jncep-45/jncep/config.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/spec.py` & `jncep-45/jncep/spec.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/cli/base.py` & `jncep-45/jncep/cli/base.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/cli/epub.py` & `jncep-45/jncep/cli/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/cli/update.py` & `jncep-45/jncep/cli/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "-j",
     "--jnc-managed",
     "is_jnc_managed",
     is_flag=True,
     help=(
         "Flag to indicate whether to use the series followed on the J-Novel Club "
         "website as the tracking reference for updating (equivalent to "
-        "running 'update --sync', 'track sync --delete' and finally 'update')"
+        "running 'track sync --delete --beginning' followed by 'update')"
     ),
 )
 @click.option(
     "-w",
     "--whole",
     "is_whole_volume",
     is_flag=True,
@@ -102,42 +102,29 @@
     is_use_events,
     is_jnc_managed,
 ):
 
     async with core.JNCEPSession(email, password) as session:
         if is_jnc_managed:
             # run the equivalent of:
-            # update --sync
-            # track sync --delete
+            # track sync --delete --beginning
             # update
 
-            # new series will be updated from the beginning
-            console.info("[important]update --sync[/]")
-            # keep the params to the update command
-            params_forward = {}
-            for param in ctx.params:
-                if param == "is_jnc_managed":
-                    continue
-                params_forward[param] = ctx.params[param]
-            params_forward["is_sync"] = True
+            # prune series that are not followed anymore + track from beginning
+            console.info("[important]track sync --delete --beginning[/]")
             # run_sync because we are already in a trio context so we wouldn't be able
             # to nest another trio.run (inside the click command) othwerwise
             await trio.to_thread.run_sync(
-                partial(ctx.invoke, update_tracked, **params_forward)
-            )
-
-            # prune series that are not followed anymore
-            console.info("[important]track sync --delete[/]")
-            await trio.to_thread.run_sync(
                 partial(
                     ctx.invoke,
                     sync_series,
                     email=email,
                     password=password,
                     is_delete=True,
+                    is_beginning=True,
                 )
             )
 
             # after that, let update run normally
             console.info("[important]update[/]")
             # set sync to False because doesn't make sense to sync again
             # TODO log to the user ?
```

### Comparing `jncep-44/jncep/cli/options.py` & `jncep-45/jncep/cli/options.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/cli/config.py` & `jncep-45/jncep/cli/config.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/cli/track.py` & `jncep-45/jncep/cli/track.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep/track.py` & `jncep-45/jncep/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             "series_id": series.series_id,
             "last_check_date": utils.isoformat_with_z(session.now),
         }
     )
 
 
 async def sync_series_forward(
-    session, follows, tracked_series, is_delete, is_beginning
+    session, follows, tracked_series, is_delete, is_beginning=False
 ):
     # sync local tracked series based on remote follows
     new_synced = []
     del_synced = []
 
     async def do_track(jnc_resource):
         series_id = await core.resolve_series(session, jnc_resource)
```

### Comparing `jncep-44/jncep/jncep.py` & `jncep-45/jncep/jncep.py`

 * *Files identical despite different names*

### Comparing `jncep-44/setup.py` & `jncep-45/setup.py`

 * *Files identical despite different names*

### Comparing `jncep-44/jncep.egg-info/PKG-INFO` & `jncep-45/jncep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 44
+Version: 45
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
```

### Comparing `jncep-44/jncep.egg-info/SOURCES.txt` & `jncep-45/jncep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jncep-44/README.md` & `jncep-45/README.md`

 * *Files identical despite different names*

