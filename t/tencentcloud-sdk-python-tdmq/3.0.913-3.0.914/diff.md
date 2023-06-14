# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.913.tar", last modified: Tue Jun 13 02:26:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.914.tar", last modified: Wed Jun 14 00:35:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.913.tar` & `tencentcloud-sdk-python-tdmq-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   110188 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   405083 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:26:29.000000 tencentcloud-sdk-python-tdmq-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   109282 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   403511 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-14 00:35:34.000000 tencentcloud-sdk-python-tdmq-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:35:35.000000 tencentcloud-sdk-python-tdmq-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2151,39 +2151,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def ModifyAMQPVHost(self, request):
-        """产品下线了，对应的接口也要下线。
-
-        更新Vhost
-
-        :param request: Request instance for ModifyAMQPVHost.
-        :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyAMQPVHostRequest`
-        :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyAMQPVHostResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("ModifyAMQPVHost", params, headers=headers)
-            response = json.loads(body)
-            model = models.ModifyAMQPVHostResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def ModifyCluster(self, request):
         """更新集群信息
 
         :param request: Request instance for ModifyCluster.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyClusterRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyClusterResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7401,67 +7401,14 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
-class ModifyAMQPVHostRequest(AbstractModel):
-    """ModifyAMQPVHost请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClusterId: 集群ID
-        :type ClusterId: str
-        :param VHostId: vhost名称，3-64个字符，只能包含字母、数字、“-”及“_”
-        :type VHostId: str
-        :param MsgTtl: 未消费消息的保留时间，以毫秒为单位，60秒-15天
-        :type MsgTtl: int
-        :param Remark: 说明，最大128个字符
-        :type Remark: str
-        """
-        self.ClusterId = None
-        self.VHostId = None
-        self.MsgTtl = None
-        self.Remark = None
-
-
-    def _deserialize(self, params):
-        self.ClusterId = params.get("ClusterId")
-        self.VHostId = params.get("VHostId")
-        self.MsgTtl = params.get("MsgTtl")
-        self.Remark = params.get("Remark")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class ModifyAMQPVHostResponse(AbstractModel):
-    """ModifyAMQPVHost返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
-
-
 class ModifyClusterRequest(AbstractModel):
     """ModifyCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.914/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.914/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.913/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.914/setup.py`

 * *Files identical despite different names*

