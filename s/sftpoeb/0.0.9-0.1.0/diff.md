# Comparing `tmp/sftpoeb-0.0.9.tar.gz` & `tmp/sftpoeb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.9.tar", last modified: Wed Jun 14 04:14:51 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.0.tar", last modified: Wed Jun 14 04:48:37 2023, max compression
```

## Comparing `sftpoeb-0.0.9.tar` & `sftpoeb-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.084075 sftpoeb-0.0.9/
--rw-rw-rw-   0        0        0      505 2023-06-14 04:14:48.000000 sftpoeb-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      927 2023-06-14 04:14:51.084075 sftpoeb-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.9/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 04:14:51.085076 sftpoeb-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-14 04:14:40.000000 sftpoeb-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:50.995077 sftpoeb-0.0.9/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.0.9/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.019079 sftpoeb-0.0.9/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.9/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.024077 sftpoeb-0.0.9/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.0.9/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-14 04:00:34.000000 sftpoeb-0.0.9/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.038079 sftpoeb-0.0.9/sftpoeb/method/
--rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.0.9/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-06-14 04:14:04.000000 sftpoeb-0.0.9/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.9/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.9/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.048076 sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.049078 sftpoeb-0.0.9/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.0.9/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.056079 sftpoeb-0.0.9/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.0.9/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.0.9/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.9/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.060077 sftpoeb-0.0.9/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.0.9/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.0.9/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.065078 sftpoeb-0.0.9/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.0.9/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.0.9/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.075078 sftpoeb-0.0.9/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.0.9/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     4436 2023-06-14 04:01:22.000000 sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1803 2023-06-14 04:01:28.000000 sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.081089 sftpoeb-0.0.9/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.0.9/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.0.9/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:14:51.017076 sftpoeb-0.0.9/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      927 2023-06-14 04:14:50.000000 sftpoeb-0.0.9/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-14 04:14:50.000000 sftpoeb-0.0.9/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 04:14:50.000000 sftpoeb-0.0.9/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-14 04:14:50.000000 sftpoeb-0.0.9/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 04:14:50.000000 sftpoeb-0.0.9/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.456323 sftpoeb-0.1.0/
+-rw-rw-rw-   0        0        0      557 2023-06-14 04:48:24.000000 sftpoeb-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      979 2023-06-14 04:48:37.456323 sftpoeb-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.0/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 04:48:37.457324 sftpoeb-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-14 04:48:34.000000 sftpoeb-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.352322 sftpoeb-0.1.0/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.1.0/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.385324 sftpoeb-0.1.0/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.390324 sftpoeb-0.1.0/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.1.0/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-14 04:00:34.000000 sftpoeb-0.1.0/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.399323 sftpoeb-0.1.0/sftpoeb/method/
+-rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.1.0/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4793 2023-06-14 04:14:04.000000 sftpoeb-0.1.0/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.408323 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.410324 sftpoeb-0.1.0/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.1.0/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.417322 sftpoeb-0.1.0/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.423322 sftpoeb-0.1.0/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.0/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.0/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.427322 sftpoeb-0.1.0/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.0/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.0/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.448321 sftpoeb-0.1.0/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     4508 2023-06-14 04:47:33.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1875 2023-06-14 04:48:01.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.452325 sftpoeb-0.1.0/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.0/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.1.0/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.383323 sftpoeb-0.1.0/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      979 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.9/LICENSE.txt` & `sftpoeb-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/PKG-INFO` & `sftpoeb-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.9
+Version: 0.1.0
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -51,7 +51,11 @@
 ------------------
 - Fixbug
 
 0.0.9 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.0 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.9/setup.py` & `sftpoeb-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.9',
+        version='0.1.0',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.0.9/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.0/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/method/callservice.py` & `sftpoeb-0.1.0/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.0/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.0/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.0/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime
 from ...method.checkpath import *
 class setgetdestination():
     def __init__(self,custPath,sftpPath,dateNow,timeNow):
+        self.formatOld = '%Y%m%d'
+        self.formatNew = '%Y-%m-%d'
         self.destinationPath = custPath + "/" + sftpPath + "/"
         self.destinationPathCSV = custPath + "/" + sftpPath + "/Inbound/CSV/"
         self.destinationPathPDF = custPath + "/" + sftpPath + "/Inbound/PDF/"
         self.destinationCsvArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Archived_File/'
         self.destinationCsvErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/CSV/Error_File/'
         self.destinationPdfArchivePath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Archived_File/'
         self.destinationPdfErrorPath = custPath + "/" + sftpPath + '/History/' + self.transformDate(dateNow) + '/PDF/Error_File/'
```

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from ...method.checkpath import *
 from datetime import datetime
 class setgetrecovery():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
+        self.formatOld = '%Y%m%d'
+        self.formatNew = '%Y-%m-%d'
         self.dateNow = dateNow
         self.timeNow = timeNow
         self.recoveryPath = myPath + "/" + sftpPath + "/Inbound/Temp_recover/"
         self.peddingPath = myPath + "/" + sftpPath + "/Inbound/Pending/"
 
 ########## SET ############
     def setRecoveryPath(self,path):
```

### Comparing `sftpoeb-0.0.9/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.0/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.9/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.0/sftpoeb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.9
+Version: 0.1.0
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -51,7 +51,11 @@
 ------------------
 - Fixbug
 
 0.0.9 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.0 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.9/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.0/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

