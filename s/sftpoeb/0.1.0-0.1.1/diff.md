# Comparing `tmp/sftpoeb-0.1.0.tar.gz` & `tmp/sftpoeb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.0.tar", last modified: Wed Jun 14 04:48:37 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.1.tar", last modified: Wed Jun 14 06:41:32 2023, max compression
```

## Comparing `sftpoeb-0.1.0.tar` & `sftpoeb-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.456323 sftpoeb-0.1.0/
--rw-rw-rw-   0        0        0      557 2023-06-14 04:48:24.000000 sftpoeb-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      979 2023-06-14 04:48:37.456323 sftpoeb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.0/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 04:48:37.457324 sftpoeb-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-14 04:48:34.000000 sftpoeb-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.352322 sftpoeb-0.1.0/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.1.0/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.385324 sftpoeb-0.1.0/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.390324 sftpoeb-0.1.0/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.1.0/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-14 04:00:34.000000 sftpoeb-0.1.0/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.399323 sftpoeb-0.1.0/sftpoeb/method/
--rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.1.0/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4793 2023-06-14 04:14:04.000000 sftpoeb-0.1.0/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.408323 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.410324 sftpoeb-0.1.0/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.1.0/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.417322 sftpoeb-0.1.0/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.423322 sftpoeb-0.1.0/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.0/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.0/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.427322 sftpoeb-0.1.0/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.0/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.0/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.448321 sftpoeb-0.1.0/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     4508 2023-06-14 04:47:33.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1875 2023-06-14 04:48:01.000000 sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.452325 sftpoeb-0.1.0/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.0/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.1.0/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:48:37.383323 sftpoeb-0.1.0/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      979 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 04:48:37.000000 sftpoeb-0.1.0/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.161103 sftpoeb-0.1.1/
+-rw-rw-rw-   0        0        0      609 2023-06-14 06:41:02.000000 sftpoeb-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1031 2023-06-14 06:41:32.160103 sftpoeb-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.1/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:41:32.161103 sftpoeb-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-14 06:41:14.000000 sftpoeb-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.040118 sftpoeb-0.1.1/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.1.1/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.073103 sftpoeb-0.1.1/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.078111 sftpoeb-0.1.1/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.1.1/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1527 2023-06-14 04:59:52.000000 sftpoeb-0.1.1/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.099127 sftpoeb-0.1.1/sftpoeb/method/
+-rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.1.1/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4793 2023-06-14 04:14:04.000000 sftpoeb-0.1.1/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.122109 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.125105 sftpoeb-0.1.1/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.1.1/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.132122 sftpoeb-0.1.1/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.137105 sftpoeb-0.1.1/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.1/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.1/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.141105 sftpoeb-0.1.1/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.1/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.1/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.153105 sftpoeb-0.1.1/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     4508 2023-06-14 04:47:33.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3999 2023-06-14 04:01:25.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1875 2023-06-14 04:59:14.000000 sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.157103 sftpoeb-0.1.1/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.1/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    29080 2023-06-14 04:01:40.000000 sftpoeb-0.1.1/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:41:32.066109 sftpoeb-0.1.1/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1031 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 06:41:31.000000 sftpoeb-0.1.1/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.1.0/CHANGELOG.txt` & `sftpoeb-0.1.1/CHANGELOG.txt`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,12 @@
 
 0.0.9 (14/06/2023)
 ------------------
 - Fixbug
 
 0.1.0 (14/06/2023)
 ------------------
+- Fixbug
+
+0.1.1 (14/06/2023)
+------------------
 - Fixbug
```

### Comparing `sftpoeb-0.1.0/LICENSE.txt` & `sftpoeb-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/PKG-INFO` & `sftpoeb-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.0
+Version: 0.1.1
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -55,7 +55,11 @@
 ------------------
 - Fixbug
 
 0.1.0 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.1 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.1.0/setup.py` & `sftpoeb-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.1.0',
+        version='0.1.1',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.1.0/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.1/sftpoeb/mainclass/c_sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.timeNow = datetime.now().strftime("%H%M%S")
         self.payloadData = payloadData
         ### Local
         self.local = setgetlocal(self.myPath,self.sftpPath,self.dateNow,self.timeNow)
         ### Destination
         self.destination = setgetdestination(self.custPath,self.sftpPath,self.dateNow,self.timeNow)
         ### Recovery
-        self.recovery = setgetrecovery(self.myPath,self.sftpPath)
+        self.recovery = setgetrecovery(self.myPath,self.sftpPath,self.dateNow,self.timeNow)
         ### inputFile
         self.input = inputFile(self.local,self.destination,self.dateNow,self.timeNow)
 
     def package1(self,quantityThread):
 
         ### เปิดคลาสกระบวนการดำเนินการไฟล์
         c_process = packageprocess(self.local,self.destination,self.recovery,self.payloadData,self.dateNow,self.timeNow)
```

### Comparing `sftpoeb-0.1.0/sftpoeb/method/callservice.py` & `sftpoeb-0.1.1/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.1/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.1/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.1/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.1/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.1/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.1/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.0/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.1/sftpoeb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.0
+Version: 0.1.1
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -55,7 +55,11 @@
 ------------------
 - Fixbug
 
 0.1.0 (14/06/2023)
 ------------------
 - Fixbug
 
+0.1.1 (14/06/2023)
+------------------
+- Fixbug
+
```

### Comparing `sftpoeb-0.1.0/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.1/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

