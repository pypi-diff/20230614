# Comparing `tmp/myl-0.8.3.tar.gz` & `tmp/myl-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.3.tar", last modified: Tue Jun 13 20:47:53 2023, max compression
+gzip compressed data, was "myl-0.8.4.tar", last modified: Wed Jun 14 17:13:06 2023, max compression
```

## Comparing `myl-0.8.3.tar` & `myl-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:47:41.000000 myl-0.8.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:47:41.000000 myl-0.8.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 20:47:41.000000 myl-0.8.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:47:41.000000 myl-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:47:41.000000 myl-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:47:53.636262 myl-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 20:47:41.000000 myl-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-13 20:47:41.000000 myl-0.8.3/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 20:47:41.000000 myl-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:47:53.636262 myl-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.744591 myl-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 17:12:52.000000 myl-0.8.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-14 17:12:52.000000 myl-0.8.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 17:12:52.000000 myl-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 17:12:52.000000 myl-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-06-14 17:13:06.744591 myl-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-14 17:12:52.000000 myl-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:13:06.740591 myl-0.8.4/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 17:13:06.000000 myl-0.8.4/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-14 17:12:52.000000 myl-0.8.4/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 17:12:52.000000 myl-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:13:06.744591 myl-0.8.4/setup.cfg
```

### Comparing `myl-0.8.3/.github/workflows/release.yaml` & `myl-0.8.4/.github/workflows/pypi.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Upload Python Package
+name: Python Package
 
 on:
   release:
     types: [created]
   push:
     tags:
       - '*'
```

### Comparing `myl-0.8.3/LICENSE` & `myl-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.3/PKG-INFO` & `myl-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.3
+Version: 0.8.4
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,21 +680,97 @@
         
 Keywords: imap,email
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# myl
+# 📧 myl
 
-## Installation
+myl is a dead simple IMAP CLI client hosted on GitHub at
+https://github.com/pschmitt/myl
 
-```shell
+## 📝 Description
+
+myl is a command-line interface client for IMAP, designed to provide a
+straightforward way to interact with IMAP servers.
+
+## ⭐ Features
+
+- Simple command-line interface
+- Support for various IMAP operations
+- Autodiscovery of the required server and port
+- Support for Google IMAP settings
+- Fetch a specific number of messages
+- Mark messages as seen
+- Fetch messages from a specific folder
+- Search for specific strings in messages
+- Output HTML email
+- Output raw email
+- Fetch a specific mail by ID
+- Fetch a specific attachment (outputs to stdout)
+
+## 🚀 Installation
+
+To install myl, follow these steps:
+
+```bash
 pipx install myl
 ```
 
+## 🛠️ Usage
 
-## Usage
+Here's how you can use myl:
 
-```shell
+```bash
 myl --help
 ```
+
+This command will display the help information for the `myl` command.
+
+Here are some examples of using flags with the `myl` command:
+
+```bash
+# Connect to an IMAP server
+myl --server imap.example.com --username $username --password "$password"
+
+# Use Google IMAP settings
+myl --google --username "$username" --password "$password"
+
+# Autodiscovery of the required server and port
+myl --auto --username "$username" --password "$password"
+
+# Fetch a specific number of messages
+myl --count 5 --username "$username" --password "$password"
+
+# Mark messages as seen
+myl --mark-seen --username "$username" --password "$password"
+
+# Fetch messages from a specific folder
+myl --folder "INBOX" --username "$username" --password "$password"
+
+# Search for specific strings in messages
+myl --search "important" --username "$username" --password "$password"
+
+# Show raw email
+myl --raw --username "$username" --password "$password"
+
+# Fetch a specific mail ID
+myl --username "$username" --password "$password" "$MAILID"
+
+# Show HTML
+myl --html --username "$username" --password "$password" "$MAILID"
+
+# raw email
+myl --raw --username "$username" --password "$password" "$MAILID" > email.eml
+
+# Fetch a specific attachment (outputs to stdout)
+myl --username "$username" --password "$password" "$MAILID" "$ATT" > att.txt
+```
+
+Please replace `imap.example.com`, `$username`, `$password`, `$MAILID`,
+and `$ATT` with your actual IMAP server details, username, password,
+mail ID, and attachment name.
+
+## 📜 License
+
+This project is licensed under the GPL-3.0 license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `myl-0.8.3/myl.egg-info/PKG-INFO` & `myl-0.8.4/myl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.3
+Version: 0.8.4
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,21 +680,97 @@
         
 Keywords: imap,email
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# myl
+# 📧 myl
 
-## Installation
+myl is a dead simple IMAP CLI client hosted on GitHub at
+https://github.com/pschmitt/myl
 
-```shell
+## 📝 Description
+
+myl is a command-line interface client for IMAP, designed to provide a
+straightforward way to interact with IMAP servers.
+
+## ⭐ Features
+
+- Simple command-line interface
+- Support for various IMAP operations
+- Autodiscovery of the required server and port
+- Support for Google IMAP settings
+- Fetch a specific number of messages
+- Mark messages as seen
+- Fetch messages from a specific folder
+- Search for specific strings in messages
+- Output HTML email
+- Output raw email
+- Fetch a specific mail by ID
+- Fetch a specific attachment (outputs to stdout)
+
+## 🚀 Installation
+
+To install myl, follow these steps:
+
+```bash
 pipx install myl
 ```
 
+## 🛠️ Usage
 
-## Usage
+Here's how you can use myl:
 
-```shell
+```bash
 myl --help
 ```
+
+This command will display the help information for the `myl` command.
+
+Here are some examples of using flags with the `myl` command:
+
+```bash
+# Connect to an IMAP server
+myl --server imap.example.com --username $username --password "$password"
+
+# Use Google IMAP settings
+myl --google --username "$username" --password "$password"
+
+# Autodiscovery of the required server and port
+myl --auto --username "$username" --password "$password"
+
+# Fetch a specific number of messages
+myl --count 5 --username "$username" --password "$password"
+
+# Mark messages as seen
+myl --mark-seen --username "$username" --password "$password"
+
+# Fetch messages from a specific folder
+myl --folder "INBOX" --username "$username" --password "$password"
+
+# Search for specific strings in messages
+myl --search "important" --username "$username" --password "$password"
+
+# Show raw email
+myl --raw --username "$username" --password "$password"
+
+# Fetch a specific mail ID
+myl --username "$username" --password "$password" "$MAILID"
+
+# Show HTML
+myl --html --username "$username" --password "$password" "$MAILID"
+
+# raw email
+myl --raw --username "$username" --password "$password" "$MAILID" > email.eml
+
+# Fetch a specific attachment (outputs to stdout)
+myl --username "$username" --password "$password" "$MAILID" "$ATT" > att.txt
+```
+
+Please replace `imap.example.com`, `$username`, `$password`, `$MAILID`,
+and `$ATT` with your actual IMAP server details, username, password,
+mail ID, and attachment name.
+
+## 📜 License
+
+This project is licensed under the GPL-3.0 license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `myl-0.8.3/myl.py` & `myl-0.8.4/myl.py`

 * *Files identical despite different names*

### Comparing `myl-0.8.3/pyproject.toml` & `myl-0.8.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 requires-python = ">=3.8"
 keywords = ["imap", "email"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
-  "imap_tools",
-  "myl-discovery",
-  "rich",
+  "imap-tools == 1.0.0",
+  "myl-discovery == 0.4.0",
+  "rich == 13.4.2",
 ]
-version = "0.8.3"
+version = "0.8.4"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

