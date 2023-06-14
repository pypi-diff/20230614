# Comparing `tmp/myl-discovery-0.1.0.tar.gz` & `tmp/myl-discovery-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.1.0.tar", last modified: Tue Jun 13 20:31:25 2023, max compression
+gzip compressed data, was "myl-discovery-0.2.0.tar", last modified: Tue Jun 13 20:45:05 2023, max compression
```

## Comparing `myl-discovery-0.1.0.tar` & `myl-discovery-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41158 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41158 2023-06-13 20:31:25.000000 myl-discovery-0.1.0/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 20:31:25.000000 myl-discovery-0.1.0/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:31:25.000000 myl-discovery-0.1.0/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 20:31:25.000000 myl-discovery-0.1.0/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 20:31:25.000000 myl-discovery-0.1.0/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 20:31:14.000000 myl-discovery-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:31:25.164243 myl-discovery-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41243 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 20:45:05.000000 myl-discovery-0.2.0/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:45:05.577722 myl-discovery-0.2.0/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 20:44:53.000000 myl-discovery-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:45:05.581722 myl-discovery-0.2.0/setup.cfg
```

### Comparing `myl-discovery-0.1.0/.github/workflows/release.yaml` & `myl-discovery-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.1.0/LICENSE` & `myl-discovery-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.1.0/PKG-INFO` & `myl-discovery-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.1.0
+Version: 0.2.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,16 +690,17 @@
 
 ## Installation
 
 ```shell
 pip install myl-discovery
 ```
 
-## Usage:
+## Usage
 
 ```python
 from myldiscovery import autodiscover
 autodiscover("me@example.com")
-# {'server': 'mail.example.com', 'port': 143, 'starttls': True}
+# {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
+#  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
 ```
```

### Comparing `myl-discovery-0.1.0/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.2.0/myl_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.1.0
+Version: 0.2.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,16 +690,17 @@
 
 ## Installation
 
 ```shell
 pip install myl-discovery
 ```
 
-## Usage:
+## Usage
 
 ```python
 from myldiscovery import autodiscover
 autodiscover("me@example.com")
-# {'server': 'mail.example.com', 'port': 143, 'starttls': True}
+# {'imap': {'server': 'mail.example.com', 'port': 993, 'starttls': False},
+#  'smtp': {'server': 'mail.example.com', 'port': 587, 'starttls': False}}
 ```
```

### Comparing `myl-discovery-0.1.0/myldiscovery/__init__.py` & `myl-discovery-0.2.0/myldiscovery/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,46 +40,69 @@
 def autodiscover_txt(domain):
     res = resolve_txt(domain, criteria="^mailconf=")
     if not res:
         return
     return res.split("=")[1]
 
 
-def autodiscover(email_addr):
+def autodiscover(email_addr, srv_only=False):
     domain = email_addr.split("@")[-1]
     if not domain:
         raise ValueError(f"Invalid email address {email_addr}")
 
-    autoconfig = autodiscover_txt(domain)
+    autoconfig = autodiscover_txt(domain) if not srv_only else None
 
     if not autoconfig:
-        srv = resolve_srv(f"_imaps._tcp.{domain}")
+        imap = resolve_srv(f"_imaps._tcp.{domain}")
+        smtp = resolve_srv(f"_submission._tcp.{domain}")
+
         return {
-            "server": srv[0].get("hostname"),
-            "port": int(srv[0].get("port")),
-            # FIXME We might want to "smartly" guess if starttls should be
-            # enabled or not, depending on the port (143 -> starttls, 993 -> no)
-            "starttls": False,
+            "imap": {
+                "server": imap[0].get("hostname"),
+                "port": int(imap[0].get("port")),
+                # FIXME We might want to "smartly" guess if starttls should be
+                # enabled or not, depending on the port:
+                # 143 -> starttls
+                # 993 -> no
+                "starttls": False,
+            },
+            "smtp": {
+                "server": smtp[0].get("hostname"),
+                "port": int(smtp[0].get("port")),
+                # FIXME We might want to "smartly" guess if starttls should be
+                # enabled or not, depending on the port:
+                # 465 -> starttls
+                # 587 -> no
+                "starttls": False,
+            }
         }
 
     res = requests.get(autoconfig)
     res.raise_for_status()
 
     data = xmltodict.parse(res.text)
     imap = (
         data.get("clientConfig", {})
         .get("emailProvider", {})
         .get("incomingServer")
     )
-    # smtp = (
-    #     data.get("clientConfig", {})
-    #     .get("emailProvider", {})
-    #     .get("outgoingServer")
-    # )
+    smtp = (
+        data.get("clientConfig", {})
+        .get("emailProvider", {})
+        .get("outgoingServer")
+    )
 
     assert imap is not None
+    assert smtp is not None
 
     return {
-        "server": imap.get("hostname"),
-        "port": int(imap.get("port")),
-        "starttls": imap.get("socketType") == "STARTTLS",
+        "imap": {
+            "server": imap.get("hostname"),
+            "port": int(imap.get("port")),
+            "starttls": imap.get("socketType") == "STARTTLS",
+        },
+        "smtp": {
+            "server": smtp.get("hostname"),
+            "port": int(smtp.get("port")),
+            "starttls": smtp.get("socketType") == "STARTTLS",
+        },
     }
```

### Comparing `myl-discovery-0.1.0/pyproject.toml` & `myl-discovery-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,11 @@
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "dnspython",
   "requests",
   "xmltodict"
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.black]
 line-length = 79
```

