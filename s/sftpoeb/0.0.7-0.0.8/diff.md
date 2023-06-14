# Comparing `tmp/sftpoeb-0.0.7.tar.gz` & `tmp/sftpoeb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.7.tar", last modified: Wed Jun 14 03:52:08 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.8.tar", last modified: Wed Jun 14 04:03:24 2023, max compression
```

## Comparing `sftpoeb-0.0.7.tar` & `sftpoeb-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.688935 sftpoeb-0.0.7/
--rw-rw-rw-   0        0        0      401 2023-06-14 03:51:56.000000 sftpoeb-0.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      823 2023-06-14 03:52:08.687938 sftpoeb-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.7/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:52:08.689936 sftpoeb-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-14 03:52:04.000000 sftpoeb-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.559935 sftpoeb-0.0.7/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.0.7/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.588934 sftpoeb-0.0.7/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.593935 sftpoeb-0.0.7/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.0.7/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-06-14 03:33:27.000000 sftpoeb-0.0.7/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.606933 sftpoeb-0.0.7/sftpoeb/method/
--rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.0.7/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.614935 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.621935 sftpoeb-0.0.7/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.0.7/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.633935 sftpoeb-0.0.7/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2889 2023-06-14 03:33:39.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.642943 sftpoeb-0.0.7/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.0.7/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.652934 sftpoeb-0.0.7/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.0.7/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.666944 sftpoeb-0.0.7/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     4433 2023-06-14 03:33:47.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-14 03:33:51.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1800 2023-06-14 03:33:54.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.683936 sftpoeb-0.0.7/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.0.7/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    29074 2023-06-14 03:33:59.000000 sftpoeb-0.0.7/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.586934 sftpoeb-0.0.7/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      823 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.227300 sftpoeb-0.0.8/
+-rw-rw-rw-   0        0        0      453 2023-06-14 04:01:49.000000 sftpoeb-0.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      875 2023-06-14 04:03:24.226310 sftpoeb-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.8/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 04:03:24.227300 sftpoeb-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-14 04:01:54.000000 sftpoeb-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.065299 sftpoeb-0.0.8/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.0.8/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.088301 sftpoeb-0.0.8/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.8/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.098298 sftpoeb-0.0.8/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.0.8/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-14 04:00:34.000000 sftpoeb-0.0.8/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.114298 sftpoeb-0.0.8/sftpoeb/method/
+-rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.0.8/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4864 2023-06-14 04:00:44.000000 sftpoeb-0.0.8/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.8/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.8/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.123297 sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.126304 sftpoeb-0.0.8/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.0.8/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.139298 sftpoeb-0.0.8/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.0.8/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.0.8/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.8/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.149299 sftpoeb-0.0.8/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.0.8/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.0.8/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.166303 sftpoeb-0.0.8/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.0.8/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.0.8/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.208301 sftpoeb-0.0.8/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.0.8/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     4436 2023-06-14 04:01:22.000000 sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1803 2023-06-14 04:01:28.000000 sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.223298 sftpoeb-0.0.8/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.0.8/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.0.8/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:03:24.085299 sftpoeb-0.0.8/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      875 2023-06-14 04:03:23.000000 sftpoeb-0.0.8/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-14 04:03:23.000000 sftpoeb-0.0.8/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 04:03:23.000000 sftpoeb-0.0.8/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 04:03:23.000000 sftpoeb-0.0.8/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 04:03:23.000000 sftpoeb-0.0.8/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.7/LICENSE.txt` & `sftpoeb-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.7/PKG-INFO` & `sftpoeb-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -43,7 +43,11 @@
 ------------------
 - Fixbug
 
 0.0.7 (14/06/2023)
 ------------------
 - Fixbug
 
+0.0.8 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.7/setup.py` & `sftpoeb-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.7',
+        version='0.0.8',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.0.7/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.8/sftpoeb/mainclass/c_sftp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from subclass.path.s_c_setgetlocal import *
-from subclass.path.s_c_setgetdestination import *
-from subclass.path.s_c_setgetrecovery import *
-from subclass.file.s_c_file import *
-from subclass.process.s_c_process_package_1 import *
+from ..subclass.path.s_c_setgetlocal import *
+from ..subclass.path.s_c_setgetdestination import *
+from ..subclass.path.s_c_setgetrecovery import *
+from ..subclass.file.s_c_file import *
+from ..subclass.process.s_c_process_package_1 import *
 from datetime import date, datetime
