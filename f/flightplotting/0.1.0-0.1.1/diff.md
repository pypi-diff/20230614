# Comparing `tmp/flightplotting-0.1.0.tar.gz` & `tmp/flightplotting-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplotting-0.1.0.tar", last modified: Thu Mar  2 08:56:59 2023, max compression
+gzip compressed data, was "flightplotting-0.1.1.tar", last modified: Wed Jun 14 09:42:33 2023, max compression
```

## Comparing `flightplotting-0.1.0.tar` & `flightplotting-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-02 08:56:59.668628 flightplotting-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)    35129 2022-12-20 14:21:13.000000 flightplotting-0.1.0/COPYING
--rw-r--r--   0 tom       (1000) tom       (1000)       34 2023-03-01 21:46:59.000000 flightplotting-0.1.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2023-03-02 08:56:59.668628 flightplotting-0.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)       88 2022-12-20 14:21:13.000000 flightplotting-0.1.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-02 08:56:59.668628 flightplotting-0.1.0/flightplotting/
--rw-r--r--   0 tom       (1000) tom       (1000)       66 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-02 08:56:59.668628 flightplotting-0.1.0/flightplotting/data/
--rw-r--r--   0 tom       (1000) tom       (1000)   142015 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/data/ColdDraftF3APlane.obj
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/data/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2976 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/model.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7171 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/plots.py
--rw-r--r--   0 tom       (1000) tom       (1000)      741 2022-12-20 14:21:13.000000 flightplotting-0.1.0/flightplotting/templates.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7118 2022-12-25 09:03:09.000000 flightplotting-0.1.0/flightplotting/traces.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-02 08:56:59.668628 flightplotting-0.1.0/flightplotting.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2023-03-02 08:56:59.000000 flightplotting-0.1.0/flightplotting.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      439 2023-03-02 08:56:59.000000 flightplotting-0.1.0/flightplotting.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-03-02 08:56:59.000000 flightplotting-0.1.0/flightplotting.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2023-03-02 08:56:59.000000 flightplotting-0.1.0/flightplotting.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       15 2023-03-02 08:56:59.000000 flightplotting-0.1.0/flightplotting.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      459 2023-03-02 08:56:59.668628 flightplotting-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      668 2023-03-01 21:47:31.000000 flightplotting-0.1.0/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35129 2023-03-28 15:54:20.000000 flightplotting-0.1.1/COPYING
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-03-28 15:54:20.000000 flightplotting-0.1.1/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      376 2023-06-14 09:42:33.808484 flightplotting-0.1.1/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       88 2023-03-28 15:54:20.000000 flightplotting-0.1.1/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.800484 flightplotting-0.1.1/flightplotting/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       66 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/flightplotting/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)   142015 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/data/ColdDraftF3APlane.obj
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2976 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/model.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7217 2023-06-05 19:30:36.000000 flightplotting-0.1.1/flightplotting/plots.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      741 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/templates.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1298 2023-05-20 13:06:57.000000 flightplotting-0.1.1/flightplotting/titlerenderer.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7118 2023-03-28 15:54:20.000000 flightplotting-0.1.1/flightplotting/traces.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/flightplotting.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      376 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      492 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       57 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 09:42:33.000000 flightplotting-0.1.1/flightplotting.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      459 2023-06-14 09:42:33.808484 flightplotting-0.1.1/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      668 2023-03-28 15:54:20.000000 flightplotting-0.1.1/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:42:33.804484 flightplotting-0.1.1/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      256 2023-03-28 15:54:20.000000 flightplotting-0.1.1/tests/test_traces.py
```

### Comparing `flightplotting-0.1.0/COPYING` & `flightplotting-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.0/flightplotting/data/ColdDraftF3APlane.obj` & `flightplotting-0.1.1/flightplotting/data/ColdDraftF3APlane.obj`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.0/flightplotting/model.py` & `flightplotting-0.1.1/flightplotting/model.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.0/flightplotting/plots.py` & `flightplotting-0.1.1/flightplotting/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,23 @@
 
 def plotdtw(sec: State, manoeuvres, span=3):
     fig = go.Figure()
 
     traces = []#tiptrace(sec, span)
 
     for i, man in enumerate(manoeuvres):
-        
-        name=man.name if hasattr(man, 'name') else "element {}".format(i)
+        name = f"el {i}"
+        if hasattr(man, 'name'):
+            name=man.name
+        elif hasattr(man, "uid"): 
+            name = man.uid
+
         try:
-            
             seg = man.get_data(sec)
-            
-
+        
             traces += ribbon(seg, span, px.colors.qualitative.Alphabet[i], name)
 
             traces.append(go.Scatter3d(
                 x=seg.pos.x, 
                 y=seg.pos.y, 
                 z=seg.pos.z,
                 mode='lines',
```

### Comparing `flightplotting-0.1.0/flightplotting/templates.py` & `flightplotting-0.1.1/flightplotting/templates.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.0/flightplotting/traces.py` & `flightplotting-0.1.1/flightplotting/traces.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.1.0/setup.py` & `flightplotting-0.1.1/setup.py`

 * *Files identical despite different names*

