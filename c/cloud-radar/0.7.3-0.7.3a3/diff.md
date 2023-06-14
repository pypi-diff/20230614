# Comparing `tmp/cloud_radar-0.7.3.tar.gz` & `tmp/cloud_radar-0.7.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.7.3.tar", max compression
+gzip compressed data, was "cloud_radar-0.7.3a3.tar", max compression
```

## Comparing `cloud_radar-0.7.3.tar` & `cloud_radar-0.7.3a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-14 00:04:21.130693 cloud_radar-0.7.3/LICENSE.txt
--rw-r--r--   0        0        0    13927 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/README.md
--rw-r--r--   0        0        0     1433 2023-06-14 00:04:37.476005 cloud_radar-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0    15434 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-06-14 00:04:21.134694 cloud_radar-0.7.3/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    15081 1970-01-01 00:00:00.000000 cloud_radar-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/LICENSE.txt
+-rw-r--r--   0        0        0    13927 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/README.md
+-rw-r--r--   0        0        0     1435 2023-06-13 23:49:16.199117 cloud_radar-0.7.3a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    15434 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-13 23:49:02.139008 cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    15083 1970-01-01 00:00:00.000000 cloud_radar-0.7.3a3/PKG-INFO
```

### Comparing `cloud_radar-0.7.3/LICENSE.txt` & `cloud_radar-0.7.3a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/README.md` & `cloud_radar-0.7.3a3/README.md`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/pyproject.toml` & `cloud_radar-0.7.3a3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.7.3"
+version = "0.7.3a3"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/_template.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.7.3a3/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.3/PKG-INFO` & `cloud_radar-0.7.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.7.3
+Version: 0.7.3a3
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.3 Summary: Run functional
-tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
-cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
-radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
-shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Testing Requires-Dist:
-cfn-flip (>=1.2.3,<2.0.0) Requires-Dist: taskcat (>=0.9.20,<0.10.0) Project-
-URL: Repository, https://github.com/DontShaveTheYak/cloud-radar Description-
-Content-Type: text/markdown   [![Python][python-shield]][pypi-url] [![Latest]
-[version-shield]][pypi-url] [![Tests][test-shield]][test-url] [![Coverage]
-[codecov-shield]][codecov-url] [![License][license-shield]][license-url]
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.3a3 Summary: Run
+functional tests on cloudformation stacks. Home-page: https://github.com/
+DontShaveTheYak/cloud-radar License: Apache-2.0 Keywords:
+aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar Author: Levi Blaney
+Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Testing
+Requires-Dist: cfn-flip (>=1.2.3,<2.0.0) Requires-Dist: taskcat
+(>=0.9.20,<0.10.0) Project-URL: Repository, https://github.com/DontShaveTheYak/
+cloud-radar Description-Content-Type: text/markdown   [![Python][python-
+shield]][pypi-url] [![Latest][version-shield]][pypi-url] [![Tests][test-
+shield]][test-url] [![Coverage][codecov-shield]][codecov-url] [![License]
+[license-shield]][license-url]
                              **** Cloud-Radar ****
            Write unit and functional tests for AWS Cloudformation.
                      Report_Bug Â· Request_Feature Â· Guide
   Table of Contents
    1. About_The_Project
           o Built_With
    2. Getting_Started
```

