# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.912.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.912.tar", last modified: Mon Jun 12 03:08:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.914.tar", last modified: Wed Jun 14 00:31:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.912.tar` & `tencentcloud-sdk-python-ocr-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   114877 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   512681 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:08:50.000000 tencentcloud-sdk-python-ocr-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   115262 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   515918 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:16.000000 tencentcloud-sdk-python-ocr-3.0.914/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.914/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.912
+Version: 3.0.914
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/README.rst` & `tencentcloud-sdk-python-ocr-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1481,15 +1481,15 @@
                 </tr>
                 <tr>
                   <td> VatElectronicSpecialInvoiceFull</td>
                   <td> 电子发票(专用发票)</td>
                   <td> 16 </td>
                 </tr>
                 <tr>
-                  <td> VatElectronicSpecialInvoiceFull</td>
+                  <td> VatElectronicInvoiceFull</td>
                   <td> 电子发票(普通发票) </td>
                   <td> 16 </td>
                 </tr>
                 <tr>
                   <td> MotorVehicleSaleInvoice </td>
                   <td> 机动车销售统一发票 </td>
                   <td> 12 </td>
@@ -1551,14 +1551,24 @@
                 </tr>
                 <tr>
                   <td> TollInvoice </td>
                   <td> 过路过桥费发票 </td>
                   <td> 13 </td>
                 </tr>
                 <tr>
+                  <td> MedicalOutpatientInvoice </td>
+                  <td> 医疗门诊收费票据（电子） </td>
+                  <td> 17 </td>
+                </tr>
+                <tr>
+                  <td> MedicalHospitalizedInvoice </td>
+                  <td> 医疗住院收费票据（电子） </td>
+                  <td> 17 </td>
+                </tr>
+                <tr>
                   <td> OtherInvoice </td>
                   <td> 其他发票 </td>
                   <td> -1 </td>
                 </tr>
               </tbody>
             </table>
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3822,15 +3822,15 @@
     """混贴票据单张发票识别信息
 
     """
 
     def __init__(self):
         r"""
         :param Code: 识别结果。
-OK：表示识别成功；FailedOperation.UnsupportedInvioce：表示不支持识别；
+OK：表示识别成功；FailedOperation.UnsupportedInvoice：表示不支持识别；
 FailedOperation.UnKnowError：表示识别失败；
 其它错误码见各个票据接口的定义。
         :type Code: str
         :param Type: 识别出的图片所属的票据类型。
 -1：未知类型
 0：出租车发票
 1：定额发票
@@ -3841,30 +3841,31 @@
 9：汽车票
 10：轮船票
 11：增值税发票（卷票）
 12：购车发票
 13：过路过桥费发票
 15：非税发票
 16：全电发票
+17：医疗发票
         :type Type: int
         :param Polygon: 旋转后的图片四点坐标。
         :type Polygon: :class:`tencentcloud.ocr.v20181119.models.Polygon`
         :param Angle: 识别出的图片在混贴票据图片中的旋转角度。
         :type Angle: float
         :param SingleInvoiceInfos: 识别到的内容。
         :type SingleInvoiceInfos: :class:`tencentcloud.ocr.v20181119.models.SingleInvoiceItem`
         :param Page: 发票处于识别图片或PDF文件中的页教，默认从1开始。
         :type Page: int
-        :param SubType: 发票详细类型，详见下方 SubType 返回值说明
+        :param SubType: 发票详细类型，详见上方 SubType 返回值说明
         :type SubType: str
-        :param TypeDescription: 发票类型描述，详见下方 TypeDescription  返回值说明
+        :param TypeDescription: 发票类型描述，详见上方 TypeDescription  返回值说明
         :type TypeDescription: str
         :param CutImage: 切割单图文件，Base64编码后的切图后的图片文件，开启 EnableCutImage 后进行返回
         :type CutImage: str
-        :param SubTypeDescription: 发票详细类型描述，详见下方 SubType 返回值说明
+        :param SubTypeDescription: 发票详细类型描述，详见上方 SubType 返回值说明
         :type SubTypeDescription: str
         """
         self.Code = None
         self.Type = None
         self.Polygon = None
         self.Angle = None
         self.SingleInvoiceInfos = None
@@ -4631,14 +4632,70 @@
         self.IssueAddress = params.get("IssueAddress")
         self.IssueNumber = params.get("IssueNumber")
         self.Type = params.get("Type")
         self.Profile = params.get("Profile")
         self.RequestId = params.get("RequestId")
 
 
