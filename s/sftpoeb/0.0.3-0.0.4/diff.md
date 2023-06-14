# Comparing `tmp/sftpoeb-0.0.3.tar.gz` & `tmp/sftpoeb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.3.tar", last modified: Wed Jun 14 03:07:06 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.4.tar", last modified: Wed Jun 14 03:12:33 2023, max compression
```

## Comparing `sftpoeb-0.0.3.tar` & `sftpoeb-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.687479 sftpoeb-0.0.3/
--rw-rw-rw-   0        0        0      193 2023-06-14 03:06:56.000000 sftpoeb-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      615 2023-06-14 03:07:06.686483 sftpoeb-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.3/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:07:06.687479 sftpoeb-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-14 03:07:02.000000 sftpoeb-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.602483 sftpoeb-0.0.3/sftpoeb/
--rw-rw-rw-   0        0        0      448 2023-06-14 03:03:11.000000 sftpoeb-0.0.3/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.631483 sftpoeb-0.0.3/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.639480 sftpoeb-0.0.3/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0     1537 2023-06-14 03:04:08.000000 sftpoeb-0.0.3/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.646526 sftpoeb-0.0.3/sftpoeb/method/
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.572480 sftpoeb-0.0.3/sftpoeb/subclass/
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.656514 sftpoeb-0.0.3/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0     2897 2023-06-14 03:05:55.000000 sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.658481 sftpoeb-0.0.3/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.662482 sftpoeb-0.0.3/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.674512 sftpoeb-0.0.3/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 11:32:38.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1808 2023-06-14 03:05:41.000000 sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.684479 sftpoeb-0.0.3/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0    29090 2023-06-14 03:05:21.000000 sftpoeb-0.0.3/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:07:06.629481 sftpoeb-0.0.3/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      615 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 03:07:06.000000 sftpoeb-0.0.3/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.321928 sftpoeb-0.0.4/
+-rw-rw-rw-   0        0        0      245 2023-06-14 03:12:30.000000 sftpoeb-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      667 2023-06-14 03:12:33.321928 sftpoeb-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.4/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:12:33.322930 sftpoeb-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      624 2023-06-14 03:12:15.000000 sftpoeb-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.229929 sftpoeb-0.0.4/sftpoeb/
+-rw-rw-rw-   0        0        0      448 2023-06-14 03:03:11.000000 sftpoeb-0.0.4/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.241932 sftpoeb-0.0.4/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.243928 sftpoeb-0.0.4/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0     1537 2023-06-14 03:04:08.000000 sftpoeb-0.0.4/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.251928 sftpoeb-0.0.4/sftpoeb/method/
+-rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.281931 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-06-14 03:12:33.000000 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      886 2023-06-14 03:12:33.000000 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:12:33.000000 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:12:33.000000 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:12:33.000000 sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.213930 sftpoeb-0.0.4/sftpoeb/subclass/
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.289933 sftpoeb-0.0.4/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0     2897 2023-06-14 03:05:55.000000 sftpoeb-0.0.4/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.293932 sftpoeb-0.0.4/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.296933 sftpoeb-0.0.4/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.315937 sftpoeb-0.0.4/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4004 2023-06-14 03:12:17.000000 sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1808 2023-06-14 03:05:41.000000 sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.318931 sftpoeb-0.0.4/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0    29090 2023-06-14 03:05:21.000000 sftpoeb-0.0.4/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:12:33.238934 sftpoeb-0.0.4/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      718 2023-06-14 03:07:06.000000 sftpoeb-0.0.4/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:07:06.000000 sftpoeb-0.0.4/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:07:06.000000 sftpoeb-0.0.4/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 03:07:06.000000 sftpoeb-0.0.4/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.3/LICENSE.txt` & `sftpoeb-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/PKG-INFO` & `sftpoeb-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.3
+Version: 0.0.4
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -27,7 +27,11 @@
 ------------------
 - Second Release
 
 0.0.3 (14/06/2023)
 ------------------
 - Fixbug
 
+0.0.4 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.3/setup.py` & `sftpoeb-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.3',
+        version='0.0.4',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
-        packages=find_packages(),
+        package_dir={"":"sftpoeb"},
+        packages=find_packages(where="sftpoeb"),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
         keywords='sftp',
         install_requires=['paramiko','Requests','requests_toolbelt','urllib3']
     )
```

### Comparing `sftpoeb-0.0.3/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.4/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/method/callservice.py` & `sftpoeb-0.0.4/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.4/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.4/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.4/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.4/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.4/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from method.checkpath import *
+from sftpoeb.method.checkpath import *
 class setgetlocal():
     def __init__(self,myPath,sftpPath,dateNow,timeNow):
         self.formatOld = '%Y%m%d'
         self.formatNew = '%Y-%m-%d'
         self.localPath = myPath + "/" + sftpPath + "/Inbound/"
         self.localFilerun = self.localPath+ '/Filerun/' + self.transformDate(dateNow) + '/'
         self.localPathNow = self.localPath + "/" + str( dateNow + timeNow ) + "/"
```

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.4/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.4/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.3/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.0.4/sftpoeb/sftpoeb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.3
+Version: 0.0.4
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -27,7 +27,11 @@
 ------------------
 - Second Release
 
 0.0.3 (14/06/2023)
 ------------------
 - Fixbug
 
+0.0.4 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.0.3/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.4/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

