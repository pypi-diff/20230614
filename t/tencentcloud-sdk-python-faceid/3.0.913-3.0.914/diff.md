# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.913.tar", last modified: Tue Jun 13 02:11:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.914.tar", last modified: Wed Jun 14 00:26:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.913.tar` & `tencentcloud-sdk-python-faceid-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)    34030 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141706 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:11:33.000000 tencentcloud-sdk-python-faceid-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)    34030 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141706 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:26:30.000000 tencentcloud-sdk-python-faceid-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/README.rst` & `tencentcloud-sdk-python-faceid-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/faceid/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.914/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.913'
+__version__ = '3.0.914'
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.914/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/setup.py` & `tencentcloud-sdk-python-faceid-3.0.914/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.913/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.914/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

