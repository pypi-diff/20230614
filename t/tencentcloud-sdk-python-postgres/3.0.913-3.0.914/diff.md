# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.913.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.913.tar", last modified: Tue Jun 13 02:22:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.914.tar", last modified: Wed Jun 14 00:31:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.913.tar` & `tencentcloud-sdk-python-postgres-3.0.914.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    85412 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   277706 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 02:22:39.000000 tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    85728 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277922 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 00:31:44.000000 tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/README.rst` & `tencentcloud-sdk-python-postgres-3.0.914/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CloseDBExtranetAccess(self, request):
-        """本接口（CloseDBExtranetAccess）用于关闭实例外网链接。
+        """本接口（CloseDBExtranetAccess）用于关闭实例公网地址。
 
         :param request: Request instance for CloseDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CloseDBExtranetAccessRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.CloseDBExtranetAccessResponse`
 
         """
         try:
@@ -92,15 +92,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CloseServerlessDBExtranetAccess(self, request):
-        """关闭serverlessDB实例外网
+        """本接口（CloseServerlessDBExtranetAccess）用于关闭serverlessDB实例公网地址
 
         :param request: Request instance for CloseServerlessDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.CloseServerlessDBExtranetAccessRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.CloseServerlessDBExtranetAccessResponse`
 
         """
         try:
@@ -483,15 +483,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAccounts(self, request):
-        """本接口（DescribeAccounts）用于获取实例用户列表。
+        """本接口（DescribeAccounts）用于查询实例的数据库账号列表。
 
         :param request: Request instance for DescribeAccounts.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeAccountsRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeAccountsResponse`
 
         """
         try:
@@ -552,15 +552,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBackupDownloadURL(self, request):
-        """本接口 (DescribeBackupDownloadURL) 用于获取备份下载链接。
+        """本接口 (DescribeBackupDownloadURL) 用于查询指定备份集的下载地址，可包括全量备份集、增量日志备份集。
 
         :param request: Request instance for DescribeBackupDownloadURL.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadURLRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadURLResponse`
 
         """
         try:
@@ -805,15 +805,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDBInstanceSecurityGroups(self, request):
-        """本接口（DescribeDBInstanceSecurityGroups）用于查询实例安全组信息。
+        """本接口（DescribeDBInstanceSecurityGroups）用于查询实例安全组。
 
         :param request: Request instance for DescribeDBInstanceSecurityGroups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceSecurityGroupsRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeDBInstanceSecurityGroupsResponse`
 
         """
         try:
@@ -874,15 +874,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDBVersions(self, request):
-        """本接口（DescribeDBVersions）用于查询支持的数据库版本号列表。
+        """本接口（DescribeDBVersions）用于查询支持的数据库版本。
 
         :param request: Request instance for DescribeDBVersions.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDBVersionsRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeDBVersionsResponse`
 
         """
         try:
@@ -920,15 +920,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDatabases(self, request):
-        """接口（DescribeDatabases）用来拉取数据库列表
+        """接口（DescribeDatabases）用来查询实例的数据库列表。
 
         :param request: Request instance for DescribeDatabases.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeDatabasesRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeDatabasesResponse`
 
         """
         try:
@@ -966,15 +966,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeEncryptionKeys(self, request):
-        """获取实例的密钥信息列表。
+        """本接口 （DescribeEncryptionKeys） 用于查询实例的密钥信息列表。
 
         :param request: Request instance for DescribeEncryptionKeys.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeEncryptionKeysRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeEncryptionKeysResponse`
 
         """
         try:
@@ -1081,15 +1081,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeParamsEvent(self, request):
-        """本接口 (DescribeParamsEvent) 用于查询参数修改事件详情。
+        """本接口（DescribeParamsEvent）用于查询参数修改事件。
 
         :param request: Request instance for DescribeParamsEvent.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeParamsEventRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeParamsEventResponse`
 
         """
         try:
