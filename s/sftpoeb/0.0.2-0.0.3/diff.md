# Comparing `tmp/sftpoeb-0.0.2.tar.gz` & `tmp/sftpoeb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.2.tar", last modified: Tue Jun 13 11:50:18 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.3.tar", last modified: Wed Jun 14 03:07:06 2023, max compression
```

## Comparing `sftpoeb-0.0.2.tar` & `sftpoeb-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.300620 sftpoeb-0.0.2/
--rw-rw-rw-   0        0        0       81 2023-06-13 11:20:29.000000 sftpoeb-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      503 2023-06-13 11:50:18.299619 sftpoeb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.2/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 11:50:18.300620 sftpoeb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-13 11:50:14.000000 sftpoeb-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.247623 sftpoeb-0.0.2/sftpoeb/
--rw-rw-rw-   0        0        0      440 2023-06-13 11:20:13.000000 sftpoeb-0.0.2/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.269620 sftpoeb-0.0.2/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.271619 sftpoeb-0.0.2/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0     1489 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.278622 sftpoeb-0.0.2/sftpoeb/method/
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.231621 sftpoeb-0.0.2/sftpoeb/subclass/
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.282619 sftpoeb-0.0.2/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0     2889 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.285620 sftpoeb-0.0.2/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.287618 sftpoeb-0.0.2/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.294661 sftpoeb-0.0.2/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1800 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.297620 sftpoeb-0.0.2/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0    29074 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.267619 sftpoeb-0.0.2/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      503 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.687479 sftpoeb-0.0.3/
+-rw-rw-rw-   0        0        0      193 2023-06-14 03:06:56.000000 sftpoeb-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      615 2023-06-14 03:07:06.686483 sftpoeb-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.3/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:07:06.687479 sftpoeb-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-14 03:07:02.000000 sftpoeb-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.602483 sftpoeb-0.0.3/sftpoeb/
+-rw-rw-rw-   0        0        0      448 2023-06-14 03:03:11.000000 sftpoeb-0.0.3/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.631483 sftpoeb-0.0.3/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.639480 sftpoeb-0.0.3/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0     1537 2023-06-14 03:04:08.000000 sftpoeb-0.0.3/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.646526 sftpoeb-0.0.3/sftpoeb/method/
+-rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.572480 sftpoeb-0.0.3/sftpoeb/subclass/
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.656514 sftpoeb-0.0.3/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0     2897 2023-06-14 03:05:55.000000 sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.658481 sftpoeb-0.0.3/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.662482 sftpoeb-0.0.3/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.674512 sftpoeb-0.0.3/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1808 2023-06-14 03:05:41.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.684479 sftpoeb-0.0.3/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0    29090 2023-06-14 03:05:21.000000 sftpoeb-0.0.3/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.629481 sftpoeb-0.0.3/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.2/LICENSE.txt` & `sftpoeb-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/setup.py` & `sftpoeb-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.2',
+        version='0.0.3',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.0.2/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.3/sftpoeb/mainclass/c_sftp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from subclass.path.s_c_setgetlocal import *
-from subclass.path.s_c_setgetdestination import *
-from subclass.path.s_c_setgetrecovery import *
-from subclass.file.s_c_file import *
-from subclass.process.s_c_process_package_1 import *
+from sftpoeb.subclass.path.s_c_setgetlocal import *
+from sftpoeb.subclass.path.s_c_setgetdestination import *
+from sftpoeb.subclass.path.s_c_setgetrecovery import *
+from sftpoeb.subclass.file.s_c_file import *
+from sftpoeb.subclass.process.s_c_process_package_1 import *
 from datetime import date, datetime
-from subclass.input.s_c_input import *
+from sftpoeb.subclass.input.s_c_input import *
 class SFTP():
     def __init__(self,myPath="None",sftpPath="None",custPath="None",payloadData="None"):
         self.myPath = myPath
         self.sftpPath = sftpPath
         self.custPath = custPath
         self.dateNow = datetime.now().strftime("%Y%m%d")
         self.timeNow = datetime.now().strftime("%H%M%S")
```

### Comparing `sftpoeb-0.0.2/sftpoeb/method/callservice.py` & `sftpoeb-0.0.3/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.3/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from method.checkpath import *
+from sftpoeb.method.checkpath import *
 from os import listdir
 import shutil
 class dofile():
     def __init__(self,local,destination,dateNow,timeNow):
         self.dateNow = dateNow
         self.timeNow = timeNow
         self.local = local
```

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.3/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.3/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from method.checkpath import *
+from sftpoeb.method.checkpath import *
 from datetime import datetime
 class setgetrecovery():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.dateNow = dateNow
         self.timeNow = timeNow
         self.recoveryPath = myPath + "/" + sftpPath + "/Inbound/Temp_recover/"
         self.peddingPath = myPath + "/" + sftpPath + "/Inbound/Pending/"
```

### Comparing `sftpoeb-0.0.2/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.3/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from method.callservice import *
-from method.debug import *
+from sftpoeb.method.callservice import *
+from sftpoeb.method.debug import *
 from os import listdir
 from os.path import isfile, join, isdir
 import threading
 import shutil,json
 class packageprocess():
     def __init__(self,local,destination,recovery,payloadData,dateNow,timeNow):
         self.local = local
```

### Comparing `sftpoeb-0.0.2/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.3/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

