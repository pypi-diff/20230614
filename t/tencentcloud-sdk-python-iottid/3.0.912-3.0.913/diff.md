# Comparing `tmp/tencentcloud-sdk-python-iottid-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-iottid-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.912.tar", last modified: Mon Jun 12 03:06:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iottid-3.0.913.tar", last modified: Tue Jun 13 02:13:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iottid-3.0.912.tar` & `tencentcloud-sdk-python-iottid-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/
--rw-r--r--   0 root         (0) root         (0)     9130 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/iottid_client.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15254 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:06:07.000000 tencentcloud-sdk-python-iottid-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/
+-rw-r--r--   0 root         (0) root         (0)     9130 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/iottid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15254 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:13:37.000000 tencentcloud-sdk-python-iottid-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/README.rst` & `tencentcloud-sdk-python-iottid-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/iottid_client.py` & `tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/iottid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/errorcodes.py` & `tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/iottid/v20190411/models.py` & `tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/iottid/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iottid-3.0.913/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.912'
+__version__ = '3.0.913'
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.913/tencentcloud_sdk_python_iottid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-iottid-3.0.913/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iottid
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Iottid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iottid-3.0.912/setup.py` & `tencentcloud-sdk-python-iottid-3.0.913/setup.py`

 * *Files identical despite different names*

