# Comparing `tmp/cloud_radar-0.7.1.tar.gz` & `tmp/cloud_radar-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.7.1.tar", max compression
+gzip compressed data, was "cloud_radar-0.7.2.tar", max compression
```

## Comparing `cloud_radar-0.7.1.tar` & `cloud_radar-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0    12370 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/README.md
--rw-r--r--   0        0        0     1433 2023-06-01 13:36:24.944476 cloud_radar-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0    11587 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-06-01 13:36:09.488122 cloud_radar-0.7.1/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    13524 1970-01-01 00:00:00.000000 cloud_radar-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 15:43:59.854068 cloud_radar-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0    12370 2023-06-01 15:43:59.854068 cloud_radar-0.7.2/README.md
+-rw-r--r--   0        0        0     1433 2023-06-01 15:44:10.498221 cloud_radar-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    11832 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-01 15:43:59.858068 cloud_radar-0.7.2/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    13524 1970-01-01 00:00:00.000000 cloud_radar-0.7.2/PKG-INFO
```

### Comparing `cloud_radar-0.7.1/LICENSE.txt` & `cloud_radar-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/README.md` & `cloud_radar-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/pyproject.toml` & `cloud_radar-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.7.1"
+version = "0.7.2"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -208,17 +208,20 @@
                         value,
                         allowed_func,
                     )
                     continue
 
                 # Takes care of the tricky 'Condition' key
                 if key == "Condition":
-                    # This takes care of conditional resources
-                    if "Properties" in data:
-                        # data[key] = functions.condition(self, value)
+                    # The real fix is to not resolve every key/value in the entire
+                    # cloudformation template. We should only attempt to resolve what is needed,
+                    # like outputs and resource properties.
+                    # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference.html
+
+                    if "Properties" in data or "Value" in data:
                         continue
 
                     # If it's an intrinsic func
                     if is_condition_func(value):
                         return functions.condition(self, value)
 
                     # Normal key like in an IAM role
```

### Comparing `cloud_radar-0.7.1/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.7.2/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.7.1/PKG-INFO` & `cloud_radar-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.7.1
+Version: 0.7.2
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.1 Summary: Run functional
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.7.2 Summary: Run functional
 tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
 cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
 radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
 shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
```

