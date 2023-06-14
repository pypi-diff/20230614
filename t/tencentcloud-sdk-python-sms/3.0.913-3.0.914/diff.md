# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.913.tar", last modified: Tue Jun 13 02:23:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.914.tar", last modified: Wed Jun 14 00:33:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.913.tar` & `tencentcloud-sdk-python-sms-3.0.914.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)    26567 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60142 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)    28333 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68439 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:23:57.000000 tencentcloud-sdk-python-sms-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)    26567 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60170 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)    28333 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68482 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:33:07.000000 tencentcloud-sdk-python-sms-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sms-3.0.913/README.rst` & `tencentcloud-sdk-python-sms-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20190711/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,18 +676,15 @@
         r"""
         :param TemplateId: 模板Id
         :type TemplateId: int
         :param International: 是否国际/港澳台短信：
 0：表示国内短信。
 1：表示国际/港澳台短信。
         :type International: int
-        :param StatusCode: 申请签名状态。其中：
-0：表示审核通过。
-1：表示审核中。
--1：表示审核未通过或审核失败。
+        :param StatusCode: 申请模板状态，其中0表示审核通过且已生效，1表示审核中，2表示审核通过待生效，-1表示审核未通过或审核失败。
         :type StatusCode: int
         :param ReviewReply: 审核回复，审核人员审核后给出的回复，通常是审核未通过的原因。
         :type ReviewReply: str
         :param TemplateName: 模板名称。
         :type TemplateName: str
         :param CreateTime: 提交审核时间，UNIX 时间戳（单位：秒）。
         :type CreateTime: int
```

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/sms/v20210111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,15 +729,15 @@
 
     def __init__(self):
         r"""
         :param TemplateId: 模板ID。
         :type TemplateId: int
         :param International: 是否国际/港澳台短信，其中0表示国内短信，1表示国际/港澳台短信。
         :type International: int
-        :param StatusCode: 申请模板状态，其中0表示审核通过，1表示审核中，-1表示审核未通过或审核失败。
+        :param StatusCode: 申请模板状态，其中0表示审核通过且已生效，1表示审核中，2表示审核通过待生效，-1表示审核未通过或审核失败。
         :type StatusCode: int
         :param ReviewReply: 审核回复，审核人员审核后给出的回复，通常是审核未通过的原因。
         :type ReviewReply: str
         :param TemplateName: 模板名称。
         :type TemplateName: str
         :param CreateTime: 提交审核时间，UNIX 时间戳（单位：秒）。
         :type CreateTime: int
```

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.913/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.914/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.914/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.913/setup.py` & `tencentcloud-sdk-python-sms-3.0.914/setup.py`

 * *Files identical despite different names*

