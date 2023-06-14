# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.913.tar", last modified: Tue Jun 13 02:11:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.914.tar", last modified: Wed Jun 14 00:25:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.913.tar` & `tencentcloud-sdk-python-eis-3.0.914.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5846 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24178 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13436 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:11:00.000000 tencentcloud-sdk-python-eis-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5846 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24178 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13436 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:25:58.000000 tencentcloud-sdk-python-eis-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-eis-3.0.913/README.rst` & `tencentcloud-sdk-python-eis-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20210601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.913/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.914/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.914/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.913/setup.py` & `tencentcloud-sdk-python-eis-3.0.914/setup.py`

 * *Files identical despite different names*