-from subclass.input.s_c_input import *
+from ..subclass.input.s_c_input import *
 class SFTP():
     def __init__(self,myPath="None",sftpPath="None",custPath="None",payloadData="None"):
         self.myPath = myPath
         self.sftpPath = sftpPath
         self.custPath = custPath
         self.dateNow = datetime.now().strftime("%Y%m%d")
         self.timeNow = datetime.now().strftime("%H%M%S")
```

### Comparing `sftpoeb-0.0.7/sftpoeb/method/callservice.py` & `sftpoeb-0.0.8/sftpoeb/method/callservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
-from config.variable import *
+from ..config.variable import *
 import os,requests,time,urllib3
 urllib3.disable_warnings()
 
 def serviceSigning(data, fileNameText, fileNamePDF, pathFile,round,serviceCode):
     multipart_data = MultipartEncoder(
         fields={
             "SellerTaxId": data['SellerTaxid'],
```

### Comparing `sftpoeb-0.0.7/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.8/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.8/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.8/sftpoeb/subclass/file/s_c_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from method.checkpath import *
+from ...method.checkpath import *
 from os import listdir
 import shutil
 class dofile():
     def __init__(self,local,destination,dateNow,timeNow):
         self.dateNow = dateNow
         self.timeNow = timeNow
         self.local = local
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.8/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.8/sftpoeb/subclass/input/s_c_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os.path import isfile, join
 from os import listdir
-from file.s_c_file import *
-from file.s_c_file_transfer import *
+from ..file.s_c_file import *
+from ..file.s_c_file_transfer import *
 import paramiko
 import json,shutil
 
 class inputFile():
     def __init__(self,local,destination,dateNow,timeNow):
         self.local = local
         self.destination = destination
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.8/sftpoeb/subclass/output/s_c_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os.path import isfile, join
 from os import listdir
-from file.s_c_file import *
-from file.s_c_file_transfer import *
+from ..file.s_c_file import *
+from ..file.s_c_file_transfer import *
 import paramiko
 import json,shutil
 
 class outputFile():
     def __init__(self,local,destination,dateNow,timeNow):
         self.local = local
         self.destination = destination
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from method.checkpath import *
+from ...method.checkpath import *
 class setgetdestination():
     def __init__(self,custPath,sftpPath,dateNow,timeNow):
         self.destinationPath = custPath + "/" + sftpPath + "/"
         self.destinationPathCSV = custPath + "/" + sftpPath + "/Inbound/CSV/"
         self.destinationPathPDF = custPath + "/" + sftpPath + "/Inbound/PDF/"
         self.destinationCsvArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Archived_File/'
         self.destinationCsvErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Error_File/'
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from method.checkpath import *
+from ...method.checkpath import *
 class setgetlocal():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.formatOld = '%Y%m%d'
         self.formatNew = '%Y-%m-%d'
         self.localPath = myPath + "/" + sftpPath + "/Inbound/"
         self.localFilerun = self.localPath+ '/Filerun/' + self.transformDate(dateNow) + '/'
         self.localPathNow = self.localPath + "/" + str( dateNow + timeNow ) + "/"
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.8/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from method.checkpath import *
+from ...method.checkpath import *
 from datetime import datetime
 class setgetrecovery():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.dateNow = dateNow
         self.timeNow = timeNow
         self.recoveryPath = myPath + "/" + sftpPath + "/Inbound/Temp_recover/"
         self.peddingPath = myPath + "/" + sftpPath + "/Inbound/Pending/"
```

### Comparing `sftpoeb-0.0.7/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.8/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from method.callservice import *
-from method.debug import *
+from ...method.callservice import *
+from ...method.debug import *
 from os import listdir
 from os.path import isfile, join, isdir
 import threading
 import shutil,json
 class packageprocess():
     def __init__(self,local,destination,recovery,payloadData,dateNow,timeNow):
         self.local = local
```

### Comparing `sftpoeb-0.0.7/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.0.8/sftpoeb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.7
+Version: 0.0.8
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -43,7 +43,11 @@
 ------------------
 - Fixbug
 
 0.0.7 (14/06/2023)
 ------------------
 - Fixbug
 
+0.0.8 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.7/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.8/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

