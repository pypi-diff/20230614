# Comparing `tmp/aliyun-python-sdk-polardb-1.8.8.tar.gz` & `tmp/aliyun-python-sdk-polardb-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-polardb-1.8.8.tar", last modified: Tue Jun 22 07:13:27 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-polardb-1.8.9.tar", last modified: Wed Jul  7 13:13:32 2021, max compression
```

## Comparing `aliyun-python-sdk-polardb-1.8.8.tar` & `aliyun-python-sdk-polardb-1.8.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1557 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1557 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7039 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/
--rw-r--r--   0 root         (0) root         (0)       21 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3304 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/
--rw-r--r--   0 root         (0) root         (0)     2386 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CancelScheduleTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2410 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CheckAccountNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2370 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CheckDBNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2478 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CloseDBClusterMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3538 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2402 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3576 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBClusterEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     6944 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2828 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     4046 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     3476 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3456 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2640 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateGlobalDatabaseNetworkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2988 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2404 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2384 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2430 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBClusterEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2570 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2584 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2396 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2678 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBNodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2376 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2408 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteGlobalDatabaseNetworkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2270 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2742 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2792 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2888 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2240 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2588 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3398 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2248 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeCharacterSetNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2264 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAccessWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     2252 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2268 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAuditLogCollectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2886 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAvailableResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2436 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2252 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2248 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2254 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1934 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2240 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2240 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     2248 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3758 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3308 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClustersWithBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2256 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBInitializeVariableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2402 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBLinksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2088 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBNodePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2714 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3414 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDetachedBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2412 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2246 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeLogBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3258 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeMetaListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2274 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2382 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2388 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3082 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2261 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePolarSQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2052 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2894 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeScheduleTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3198 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3186 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2608 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/FailoverDBClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2776 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/GrantAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3094 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2646 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2640 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2978 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAutoRenewAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3838 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3502 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAccessWhitelistRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAuditLogCollectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2484 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3398 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2438 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3134 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMigrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2392 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2630 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3172 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterPrimaryZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     2936 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2954 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     2576 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3422 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBEndpointAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3202 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBNodeClassRequest.py
--rw-r--r--   0 root         (0) root         (0)     2604 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyGlobalDatabaseNetworkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2498 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyLogBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2574 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyPendingMaintenanceActionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2576 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RemoveDBClusterFromGDNRequest.py
--rw-r--r--   0 root         (0) root         (0)     2604 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ResetAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2208 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RestartDBNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2918 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RestoreTableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2570 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RevokeAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2920 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3092 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/TransformDBClusterPayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2912 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2862 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterMinorVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3030 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-06-22 07:13:27.000000 aliyun-python-sdk-polardb-1.8.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2472 2021-06-22 07:13:26.000000 aliyun-python-sdk-polardb-1.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1557 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1557 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7039 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/
+-rw-r--r--   0 root         (0) root         (0)     2386 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CancelScheduleTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CheckAccountNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CheckDBNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CloseDBClusterMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3538 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBClusterEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6944 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3476 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateGlobalDatabaseNetworkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBClusterEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBNodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteGlobalDatabaseNetworkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeCharacterSetNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAccessWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAuditLogCollectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAvailableResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterTDERequest.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClustersWithBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBInitializeVariableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBLinksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBNodePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDetachedBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeLogBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeMetaListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePolarSQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeScheduleTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/FailoverDBClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/GrantAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAutoRenewAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAccessWhitelistRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAuditLogCollectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3134 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMigrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterPrimaryZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterTDERequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBEndpointAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBNodeClassRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyGlobalDatabaseNetworkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyLogBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyPendingMaintenanceActionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RemoveDBClusterFromGDNRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ResetAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RestartDBNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RestoreTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RevokeAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3092 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/TransformDBClusterPayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterMinorVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2472 2021-07-07 13:13:32.000000 aliyun-python-sdk-polardb-1.8.9/setup.py
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/LICENSE` & `aliyun-python-sdk-polardb-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/PKG-INFO` & `aliyun-python-sdk-polardb-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-polardb
-Version: 1.8.8
+Version: 1.8.9
 Summary: The polardb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-polardb
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/README.rst` & `aliyun-python-sdk-polardb-1.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/PKG-INFO` & `aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-polardb
-Version: 1.8.8
+Version: 1.8.9
 Summary: The polardb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-polardb
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyun_python_sdk_polardb.egg-info/SOURCES.txt` & `aliyun-python-sdk-polardb-1.8.9/aliyun_python_sdk_polardb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/endpoint.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CancelScheduleTasksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CancelScheduleTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CheckAccountNameRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CheckAccountNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CheckDBNameRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CheckDBNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CloseDBClusterMigrationRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CloseDBClusterMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateAccountRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateBackupRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBClusterEndpointRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBClusterEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBClusterRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBEndpointAddressRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBLinkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDBNodesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDBNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateDatabaseRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateGlobalDatabaseNetworkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateGlobalDatabaseNetworkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/CreateParameterGroupRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/CreateParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteAccountRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteBackupRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBClusterEndpointRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBClusterEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBClusterRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBEndpointAddressRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBLinkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDBNodesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDBNodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteDatabaseRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteGlobalDatabaseNetworkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteGlobalDatabaseNetworkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DeleteParameterGroupRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DeleteParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeAccountsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeAutoRenewAttributeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupLogsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupTasksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeBackupsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeCharacterSetNameRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeCharacterSetNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAccessWhitelistRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAccessWhitelistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAttributeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAuditLogCollectorRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAuditLogCollectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAvailableResourcesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterAvailableResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterEndpointsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMigrationRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMonitorRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterParametersRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterPerformanceRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterSSLRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterTDERequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterTDERequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClusterVersionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClusterVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClustersRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBClustersWithBackupsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBClustersWithBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBInitializeVariableRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBInitializeVariableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBLinksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBLinksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDBNodePerformanceRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDBNodePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDatabasesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeDetachedBackupsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeDetachedBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,49 +16,49 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkpolardb.endpoint import endpoint_data
 
