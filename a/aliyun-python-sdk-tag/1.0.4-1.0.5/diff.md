# Comparing `tmp/aliyun-python-sdk-tag-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-tag-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-tag-1.0.4.tar", last modified: Wed Jul  6 06:56:03 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-tag-1.0.5.tar", last modified: Wed Jun 14 02:30:08 2023, max compression
```

## Comparing `aliyun-python-sdk-tag-1.0.4.tar` & `aliyun-python-sdk-tag-1.0.5.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1894 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2921 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/
--rw-r--r--   0 root         (0) root         (0)     2438 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/AttachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2828 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/CreatePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3283 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/CreateTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2068 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DeletePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2193 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DeleteTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DetachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2299 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DisablePolicyTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2297 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/EnablePolicyTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GenerateConfigRuleReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2452 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetConfigRuleReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2271 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetEffectivePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2307 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetPolicyEnableStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListConfigRulesForTargetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2649 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListPoliciesForTargetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2980 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3300 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListResourcesByTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     3063 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListSupportResourceTypesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3210 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3196 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTargetsForPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2828 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ModifyPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2321 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2412 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-07-06 06:56:03.000000 aliyun-python-sdk-tag-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/
+-rw-r--r--   0 root         (0) root         (0)     2438 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/AttachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CheckCreatedByEnabledRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CloseCreatedByRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CreatePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CreateTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DeletePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DeleteTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DetachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DisablePolicyTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/EnablePolicyTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GenerateConfigRuleReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetConfigRuleReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetEffectivePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetPolicyEnableStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListConfigRulesForTargetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListPoliciesForTargetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListResourcesByTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListSupportResourceTypesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTargetsForPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ModifyPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/OpenCreatedByRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-06-14 02:30:08.000000 aliyun-python-sdk-tag-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-tag-1.0.4/LICENSE` & `aliyun-python-sdk-tag-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/PKG-INFO` & `aliyun-python-sdk-tag-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tag
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tag module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tag
```

### Comparing `aliyun-python-sdk-tag-1.0.4/README.rst` & `aliyun-python-sdk-tag-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/PKG-INFO` & `aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tag
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tag module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tag
```

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyun_python_sdk_tag.egg-info/SOURCES.txt` & `aliyun-python-sdk-tag-1.0.5/aliyun_python_sdk_tag.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 aliyun_python_sdk_tag.egg-info/dependency_links.txt
 aliyun_python_sdk_tag.egg-info/requires.txt
 aliyun_python_sdk_tag.egg-info/top_level.txt
 aliyunsdktag/__init__.py
 aliyunsdktag/endpoint.py
 aliyunsdktag/request/__init__.py
 aliyunsdktag/request/v20180828/AttachPolicyRequest.py
+aliyunsdktag/request/v20180828/CheckCreatedByEnabledRequest.py
+aliyunsdktag/request/v20180828/CloseCreatedByRequest.py
 aliyunsdktag/request/v20180828/CreatePolicyRequest.py
 aliyunsdktag/request/v20180828/CreateTagsRequest.py
 aliyunsdktag/request/v20180828/DeletePolicyRequest.py
 aliyunsdktag/request/v20180828/DeleteTagRequest.py
 aliyunsdktag/request/v20180828/DescribeRegionsRequest.py
 aliyunsdktag/request/v20180828/DetachPolicyRequest.py
 aliyunsdktag/request/v20180828/DisablePolicyTypeRequest.py
@@ -31,10 +33,11 @@
 aliyunsdktag/request/v20180828/ListResourcesByTagRequest.py
 aliyunsdktag/request/v20180828/ListSupportResourceTypesRequest.py
 aliyunsdktag/request/v20180828/ListTagKeysRequest.py
 aliyunsdktag/request/v20180828/ListTagResourcesRequest.py
 aliyunsdktag/request/v20180828/ListTagValuesRequest.py
 aliyunsdktag/request/v20180828/ListTargetsForPolicyRequest.py
 aliyunsdktag/request/v20180828/ModifyPolicyRequest.py
+aliyunsdktag/request/v20180828/OpenCreatedByRequest.py
 aliyunsdktag/request/v20180828/TagResourcesRequest.py
 aliyunsdktag/request/v20180828/UntagResourcesRequest.py
 aliyunsdktag/request/v20180828/__init__.py
```

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/endpoint.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/AttachPolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/AttachPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/CreatePolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CreatePolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/CreateTagsRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/CreateTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DeletePolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DeletePolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DeleteTagRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DeleteTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DescribeRegionsRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DetachPolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DetachPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/DisablePolicyTypeRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/DisablePolicyTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/EnablePolicyTypeRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/EnablePolicyTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GenerateConfigRuleReportRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GenerateConfigRuleReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetConfigRuleReportRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetConfigRuleReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetEffectivePolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetEffectivePolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetPolicyEnableStatusRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetPolicyEnableStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/GetPolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/GetPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListConfigRulesForTargetRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListConfigRulesForTargetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListPoliciesForTargetRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListPoliciesForTargetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListPoliciesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListResourcesByTagRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListResourcesByTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListSupportResourceTypesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListSupportResourceTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagKeysRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagResourcesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTagValuesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ListTargetsForPolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ListTargetsForPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/ModifyPolicyRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/ModifyPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/TagResourcesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/aliyunsdktag/request/v20180828/UntagResourcesRequest.py` & `aliyun-python-sdk-tag-1.0.5/aliyunsdktag/request/v20180828/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tag-1.0.4/setup.py` & `aliyun-python-sdk-tag-1.0.5/setup.py`

 * *Files identical despite different names*