@@ -1127,15 +1127,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeReadOnlyGroups(self, request):
-        """本接口(DescribeReadOnlyGroups)用于查询用户输入指定实例的只读组
+        """本接口（DescribeReadOnlyGroups）用于查询只读组列表
 
         :param request: Request instance for DescribeReadOnlyGroups.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeReadOnlyGroupsRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeReadOnlyGroupsResponse`
 
         """
         try:
@@ -1265,15 +1265,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DestroyDBInstance(self, request):
-        """本接口 (DestroyDBInstance) 用于彻底销毁指定DBInstanceId对应的实例，销毁后实例数据将彻底删除，无法找回，只能销毁隔离中的实例。
+        """本接口 (DestroyDBInstance) 用于彻底销毁指定DBInstanceId对应的实例，销毁后实例数据将彻底删除，无法找回，调用前请仔细确认要操作的实例。只能销毁隔离中的实例。
 
         :param request: Request instance for DestroyDBInstance.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DestroyDBInstanceRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DestroyDBInstanceResponse`
 
         """
         try:
@@ -1334,15 +1334,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def InquiryPriceCreateDBInstances(self, request):
-        """本接口 (InquiryPriceCreateDBInstances) 用于查询购买一个或多个实例的价格信息。
+        """本接口 (InquiryPriceCreateDBInstances) 用于查询购买实例的价格信息。
 
         :param request: Request instance for InquiryPriceCreateDBInstances.
         :type request: :class:`tencentcloud.postgres.v20170312.models.InquiryPriceCreateDBInstancesRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.InquiryPriceCreateDBInstancesResponse`
 
         """
         try:
@@ -1587,15 +1587,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDBInstanceParameters(self, request):
-        """批量修改参数
+        """本接口 (ModifyDBInstanceParameters) 用于修改实例参数。
 
         :param request: Request instance for ModifyDBInstanceParameters.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceParametersRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceParametersResponse`
 
         """
         try:
@@ -1656,15 +1656,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDBInstanceSpec(self, request):
-        """本接口（ModifyDBInstanceSpec）用于调整实例规格，包括内存、磁盘。
+        """本接口（ModifyDBInstanceSpec）用于修改实例规格，包括内存、磁盘。
 
         :param request: Request instance for ModifyDBInstanceSpec.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceSpecRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceSpecResponse`
 
         """
         try:
@@ -1679,15 +1679,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDBInstancesProject(self, request):
-        """本接口（ModifyDBInstancesProject）用于将实例转至其他项目。
+        """本接口（ModifyDBInstancesProject）用于修改实例所属项目。
 
         :param request: Request instance for ModifyDBInstancesProject.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstancesProjectRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstancesProjectResponse`
 
         """
         try:
@@ -1702,15 +1702,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyParameterTemplate(self, request):
-        """本接口（ModifyParameterTemplate）主要用于修改参数模板名称，描述，修改，添加和删除参数模板参数。
+        """本接口（ModifyParameterTemplate）主要用于修改参数模板名称，描述等配置，也可用于管理参数模板中的参数列表。
 
         :param request: Request instance for ModifyParameterTemplate.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyParameterTemplateRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyParameterTemplateResponse`
 
         """
         try:
@@ -1771,15 +1771,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def OpenDBExtranetAccess(self, request):
-        """本接口（OpenDBExtranetAccess）用于开通外网。
+        """本接口（OpenDBExtranetAccess）用于开通实例公网地址。
 
         :param request: Request instance for OpenDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.OpenDBExtranetAccessRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.OpenDBExtranetAccessResponse`
 
         """
         try:
@@ -1794,15 +1794,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def OpenServerlessDBExtranetAccess(self, request):
-        """开通serverlessDB实例外网
+        """本接口（OpenServerlessDBExtranetAccess）用于开通serverlessDB实例公网地址。
 
         :param request: Request instance for OpenServerlessDBExtranetAccess.
         :type request: :class:`tencentcloud.postgres.v20170312.models.OpenServerlessDBExtranetAccessRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.OpenServerlessDBExtranetAccessResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/postgres/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,14 +961,16 @@
 1、mssql_compatible引擎：
 migrationMode：数据库模式，可选参数，可取值：single-db（单数据库模式），multi-db（多数据库模式）。默认为single-db。
 defaultLocale：排序区域规则，可选参数，在初始化后不可修改，默认为en_US，可选值如下：
 "af_ZA", "sq_AL", "ar_DZ", "ar_BH", "ar_EG", "ar_IQ", "ar_JO", "ar_KW", "ar_LB", "ar_LY", "ar_MA", "ar_OM", "ar_QA", "ar_SA", "ar_SY", "ar_TN", "ar_AE", "ar_YE", "hy_AM", "az_Cyrl_AZ", "az_Latn_AZ", "eu_ES", "be_BY", "bg_BG", "ca_ES", "zh_HK", "zh_MO", "zh_CN", "zh_SG", "zh_TW", "hr_HR", "cs_CZ", "da_DK", "nl_BE", "nl_NL", "en_AU", "en_BZ", "en_CA", "en_IE", "en_JM", "en_NZ", "en_PH", "en_ZA", "en_TT", "en_GB", "en_US", "en_ZW", "et_EE", "fo_FO", "fa_IR", "fi_FI", "fr_BE", "fr_CA", "fr_FR", "fr_LU", "fr_MC", "fr_CH", "mk_MK", "ka_GE", "de_AT", "de_DE", "de_LI", "de_LU", "de_CH", "el_GR", "gu_IN", "he_IL", "hi_IN", "hu_HU", "is_IS", "id_ID", "it_IT", "it_CH", "ja_JP", "kn_IN", "kok_IN", "ko_KR", "ky_KG", "lv_LV", "lt_LT", "ms_BN", "ms_MY", "mr_IN", "mn_MN", "nb_NO", "nn_NO", "pl_PL", "pt_BR", "pt_PT", "pa_IN", "ro_RO", "ru_RU", "sa_IN", "sr_Cyrl_RS", "sr_Latn_RS", "sk_SK", "sl_SI", "es_AR", "es_BO", "es_CL", "es_CO", "es_CR", "es_DO", "es_EC", "es_SV", "es_GT", "es_HN", "es_MX", "es_NI", "es_PA", "es_PY","es_PE", "es_PR", "es_ES", "es_TRADITIONAL", "es_UY", "es_VE", "sw_KE", "sv_FI", "sv_SE", "tt_RU", "te_IN", "th_TH", "tr_TR", "uk_UA", "ur_IN", "ur_PK", "uz_Cyrl_UZ", "uz_Latn_UZ", "vi_VN"。
 serverCollationName：排序规则名称，可选参数，在初始化后不可修改，默认为sql_latin1_general_cp1_ci_as，可选值如下：
 "bbf_unicode_general_ci_as", "bbf_unicode_cp1_ci_as", "bbf_unicode_CP1250_ci_as", "bbf_unicode_CP1251_ci_as", "bbf_unicode_cp1253_ci_as", "bbf_unicode_cp1254_ci_as", "bbf_unicode_cp1255_ci_as", "bbf_unicode_cp1256_ci_as", "bbf_unicode_cp1257_ci_as", "bbf_unicode_cp1258_ci_as", "bbf_unicode_cp874_ci_as", "sql_latin1_general_cp1250_ci_as", "sql_latin1_general_cp1251_ci_as", "sql_latin1_general_cp1_ci_as", "sql_latin1_general_cp1253_ci_as", "sql_latin1_general_cp1254_ci_as", "sql_latin1_general_cp1255_ci_as","sql_latin1_general_cp1256_ci_as", "sql_latin1_general_cp1257_ci_as", "sql_latin1_general_cp1258_ci_as", "chinese_prc_ci_as", "cyrillic_general_ci_as", "finnish_swedish_ci_as", "french_ci_as", "japanese_ci_as", "korean_wansung_ci_as", "latin1_general_ci_as", "modern_spanish_ci_as", "polish_ci_as", "thai_ci_as", "traditional_spanish_ci_as", "turkish_ci_as", "ukrainian_ci_as", "vietnamese_ci_as"。
         :type DBEngineConfig: str
+        :param SyncMode: 主从同步方式，取值： 1)Semi-sync：半同步 2)Async：异步 默认为Async
+        :type SyncMode: str
         """
         self.SpecCode = None
         self.Storage = None
         self.InstanceCount = None
         self.Period = None
         self.Zone = None
         self.Charset = None
@@ -991,14 +993,15 @@
         self.DBKernelVersion = None
         self.DBNodeSet = None
         self.NeedSupportTDE = None
         self.KMSKeyId = None
         self.KMSRegion = None
         self.DBEngine = None
         self.DBEngineConfig = None
+        self.SyncMode = None
 
 
     def _deserialize(self, params):
         self.SpecCode = params.get("SpecCode")
         self.Storage = params.get("Storage")
         self.InstanceCount = params.get("InstanceCount")
         self.Period = params.get("Period")
@@ -1033,14 +1036,15 @@
                 obj._deserialize(item)
                 self.DBNodeSet.append(obj)
         self.NeedSupportTDE = params.get("NeedSupportTDE")
         self.KMSKeyId = params.get("KMSKeyId")
         self.KMSRegion = params.get("KMSRegion")
         self.DBEngine = params.get("DBEngine")
         self.DBEngineConfig = params.get("DBEngineConfig")
+        self.SyncMode = params.get("SyncMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.914/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/setup.py` & `tencentcloud-sdk-python-postgres-3.0.914/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.913/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.914/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.913
+Version: 3.0.914
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

