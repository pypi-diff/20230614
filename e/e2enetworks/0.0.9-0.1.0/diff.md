# Comparing `tmp/e2enetworks-0.0.9.tar.gz` & `tmp/e2enetworks-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.9.tar", last modified: Tue May 16 10:51:26 2023, max compression
+gzip compressed data, was "e2enetworks-0.1.0.tar", last modified: Wed Jun  7 11:16:20 2023, max compression
```

## Comparing `e2enetworks-0.0.9.tar` & `e2enetworks-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069581 e2enetworks-0.0.9/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.9/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:51:26.069665 e2enetworks-0.0.9/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.9/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067012 e2enetworks-0.0.9/e2enetworks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067991 e2enetworks-0.0.9/e2enetworks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/cloud/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.068579 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.068836 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Dataset/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      838 2023-05-16 09:50:41.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Dataset/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069077 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/EndPoint/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      290 2023-05-16 06:13:24.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069336 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Model/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2149 2023-05-16 10:14:22.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Model/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      220 2023-05-16 06:52:59.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      275 2023-05-16 06:15:26.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/init.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/cloud/test.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      137 2023-05-16 09:55:48.000000 e2enetworks-0.0.9/e2enetworks/constants.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067748 e2enetworks-0.0.9/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      510 2023-05-16 10:51:26.000000 e2enetworks-0.0.9/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-16 10:51:26.069917 e2enetworks-0.0.9/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-16 10:51:06.000000 e2enetworks-0.0.9/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.939606 e2enetworks-0.1.0/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-17 07:28:09.000000 e2enetworks-0.1.0/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5909 2023-06-07 11:16:20.939480 e2enetworks-0.1.0/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-17 07:28:09.000000 e2enetworks-0.1.0/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.936067 e2enetworks-0.1.0/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.0/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.937152 e2enetworks-0.1.0/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-17 07:28:09.000000 e2enetworks-0.1.0/e2enetworks/cloud/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.937829 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.938090 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/APIToken/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1607 2023-05-29 09:33:00.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/APIToken/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.938326 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Dataset/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      895 2023-05-29 07:07:35.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Dataset/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.938538 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/EndPoint/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2822 2023-05-29 09:03:03.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.938783 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Model/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2335 2023-05-29 07:07:35.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Model/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.939022 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Project/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1964 2023-05-29 07:07:35.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Project/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.939265 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Teams/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1779 2023-05-29 07:07:35.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/Teams/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      394 2023-05-29 09:19:59.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       32 2023-05-29 06:58:13.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/config.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      845 2023-05-29 07:07:35.000000 e2enetworks-0.1.0/e2enetworks/cloud/aiplatform/init.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-17 07:28:09.000000 e2enetworks-0.1.0/e2enetworks/cloud/test.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      216 2023-06-07 11:14:26.000000 e2enetworks-0.1.0/e2enetworks/constants.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-06-07 11:16:20.936868 e2enetworks-0.1.0/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5909 2023-06-07 11:16:20.000000 e2enetworks-0.1.0/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      719 2023-06-07 11:16:20.000000 e2enetworks-0.1.0/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-06-07 11:16:20.000000 e2enetworks-0.1.0/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       25 2023-06-07 11:16:20.000000 e2enetworks-0.1.0/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-06-07 11:16:20.000000 e2enetworks-0.1.0/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       38 2023-06-07 11:16:20.939653 e2enetworks-0.1.0/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1871 2023-06-07 11:15:04.000000 e2enetworks-0.1.0/setup.py
```

### Comparing `e2enetworks-0.0.9/LICENSE.txt` & `e2enetworks-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.9/PKG-INFO` & `e2enetworks-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.9
+Version: 0.1.0
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -159,9 +158,7 @@
        --keep-until-expiring --non-interactive --expand \
        --server https://acme-v02.api.letsencrypt.org/directory \
        -d example.com -d '*.example.com'
 
 It is suggested to secure the folder as follows::
 chown root:root /etc/letsencrypt/.secrets
 chmod 600 /etc/letsencrypt/.secrets
-
-
```

### Comparing `e2enetworks-0.0.9/README.rst` & `e2enetworks-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.9/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.1.0/e2enetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.9
+Version: 0.1.0
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -159,9 +158,7 @@
        --keep-until-expiring --non-interactive --expand \
        --server https://acme-v02.api.letsencrypt.org/directory \
        -d example.com -d '*.example.com'
 
 It is suggested to secure the folder as follows::
 chown root:root /etc/letsencrypt/.secrets
 chmod 600 /etc/letsencrypt/.secrets
-
-
```

### Comparing `e2enetworks-0.0.9/setup.py` & `e2enetworks-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.9"
+version = "0.1.0"
 install_requires = [
-
+    "requests",
+    "urllib3==1.26.6",
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
     long_description = f.read()
```

