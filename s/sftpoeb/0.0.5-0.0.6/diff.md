# Comparing `tmp/sftpoeb-0.0.5.tar.gz` & `tmp/sftpoeb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.5.tar", last modified: Wed Jun 14 03:38:36 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.6.tar", last modified: Wed Jun 14 03:40:47 2023, max compression
```

## Comparing `sftpoeb-0.0.5.tar` & `sftpoeb-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:36.057851 sftpoeb-0.0.5/
--rw-rw-rw-   0        0        0      297 2023-06-14 03:34:13.000000 sftpoeb-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      719 2023-06-14 03:38:36.056852 sftpoeb-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.5/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:38:36.057851 sftpoeb-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      624 2023-06-14 03:32:46.000000 sftpoeb-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.639987 sftpoeb-0.0.5/sftpoeb/
--rw-rw-rw-   0        0        0       69 2023-06-14 03:35:19.000000 sftpoeb-0.0.5/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.651987 sftpoeb-0.0.5/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.660992 sftpoeb-0.0.5/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       20 2023-06-14 03:36:57.000000 sftpoeb-0.0.5/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-06-14 03:33:27.000000 sftpoeb-0.0.5/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.667989 sftpoeb-0.0.5/sftpoeb/method/
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.693987 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      719 2023-06-14 03:38:35.000000 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.695987 sftpoeb-0.0.5/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      104 2023-06-14 03:38:06.000000 sftpoeb-0.0.5/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.704987 sftpoeb-0.0.5/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0     2889 2023-06-14 03:33:39.000000 sftpoeb-0.0.5/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.707996 sftpoeb-0.0.5/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.709986 sftpoeb-0.0.5/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.5/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.718989 sftpoeb-0.0.5/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0     4433 2023-06-14 03:33:47.000000 sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-14 03:33:51.000000 sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1800 2023-06-14 03:33:54.000000 sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:36.054843 sftpoeb-0.0.5/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0    29074 2023-06-14 03:33:59.000000 sftpoeb-0.0.5/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:38:35.648991 sftpoeb-0.0.5/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      718 2023-06-14 03:07:06.000000 sftpoeb-0.0.5/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:07:06.000000 sftpoeb-0.0.5/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:07:06.000000 sftpoeb-0.0.5/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 03:07:06.000000 sftpoeb-0.0.5/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.909951 sftpoeb-0.0.6/
+-rw-rw-rw-   0        0        0      297 2023-06-14 03:34:13.000000 sftpoeb-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      719 2023-06-14 03:40:47.908946 sftpoeb-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.6/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:40:47.909951 sftpoeb-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-14 03:40:44.000000 sftpoeb-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.839939 sftpoeb-0.0.6/sftpoeb/
+-rw-rw-rw-   0        0        0       69 2023-06-14 03:35:19.000000 sftpoeb-0.0.6/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.863940 sftpoeb-0.0.6/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.867942 sftpoeb-0.0.6/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       20 2023-06-14 03:36:57.000000 sftpoeb-0.0.6/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-06-14 03:33:27.000000 sftpoeb-0.0.6/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.874940 sftpoeb-0.0.6/sftpoeb/method/
+-rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.885941 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.887940 sftpoeb-0.0.6/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      104 2023-06-14 03:38:06.000000 sftpoeb-0.0.6/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.890938 sftpoeb-0.0.6/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0     2889 2023-06-14 03:33:39.000000 sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.893941 sftpoeb-0.0.6/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.896940 sftpoeb-0.0.6/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.904940 sftpoeb-0.0.6/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0     4433 2023-06-14 03:33:47.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3996 2023-06-14 03:33:51.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1800 2023-06-14 03:33:54.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.905939 sftpoeb-0.0.6/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0    29074 2023-06-14 03:33:59.000000 sftpoeb-0.0.6/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.861941 sftpoeb-0.0.6/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      719 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      937 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.5/LICENSE.txt` & `sftpoeb-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/PKG-INFO` & `sftpoeb-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.5
+Version: 0.0.6
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
```

### Comparing `sftpoeb-0.0.5/setup.py` & `sftpoeb-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.5',
+        version='0.0.6',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
-        package_dir={"":"sftpoeb"},
-        packages=find_packages(where="sftpoeb"),
+        packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
         keywords='sftp',
         install_requires=['paramiko','Requests','requests_toolbelt','urllib3']
     )
```

### Comparing `sftpoeb-0.0.5/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.6/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/method/callservice.py` & `sftpoeb-0.0.6/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.6/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.0.6/sftpoeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.0.5
+Version: 0.0.6
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
```

### Comparing `sftpoeb-0.0.5/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.6/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.6/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.5/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.6/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

