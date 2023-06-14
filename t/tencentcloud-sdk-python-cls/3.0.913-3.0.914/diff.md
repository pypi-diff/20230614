# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.913.tar", last modified: Tue Jun 13 02:07:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.914.tar", last modified: Wed Jun 14 00:22:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.913.tar` & `tencentcloud-sdk-python-cls-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8715 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254814 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67913 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:07:59.000000 tencentcloud-sdk-python-cls-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   254810 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67913 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:22:50.000000 tencentcloud-sdk-python-cls-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.913/README.rst` & `tencentcloud-sdk-python-cls-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2073,15 +2073,15 @@
         :type Bucket: str
         :param Prefix: 创建的投递规则投递目录的前缀
         :type Prefix: str
         :param ShipperName: 投递规则的名字
         :type ShipperName: str
         :param Interval: 投递的时间间隔，单位 秒，默认300，范围 300-900
         :type Interval: int
-        :param MaxSize: 投递的文件的最大值，单位 MB，默认256，范围 100-256
+        :param MaxSize: 投递的文件的最大值，单位 MB，默认256，范围 5-256
         :type MaxSize: int
         :param FilterRules: 投递日志的过滤规则，匹配的日志进行投递，各rule之间是and关系，最多5个，数组为空则表示不过滤而全部投递
         :type FilterRules: list of FilterRuleInfo
         :param Partition: 投递日志的分区规则，支持strftime的时间格式表示
         :type Partition: str
         :param Compress: 投递日志的压缩配置
         :type Compress: :class:`tencentcloud.cls.v20201016.models.CompressInfo`
@@ -6082,15 +6082,15 @@
         :type Prefix: str
         :param Status: 投递规则的开关状态
         :type Status: bool
         :param ShipperName: 投递规则的名字
         :type ShipperName: str
         :param Interval: 投递的时间间隔，单位 秒，默认300，范围 300-900
         :type Interval: int
-        :param MaxSize: 投递的文件的最大值，单位 MB，默认256，范围 100-256
+        :param MaxSize: 投递的文件的最大值，单位 MB，默认256，范围 5-256
         :type MaxSize: int
         :param FilterRules: 投递日志的过滤规则，匹配的日志进行投递，各rule之间是and关系，最多5个，数组为空则表示不过滤而全部投递
         :type FilterRules: list of FilterRuleInfo
         :param Partition: 投递日志的分区规则，支持strftime的时间格式表示
         :type Partition: str
         :param Compress: 投递日志的压缩配置
         :type Compress: :class:`tencentcloud.cls.v20201016.models.CompressInfo`
```

### Comparing `tencentcloud-sdk-python-cls-3.0.913/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.914/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.913/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.914/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.914/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.913/setup.py` & `tencentcloud-sdk-python-cls-3.0.914/setup.py`

 * *Files identical despite different names*

