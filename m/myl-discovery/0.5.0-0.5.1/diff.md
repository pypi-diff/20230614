# Comparing `tmp/myl-discovery-0.5.0.tar.gz` & `tmp/myl-discovery-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.5.0.tar", last modified: Wed Jun 14 21:23:19 2023, max compression
+gzip compressed data, was "myl-discovery-0.5.1.tar", last modified: Wed Jun 14 21:28:56 2023, max compression
```

## Comparing `myl-discovery-0.5.0.tar` & `myl-discovery-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:28:56.614734 myl-discovery-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:28:56.610734 myl-discovery-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:28:56.610734 myl-discovery-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:28:56.614734 myl-discovery-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:28:56.610734 myl-discovery-0.5.1/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:28:56.000000 myl-discovery-0.5.1/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:28:56.614734 myl-discovery-0.5.1/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-14 21:28:45.000000 myl-discovery-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:28:56.614734 myl-discovery-0.5.1/setup.cfg
```

### Comparing `myl-discovery-0.5.0/.github/workflows/pypi.yaml` & `myl-discovery-0.5.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.0/.github/workflows/release.yaml` & `myl-discovery-0.5.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.0/LICENSE` & `myl-discovery-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.0/PKG-INFO` & `myl-discovery-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.0
+Version: 0.5.1
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.5.0/README.md` & `myl-discovery-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.0/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.5.1/myl_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.5.0
+Version: 0.5.1
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.5.0/myldiscovery/discovery.py` & `myl-discovery-0.5.1/myldiscovery/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
 def check_email_ports(host):
     res = {}
     for port in [25, 465, 587, 993]:
         res[port] = port_check(host, port)
     return res
 
 
-def autodiscover_exchange(email, username, password):
+def autodiscover_exchange(email, password, username=None):
+    if not username:
+        username = email
     creds = Credentials(username=username, password=password)
     account = Account(
         primary_smtp_address=email, credentials=creds, autodiscover=True
     )
     server = account.protocol.server
 
     portscan = check_email_ports(server)
@@ -237,15 +239,15 @@
     autoconfig = autodiscover_txt(domain)
 
     if not autoconfig:
         try:
             return autodiscover_srv(domain)
         except Exception:
             LOGGER.warning("Failed to autodiscover using SRV records")
-            if username and password:
+            if password:
                 LOGGER.info("Trying autodiscover using Exchange credentials")
                 return autodiscover_exchange(email_addr, username, password)
             return
 
     res = requests.get(autoconfig)
     res.raise_for_status()
```

### Comparing `myl-discovery-0.5.0/myldiscovery/main.py` & `myl-discovery-0.5.1/myldiscovery/main.py`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.5.0/pyproject.toml` & `myl-discovery-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 dependencies = [
   "dnspython == 2.3.0",
   "exchangelib == 5.0.3",
   "requests == 2.31.0",
   "rich == 13.4.2",
   "xmltodict == 0.13.0"
 ]
-version = "0.5.0"
+version = "0.5.1"
 
 [project.scripts]
 myl-discovery = "myldiscovery:main"
 
 [tool.black]
 line-length = 79
```

