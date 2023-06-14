# Comparing `tmp/sftpoeb-0.0.6.tar.gz` & `tmp/sftpoeb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.6.tar", last modified: Wed Jun 14 03:40:47 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.7.tar", last modified: Wed Jun 14 03:52:08 2023, max compression
```

## Comparing `sftpoeb-0.0.6.tar` & `sftpoeb-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.909951 sftpoeb-0.0.6/
--rw-rw-rw-   0        0        0      297 2023-06-14 03:34:13.000000 sftpoeb-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      719 2023-06-14 03:40:47.908946 sftpoeb-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.6/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:40:47.909951 sftpoeb-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-14 03:40:44.000000 sftpoeb-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.839939 sftpoeb-0.0.6/sftpoeb/
--rw-rw-rw-   0        0        0       69 2023-06-14 03:35:19.000000 sftpoeb-0.0.6/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.863940 sftpoeb-0.0.6/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.867942 sftpoeb-0.0.6/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       20 2023-06-14 03:36:57.000000 sftpoeb-0.0.6/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-06-14 03:33:27.000000 sftpoeb-0.0.6/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.874940 sftpoeb-0.0.6/sftpoeb/method/
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.885941 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.887940 sftpoeb-0.0.6/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      104 2023-06-14 03:38:06.000000 sftpoeb-0.0.6/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.890938 sftpoeb-0.0.6/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0     2889 2023-06-14 03:33:39.000000 sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.893941 sftpoeb-0.0.6/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.896940 sftpoeb-0.0.6/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.6/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.904940 sftpoeb-0.0.6/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0     4433 2023-06-14 03:33:47.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-14 03:33:51.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1800 2023-06-14 03:33:54.000000 sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.905939 sftpoeb-0.0.6/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0    29074 2023-06-14 03:33:59.000000 sftpoeb-0.0.6/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:40:47.861941 sftpoeb-0.0.6/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      719 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      937 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 03:40:47.000000 sftpoeb-0.0.6/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.688935 sftpoeb-0.0.7/
+-rw-rw-rw-   0        0        0      401 2023-06-14 03:51:56.000000 sftpoeb-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      823 2023-06-14 03:52:08.687938 sftpoeb-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.7/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 03:52:08.689936 sftpoeb-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-14 03:52:04.000000 sftpoeb-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.559935 sftpoeb-0.0.7/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-14 03:50:21.000000 sftpoeb-0.0.7/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.588934 sftpoeb-0.0.7/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.593935 sftpoeb-0.0.7/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       21 2023-06-14 03:49:30.000000 sftpoeb-0.0.7/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-06-14 03:33:27.000000 sftpoeb-0.0.7/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.606933 sftpoeb-0.0.7/sftpoeb/method/
+-rw-rw-rw-   0        0        0       74 2023-06-14 03:49:57.000000 sftpoeb-0.0.7/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.614935 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.621935 sftpoeb-0.0.7/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      109 2023-06-14 03:50:15.000000 sftpoeb-0.0.7/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.633935 sftpoeb-0.0.7/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2889 2023-06-14 03:33:39.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.642943 sftpoeb-0.0.7/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.0.7/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.652934 sftpoeb-0.0.7/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.0.7/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.7/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.666944 sftpoeb-0.0.7/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-06-14 03:33:47.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3996 2023-06-14 03:33:51.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1800 2023-06-14 03:33:54.000000 sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.683936 sftpoeb-0.0.7/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.0.7/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    29074 2023-06-14 03:33:59.000000 sftpoeb-0.0.7/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-14 03:52:08.586934 sftpoeb-0.0.7/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      823 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 03:52:08.000000 sftpoeb-0.0.7/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.6/LICENSE.txt` & `sftpoeb-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/setup.py` & `sftpoeb-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.6',
+        version='0.0.7',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.0.6/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.7/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/method/callservice.py` & `sftpoeb-0.0.7/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.7/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.7/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.7/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.7/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.7/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.7/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.6/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.7/sftpoeb.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,23 +9,29 @@
 sftpoeb.egg-info/SOURCES.txt
 sftpoeb.egg-info/dependency_links.txt
 sftpoeb.egg-info/requires.txt
 sftpoeb.egg-info/top_level.txt
 sftpoeb/config/variable.py
 sftpoeb/mainclass/__init__.py
 sftpoeb/mainclass/c_sftp.py
+sftpoeb/method/__init__.py
 sftpoeb/method/callservice.py
 sftpoeb/method/checkpath.py
 sftpoeb/method/debug.py
 sftpoeb/sftpoeb.egg-info/SOURCES.txt
 sftpoeb/sftpoeb.egg-info/dependency_links.txt
 sftpoeb/sftpoeb.egg-info/requires.txt
 sftpoeb/sftpoeb.egg-info/top_level.txt
 sftpoeb/subclass/__init__.py
+sftpoeb/subclass/file/__init__.py
 sftpoeb/subclass/file/s_c_file.py
 sftpoeb/subclass/file/s_c_file_transfer.py
+sftpoeb/subclass/input/__init__.py
 sftpoeb/subclass/input/s_c_input.py
+sftpoeb/subclass/output/__init__.py
 sftpoeb/subclass/output/s_c_output.py
+sftpoeb/subclass/path/__init__.py
 sftpoeb/subclass/path/s_c_setgetdestination.py
 sftpoeb/subclass/path/s_c_setgetlocal.py
 sftpoeb/subclass/path/s_c_setgetrecovery.py
+sftpoeb/subclass/process/__init__.py
 sftpoeb/subclass/process/s_c_process_package_1.py
```

