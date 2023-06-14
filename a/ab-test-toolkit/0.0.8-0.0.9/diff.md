# Comparing `tmp/ab-test-toolkit-0.0.8.tar.gz` & `tmp/ab-test-toolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-toolkit-0.0.8.tar", last modified: Wed Jun 14 07:44:18 2023, max compression
+gzip compressed data, was "ab-test-toolkit-0.0.9.tar", last modified: Wed Jun 14 07:49:21 2023, max compression
```

## Comparing `ab-test-toolkit-0.0.8.tar` & `ab-test-toolkit-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:44:18.009104 ab-test-toolkit-0.0.8/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.8/LICENSE
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.8/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-14 07:44:18.009009 ab-test-toolkit-0.0.8/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5301 2023-06-13 11:53:01.000000 ab-test-toolkit-0.0.8/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:44:18.007964 ab-test-toolkit-0.0.8/ab_test_toolkit/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     6337 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1076 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/analyze.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4453 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7329 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     8370 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)    11330 2023-06-14 07:35:28.000000 ab-test-toolkit-0.0.8/ab_test_toolkit/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:44:18.008834 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-14 07:44:17.000000 ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-14 07:32:13.000000 ab-test-toolkit-0.0.8/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-14 07:44:18.009137 ab-test-toolkit-0.0.8/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.8/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:49:21.214077 ab-test-toolkit-0.0.9/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.9/LICENSE
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.9/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-14 07:49:21.213966 ab-test-toolkit-0.0.9/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5301 2023-06-13 11:53:01.000000 ab-test-toolkit-0.0.9/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:49:21.212866 ab-test-toolkit-0.0.9/ab_test_toolkit/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     6337 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1076 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/analyze.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     4453 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7329 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     8370 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)    11651 2023-06-14 07:46:30.000000 ab-test-toolkit-0.0.9/ab_test_toolkit/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-14 07:49:21.213784 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-14 07:49:21.000000 ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-14 07:47:23.000000 ab-test-toolkit-0.0.9/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-14 07:49:21.214112 ab-test-toolkit-0.0.9/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.9/setup.py
```

### Comparing `ab-test-toolkit-0.0.8/LICENSE` & `ab-test-toolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/PKG-INFO` & `ab-test-toolkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-toolkit
```

### Comparing `ab-test-toolkit-0.0.8/README.md` & `ab-test-toolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/_modidx.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/_modidx.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/analyze.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/analyze.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/generator.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/generator.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/plotting.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/power.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit/wrappers.py` & `ab-test-toolkit-0.0.9/ab_test_toolkit/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,27 @@
         ),
         row=2,
         col=1,
     )
     fig.add_trace(
         go.Scatter(
             x=plot_df["size"],
+            y=[0.05]*len(plot_df["size"]),
+            mode=mode,
+            name=f"p=0.05",
+            line_color="gray",
+            line_dash='dash',
+            legendgroup="2",
+        ),
+        row=2,
+        col=1,
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=plot_df["size"],
             y=multiply_ate * plot_df[f"ate"],
             mode=mode,
             name=f"ate",
             line_color="#1f77b4",
             legendgroup="2",
         ),
         row=2,
@@ -164,14 +177,15 @@
         col=1,
     )
     fig.update_yaxes(
         title_text="pvalue",
         secondary_y=False,
         row=2,
         col=1,
+        range=[0,1]
     )
     fig.update_yaxes(
         title_text="Conversions",
         secondary_y=False,
         row=1,
         col=1,
     )
```

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/PKG-INFO` & `ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-toolkit
```

### Comparing `ab-test-toolkit-0.0.8/ab_test_toolkit.egg-info/SOURCES.txt` & `ab-test-toolkit-0.0.9/ab_test_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.8/settings.ini` & `ab-test-toolkit-0.0.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-toolkit
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_toolkit
```

### Comparing `ab-test-toolkit-0.0.8/setup.py` & `ab-test-toolkit-0.0.9/setup.py`

 * *Files identical despite different names*

