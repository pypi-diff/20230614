# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.912.tar", last modified: Mon Jun 12 03:11:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.913.tar", last modified: Tue Jun 13 02:24:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.912.tar` & `tencentcloud-sdk-python-ssl-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     9587 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223934 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    49507 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     9587 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   225118 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    49507 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:24:26.000000 tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/README.rst` & `tencentcloud-sdk-python-ssl-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,17 +76,17 @@
         :type PackageType: str
         :param ContactEmail: 邮箱。
         :type ContactEmail: str
         :param ContactPhone: 手机。
         :type ContactPhone: str
         :param ValidityPeriod: 有效期，默认12个月，目前仅支持12个月。
         :type ValidityPeriod: str
-        :param CsrEncryptAlgo: 加密算法，仅支持 RSA。
+        :param CsrEncryptAlgo: 加密算法，支持 RSA及ECC。
         :type CsrEncryptAlgo: str
-        :param CsrKeyParameter: 密钥对参数，仅支持2048。
+        :param CsrKeyParameter: 密钥对参数，RSA仅支持2048。ECC仅支持prime256v1
         :type CsrKeyParameter: str
         :param CsrKeyPassword: CSR 的加密密码。
         :type CsrKeyPassword: str
         :param Alias: 备注名称。
         :type Alias: str
         :param OldCertificateId: 原证书 ID，用于重新申请。
         :type OldCertificateId: str
@@ -3303,20 +3303,28 @@
 
     """
 
     def __init__(self):
         r"""
         :param DeployRecordId: 待部署的证书ID
         :type DeployRecordId: str
+        :param Limit: 每页数量，默认10。
+        :type Limit: str
+        :param Offset: 分页偏移量，从0开始。
+        :type Offset: str
         """
         self.DeployRecordId = None
+        self.Limit = None
+        self.Offset = None
 
 
     def _deserialize(self, params):
         self.DeployRecordId = params.get("DeployRecordId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5649,29 +5657,38 @@
         :type UpdateTime: str
         :param InstanceId: 部署实例ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceId: str
         :param InstanceName: 部署实例名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceName: str
-        :param ListenerId: 部署监听器ID
+        :param ListenerId: 部署监听器ID（CLB专用）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ListenerId: str
-        :param ListenerName: 部署监听器名称
+        :param ListenerName: 部署监听器名称（CLB专用）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ListenerName: str
         :param Protocol: 协议
 注意：此字段可能返回 null，表示取不到有效值。
         :type Protocol: str
-        :param SniSwitch: 是否开启SNI
+        :param SniSwitch: 是否开启SNI（CLB专用）
 注意：此字段可能返回 null，表示取不到有效值。
         :type SniSwitch: int
-        :param Bucket: bucket名称
+        :param Bucket: bucket名称（COS专用）
 注意：此字段可能返回 null，表示取不到有效值。
         :type Bucket: str
+        :param Port: 端口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Port: int
+        :param Namespace: 命名空间（TKE专用）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Namespace: str
+        :param SecretName: secret名称（TKE专用）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SecretName: str
         """
         self.Id = None
         self.CertId = None
         self.OldCertId = None
         self.Domains = None
         self.ResourceType = None
         self.Region = None
@@ -5682,14 +5699,17 @@
         self.InstanceId = None
         self.InstanceName = None
         self.ListenerId = None
         self.ListenerName = None
         self.Protocol = None
         self.SniSwitch = None
         self.Bucket = None
+        self.Port = None
+        self.Namespace = None
+        self.SecretName = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.CertId = params.get("CertId")
         self.OldCertId = params.get("OldCertId")
         self.Domains = params.get("Domains")
@@ -5702,14 +5722,17 @@
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.ListenerId = params.get("ListenerId")
         self.ListenerName = params.get("ListenerName")
         self.Protocol = params.get("Protocol")
         self.SniSwitch = params.get("SniSwitch")
         self.Bucket = params.get("Bucket")
+        self.Port = params.get("Port")
+        self.Namespace = params.get("Namespace")
+        self.SecretName = params.get("SecretName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5722,27 +5745,31 @@
 
     def __init__(self):
         r"""
         :param ResourceType: 部署资源类型
         :type ResourceType: str
         :param List: 部署资源详情列表
         :type List: list of UpdateRecordDetail
+        :param TotalCount: 该部署资源总数
+        :type TotalCount: int
         """
         self.ResourceType = None
         self.List = None
+        self.TotalCount = None
 
 
     def _deserialize(self, params):
         self.ResourceType = params.get("ResourceType")
         if params.get("List") is not None:
             self.List = []
             for item in params.get("List"):
                 obj = UpdateRecordDetail()
                 obj._deserialize(item)
                 self.List.append(obj)
+        self.TotalCount = params.get("TotalCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.913/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.913/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/setup.py` & `tencentcloud-sdk-python-ssl-3.0.913/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.913/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