+class MedicalInvoice(AbstractModel):
+    """医疗票据信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Title: 发票名称
+        :type Title: str
+        :param Code: 发票代码
+        :type Code: str
+        :param Number: 发票号码
+        :type Number: str
+        :param Total: 价税合计（小写）
+        :type Total: str
+        :param TotalCn: 价税合计（大写）
+        :type TotalCn: str
+        :param Date: 开票日期
+        :type Date: str
+        :param CheckCode: 校验码
+        :type CheckCode: str
+        :param Place: 发票属地
+        :type Place: str
+        :param Reviewer: 复核人
+        :type Reviewer: str
+        """
+        self.Title = None
+        self.Code = None
+        self.Number = None
+        self.Total = None
+        self.TotalCn = None
+        self.Date = None
+        self.CheckCode = None
+        self.Place = None
+        self.Reviewer = None
+
+
+    def _deserialize(self, params):
+        self.Title = params.get("Title")
+        self.Code = params.get("Code")
+        self.Number = params.get("Number")
+        self.Total = params.get("Total")
+        self.TotalCn = params.get("TotalCn")
+        self.Date = params.get("Date")
+        self.CheckCode = params.get("CheckCode")
+        self.Place = params.get("Place")
+        self.Reviewer = params.get("Reviewer")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class MedicalInvoiceInfo(AbstractModel):
     """医疗发票识别结果
 
     """
 
     def __init__(self):
         r"""
@@ -6531,43 +6588,41 @@
     """
 
     def __init__(self):
         r"""
         :param ImageBase64: 图片的 Base64 值。
 支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
-支持的图片像素：需介于20-10000px之间。
+支持的图片像素：单边介于20-10000px之间。
 图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
         :type ImageBase64: str
         :param ImageUrl: 图片的 Url 地址。
 支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
-支持的图片像素：需介于20-10000px之间。
+支持的图片像素：单边介于20-10000px之间。
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
-        :param Types: 需要识别的票据类型列表，为空或不填表示识别全部类型。
+        :param Types: 需要识别的票据类型列表，为空或不填表示识别全部类型。当传入单个类型时，图片均采用该票类型进行处理。
+暂不支持多个参数进行局部控制。
 0：出租车发票
 1：定额发票
 2：火车票
 3：增值税发票
 5：机票行程单
 8：通用机打发票
 9：汽车票
 10：轮船票
 11：增值税发票（卷票 ）
 12：购车发票
 13：过路过桥费发票
 15：非税发票
 16：全电发票
+17：医疗发票
 -1：其他发票
-
-默认为空，识别所有类型发票。
-当传入单个类型时，图片均采用该票类型进行处理。
-暂不支持多个参数进行局部控制。
         :type Types: list of int
         :param EnableOther: 是否开启其他票识别，默认值为true，开启后可支持其他发票的智能识别。	
         :type EnableOther: bool
         :param EnablePdf: 是否开启PDF识别，默认值为true，开启后可同时支持图片和PDF的识别。
         :type EnablePdf: bool
         :param PdfPageNumber: 需要识别的PDF页面的对应页码，传入时仅支持PDF单页识别，当上传文件为PDF且EnablePdf参数值为true时有效，默认值为1。
         :type PdfPageNumber: int
@@ -7733,17 +7788,17 @@
         :type ThaiName: str
         :param EnFirstName: 英文姓名
         :type EnFirstName: str
         :param Address: 地址
         :type Address: str
         :param Birthday: 出生日期
         :type Birthday: str
-        :param IssueDate: 首次领用日期
+        :param IssueDate: 签发日期
         :type IssueDate: str
-        :param ExpirationDate: 签发日期
+        :param ExpirationDate: 到期日期
         :type ExpirationDate: str
         :param EnLastName: 英文姓名
         :type EnLastName: str
         :param PortraitImage: 证件人像照片抠取
         :type PortraitImage: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -8590,14 +8645,20 @@
         :type NonTaxIncomeGeneralBill: :class:`tencentcloud.ocr.v20181119.models.NonTaxIncomeBill`
         :param NonTaxIncomeElectronicBill: 非税收入一般缴款书(电子)
 注意：此字段可能返回 null，表示取不到有效值。
         :type NonTaxIncomeElectronicBill: :class:`tencentcloud.ocr.v20181119.models.NonTaxIncomeBill`
         :param TrainTicket: 火车票
 注意：此字段可能返回 null，表示取不到有效值。
         :type TrainTicket: :class:`tencentcloud.ocr.v20181119.models.TrainTicket`
+        :param MedicalOutpatientInvoice: 医疗门诊收费票据（电子）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MedicalOutpatientInvoice: :class:`tencentcloud.ocr.v20181119.models.MedicalInvoice`
+        :param MedicalHospitalizedInvoice: 医疗住院收费票据（电子）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MedicalHospitalizedInvoice: :class:`tencentcloud.ocr.v20181119.models.MedicalInvoice`
         """
         self.VatSpecialInvoice = None
         self.VatCommonInvoice = None
         self.VatElectronicCommonInvoice = None
         self.VatElectronicSpecialInvoice = None
         self.VatElectronicInvoiceBlockchain = None
         self.VatElectronicInvoiceToll = None
