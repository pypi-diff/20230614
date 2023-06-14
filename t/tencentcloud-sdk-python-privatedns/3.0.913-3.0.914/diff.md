# Comparing `tmp/tencentcloud-sdk-python-privatedns-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-privatedns-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.913.tar", last modified: Tue Jun 13 02:22:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-privatedns-3.0.914.tar", last modified: Wed Jun 14 00:31:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-privatedns-3.0.913.tar` & `tencentcloud-sdk-python-privatedns-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/
--rw-r--r--   0 root         (0) root         (0)     7186 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57994 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)    20216 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/privatedns_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:22:46.000000 tencentcloud-sdk-python-privatedns-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/
+-rw-r--r--   0 root         (0) root         (0)     7535 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59039 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)    21077 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/privatedns_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:49.000000 tencentcloud-sdk-python-privatedns-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/README.rst` & `tencentcloud-sdk-python-privatedns-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/errorcodes.py` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 # 当前私有域已关联 VPC，如需清空解析记录请先解除 VPC 关联。
 FAILEDOPERATION_DELETELASTBINDVPCRECORDFAILED = 'FailedOperation.DeleteLastBindVpcRecordFailed'
 
 # 记录删除失败。
 FAILEDOPERATION_DELETERECORDFAILED = 'FailedOperation.DeleteRecordFailed'
 
+# 删除终端节点失败。
+FAILEDOPERATION_DELETEVPCENDPOINTFAILED = 'FailedOperation.DeleteVpcEndPointFailed'
+
 # 解析域删除失败。
 FAILEDOPERATION_DELETEZONEFAILED = 'FailedOperation.DeleteZoneFailed'
 
 # 记录修改失败。
 FAILEDOPERATION_MODIFYRECORDFAILED = 'FailedOperation.ModifyRecordFailed'
 
 # 私有域修改失败。
@@ -61,14 +64,20 @@
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 已经存在绑定的账号。
 INVALIDPARAMETER_ACCOUNTEXIST = 'InvalidParameter.AccountExist'
 
+# 终端节点已经绑定了转发规则。
+INVALIDPARAMETER_ENDPOINTBINDFORWARDRULE = 'InvalidParameter.EndPointBindForwardRule'
+
+# 终端节点不存在。
+INVALIDPARAMETER_ENDPOINTNOTEXISTS = 'InvalidParameter.EndPointNotExists'
+
 # 非法CIDR。
 INVALIDPARAMETER_ILLEGALCIDR = 'InvalidParameter.IllegalCidr'
 
 # 域名不正确。
 INVALIDPARAMETER_ILLEGALDOMAIN = 'InvalidParameter.IllegalDomain'
 
 # 顶级域名不正确。
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/models.py` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,14 +431,55 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteEndPointRequest(AbstractModel):
+    """DeleteEndPoint请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EndPointId: 终端节点ID
+        :type EndPointId: str
+        """
+        self.EndPointId = None
+
+
+    def _deserialize(self, params):
+        self.EndPointId = params.get("EndPointId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteEndPointResponse(AbstractModel):
+    """DeleteEndPoint返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeletePrivateDNSAccountRequest(AbstractModel):
     """DeletePrivateDNSAccount请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/privatedns/v20201028/privatedns_client.py` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/privatedns/v20201028/privatedns_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteEndPoint(self, request):
+        """删除终端节点
+
+        :param request: Request instance for DeleteEndPoint.
+        :type request: :class:`tencentcloud.privatedns.v20201028.models.DeleteEndPointRequest`
+        :rtype: :class:`tencentcloud.privatedns.v20201028.models.DeleteEndPointResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteEndPoint", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteEndPointResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeletePrivateDNSAccount(self, request):
         """删除私有域解析账号
 
         :param request: Request instance for DeletePrivateDNSAccount.
         :type request: :class:`tencentcloud.privatedns.v20201028.models.DeletePrivateDNSAccountRequest`
         :rtype: :class:`tencentcloud.privatedns.v20201028.models.DeletePrivateDNSAccountResponse`
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.914/tencentcloud_sdk_python_privatedns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-privatedns-3.0.914/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-privatedns
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Privatedns SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-privatedns-3.0.913/setup.py` & `tencentcloud-sdk-python-privatedns-3.0.914/setup.py`

 * *Files identical despite different names*

