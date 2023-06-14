# Comparing `tmp/netdevice-1.3.0.tar.gz` & `tmp/netdevice-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdevice-1.3.0.tar", last modified: Wed May 31 09:29:08 2023, max compression
+gzip compressed data, was "netdevice-1.3.1.tar", last modified: Wed Jun 14 01:36:22 2023, max compression
```

## Comparing `netdevice-1.3.0.tar` & `netdevice-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:29:08.555769 netdevice-1.3.0/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       39 2022-08-17 08:17:30.000000 netdevice-1.3.0/MANIFEST.in
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28138 2023-05-31 09:29:08.555769 netdevice-1.3.0/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27872 2022-09-06 03:24:48.000000 netdevice-1.3.0/README.rst
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:29:08.517765 netdevice-1.3.0/demo/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1988 2022-08-17 08:17:30.000000 netdevice-1.3.0/demo/demo.py
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:29:08.532767 netdevice-1.3.0/netdevice/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      447 2022-08-17 08:17:30.000000 netdevice-1.3.0/netdevice/__init__.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      385 2022-08-17 08:17:30.000000 netdevice-1.3.0/netdevice/cisco.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    35106 2022-08-17 08:17:30.000000 netdevice-1.3.0/netdevice/junos.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    52051 2023-05-31 09:27:06.000000 netdevice-1.3.0/netdevice/linux.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27847 2022-08-17 08:17:30.000000 netdevice-1.3.0/netdevice/ovn.py
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    24965 2022-08-17 08:17:30.000000 netdevice-1.3.0/netdevice/ovs.py
-drwxr-xr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-05-31 09:29:08.553774 netdevice-1.3.0/netdevice.egg-info/
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28138 2023-05-31 09:29:08.000000 netdevice-1.3.0/netdevice.egg-info/PKG-INFO
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      331 2023-05-31 09:29:08.000000 netdevice-1.3.0/netdevice.egg-info/SOURCES.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-05-31 09:29:08.000000 netdevice-1.3.0/netdevice.egg-info/dependency_links.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       53 2023-05-31 09:29:08.000000 netdevice-1.3.0/netdevice.egg-info/requires.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       10 2023-05-31 09:29:08.000000 netdevice-1.3.0/netdevice.egg-info/top_level.txt
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       38 2023-05-31 09:29:08.557771 netdevice-1.3.0/setup.cfg
--rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      570 2023-05-31 09:28:27.000000 netdevice-1.3.0/setup.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-06-14 01:36:22.892691 netdevice-1.3.1/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       39 2022-08-17 08:17:30.000000 netdevice-1.3.1/MANIFEST.in
+-rw-rw-r--   0 ypguo    (19391612) Domain Users (1049089)    28138 2023-06-14 01:36:22.892691 netdevice-1.3.1/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27872 2022-09-06 03:24:48.000000 netdevice-1.3.1/README.rst
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-06-14 01:36:22.858695 netdevice-1.3.1/demo/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)     1988 2022-08-17 08:17:30.000000 netdevice-1.3.1/demo/demo.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-06-14 01:36:22.875692 netdevice-1.3.1/netdevice/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      447 2022-08-17 08:17:30.000000 netdevice-1.3.1/netdevice/__init__.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      385 2022-08-17 08:17:30.000000 netdevice-1.3.1/netdevice/cisco.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    35106 2022-08-17 08:17:30.000000 netdevice-1.3.1/netdevice/junos.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    52051 2023-06-14 01:35:46.000000 netdevice-1.3.1/netdevice/linux.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    27847 2022-08-17 08:17:30.000000 netdevice-1.3.1/netdevice/ovn.py
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    24965 2022-08-17 08:17:30.000000 netdevice-1.3.1/netdevice/ovs.py
+drwxrwxr-x   0 ypguo    (19391612) Domain Users (1049089)        0 2023-06-14 01:36:22.890693 netdevice-1.3.1/netdevice.egg-info/
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)    28138 2023-06-14 01:36:22.000000 netdevice-1.3.1/netdevice.egg-info/PKG-INFO
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      331 2023-06-14 01:36:22.000000 netdevice-1.3.1/netdevice.egg-info/SOURCES.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)        1 2023-06-14 01:36:22.000000 netdevice-1.3.1/netdevice.egg-info/dependency_links.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       53 2023-06-14 01:36:22.000000 netdevice-1.3.1/netdevice.egg-info/requires.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       10 2023-06-14 01:36:22.000000 netdevice-1.3.1/netdevice.egg-info/top_level.txt
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)       38 2023-06-14 01:36:22.894692 netdevice-1.3.1/setup.cfg
+-rw-r--r--   0 ypguo    (19391612) Domain Users (1049089)      570 2023-06-14 01:35:56.000000 netdevice-1.3.1/setup.py
```

### Comparing `netdevice-1.3.0/PKG-INFO` & `netdevice-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netdevice
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python modules to execute command on remote network device based on pexpect.
 Home-page: https://github.com/guoyoooping/networkdevice
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
 
 netdevice
```

### Comparing `netdevice-1.3.0/README.rst` & `netdevice-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `netdevice-1.3.0/demo/demo.py` & `netdevice-1.3.1/demo/demo.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.3.0/netdevice/junos.py` & `netdevice-1.3.1/netdevice/junos.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.3.0/netdevice/linux.py` & `netdevice-1.3.1/netdevice/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     # ...
 }
 
 class LinuxDevice(object):
     '''
     A base class for common linux devices.
     '''
-    release = '1.2.5'
+    release = '1.3.1'
 
     LOG_EMERG = 0   # not used
     LOG_ALERT = 1   # not used
     LOG_CRIT = 2    # not used
     LOG_ERR = 3     # Error message, maybe encounter error.
     LOG_WARNING = 4 # + Warning message
     LOG_NOTICE = 5  # + command
```

### Comparing `netdevice-1.3.0/netdevice/ovn.py` & `netdevice-1.3.1/netdevice/ovn.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.3.0/netdevice/ovs.py` & `netdevice-1.3.1/netdevice/ovs.py`

 * *Files identical despite different names*

### Comparing `netdevice-1.3.0/netdevice.egg-info/PKG-INFO` & `netdevice-1.3.1/netdevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netdevice
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python modules to execute command on remote network device based on pexpect.
 Home-page: https://github.com/guoyoooping/networkdevice
 Author: Yongping Guo
 Author-email: guoyoooping@163.com
 License: GPLv3
 
 netdevice
```

### Comparing `netdevice-1.3.0/setup.py` & `netdevice-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='netdevice',
-      version='1.3.0',
+      version='1.3.1',
       author='Yongping Guo',
       author_email='guoyoooping@163.com',
       description='Python modules to execute command on remote network device based on pexpect.',
       long_description=open('README.rst').read(),
       install_requires = ["ipaddress", "pexpect", "lxml", "IPy", "xmltodict", "dpkt", "simplejson"],
       url='https://github.com/guoyoooping/networkdevice',
       license="GPLv3",
```

