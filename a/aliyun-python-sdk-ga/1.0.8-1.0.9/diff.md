# Comparing `tmp/aliyun-python-sdk-ga-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-ga-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ga-1.0.8.tar", last modified: Tue Dec  6 09:40:50 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ga-1.0.9.tar", last modified: Tue Dec  6 12:47:42 2022, max compression
```

## Comparing `aliyun-python-sdk-ga-1.0.8.tar` & `aliyun-python-sdk-ga-1.0.9.tar`

### file list

```diff
@@ -1,138 +1,145 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8048 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/
--rw-r--r--   0 root         (0) root         (0)     2335 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AddEntriesToAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2265 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AssociateAclsWithListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AssociateAdditionalCertificatesWithListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AttachDdosToAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2843 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AttachLogStoreToEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1751 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/BandwidthPackageAddAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1757 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/BandwidthPackageRemoveAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2111 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2642 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ConfigEndpointProbeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3722 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2783 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     3263 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     4521 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3146 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2957 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2274 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2920 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     7818 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2860 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointTrafficPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4139 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     6546 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     7893 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     5023 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateForwardingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2656 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateIpSetsRequest.py
--rw-r--r--   0 root         (0) root         (0)    13016 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2102 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateSpareIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1788 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1723 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1496 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2216 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2196 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointTrafficPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1994 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1908 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1961 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2177 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteForwardingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1523 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteIpSetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2102 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteSpareIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1526 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeAcceleratorAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1490 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1659 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1518 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeBandwidthPackageAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1530 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndPointTrafficPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1544 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1442 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1273 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1502 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetachDdosFromAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2214 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetachLogStoreFromEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetectApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DisableApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2094 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DissociateAclsFromListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2177 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DissociateAdditionalCertificatesFromListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/EnableApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1416 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     1490 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1639 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2039 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2011 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetSpareIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAccelerateAreasRequest.py
--rw-r--r--   0 root         (0) root         (0)     2659 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAcceleratorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2876 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAclsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2202 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListApplicationMonitorDetectResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1508 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAvailableAccelerateAreasRequest.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAvailableBusiRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2854 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBandwidthPackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBandwidthackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2669 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBasicAcceleratorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1273 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBusiRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2931 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2296 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2678 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointTrafficPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2286 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2127 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsByDestinationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2292 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2728 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2483 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListForwardingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1846 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListIpSetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2224 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListListenerCertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1852 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListListenersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1842 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListSpareIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1669 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListSystemSecurityPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2157 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/RemoveEntriesFromAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ReplaceBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2505 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorConfirmRequest.py
--rw-r--r--   0 root         (0) root         (0)     2576 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAclAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2463 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAdditionalCertificateWithListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3221 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateApplicationMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2497 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBandwidthPackagaAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2660 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBandwidthPackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2045 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicAcceleratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2724 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1832 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2095 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3144 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupDestinationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointTrafficPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3957 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2069 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     6134 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     7430 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     5192 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateForwardingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1822 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateIpSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1743 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateIpSetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     5380 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2447 2022-12-06 09:40:50.000000 aliyun-python-sdk-ga-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8538 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/
+-rw-r--r--   0 root         (0) root         (0)     2335 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AddEntriesToAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AssociateAclsWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AssociateAdditionalCertificatesWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AttachDdosToAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AttachLogStoreToEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/BandwidthPackageAddAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/BandwidthPackageRemoveAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ConfigEndpointProbeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3263 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicAccelerateIpEndpointRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicAccelerateIpEndpointRelationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicAccelerateIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointTrafficPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7893 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateForwardingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateIpSetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)    13016 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateSpareIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicAccelerateIpEndpointRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicAccelerateIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointTrafficPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteForwardingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteIpSetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteSpareIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeAcceleratorAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeBandwidthPackageAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndPointTrafficPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetachDdosFromAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetachLogStoreFromEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetectApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DisableApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DissociateAclsFromListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DissociateAdditionalCertificatesFromListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/EnableApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicAccelerateIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetSpareIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAccelerateAreasRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAcceleratorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAclsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListApplicationMonitorDetectResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAvailableAccelerateAreasRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAvailableBusiRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBandwidthPackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBandwidthackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBasicAcceleratorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBusiRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointTrafficPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsByDestinationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListForwardingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListIpSetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListListenerCertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListListenersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListSpareIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListSystemSecurityPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/RemoveEntriesFromAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ReplaceBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorConfirmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAclAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAdditionalCertificateWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateApplicationMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBandwidthPackagaAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBandwidthPackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicAcceleratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupDestinationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointTrafficPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3957 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6134 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateForwardingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateIpSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateIpSetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5380 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2447 2022-12-06 12:47:42.000000 aliyun-python-sdk-ga-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-ga-1.0.8/LICENSE` & `aliyun-python-sdk-ga-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/PKG-INFO` & `aliyun-python-sdk-ga-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ga
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ga module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ga
```

### Comparing `aliyun-python-sdk-ga-1.0.8/README.rst` & `aliyun-python-sdk-ga-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/PKG-INFO` & `aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ga
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ga module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ga
```

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyun_python_sdk_ga.egg-info/SOURCES.txt` & `aliyun-python-sdk-ga-1.0.9/aliyun_python_sdk_ga.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 aliyunsdkga/request/v20191120/BandwidthPackageRemoveAcceleratorRequest.py
 aliyunsdkga/request/v20191120/ChangeResourceGroupRequest.py
 aliyunsdkga/request/v20191120/ConfigEndpointProbeRequest.py
 aliyunsdkga/request/v20191120/CreateAcceleratorRequest.py
 aliyunsdkga/request/v20191120/CreateAclRequest.py
 aliyunsdkga/request/v20191120/CreateApplicationMonitorRequest.py
 aliyunsdkga/request/v20191120/CreateBandwidthPackageRequest.py
+aliyunsdkga/request/v20191120/CreateBasicAccelerateIpEndpointRelationRequest.py
+aliyunsdkga/request/v20191120/CreateBasicAccelerateIpEndpointRelationsRequest.py
+aliyunsdkga/request/v20191120/CreateBasicAccelerateIpRequest.py
 aliyunsdkga/request/v20191120/CreateBasicAcceleratorRequest.py
 aliyunsdkga/request/v20191120/CreateBasicEndpointGroupRequest.py
 aliyunsdkga/request/v20191120/CreateBasicIpSetRequest.py
 aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupDestinationsRequest.py
 aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupsRequest.py
 aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointTrafficPoliciesRequest.py
 aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointsRequest.py
@@ -37,16 +40,19 @@
 aliyunsdkga/request/v20191120/CreateIpSetsRequest.py
 aliyunsdkga/request/v20191120/CreateListenerRequest.py
 aliyunsdkga/request/v20191120/CreateSpareIpsRequest.py
 aliyunsdkga/request/v20191120/DeleteAcceleratorRequest.py
 aliyunsdkga/request/v20191120/DeleteAclRequest.py
 aliyunsdkga/request/v20191120/DeleteApplicationMonitorRequest.py
 aliyunsdkga/request/v20191120/DeleteBandwidthPackageRequest.py
+aliyunsdkga/request/v20191120/DeleteBasicAccelerateIpEndpointRelationRequest.py
+aliyunsdkga/request/v20191120/DeleteBasicAccelerateIpRequest.py
 aliyunsdkga/request/v20191120/DeleteBasicAcceleratorRequest.py
 aliyunsdkga/request/v20191120/DeleteBasicEndpointGroupRequest.py
+aliyunsdkga/request/v20191120/DeleteBasicEndpointRequest.py
 aliyunsdkga/request/v20191120/DeleteBasicIpSetRequest.py
 aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupDestinationsRequest.py
 aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupsRequest.py
 aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointTrafficPoliciesRequest.py
 aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointsRequest.py
 aliyunsdkga/request/v20191120/DeleteEndpointGroupRequest.py
 aliyunsdkga/request/v20191120/DeleteEndpointGroupsRequest.py
@@ -72,14 +78,15 @@
 aliyunsdkga/request/v20191120/DetachLogStoreFromEndpointGroupRequest.py
 aliyunsdkga/request/v20191120/DetectApplicationMonitorRequest.py
 aliyunsdkga/request/v20191120/DisableApplicationMonitorRequest.py
 aliyunsdkga/request/v20191120/DissociateAclsFromListenerRequest.py
 aliyunsdkga/request/v20191120/DissociateAdditionalCertificatesFromListenerRequest.py
 aliyunsdkga/request/v20191120/EnableApplicationMonitorRequest.py
 aliyunsdkga/request/v20191120/GetAclRequest.py
+aliyunsdkga/request/v20191120/GetBasicAccelerateIpRequest.py
 aliyunsdkga/request/v20191120/GetBasicAcceleratorRequest.py
 aliyunsdkga/request/v20191120/GetBasicEndpointGroupRequest.py
 aliyunsdkga/request/v20191120/GetBasicIpSetRequest.py
 aliyunsdkga/request/v20191120/GetHealthStatusRequest.py
 aliyunsdkga/request/v20191120/GetSpareIpRequest.py
 aliyunsdkga/request/v20191120/ListAccelerateAreasRequest.py
 aliyunsdkga/request/v20191120/ListAcceleratorsRequest.py
```

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/endpoint.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AddEntriesToAclRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AddEntriesToAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AssociateAclsWithListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AssociateAclsWithListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AssociateAdditionalCertificatesWithListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AssociateAdditionalCertificatesWithListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AttachDdosToAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AttachDdosToAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/AttachLogStoreToEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/AttachLogStoreToEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/BandwidthPackageAddAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/BandwidthPackageAddAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/BandwidthPackageRemoveAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/BandwidthPackageRemoveAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ConfigEndpointProbeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ConfigEndpointProbeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateAclRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBandwidthPackageRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateBasicIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateBasicIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupDestinationsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointTrafficPoliciesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointTrafficPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateCustomRoutingEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateForwardingRulesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateForwardingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateIpSetsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateIpSetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/CreateSpareIpsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/CreateSpareIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteAclRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBandwidthPackageRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteBasicIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteBasicIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupDestinationsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointTrafficPoliciesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointTrafficPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteCustomRoutingEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteForwardingRulesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteForwardingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteIpSetsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteIpSetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DeleteSpareIpsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DeleteSpareIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeAcceleratorAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeAcceleratorAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeBandwidthPackageAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeBandwidthPackageAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeBandwidthPackageRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndPointTrafficPolicyRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndPointTrafficPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupDestinationsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeCustomRoutingEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DescribeRegionsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetachDdosFromAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetachDdosFromAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetachLogStoreFromEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetachLogStoreFromEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DetectApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DetectApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DisableApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DisableApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DissociateAclsFromListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DissociateAclsFromListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/DissociateAdditionalCertificatesFromListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/DissociateAdditionalCertificatesFromListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/EnableApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/EnableApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetAclRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetBasicIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetBasicIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetHealthStatusRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetHealthStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/GetSpareIpRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/GetSpareIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAccelerateAreasRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAccelerateAreasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAcceleratorsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAcceleratorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAclsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAclsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListApplicationMonitorDetectResultRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListApplicationMonitorDetectResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAvailableAccelerateAreasRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAvailableAccelerateAreasRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListAvailableBusiRegionsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListAvailableBusiRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBandwidthPackagesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBandwidthPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBandwidthackagesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBandwidthackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBasicAcceleratorsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBasicAcceleratorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListBusiRegionsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListBusiRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupDestinationsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointTrafficPoliciesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointTrafficPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsByDestinationRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsByDestinationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListCustomRoutingPortMappingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListEndpointGroupsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,12 +57,21 @@
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_AcceleratorId(self): # String
 		return self.get_query_params().get('AcceleratorId')
 
 	def set_AcceleratorId(self, AcceleratorId):  # String
 		self.add_query_param('AcceleratorId', AcceleratorId)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_EndpointGroupId(self): # String
 		return self.get_query_params().get('EndpointGroupId')
 
 	def set_EndpointGroupId(self, EndpointGroupId):  # String
 		self.add_query_param('EndpointGroupId', EndpointGroupId)