-class DescribeGlobalDatabaseNetworksRequest(RpcRequest):
+class DescribePendingMaintenanceActionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribeGlobalDatabaseNetworks','polardb')
+		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribePendingMaintenanceActions','polardb')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_IsHistory(self):
+		return self.get_query_params().get('IsHistory')
+
+	def set_IsHistory(self,IsHistory):
+		self.add_query_param('IsHistory',IsHistory)
+
 	def get_SecurityToken(self):
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self,SecurityToken):
 		self.add_query_param('SecurityToken',SecurityToken)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_DBClusterId(self):
-		return self.get_query_params().get('DBClusterId')
-
-	def set_DBClusterId(self,DBClusterId):
-		self.add_query_param('DBClusterId',DBClusterId)
-
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeLogBackupPolicyRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeLogBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeMetaListRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeMetaListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeParameterTemplatesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeParameterTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePendingMaintenanceActionsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeRegionsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,31 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkpolardb.endpoint import endpoint_data
 
-class DescribePendingMaintenanceActionsRequest(RpcRequest):
+class DescribeRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribePendingMaintenanceActions','polardb')
+		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribeRegions','polardb')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_IsHistory(self):
-		return self.get_query_params().get('IsHistory')
-
-	def set_IsHistory(self,IsHistory):
-		self.add_query_param('IsHistory',IsHistory)
-
-	def get_SecurityToken(self):
-		return self.get_query_params().get('SecurityToken')
-
-	def set_SecurityToken(self,SecurityToken):
-		self.add_query_param('SecurityToken',SecurityToken)
-
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribePolarSQLCollectorPolicyRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribePolarSQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeRegionsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RestartDBNodeRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,31 +16,37 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkpolardb.endpoint import endpoint_data
 
-class DescribeRegionsRequest(RpcRequest):
+class RestartDBNodeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribeRegions','polardb')
+		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'RestartDBNode','polardb')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
+	def get_DBNodeId(self):
+		return self.get_query_params().get('DBNodeId')
+
+	def set_DBNodeId(self,DBNodeId):
+		self.add_query_param('DBNodeId',DBNodeId)
+
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_OwnerAccount(self):
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeScheduleTasksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeScheduleTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/DescribeTasksRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/FailoverDBClusterRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/FailoverDBClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/GrantAccountPrivilegeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/GrantAccountPrivilegeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ListTagResourcesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAccountPasswordRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyAutoRenewAttributeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAccessWhitelistRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAccessWhitelistRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAuditLogCollectorRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterAuditLogCollectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterDescriptionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterEndpointRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMaintainTimeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMigrationRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMigrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMonitorRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterParametersRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterPrimaryZoneRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterPrimaryZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterSSLRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBClusterTDERequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBClusterTDERequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBDescriptionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBEndpointAddressRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBEndpointAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyDBNodeClassRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyDBNodeClassRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyGlobalDatabaseNetworkRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyGlobalDatabaseNetworkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyLogBackupPolicyRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyLogBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ModifyPendingMaintenanceActionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ModifyPendingMaintenanceActionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RemoveDBClusterFromGDNRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RemoveDBClusterFromGDNRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/ResetAccountRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/ResetAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RestartDBNodeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/DescribeGlobalDatabaseNetworksRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,43 +16,61 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkpolardb.endpoint import endpoint_data
 
-class RestartDBNodeRequest(RpcRequest):
+class DescribeGlobalDatabaseNetworksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'RestartDBNode','polardb')
+		RpcRequest.__init__(self, 'polardb', '2017-08-01', 'DescribeGlobalDatabaseNetworks','polardb')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_DBNodeId(self):
-		return self.get_query_params().get('DBNodeId')
+	def get_PageNumber(self):
+		return self.get_query_params().get('PageNumber')
 
-	def set_DBNodeId(self,DBNodeId):
-		self.add_query_param('DBNodeId',DBNodeId)
+	def set_PageNumber(self,PageNumber):
+		self.add_query_param('PageNumber',PageNumber)
+
+	def get_SecurityToken(self):
+		return self.get_query_params().get('SecurityToken')
+
+	def set_SecurityToken(self,SecurityToken):
+		self.add_query_param('SecurityToken',SecurityToken)
+
+	def get_PageSize(self):
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
+	def get_DBClusterId(self):
+		return self.get_query_params().get('DBClusterId')
+
+	def set_DBClusterId(self,DBClusterId):
+		self.add_query_param('DBClusterId',DBClusterId)
+
 	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self,OwnerAccount):
 		self.add_query_param('OwnerAccount',OwnerAccount)
 
 	def get_OwnerId(self):
```

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RestoreTableRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RestoreTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/RevokeAccountPrivilegeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/RevokeAccountPrivilegeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/TagResourcesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/TransformDBClusterPayTypeRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/TransformDBClusterPayTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UntagResourcesRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterMinorVersionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterMinorVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterVersionRequest.py` & `aliyun-python-sdk-polardb-1.8.9/aliyunsdkpolardb/request/v20170801/UpgradeDBClusterVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardb-1.8.8/setup.py` & `aliyun-python-sdk-polardb-1.8.9/setup.py`

 * *Files identical despite different names*

