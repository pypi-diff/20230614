# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.913.tar", last modified: Tue Jun 13 02:11:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.914.tar", last modified: Wed Jun 14 00:26:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.913.tar` & `tencentcloud-sdk-python-ess-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    56524 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   240704 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:11:15.000000 tencentcloud-sdk-python-ess-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    57665 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   246979 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:26:15.000000 tencentcloud-sdk-python-ess-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:26:16.000000 tencentcloud-sdk-python-ess-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.913/README.rst` & `tencentcloud-sdk-python-ess-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,14 +737,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeExtendedServiceAuthInfos(self, request):
+        """查询企业扩展服务授权信息，目前支持查询：企业静默签，企业与港澳台居民签署合同，使用手机号验证签署方身份，骑缝章，批量签署能力是否已经开通
+
+        :param request: Request instance for DescribeExtendedServiceAuthInfos.
+        :type request: :class:`tencentcloud.ess.v20201111.models.DescribeExtendedServiceAuthInfosRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeExtendedServiceAuthInfosResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeExtendedServiceAuthInfos", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeExtendedServiceAuthInfosResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeFileUrls(self, request):
         """查询文件下载URL。
         适用场景：通过传参合同流程编号，下载对应的合同PDF文件流到本地。
 
         :param request: Request instance for DescribeFileUrls.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFileUrlsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFileUrlsResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.913/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.914/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,19 +711,18 @@
 NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
 FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
 
 ComponentType为SIGN_SIGNATURE类型可以控制签署方式
 {“ComponentTypeLimit”: [“xxx”]}
 xxx可以为：
 HANDWRITE – 手写签名
-BORDERLESS_ESIGN – 自动生成无边框腾讯体
 OCR_ESIGN -- AI智能识别手写签名
 ESIGN -- 个人印章类型
 SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
-如：{“ComponentTypeLimit”: [“BORDERLESS_ESIGN”]}
+如：{“ComponentTypeLimit”: [“SYSTEM_ESIGN”]}
 
 ComponentType为SIGN_DATE时，支持以下参数：
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
@@ -1853,15 +1852,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Employees: 待创建员工的信息，Mobile和DisplayName必填
+        :param Employees: 待创建员工的信息，Mobile和DisplayName必填,OpenId和Email选填，其他字段暂不支持
         :type Employees: list of Staff
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.Employees = None
         self.Agent = None
