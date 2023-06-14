# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.913.tar", last modified: Tue Jun 13 02:22:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.914.tar", last modified: Wed Jun 14 00:31:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.913.tar` & `tencentcloud-sdk-python-partners-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)      885 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84247 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)    23877 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:22:24.000000 tencentcloud-sdk-python-partners-3.0.913/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)      885 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65298 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)    19334 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:33.000000 tencentcloud-sdk-python-partners-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-partners-3.0.913/README.rst` & `tencentcloud-sdk-python-partners-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -243,177 +243,14 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AgentDealElem(AbstractModel):
-    """描述代理商代付的订单信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param DealId: 订单自增 ID【请勿依赖该字段作为唯一标识】
-        :type DealId: str
-        :param DealName: 订单号【订单唯一键】
-        :type DealName: str
-        :param GoodsCategoryId: 商品类型 ID
-        :type GoodsCategoryId: str
-        :param OwnerUin: 订单所有者
-        :type OwnerUin: str
-        :param AppId: 订单所有者对应 appId
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AppId: str
-        :param GoodsNum: 商品数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GoodsNum: str
-        :param GoodsPrice: 价格详情
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GoodsPrice: :class:`tencentcloud.partners.v20180321.models.DealGoodsPriceElem`
-        :param Creater: 下单人
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Creater: str
-        :param CreatTime: 下单时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type CreatTime: str
-        :param PayEndTime: 支付结束时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PayEndTime: str
-        :param BillId: 扣费流水号
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BillId: str
-        :param Payer: 支付人
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Payer: str
-        :param DealStatus: 订单状态，中文描述
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DealStatus: str
-        :param Status: 订单的状态(1：未支付;2：已支付;3：发货中;4：已发货;5：发货失败;6：已退款;7：已关单;8：订单过期;9：订单已失效;10：产品已失效;11：代付拒绝;12：支付中)
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Status: str
-        :param GoodsName: 产品名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GoodsName: str
-        :param ClientRemark: 客户备注
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ClientRemark: str
-        :param ActionType: 订单操作类型，purchase（新购），renew（续费），modify（配置变更）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ActionType: str
-        :param VoucherDecline: 代金券抵扣金额，单位分
-注意：此字段可能返回 null，表示取不到有效值。
-        :type VoucherDecline: str
-        :param BigDealId: 大订单号
-注意：此字段可能返回 null，表示取不到有效值。
-        :type BigDealId: str
-        :param ClientType: 客户类型（new：自拓；old：官网；assign：指派；direct：直销；direct_newopp：直销(新商机)）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ClientType: str
-        :param ProjectType: 项目类型（self：自拓；repeat：直销；platform：官网合作）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProjectType: str
-        :param SalesUin: 业务员账号ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type SalesUin: str
-        :param PayerMode: 支付方式，0：自付；1：代付
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PayerMode: str
-        :param ActivityId: 活动ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ActivityId: str
-        :param OverdueTime: 订单过期时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type OverdueTime: str
-        :param ProductInfo: 产品详情
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ProductInfo: list of ProductInfoElem
-        :param PaymentMethod: 付款方式
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PaymentMethod: str
-        :param UpdateTime: 订单更新时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type UpdateTime: str
-        """
-        self.DealId = None
-        self.DealName = None
-        self.GoodsCategoryId = None
-        self.OwnerUin = None
-        self.AppId = None
-        self.GoodsNum = None
-        self.GoodsPrice = None
-        self.Creater = None
-        self.CreatTime = None
-        self.PayEndTime = None
-        self.BillId = None
-        self.Payer = None
-        self.DealStatus = None
-        self.Status = None
-        self.GoodsName = None
-        self.ClientRemark = None
-        self.ActionType = None
-        self.VoucherDecline = None
-        self.BigDealId = None
-        self.ClientType = None
-        self.ProjectType = None
-        self.SalesUin = None
-        self.PayerMode = None
-        self.ActivityId = None
-        self.OverdueTime = None
-        self.ProductInfo = None
-        self.PaymentMethod = None
-        self.UpdateTime = None
-
-
-    def _deserialize(self, params):
-        self.DealId = params.get("DealId")
-        self.DealName = params.get("DealName")
-        self.GoodsCategoryId = params.get("GoodsCategoryId")
-        self.OwnerUin = params.get("OwnerUin")
-        self.AppId = params.get("AppId")
-        self.GoodsNum = params.get("GoodsNum")
-        if params.get("GoodsPrice") is not None:
-            self.GoodsPrice = DealGoodsPriceElem()
-            self.GoodsPrice._deserialize(params.get("GoodsPrice"))
-        self.Creater = params.get("Creater")
-        self.CreatTime = params.get("CreatTime")
-        self.PayEndTime = params.get("PayEndTime")
-        self.BillId = params.get("BillId")
-        self.Payer = params.get("Payer")
-        self.DealStatus = params.get("DealStatus")
-        self.Status = params.get("Status")
-        self.GoodsName = params.get("GoodsName")
-        self.ClientRemark = params.get("ClientRemark")
-        self.ActionType = params.get("ActionType")
-        self.VoucherDecline = params.get("VoucherDecline")
-        self.BigDealId = params.get("BigDealId")
-        self.ClientType = params.get("ClientType")
-        self.ProjectType = params.get("ProjectType")
-        self.SalesUin = params.get("SalesUin")
-        self.PayerMode = params.get("PayerMode")
-        self.ActivityId = params.get("ActivityId")
-        self.OverdueTime = params.get("OverdueTime")
-        if params.get("ProductInfo") is not None:
-            self.ProductInfo = []
-            for item in params.get("ProductInfo"):
-                obj = ProductInfoElem()
-                obj._deserialize(item)
-                self.ProductInfo.append(obj)
-        self.PaymentMethod = params.get("PaymentMethod")
-        self.UpdateTime = params.get("UpdateTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class AgentDealNewElem(AbstractModel):
     """描述代理商代付的订单信息
 
     """
 
     def __init__(self):
         r"""
@@ -869,42 +706,14 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
-class DealGoodsPriceElem(AbstractModel):
-    """订单价格详情
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RealTotalCost: 实付金额（单位：分）
-        :type RealTotalCost: int
-        :param OriginalTotalCost: 订单实际金额（不含折扣，单位：分）
-        :type OriginalTotalCost: int
-        """
-        self.RealTotalCost = None
-        self.OriginalTotalCost = None
-
-
-    def _deserialize(self, params):
-        self.RealTotalCost = params.get("RealTotalCost")
-        self.OriginalTotalCost = params.get("OriginalTotalCost")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class DealGoodsPriceNewElem(AbstractModel):
     """订单价格详情
 
     """
 
     def __init__(self):
         r"""
@@ -1334,182 +1143,14 @@
                 obj = AgentDealNewElem()
                 obj._deserialize(item)
                 self.AgentDealSet.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
-class DescribeAgentDealsCacheRequest(AbstractModel):
-    """DescribeAgentDealsCache请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Offset: 偏移量
-        :type Offset: int
-        :param Limit: 限制数目 最大200
-        :type Limit: int
-        :param CreatTimeRangeStart: 下单时间范围起始点【请保持时间范围最大90天】
-        :type CreatTimeRangeStart: str
-        :param CreatTimeRangeEnd: 下单时间范围终止点【请保持时间范围最大90天】
-        :type CreatTimeRangeEnd: str
-        :param Order: 0:下单时间降序；其他：下单时间升序
-        :type Order: int
-        :param Status: 订单的状态(1：未支付;2：已支付;3：发货中;4：已发货;5：发货失败;6：已退款;7：已关单;8：订单过期;9：订单已失效;10：产品已失效;11：代付拒绝;12：支付中)
-        :type Status: int
-        :param OwnerUins: 下单人账号ID列表
-        :type OwnerUins: list of str
-        :param DealNames: 订单号列表
-        :type DealNames: list of str
-        :param PayerMode: 支付方式，0：自付；1：代付
-        :type PayerMode: int
-        """
-        self.Offset = None
-        self.Limit = None
-        self.CreatTimeRangeStart = None
-        self.CreatTimeRangeEnd = None
-        self.Order = None
-        self.Status = None
-        self.OwnerUins = None
-        self.DealNames = None
-        self.PayerMode = None
-
-
-    def _deserialize(self, params):
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
-        self.CreatTimeRangeStart = params.get("CreatTimeRangeStart")
-        self.CreatTimeRangeEnd = params.get("CreatTimeRangeEnd")
-        self.Order = params.get("Order")
-        self.Status = params.get("Status")
-        self.OwnerUins = params.get("OwnerUins")
-        self.DealNames = params.get("DealNames")
-        self.PayerMode = params.get("PayerMode")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeAgentDealsCacheResponse(AbstractModel):
-    """DescribeAgentDealsCache返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param AgentDealSet: 订单数组
-        :type AgentDealSet: list of AgentDealElem
-        :param TotalCount: 符合条件的订单总数量
-        :type TotalCount: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.AgentDealSet = None
-        self.TotalCount = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("AgentDealSet") is not None:
-            self.AgentDealSet = []
-            for item in params.get("AgentDealSet"):
-                obj = AgentDealElem()
-                obj._deserialize(item)
-                self.AgentDealSet.append(obj)
-        self.TotalCount = params.get("TotalCount")
-        self.RequestId = params.get("RequestId")
-
-
-class DescribeAgentPayDealsRequest(AbstractModel):
-    """DescribeAgentPayDeals请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Offset: 偏移量
-        :type Offset: int
-        :param Limit: 限制数目 最大100
-        :type Limit: int
-        :param CreatTimeRangeStart: 下单时间范围起始点(不传时会默认查15天内订单，传值时需要传15天内的起始时间)
-        :type CreatTimeRangeStart: str
-        :param CreatTimeRangeEnd: 下单时间范围终止点
-        :type CreatTimeRangeEnd: str
-        :param Order: 0:下单时间降序；其他：下单时间升序
-        :type Order: int
-        :param Status: 订单的状态(1：未支付;2：已支付;3：发货中;4：已发货;5：发货失败;6：已退款;7：已关单;8：订单过期;9：订单已失效;10：产品已失效;11：代付拒绝;12：支付中)
-        :type Status: int
-        :param OwnerUins: 下单人账号ID列表
-        :type OwnerUins: list of str
-        :param DealNames: 订单号列表
-        :type DealNames: list of str
-        """
-        self.Offset = None
-        self.Limit = None
-        self.CreatTimeRangeStart = None
-        self.CreatTimeRangeEnd = None
-        self.Order = None
-        self.Status = None
-        self.OwnerUins = None
-        self.DealNames = None
-
-
-    def _deserialize(self, params):
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
-        self.CreatTimeRangeStart = params.get("CreatTimeRangeStart")
-        self.CreatTimeRangeEnd = params.get("CreatTimeRangeEnd")
-        self.Order = params.get("Order")
-        self.Status = params.get("Status")
-        self.OwnerUins = params.get("OwnerUins")
-        self.DealNames = params.get("DealNames")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeAgentPayDealsResponse(AbstractModel):
-    """DescribeAgentPayDeals返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param AgentPayDealSet: 订单数组
-        :type AgentPayDealSet: list of AgentDealElem
-        :param TotalCount: 符合条件的订单总数量
-        :type TotalCount: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.AgentPayDealSet = None
-        self.TotalCount = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("AgentPayDealSet") is not None:
-            self.AgentPayDealSet = []
-            for item in params.get("AgentPayDealSet"):
-                obj = AgentDealElem()
-                obj._deserialize(item)
-                self.AgentPayDealSet.append(obj)
-        self.TotalCount = params.get("TotalCount")
-        self.RequestId = params.get("RequestId")
-
-
 class DescribeAgentPayDealsV2Request(AbstractModel):
     """DescribeAgentPayDealsV2请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1588,96 +1229,14 @@
                 obj = AgentDealNewElem()
                 obj._deserialize(item)
                 self.AgentPayDealSet.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
-class DescribeAgentSelfPayDealsRequest(AbstractModel):
-    """DescribeAgentSelfPayDeals请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param OwnerUin: 下单人账号ID
-        :type OwnerUin: str
-        :param Offset: 偏移量
-        :type Offset: int
-        :param Limit: 限制数目 最大100
-        :type Limit: int
-        :param CreatTimeRangeStart: 下单时间范围起始点(不传时会默认查15天内订单，传值时需要传15天内的起始时间)
-        :type CreatTimeRangeStart: str
-        :param CreatTimeRangeEnd: 下单时间范围终止点
-        :type CreatTimeRangeEnd: str
-        :param Order: 0:下单时间降序；其他：下单时间升序
-        :type Order: int
-        :param Status: 订单的状态(1：未支付;2：已支付;3：发货中;4：已发货;5：发货失败;6：已退款;7：已关单;8：订单过期;9：订单已失效;10：产品已失效;11：代付拒绝;12：支付中)
-        :type Status: int
-        :param DealNames: 订单号列表
-        :type DealNames: list of str
-        """
-        self.OwnerUin = None
-        self.Offset = None
-        self.Limit = None
-        self.CreatTimeRangeStart = None
-        self.CreatTimeRangeEnd = None
-        self.Order = None
-        self.Status = None
-        self.DealNames = None
-
-
-    def _deserialize(self, params):
-        self.OwnerUin = params.get("OwnerUin")
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
-        self.CreatTimeRangeStart = params.get("CreatTimeRangeStart")
-        self.CreatTimeRangeEnd = params.get("CreatTimeRangeEnd")
-        self.Order = params.get("Order")
-        self.Status = params.get("Status")
-        self.DealNames = params.get("DealNames")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeAgentSelfPayDealsResponse(AbstractModel):
-    """DescribeAgentSelfPayDeals返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param AgentPayDealSet: 订单数组
-        :type AgentPayDealSet: list of AgentDealElem
-        :param TotalCount: 符合条件的订单总数量
-        :type TotalCount: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.AgentPayDealSet = None
-        self.TotalCount = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("AgentPayDealSet") is not None:
-            self.AgentPayDealSet = []
-            for item in params.get("AgentPayDealSet"):
-                obj = AgentDealElem()
-                obj._deserialize(item)
-                self.AgentPayDealSet.append(obj)
-        self.TotalCount = params.get("TotalCount")
-        self.RequestId = params.get("RequestId")
-
-
 class DescribeAgentSelfPayDealsV2Request(AbstractModel):
     """DescribeAgentSelfPayDealsV2请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1795,63 +1354,14 @@
         :type Balance: int
         :param Cash: 账户现金余额，单位分
         :type Cash: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Balance = None
-        self.Cash = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.Balance = params.get("Balance")
-        self.Cash = params.get("Cash")
-        self.RequestId = params.get("RequestId")
-
-
-class DescribeClientBalanceRequest(AbstractModel):
-    """DescribeClientBalance请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param ClientUin: 客户(代客)账号ID
-        :type ClientUin: str
-        """
-        self.ClientUin = None
-
-
-    def _deserialize(self, params):
-        self.ClientUin = params.get("ClientUin")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeClientBalanceResponse(AbstractModel):
-    """DescribeClientBalance返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Balance: 账户可用余额，单位分 （可用余额 = 现金余额 - 冻结金额）  【注：该数据准确性存疑，请切换至DescribeClientBalanceNew取值】
-        :type Balance: int
-        :param Cash: 账户现金余额，单位分
-        :type Cash: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.Balance = None
         self.Cash = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Balance = params.get("Balance")
         self.Cash = params.get("Cash")
```

### Comparing `tencentcloud-sdk-python-partners-3.0.913/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.914/tencentcloud/partners/v20180321/partners_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -255,64 +255,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeAgentDealsCache(self, request):
-        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
-
-        【该接口已下线，请使用升级版本DescribeAgentDealsByCache】代理商拉取缓存的全量客户订单
-
-        :param request: Request instance for DescribeAgentDealsCache.
-        :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentDealsCacheRequest`
-        :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentDealsCacheResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeAgentDealsCache", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeAgentDealsCacheResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeAgentPayDeals(self, request):
-        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
-
-        【该接口已下线，请切换使用升级版本DescribeAgentPayDealsV2】可以查询代理商代付的所有订单
-
-        :param request: Request instance for DescribeAgentPayDeals.
-        :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsRequest`
-        :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeAgentPayDeals", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeAgentPayDealsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeAgentPayDealsV2(self, request):
         """可以查询代理商代付的预付费订单
 
         :param request: Request instance for DescribeAgentPayDealsV2.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsV2Request`
         :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsV2Response`
 
@@ -328,39 +278,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeAgentSelfPayDeals(self, request):
-        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
-
-        【该接口已下线，请切换使用升级版本DescribeAgentSelfPayDealsV2】可以查询代理商下指定客户的自付订单
-
-        :param request: Request instance for DescribeAgentSelfPayDeals.
-        :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsRequest`
-        :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeAgentSelfPayDeals", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeAgentSelfPayDealsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeAgentSelfPayDealsV2(self, request):
         """查询代理商名下指定代客的自付订单（预付费）
 
         :param request: Request instance for DescribeAgentSelfPayDealsV2.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsV2Request`
         :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsV2Response`
 
@@ -374,39 +299,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
-
-
-    def DescribeClientBalance(self, request):
-        """已提供新接口并推进切换，白名单禁用控制访问观察后无反馈，可以下线
-
-        【该接口将逐步下线，请切换使用升级版本DescribeClientBalanceNew】为合作伙伴提供查询客户余额能力。调用者必须是合作伙伴，只能查询自己名下客户余额.
-
-        :param request: Request instance for DescribeClientBalance.
-        :type request: :class:`tencentcloud.partners.v20180321.models.DescribeClientBalanceRequest`
-        :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeClientBalanceResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeClientBalance", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeClientBalanceResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeClientBalanceNew(self, request):
         """为合作伙伴提供查询客户余额能力。调用者必须是合作伙伴，只能查询自己名下客户余额
 
         :param request: Request instance for DescribeClientBalanceNew.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeClientBalanceNewRequest`
```

### Comparing `tencentcloud-sdk-python-partners-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-partners-3.0.913/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.914/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.914/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.913/setup.py` & `tencentcloud-sdk-python-partners-3.0.914/setup.py`

 * *Files identical despite different names*

