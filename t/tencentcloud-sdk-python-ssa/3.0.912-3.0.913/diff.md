# Comparing `tmp/tencentcloud-sdk-python-ssa-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-ssa-3.0.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.912.tar", last modified: Mon Jun 12 03:11:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssa-3.0.913.tar", last modified: Tue Jun 13 02:24:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssa-3.0.912.tar` & `tencentcloud-sdk-python-ssa-3.0.913.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158213 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)    21767 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/ssa_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:11:07.000000 tencentcloud-sdk-python-ssa-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165915 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)    22641 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/ssa_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:24:21.000000 tencentcloud-sdk-python-ssa-3.0.913/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/README.rst` & `tencentcloud-sdk-python-ssa-3.0.913/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/errorcodes.py` & `tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/models.py` & `tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2445,14 +2445,117 @@
             for item in params.get("Data"):
                 obj = DataCheck()
                 obj._deserialize(item)
                 self.Data.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDomainListRequest(AbstractModel):
+    """DescribeDomainList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Offset: -
+        :type Offset: int
+        :param Limit: -
+        :type Limit: int
+        :param AssetBasicType: -
+        :type AssetBasicType: int
+        :param Filter: -
+        :type Filter: list of QueryFilterV3
+        :param Order: -
+        :type Order: str
+        :param By: -
+        :type By: str
+        :param Field: -
+        :type Field: list of str
+        :param TimeRange: -
+        :type TimeRange: int
+        :param Logic: -
+        :type Logic: int
+        :param GroupByField: -
+        :type GroupByField: str
+        :param Task: -
+        :type Task: str
+        :param RequestFrom: -
+        :type RequestFrom: int
+        """
+        self.Offset = None
+        self.Limit = None
+        self.AssetBasicType = None
+        self.Filter = None
+        self.Order = None
+        self.By = None
+        self.Field = None
+        self.TimeRange = None
+        self.Logic = None
+        self.GroupByField = None
+        self.Task = None
+        self.RequestFrom = None
+
+
+    def _deserialize(self, params):
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.AssetBasicType = params.get("AssetBasicType")
+        if params.get("Filter") is not None:
+            self.Filter = []
+            for item in params.get("Filter"):
+                obj = QueryFilterV3()
+                obj._deserialize(item)
+                self.Filter.append(obj)
+        self.Order = params.get("Order")
+        self.By = params.get("By")
+        self.Field = params.get("Field")
+        self.TimeRange = params.get("TimeRange")
+        self.Logic = params.get("Logic")
+        self.GroupByField = params.get("GroupByField")
+        self.Task = params.get("Task")
+        self.RequestFrom = params.get("RequestFrom")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDomainListResponse(AbstractModel):
+    """DescribeDomainList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 无
+        :type Total: int
+        :param DomainInfoCollection: 无
+        :type DomainInfoCollection: list of DomainInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.DomainInfoCollection = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("DomainInfoCollection") is not None:
+            self.DomainInfoCollection = []
+            for item in params.get("DomainInfoCollection"):
+                obj = DomainInfo()
+                obj._deserialize(item)
+                self.DomainInfoCollection.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeEventDetailRequest(AbstractModel):
     """DescribeEventDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3323,14 +3426,98 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self.Data = VulList()
             self.Data._deserialize(params.get("Data"))
         self.RequestId = params.get("RequestId")
 
 