@@ -2945,14 +2944,81 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeExtendedServiceAuthInfosRequest(AbstractModel):
+    """DescribeExtendedServiceAuthInfos请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param ExtendServiceType: 扩展服务类型，默认为空，查询目前支持的所有扩展服务信息，单个指定则查询单个扩展服务开通信息，取值：
+OPEN_SERVER_SIGN：开通企业静默签署
+OVERSEA_SIGN：企业与港澳台居民签署合同
+MOBILE_CHECK_APPROVER：使用手机号验证签署方身份
+PAGING_SEAL：骑缝章
+BATCH_SIGN：批量签署
+        :type ExtendServiceType: str
+        """
+        self.Operator = None
+        self.Agent = None
+        self.ExtendServiceType = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
+        self.ExtendServiceType = params.get("ExtendServiceType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeExtendedServiceAuthInfosResponse(AbstractModel):
+    """DescribeExtendedServiceAuthInfos返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuthInfoList: 授权服务信息列表
+        :type AuthInfoList: list of ExtendAuthInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.AuthInfoList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("AuthInfoList") is not None:
+            self.AuthInfoList = []
+            for item in params.get("AuthInfoList"):
+                obj = ExtendAuthInfo()
+                obj._deserialize(item)
+                self.AuthInfoList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeFileUrlsRequest(AbstractModel):
     """DescribeFileUrls请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3250,17 +3316,15 @@
         :type ContentType: int
         :param Filters: 搜索条件，具体参考Filter结构体。本接口取值：template-id：按照【 **模板唯一标识** 】进行过滤
         :type Filters: list of Filter
         :param Offset: 查询偏移位置，默认0
         :type Offset: int
         :param Limit: 查询个数，默认20，最大200
         :type Limit: int
-        :param ApplicationId: 这个参数跟下面的IsChannel参数配合使用。
-IsChannel=false时，ApplicationId参数不起任何作用。
-IsChannel=true时，ApplicationId为空，查询所有第三方应用集成平台企业模板列表；ApplicationId不为空，查询指定应用下的模板列表
+        :param ApplicationId: ApplicationId不为空，查询指定应用下的模板列表
 ApplicationId为空，查询所有应用下的模板列表
         :type ApplicationId: str
         :param IsChannel: 默认为false，查询SaaS模板库列表；
 为true，查询第三方应用集成平台企业模板库管理列表
         :type IsChannel: bool
         :param Organization: 暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
@@ -3980,14 +4044,72 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ExtendAuthInfo(AbstractModel):
+    """授权服务信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 授权服务类型
+OPEN_SERVER_SIGN：开通企业静默签署
+OVERSEA_SIGN：企业与港澳台居民签署合同
+MOBILE_CHECK_APPROVER：使用手机号验证签署方身份
+PAGING_SEAL：骑缝章
+BATCH_SIGN：批量签署
+        :type Type: str
+        :param Name: 授权服务名称
+        :type Name: str
+        :param Status: 授权服务状态，ENABLE：开通
+DISABLE：未开通
+        :type Status: str
+        :param OperatorUserId: 授权人用户id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OperatorUserId: str
+        :param OperateOn: 授权时间戳，单位秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OperateOn: int
+        :param HasAuthUserList: 被授权用户列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HasAuthUserList: list of HasAuthUser
+        """
+        self.Type = None
+        self.Name = None
+        self.Status = None
+        self.OperatorUserId = None
+        self.OperateOn = None
+        self.HasAuthUserList = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        self.Name = params.get("Name")
+        self.Status = params.get("Status")
+        self.OperatorUserId = params.get("OperatorUserId")
+        self.OperateOn = params.get("OperateOn")
+        if params.get("HasAuthUserList") is not None:
+            self.HasAuthUserList = []
+            for item in params.get("HasAuthUserList"):
+                obj = HasAuthUser()
+                obj._deserialize(item)
+                self.HasAuthUserList.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FailedCreateRoleData(AbstractModel):
     """绑定角色失败信息
 
     """
 
     def __init__(self):
         r"""
@@ -4965,14 +5087,46 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class HasAuthUser(AbstractModel):
+    """被授权用户信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserId: 用户id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserId: str
+        :param BelongTo: 用户归属
+MainOrg：主企业
+CurrentOrg：当前企业
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BelongTo: str
+        """
+        self.UserId = None
+        self.BelongTo = None
+
+
+    def _deserialize(self, params):
+        self.UserId = params.get("UserId")
+        self.BelongTo = params.get("BelongTo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class IntegrateRole(AbstractModel):
     """企业角色数据信息
 
     """
 
     def __init__(self):
         r"""
@@ -5605,14 +5759,20 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SealInfo(AbstractModel):
+    """模板结构体中的印章信息
+
+    """
+
+
 class SignQrCode(AbstractModel):
     """一码多扫签署二维码对象
 
     """
 
     def __init__(self):
         r"""
@@ -6003,14 +6163,20 @@
         :type PreviewUrl: str
         :param TemplateVersion: 模板版本。默认为空时，全数字字符，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateVersion: str
         :param Published: 模板是否已发布。true-已发布；false-未发布
 注意：此字段可能返回 null，表示取不到有效值。
         :type Published: bool
+        :param TemplateSeals: 模板内部指定的印章列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TemplateSeals: list of SealInfo
+        :param Seals: 模板内部指定的印章列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Seals: list of SealInfo
         """
         self.TemplateId = None
         self.TemplateName = None
         self.Description = None
         self.DocumentResourceIds = None
         self.FileInfos = None
         self.AttachmentResourceIds = None
@@ -6024,14 +6190,16 @@
         self.Promoter = None
         self.TemplateType = None
         self.Available = None
         self.OrganizationId = None
         self.PreviewUrl = None
         self.TemplateVersion = None
         self.Published = None
+        self.TemplateSeals = None
+        self.Seals = None
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.TemplateName = params.get("TemplateName")
         self.Description = params.get("Description")
         self.DocumentResourceIds = params.get("DocumentResourceIds")
@@ -6069,14 +6237,26 @@
             self.Promoter._deserialize(params.get("Promoter"))
         self.TemplateType = params.get("TemplateType")
         self.Available = params.get("Available")
         self.OrganizationId = params.get("OrganizationId")
         self.PreviewUrl = params.get("PreviewUrl")
         self.TemplateVersion = params.get("TemplateVersion")
         self.Published = params.get("Published")
+        if params.get("TemplateSeals") is not None:
+            self.TemplateSeals = []
+            for item in params.get("TemplateSeals"):
+                obj = SealInfo()
+                obj._deserialize(item)
+                self.TemplateSeals.append(obj)
+        if params.get("Seals") is not None:
+            self.Seals = []
+            for item in params.get("Seals"):
+                obj = SealInfo()
+                obj._deserialize(item)
+                self.Seals.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6140,17 +6320,17 @@
 class UpdateIntegrationEmployeesRequest(AbstractModel):
     """UpdateIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param Employees: 员工信息
+        :param Employees: 员工信息，OpenId和UserId必填一个,Email、DisplayName和Email选填，其他字段暂不支持
         :type Employees: list of Staff
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.Employees = None
         self.Agent = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.913/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.914/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.914/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.913/setup.py` & `tencentcloud-sdk-python-ess-3.0.914/setup.py`

 * *Files identical despite different names*