```

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListForwardingRulesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListForwardingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListIpSetsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListIpSetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListListenerCertificatesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListListenerCertificatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListListenersRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListListenersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListSpareIpsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListSpareIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ListSystemSecurityPoliciesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ListSystemSecurityPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/RemoveEntriesFromAclRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/RemoveEntriesFromAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/ReplaceBandwidthPackageRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/ReplaceBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorConfirmRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorConfirmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAclAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAclAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateAdditionalCertificateWithListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateAdditionalCertificateWithListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateApplicationMonitorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateApplicationMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBandwidthPackagaAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBandwidthPackagaAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBandwidthPackageRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicAcceleratorRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicAcceleratorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateBasicIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateBasicIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupDestinationsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointGroupDestinationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointTrafficPoliciesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointTrafficPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateCustomRoutingEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupAttributeRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateEndpointGroupsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateEndpointGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateForwardingRulesRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateForwardingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateIpSetRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateIpSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateIpSetsRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateIpSetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/aliyunsdkga/request/v20191120/UpdateListenerRequest.py` & `aliyun-python-sdk-ga-1.0.9/aliyunsdkga/request/v20191120/UpdateListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ga-1.0.8/setup.py` & `aliyun-python-sdk-ga-1.0.9/setup.py`

 * *Files identical despite different names*

