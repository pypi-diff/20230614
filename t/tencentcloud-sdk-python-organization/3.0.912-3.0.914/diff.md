# Comparing `tmp/tencentcloud-sdk-python-organization-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-organization-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.912.tar", last modified: Mon Jun 12 03:09:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-organization-3.0.914.tar", last modified: Wed Jun 14 00:31:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-organization-3.0.912.tar` & `tencentcloud-sdk-python-organization-3.0.914.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)    20412 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)    10169 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61815 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)    19620 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30659 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:09:04.000000 tencentcloud-sdk-python-organization-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      764 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)    23487 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)    10169 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73820 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)    19620 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30659 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:27.000000 tencentcloud-sdk-python-organization-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/README.rst` & `tencentcloud-sdk-python-organization-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/organization_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -252,14 +252,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeOrganizationFinancialByMember(self, request):
+        """以成员维度获取组织财务信息
+
+        :param request: Request instance for DescribeOrganizationFinancialByMember.
+        :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMemberRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMemberResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOrganizationFinancialByMember", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOrganizationFinancialByMemberResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeOrganizationFinancialByMonth(self, request):
+        """以月维度获取组织财务信息趋势
+
+        :param request: Request instance for DescribeOrganizationFinancialByMonth.
+        :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMonthRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByMonthResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOrganizationFinancialByMonth", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOrganizationFinancialByMonthResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeOrganizationFinancialByProduct(self, request):
+        """以产品维度获取组织财务信息
+
+        :param request: Request instance for DescribeOrganizationFinancialByProduct.
+        :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByProductRequest`
+        :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationFinancialByProductResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOrganizationFinancialByProduct", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOrganizationFinancialByProductResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeOrganizationMemberAuthAccounts(self, request):
         """获取组织成员被绑定授权关系的子账号列表
 
         :param request: Request instance for DescribeOrganizationMemberAuthAccounts.
         :type request: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberAuthAccountsRequest`
         :rtype: :class:`tencentcloud.organization.v20210331.models.DescribeOrganizationMemberAuthAccountsResponse`
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20210331/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -541,14 +541,239 @@
             for item in params.get("Items"):
                 obj = AuthNode()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeOrganizationFinancialByMemberRequest(AbstractModel):
+    """DescribeOrganizationFinancialByMember请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Month: 查询开始月份。格式：yyyy-mm，例如：2021-01。
+        :type Month: str
+        :param Limit: 限制数目。取值范围：1~50，默认值：10	
+        :type Limit: int
+        :param Offset: 偏移量。取值是limit的整数倍，默认值 : 0
+        :type Offset: int
+        :param EndMonth: 查询结束月份。格式：yyyy-mm，例如：2021-01,默认值为查询开始月份。
+        :type EndMonth: str
+        :param MemberUins: 查询成员列表。 最大100个
+        :type MemberUins: list of int
+        :param ProductCodes: 查询产品列表。 最大100个
+        :type ProductCodes: list of str
+        """
+        self.Month = None
+        self.Limit = None
+        self.Offset = None
+        self.EndMonth = None
+        self.MemberUins = None
+        self.ProductCodes = None
+
+
+    def _deserialize(self, params):
+        self.Month = params.get("Month")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.EndMonth = params.get("EndMonth")
+        self.MemberUins = params.get("MemberUins")
+        self.ProductCodes = params.get("ProductCodes")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOrganizationFinancialByMemberResponse(AbstractModel):
+    """DescribeOrganizationFinancialByMember返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCost: 当月总消耗。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: float
+        :param Items: 成员消耗详情。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Items: list of OrgMemberFinancial
+        :param Total: 总数目。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCost = None
+        self.Items = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCost = params.get("TotalCost")
+        if params.get("Items") is not None:
+            self.Items = []
+            for item in params.get("Items"):
+                obj = OrgMemberFinancial()
+                obj._deserialize(item)
+                self.Items.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeOrganizationFinancialByMonthRequest(AbstractModel):
+    """DescribeOrganizationFinancialByMonth请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Limit: 查询月数。取值范围：1~6，默认值：6
+        :type Limit: int
+        :param EndMonth: 查询结束月份。格式：yyyy-mm，例如：2021-01
+        :type EndMonth: str
+        :param MemberUins: 查询成员列表。 最大100个
+        :type MemberUins: list of int
+        :param ProductCodes: 查询产品列表。 最大100个
+        :type ProductCodes: list of str
+        """
+        self.Limit = None
+        self.EndMonth = None
+        self.MemberUins = None
+        self.ProductCodes = None
+
+
+    def _deserialize(self, params):
+        self.Limit = params.get("Limit")
+        self.EndMonth = params.get("EndMonth")
+        self.MemberUins = params.get("MemberUins")
+        self.ProductCodes = params.get("ProductCodes")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOrganizationFinancialByMonthResponse(AbstractModel):
+    """DescribeOrganizationFinancialByMonth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Items: 产品消耗详情。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Items: list of OrgFinancialByMonth
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Items = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Items") is not None:
+            self.Items = []
+            for item in params.get("Items"):
+                obj = OrgFinancialByMonth()
+                obj._deserialize(item)
+                self.Items.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeOrganizationFinancialByProductRequest(AbstractModel):
+    """DescribeOrganizationFinancialByProduct请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Month: 查询开始月份。格式：yyyy-mm，例如：2021-01
+        :type Month: str
+        :param Limit: 限制数目。取值范围：1~50，默认值：10	
+        :type Limit: int
+        :param Offset: 偏移量。取值是limit的整数倍，默认值 : 0
+        :type Offset: int
+        :param EndMonth: 查询结束月份。格式：yyyy-mm，例如：2021-01,默认值为查询开始月份
+        :type EndMonth: str
+        :param MemberUins: 查询成员列表。 最大100个
+        :type MemberUins: list of int
+        :param ProductCodes: 查询产品列表。 最大100个
+        :type ProductCodes: list of str
+        """
+        self.Month = None
+        self.Limit = None
+        self.Offset = None
+        self.EndMonth = None
+        self.MemberUins = None
+        self.ProductCodes = None
+
+
+    def _deserialize(self, params):
+        self.Month = params.get("Month")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.EndMonth = params.get("EndMonth")
+        self.MemberUins = params.get("MemberUins")
+        self.ProductCodes = params.get("ProductCodes")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOrganizationFinancialByProductResponse(AbstractModel):
+    """DescribeOrganizationFinancialByProduct返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCost: 当月总消耗。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: float
+        :param Items: 产品消耗详情。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Items: list of OrgProductFinancial
+        :param Total: 总数目。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCost = None
+        self.Items = None
+        self.Total = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCost = params.get("TotalCost")
+        if params.get("Items") is not None:
+            self.Items = []
+            for item in params.get("Items"):
+                obj = OrgProductFinancial()
+                obj._deserialize(item)
+                self.Items.append(obj)
+        self.Total = params.get("Total")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeOrganizationMemberAuthAccountsRequest(AbstractModel):
     """DescribeOrganizationMemberAuthAccounts请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1296,14 +1521,54 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class OrgFinancialByMonth(AbstractModel):
+    """按月获取组织财务信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: 记录ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param Month: 月份，格式：yyyy-mm，示例：2021-01。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Month: str
+        :param TotalCost: 消耗金额，单元：元。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: float
+        :param GrowthRate: 比上月增长率%。正数增长，负数下降，空值无法统计。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GrowthRate: str
+        """
+        self.Id = None
+        self.Month = None
+        self.TotalCost = None
+        self.GrowthRate = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.Month = params.get("Month")
+        self.TotalCost = params.get("TotalCost")
+        self.GrowthRate = params.get("GrowthRate")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OrgIdentity(AbstractModel):
     """组织身份
 
     """
 
     def __init__(self):
         r"""
@@ -1586,14 +1851,54 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class OrgMemberFinancial(AbstractModel):
+    """组织成员财务信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param MemberUin: 成员Uin。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MemberUin: int
+        :param MemberName: 成员名称。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MemberName: str
+        :param TotalCost: 消耗金额，单位：元。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: float
+        :param Ratio: 占比%。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Ratio: str
+        """
+        self.MemberUin = None
+        self.MemberName = None
+        self.TotalCost = None
+        self.Ratio = None
+
+
+    def _deserialize(self, params):
+        self.MemberUin = params.get("MemberUin")
+        self.MemberName = params.get("MemberName")
+        self.TotalCost = params.get("TotalCost")
+        self.Ratio = params.get("Ratio")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class OrgMemberPolicy(AbstractModel):
     """组织成员被授权的策略
 
     """
 
     def __init__(self):
         r"""
@@ -1722,14 +2027,54 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class OrgProductFinancial(AbstractModel):
+    """组织产品财务信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProductName: 产品Code。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductName: str
+        :param ProductCode: 产品名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProductCode: str
+        :param TotalCost: 产品消耗，单位：元。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: float
+        :param Ratio: 占比%。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Ratio: str
+        """
+        self.ProductName = None
+        self.ProductCode = None
+        self.TotalCost = None
+        self.Ratio = None
+
+
+    def _deserialize(self, params):
+        self.ProductName = params.get("ProductName")
+        self.ProductCode = params.get("ProductCode")
+        self.TotalCost = params.get("TotalCost")
+        self.Ratio = params.get("Ratio")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class UpdateOrganizationMemberEmailBindRequest(AbstractModel):
     """UpdateOrganizationMemberEmailBind请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.912'
+__version__ = '3.0.914'
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-organization-3.0.912/tencentcloud_sdk_python_organization.egg-info/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.914/tencentcloud_sdk_python_organization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.912
+Version: 3.0.914
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-organization-3.0.914/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-organization
-Version: 3.0.912
+Version: 3.0.914
 Summary: Tencent Cloud Organization SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-organization-3.0.912/setup.py` & `tencentcloud-sdk-python-organization-3.0.914/setup.py`

 * *Files identical despite different names*

