# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.913.tar", last modified: Tue Jun 13 02:09:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.914.tar", last modified: Wed Jun 14 00:24:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.913.tar` & `tencentcloud-sdk-python-dbbrain-3.0.914.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    48612 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185526 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114440 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:09:31.000000 tencentcloud-sdk-python-dbbrain-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185526 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114440 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2560,15 +2560,15 @@
         :type InstanceId: str
         :param StartTime: 查询范围的开始时间，时间格式如：2019-09-10 12:13:14。
         :type StartTime: str
         :param EndTime: 查询范围的结束时间，时间格式如：2019-09-10 12:13:14。
         :type EndTime: str
         :param Product: 服务产品类型，支持值："mysql" - 云数据库 MySQL；"cynosdb" - 云数据库 TDSQL-C for MySQL，默认为"mysql"。
         :type Product: str
-        :param Md5: SOL模板的MD5值
+        :param Md5: SQL模板的MD5值
         :type Md5: str
         """
         self.InstanceId = None
         self.StartTime = None
         self.EndTime = None
         self.Product = None
         self.Md5 = None
@@ -4858,15 +4858,15 @@
         :type QueryTimeAvg: float
         :param RowsSentAvg: 平均返回行数
         :type RowsSentAvg: float
         :param LockTimeAvg: 平均锁等待时间，单位秒
         :type LockTimeAvg: float
         :param RowsExaminedAvg: 平均扫描行数
         :type RowsExaminedAvg: float
-        :param Md5: SOL模板的MD5值
+        :param Md5: SQL模板的MD5值
         :type Md5: str
         """
         self.LockTime = None
         self.LockTimeMax = None
         self.LockTimeMin = None
         self.RowsExamined = None
         self.RowsExaminedMax = None
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.914/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.914/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.913/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.914/setup.py`

 * *Files identical despite different names*