+class DomainInfo(AbstractModel):
+    """域名列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Domain: 域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Domain: str
+        :param ResolveAddr: 解析地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResolveAddr: list of str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: list of str
+        :param AssetType: 资产类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetType: list of str
+        :param RiskVulCount: 漏洞风险
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RiskVulCount: int
+        :param SensitiveCount: 敏感内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SensitiveCount: int
+        :param HorseLinkCount: 挂马暗链
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HorseLinkCount: int
+        :param WebModifyCount: 网页篡改
+        :type WebModifyCount: int
+        :param ScanTime: 上次扫描时间
+        :type ScanTime: str
+        :param DiscoverTime: 最近发现时间
+        :type DiscoverTime: str
+        :param ScanTaskCount: 扫描次数
+        :type ScanTaskCount: int
+        :param PortRisk: 端口
+        :type PortRisk: int
+        :param WeekPwdCount: 弱口令
+        :type WeekPwdCount: int
+        :param AssetLocation: -
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetLocation: str
+        """
+        self.Domain = None
+        self.ResolveAddr = None
+        self.Region = None
+        self.AssetType = None
+        self.RiskVulCount = None
+        self.SensitiveCount = None
+        self.HorseLinkCount = None
+        self.WebModifyCount = None
+        self.ScanTime = None
+        self.DiscoverTime = None
+        self.ScanTaskCount = None
+        self.PortRisk = None
+        self.WeekPwdCount = None
+        self.AssetLocation = None
+
+
+    def _deserialize(self, params):
+        self.Domain = params.get("Domain")
+        self.ResolveAddr = params.get("ResolveAddr")
+        self.Region = params.get("Region")
+        self.AssetType = params.get("AssetType")
+        self.RiskVulCount = params.get("RiskVulCount")
+        self.SensitiveCount = params.get("SensitiveCount")
+        self.HorseLinkCount = params.get("HorseLinkCount")
+        self.WebModifyCount = params.get("WebModifyCount")
+        self.ScanTime = params.get("ScanTime")
+        self.DiscoverTime = params.get("DiscoverTime")
+        self.ScanTaskCount = params.get("ScanTaskCount")
+        self.PortRisk = params.get("PortRisk")
+        self.WeekPwdCount = params.get("WeekPwdCount")
+        self.AssetLocation = params.get("AssetLocation")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Filter(AbstractModel):
     """描述键值对过滤器，用于条件过滤查询。例如过滤ID、名称、状态等
 
     若存在多个Filter时，Filter间的关系为逻辑与（AND）关系。
     若同一个Filter存在多个Values，同一Filter下Values间的关系为逻辑或（OR）关系。
 
     """
@@ -3610,14 +3797,57 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class QueryFilterV3(AbstractModel):
+    """过滤
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filter: 过滤条件
+        :type Filter: :class:`tencentcloud.ssa.v20180608.models.QueryFilter`
+        :param HasSub: 有无子条件
+        :type HasSub: bool
+        :param SubFilters: 查询条件
+        :type SubFilters: list of QueryFilter
+        :param Logic: 逻辑操作(只支持32位)
+        :type Logic: int
+        """
+        self.Filter = None
+        self.HasSub = None
+        self.SubFilters = None
+        self.Logic = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filter") is not None:
+            self.Filter = QueryFilter()
+            self.Filter._deserialize(params.get("Filter"))
+        self.HasSub = params.get("HasSub")
+        if params.get("SubFilters") is not None:
+            self.SubFilters = []
+            for item in params.get("SubFilters"):
+                obj = QueryFilter()
+                obj._deserialize(item)
+                self.SubFilters.append(obj)
+        self.Logic = params.get("Logic")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class QuerySort(AbstractModel):
     """排序的字段
 
     """
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/tencentcloud/ssa/v20180608/ssa_client.py` & `tencentcloud-sdk-python-ssa-3.0.913/tencentcloud/ssa/v20180608/ssa_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDomainList(self, request):
+        """域名列表信息啊
+
+        :param request: Request instance for DescribeDomainList.
+        :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeDomainListRequest`
+        :rtype: :class:`tencentcloud.ssa.v20180608.models.DescribeDomainListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDomainList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDomainListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeEventDetail(self, request):
         """获取安全事件详情
 
         :param request: Request instance for DescribeEventDetail.
         :type request: :class:`tencentcloud.ssa.v20180608.models.DescribeEventDetailRequest`
         :rtype: :class:`tencentcloud.ssa.v20180608.models.DescribeEventDetailResponse`
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.913/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/setup.py` & `tencentcloud-sdk-python-ssa-3.0.913/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssa-3.0.912/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssa-3.0.913/tencentcloud_sdk_python_ssa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssa
-Version: 3.0.912
+Version: 3.0.913
 Summary: Tencent Cloud Ssa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

