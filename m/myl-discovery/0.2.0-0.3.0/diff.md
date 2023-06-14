# Comparing `tmp/myl-discovery-0.2.0.tar.gz` & `tmp/myl-discovery-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.2.0.tar", last modified: Tue Jun 13 20:45:05 2023, max compression
+gzip compressed data, was "myl-discovery-0.3.0.tar", last modified: Wed Jun 14 07:37:46 2023, max compression
```

## Comparing `myl-discovery-0.2.0.tar` & `myl-discovery-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 07:37:46.000000 myl-discovery-0.3.0/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 07:37:31.000000 myl-discovery-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:37:46.917632 myl-discovery-0.3.0/setup.cfg
```

### Comparing `myl-discovery-0.2.0/.github/workflows/release.yaml` & `myl-discovery-0.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.2.0/LICENSE` & `myl-discovery-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.2.0/PKG-INFO` & `myl-discovery-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.2.0
+Version: 0.3.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.2.0/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.3.0/myl_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.2.0
+Version: 0.3.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.2.0/myldiscovery/__init__.py` & `myl-discovery-0.3.0/myldiscovery/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 "server": smtp[0].get("hostname"),
                 "port": int(smtp[0].get("port")),
                 # FIXME We might want to "smartly" guess if starttls should be
                 # enabled or not, depending on the port:
                 # 465 -> starttls
                 # 587 -> no
                 "starttls": False,
-            }
+            },
         }
 
     res = requests.get(autoconfig)
     res.raise_for_status()
 
     data = xmltodict.parse(res.text)
     imap = (
```

### Comparing `myl-discovery-0.2.0/pyproject.toml` & `myl-discovery-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,17 @@
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "dnspython",
   "requests",
+  "rich",
   "xmltodict"
 ]
-version = "0.2.0"
+version = "0.3.0"
+
+[project.scripts]
+myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

