# Comparing `tmp/wads-0.0.8.tar.gz` & `tmp/wads-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wads-0.0.8.tar", last modified: Mon Nov 30 23:00:52 2020, max compression
+gzip compressed data, was "dist/wads-0.0.9.tar", last modified: Tue Dec  1 21:08:37 2020, max compression
```

## Comparing `wads-0.0.8.tar` & `wads-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-11-30 23:00:52.129591 wads-0.0.8/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       82 2020-09-30 23:55:15.000000 wads-0.0.8/MANIFEST.in
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      452 2020-11-30 23:00:52.129855 wads-0.0.8/PKG-INFO
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       80 2020-10-12 19:02:28.000000 wads-0.0.8/README.md
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      645 2020-11-30 23:00:52.130813 wads-0.0.8/setup.cfg
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      371 2020-10-12 19:36:38.000000 wads-0.0.8/setup.py
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-11-30 23:00:52.122612 wads-0.0.8/wads/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     1121 2020-11-10 22:05:19.000000 wads-0.0.8/wads/__init__.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     1884 2020-09-20 00:20:38.000000 wads-0.0.8/wads/licensing.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)    17368 2020-11-30 22:46:22.000000 wads-0.0.8/wads/pack.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)     7553 2020-11-17 20:46:45.000000 wads-0.0.8/wads/populate.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      356 2020-11-30 22:53:34.000000 wads-0.0.8/wads/trans.py
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)    10148 2020-10-10 00:15:45.000000 wads-0.0.8/wads/util.py
-drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-11-30 23:00:52.128782 wads-0.0.8/wads.egg-info/
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      452 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/PKG-INFO
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)      302 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/SOURCES.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/dependency_links.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)       36 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/entry_points.txt
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/not-zip-safe
--rw-r--r--   0 Thor.Whalen   (502) staff       (20)        5 2020-11-30 23:00:51.000000 wads-0.0.8/wads.egg-info/top_level.txt
+drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-12-01 21:08:37.053979 wads-0.0.9/
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)       82 2020-09-30 23:55:15.000000 wads-0.0.9/MANIFEST.in
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      452 2020-12-01 21:08:37.054239 wads-0.0.9/PKG-INFO
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)       80 2020-10-12 19:02:28.000000 wads-0.0.9/README.md
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      645 2020-12-01 21:08:37.055165 wads-0.0.9/setup.cfg
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      371 2020-10-12 19:36:38.000000 wads-0.0.9/setup.py
+drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-12-01 21:08:37.047550 wads-0.0.9/wads/
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)     1121 2020-11-10 22:05:19.000000 wads-0.0.9/wads/__init__.py
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)     1884 2020-09-20 00:20:38.000000 wads-0.0.9/wads/licensing.py
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)    17449 2020-12-01 19:33:01.000000 wads-0.0.9/wads/pack.py
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)     7553 2020-11-17 20:46:45.000000 wads-0.0.9/wads/populate.py
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      815 2020-12-01 16:22:28.000000 wads-0.0.9/wads/trans.py
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)    10148 2020-10-10 00:15:45.000000 wads-0.0.9/wads/util.py
+drwxr-xr-x   0 Thor.Whalen   (502) staff       (20)        0 2020-12-01 21:08:37.053031 wads-0.0.9/wads.egg-info/
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      452 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/PKG-INFO
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)      302 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/SOURCES.txt
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/dependency_links.txt
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)       36 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/entry_points.txt
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)        1 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/not-zip-safe
+-rw-r--r--   0 Thor.Whalen   (502) staff       (20)        5 2020-12-01 21:08:36.000000 wads-0.0.9/wads.egg-info/top_level.txt
```

### Comparing `wads-0.0.8/setup.cfg` & `wads-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wads
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/i2mint/wads
 platforms = any
 description_file = README.md
 long-description = file: README.md
 long_description_content_type = text/markdown
 root_url = https://github.com/i2mint
 description = Tools for documentation and packaging
```

### Comparing `wads-0.0.8/wads/__init__.py` & `wads-0.0.9/wads/__init__.py`

 * *Files identical despite different names*

### Comparing `wads-0.0.8/wads/licensing.py` & `wads-0.0.9/wads/licensing.py`

 * *Files identical despite different names*

### Comparing `wads-0.0.8/wads/pack.py` & `wads-0.0.9/wads/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,18 +249,21 @@
         section=METADATA_SECTION,
 ):
     assert isinstance(pkg_dir, Path), \
         "It doesn't look like pkg_dir is a path. Did you perhaps invert pkg_dir and postproc order"
     pkg_dir = _get_pkg_dir(pkg_dir)
     config_filepath = pjoin(pkg_dir, CONFIG_FILE_NAME)
     c = ConfigParser()
-    c.read_file(open(config_filepath, 'r'))
-    d = dict(c[section])
-    if postproc:
-        d = dict(postproc(d))
+    if os.path.isfile(config_filepath):
+        c.read_file(open(config_filepath, 'r'))
+        d = dict(c[section])
+        if postproc:
+            d = dict(postproc(d))
+    else:
+        d = {}
     return d
 
 
 def write_configs(
         pkg_dir: Path,
         configs,
         preproc=preprocess_ini_section_items,
```

### Comparing `wads-0.0.8/wads/populate.py` & `wads-0.0.9/wads/populate.py`

 * *Files identical despite different names*

### Comparing `wads-0.0.8/wads/util.py` & `wads-0.0.9/wads/util.py`

 * *Files identical despite different names*