@@ -8613,14 +8674,16 @@
         self.VatInvoiceRoll = None
         self.TaxiTicket = None
         self.QuotaInvoice = None
         self.AirTransport = None
         self.NonTaxIncomeGeneralBill = None
         self.NonTaxIncomeElectronicBill = None
         self.TrainTicket = None
+        self.MedicalOutpatientInvoice = None
+        self.MedicalHospitalizedInvoice = None
 
 
     def _deserialize(self, params):
         if params.get("VatSpecialInvoice") is not None:
             self.VatSpecialInvoice = VatInvoiceInfo()
             self.VatSpecialInvoice._deserialize(params.get("VatSpecialInvoice"))
         if params.get("VatCommonInvoice") is not None:
@@ -8682,14 +8745,20 @@
             self.NonTaxIncomeGeneralBill._deserialize(params.get("NonTaxIncomeGeneralBill"))
         if params.get("NonTaxIncomeElectronicBill") is not None:
             self.NonTaxIncomeElectronicBill = NonTaxIncomeBill()
             self.NonTaxIncomeElectronicBill._deserialize(params.get("NonTaxIncomeElectronicBill"))
         if params.get("TrainTicket") is not None:
             self.TrainTicket = TrainTicket()
             self.TrainTicket._deserialize(params.get("TrainTicket"))
+        if params.get("MedicalOutpatientInvoice") is not None:
+            self.MedicalOutpatientInvoice = MedicalInvoice()
+            self.MedicalOutpatientInvoice._deserialize(params.get("MedicalOutpatientInvoice"))
+        if params.get("MedicalHospitalizedInvoice") is not None:
+            self.MedicalHospitalizedInvoice = MedicalInvoice()
+            self.MedicalHospitalizedInvoice._deserialize(params.get("MedicalHospitalizedInvoice"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11361,14 +11430,20 @@
         :type Province: str
         :param VatInvoiceItemInfos: 增值税发票项目信息
         :type VatInvoiceItemInfos: list of VatInvoiceItemInfo
         :param CodeConfirm: 机打发票代码
         :type CodeConfirm: str
         :param Receiptor: 收款人
         :type Receiptor: str
+        :param ElectronicFullMark: 是否有全电纸质票（0：没有，1：有）
+        :type ElectronicFullMark: int
+        :param ElectronicFullNumber: 全电号码
+        :type ElectronicFullNumber: str
+        :param FormName: 发票联名
+        :type FormName: str
         """
         self.CheckCode = None
         self.FormType = None
         self.TravelTax = None
         self.BuyerAddrTel = None
         self.BuyerBankAccount = None
         self.CompanySealContent = None
@@ -11401,14 +11476,17 @@
         self.CompanySealMark = None
         self.Issuer = None
         self.Reviewer = None
         self.Province = None
         self.VatInvoiceItemInfos = None
         self.CodeConfirm = None
         self.Receiptor = None
+        self.ElectronicFullMark = None
+        self.ElectronicFullNumber = None
+        self.FormName = None
 
 
     def _deserialize(self, params):
         self.CheckCode = params.get("CheckCode")
         self.FormType = params.get("FormType")
         self.TravelTax = params.get("TravelTax")
         self.BuyerAddrTel = params.get("BuyerAddrTel")
@@ -11448,14 +11526,17 @@
             self.VatInvoiceItemInfos = []
             for item in params.get("VatInvoiceItemInfos"):
                 obj = VatInvoiceItemInfo()
                 obj._deserialize(item)
                 self.VatInvoiceItemInfos.append(obj)
         self.CodeConfirm = params.get("CodeConfirm")
         self.Receiptor = params.get("Receiptor")
+        self.ElectronicFullMark = params.get("ElectronicFullMark")
+        self.ElectronicFullNumber = params.get("ElectronicFullNumber")
+        self.FormName = params.get("FormName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.914/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.912
+Version: 3.0.914
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.912/setup.py` & `tencentcloud-sdk-python-ocr-3.0.914/setup.py`

 * *Files identical despite different names*

