# Comparing `tmp/myl-discovery-0.4.0.tar.gz` & `tmp/myl-discovery-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-discovery-0.4.0.tar", last modified: Wed Jun 14 13:32:05 2023, max compression
+gzip compressed data, was "myl-discovery-0.5.0.tar", last modified: Wed Jun 14 21:23:19 2023, max compression
```

## Comparing `myl-discovery-0.4.0.tar` & `myl-discovery-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/myl_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 13:32:05.000000 myl-discovery-0.4.0/myl_discovery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/myldiscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/myldiscovery/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 13:31:56.000000 myl-discovery-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:32:05.962333 myl-discovery-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/myl_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44811 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:23:19.000000 myl-discovery-0.5.0/myl_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/myldiscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2016 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/myldiscovery/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-14 21:23:08.000000 myl-discovery-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:23:19.474144 myl-discovery-0.5.0/setup.cfg
```

### Comparing `myl-discovery-0.4.0/.github/workflows/release.yaml` & `myl-discovery-0.5.0/.github/workflows/pypi.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Upload Python Package
+name: Python package
 
 on:
   release:
     types: [created]
   push:
     tags:
       - '*'
```

### Comparing `myl-discovery-0.4.0/LICENSE` & `myl-discovery-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.4.0/PKG-INFO` & `myl-discovery-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.4.0
+Version: 0.5.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.4.0/README.md` & `myl-discovery-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `myl-discovery-0.4.0/myl_discovery.egg-info/PKG-INFO` & `myl-discovery-0.5.0/myl_discovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl-discovery
-Version: 0.4.0
+Version: 0.5.0
 Summary: email autodiscovery
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-discovery-0.4.0/myldiscovery/discovery.py` & `myl-discovery-0.5.0/myldiscovery/discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 import os
 import re
 import shutil
+import socket
 
 import dns.resolver
 import requests
 import xmltodict
+from exchangelib import Account, Credentials
 
 LOGGER = logging.getLogger(__name__)
 
 
 def is_termux():
     if os.getenv("TERMUX_VERSION"):
         return True
@@ -166,26 +168,87 @@
             # 465 -> starttls
             # 587 -> no
             "starttls": False,
         },
     }
 
 
-def autodiscover(email_addr, srv_only=False):
+def port_check(host, port):
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    result = sock.connect_ex((host, int(port)))
+    sock.close()
+    return result == 0
+
+
+def check_email_ports(host):
+    res = {}
+    for port in [25, 465, 587, 993]:
+        res[port] = port_check(host, port)
+    return res
+
+
+def autodiscover_exchange(email, username, password):
+    creds = Credentials(username=username, password=password)
+    account = Account(
+        primary_smtp_address=email, credentials=creds, autodiscover=True
+    )
+    server = account.protocol.server
+
+    portscan = check_email_ports(server)
+    LOGGER.info(f"Port scan results: {portscan}")
+
+    imap_port = imap_starttls = None
+    if portscan.get(993):
+        imap_port = 993
+        imap_starttls = False
+    elif portscan.get(143):
+        imap_port = 143
+        imap_starttls = True
+
+    smtp_port = smtp_starttls = None
+    if portscan.get(465):
+        smtp_port = 465
+        smtp_starttls = False
+    elif portscan.get(587):
+        smtp_port = 587
+        smtp_starttls = True
+
+    return {
+        "imap": {
+            "server": server,
+            "port": imap_port,
+            "starttls": imap_starttls,
+        },
+        "smtp": {
+            "server": server,
+            "port": smtp_port,
+            "starttls": smtp_starttls,
+        },
+    }
+
+
+def autodiscover(email_addr, srv_only=False, username=None, password=None):
     domain = email_addr.split("@")[-1]
     if not domain:
         raise ValueError(f"Invalid email address {email_addr}")
 
     if srv_only:
         return autodiscover_srv(domain)
 
     autoconfig = autodiscover_txt(domain)
 
     if not autoconfig:
-        return autodiscover_srv(domain)
+        try:
+            return autodiscover_srv(domain)
+        except Exception:
+            LOGGER.warning("Failed to autodiscover using SRV records")
+            if username and password:
+                LOGGER.info("Trying autodiscover using Exchange credentials")
+                return autodiscover_exchange(email_addr, username, password)
+            return
 
     res = requests.get(autoconfig)
     res.raise_for_status()
 
     try:
         return parse_autoconfig(res.text)
     except Exception:
```

### Comparing `myl-discovery-0.4.0/myldiscovery/main.py` & `myl-discovery-0.5.0/myldiscovery/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 LOGGER = logging.getLogger(__name__)
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-j", "--json", action="store_true", default=False)
     parser.add_argument("-d", "--debug", action="store_true", default=False)
+    parser.add_argument(
+        "-u", "--username", required=False, help="Username (Exchange only)"
+    )
+    parser.add_argument(
+        "-p", "--password", required=False, help="Password (Exchange only)"
+    )
     parser.add_argument("EMAIL")
     return parser.parse_args()
 
 
 def main():
     console = Console()
     args = parse_args()
@@ -29,15 +35,17 @@
     logging.basicConfig(
         handlers=[RichHandler(console=console, show_time=False)],
         level=logging.DEBUG if args.debug else logging.INFO,
     )
     LOGGER.debug(args)
 
     try:
-        res = autodiscover(args.EMAIL)
+        res = autodiscover(
+            args.EMAIL, username=args.username, password=args.password
+        )
         if args.json:
             print_json(data=res)
         else:
             table = Table(
                 expand=True,
                 show_header=True,
                 header_style="bold",
```

