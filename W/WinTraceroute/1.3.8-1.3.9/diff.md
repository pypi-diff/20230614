# Comparing `tmp/WinTraceroute-1.3.8.tar.gz` & `tmp/WinTraceroute-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.3.8.tar", last modified: Wed Jun 14 00:03:10 2023, max compression
+gzip compressed data, was "WinTraceroute-1.3.9.tar", last modified: Wed Jun 14 00:18:03 2023, max compression
```

## Comparing `WinTraceroute-1.3.8.tar` & `WinTraceroute-1.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:03:10.125415 WinTraceroute-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-06-14 00:03:10.125415 WinTraceroute-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:03:10.121415 WinTraceroute-1.3.8/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 00:03:10.000000 WinTraceroute-1.3.8/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-14 00:02:56.000000 WinTraceroute-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:03:10.125415 WinTraceroute-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:03:10.125415 WinTraceroute-1.3.8/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/traceroute/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-14 00:02:37.000000 WinTraceroute-1.3.8/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:18:03.955777 WinTraceroute-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-06-14 00:18:03.955777 WinTraceroute-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:18:03.955777 WinTraceroute-1.3.9/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 00:18:03.000000 WinTraceroute-1.3.9/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-14 00:17:52.000000 WinTraceroute-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:18:03.955777 WinTraceroute-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:18:03.955777 WinTraceroute-1.3.9/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/traceroute/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-14 00:17:30.000000 WinTraceroute-1.3.9/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.3.8/LICENSE` & `WinTraceroute-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.8/PKG-INFO` & `WinTraceroute-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.8
+Version: 1.3.9
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.8/README.md` & `WinTraceroute-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.8/WinTraceroute.egg-info/PKG-INFO` & `WinTraceroute-1.3.9/WinTraceroute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.8
+Version: 1.3.9
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.8/pyproject.toml` & `WinTraceroute-1.3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.3.8"
+version = "1.3.9"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.3.8"
+current_version = "1.3.9"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.3.8/traceroute/__main__.py` & `WinTraceroute-1.3.9/traceroute/__main__.py`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.8/traceroute/lorem.py` & `WinTraceroute-1.3.9/traceroute/lorem.py`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.8/traceroute/traceroute.py` & `WinTraceroute-1.3.9/traceroute/traceroute.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,28 +175,27 @@
             file=_WINTRACEROUTE_PRINT_FILE)
         print("If you wish to continue the search, consider increasing the `--maxttl`\n" + \
             "  setting on the next try. Besides that, try a different `--module`, maybe?", \
             file=_WINTRACEROUTE_PRINT_FILE)
 
 def summarize_times(times:list,
                     as_string:bool=False):
+    times = [t for t in times if t is not None]
+    
     min = times[0]
     max = times[0]
     sum = times[0]
 
     if len(times) > 1:
         for t in times[1:]:
-            if t == None:
-                continue
-            else:
-                if t < min:
-                    min = t
-                if t > max:
-                    max = t
-                sum += t
+            if t < min:
+                min = t
+            if t > max:
+                max = t
+            sum += t
 
     avg = sum / len(times)
 
     if as_string:
         return "min. %.3f, avg. %.3f, max. %.3f" % (min, avg, max)
     else:
         return (min, avg, max)
```

