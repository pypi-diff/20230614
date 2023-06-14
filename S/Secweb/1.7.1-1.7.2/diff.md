# Comparing `tmp/Secweb-1.7.1.tar.gz` & `tmp/Secweb-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Secweb-1.7.1.tar", last modified: Mon Jun 12 14:19:55 2023, max compression
+gzip compressed data, was "Secweb-1.7.2.tar", last modified: Wed Jun 14 06:40:33 2023, max compression
```

## Comparing `Secweb-1.7.1.tar` & `Secweb-1.7.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.874220 Secweb-1.7.1/
--rw-rw-rw-   0        0        0    17154 2023-06-11 15:32:03.000000 Secweb-1.7.1/LICENSE
--rw-rw-rw-   0        0        0    18130 2023-06-12 14:19:55.873223 Secweb-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    17396 2023-06-11 15:31:47.000000 Secweb-1.7.1/README.md
--rw-rw-rw-   0        0        0      800 2023-06-11 15:24:00.000000 Secweb-1.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 14:19:55.874220 Secweb-1.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.763217 Secweb-1.7.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.781219 Secweb-1.7.1/src/Secweb/
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.791220 Secweb-1.7.1/src/Secweb/CacheControl/
--rw-rw-rw-   0        0        0     4392 2023-06-10 14:44:58.000000 Secweb-1.7.1/src/Secweb/CacheControl/CacheControlMiddleware.py
--rw-rw-rw-   0        0        0       48 2022-04-09 06:01:04.000000 Secweb-1.7.1/src/Secweb/CacheControl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.796220 Secweb-1.7.1/src/Secweb/ClearSiteData/
--rw-rw-rw-   0        0        0     3768 2023-06-11 06:37:05.000000 Secweb-1.7.1/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py
--rw-rw-rw-   0        0        0       50 2022-04-09 06:01:25.000000 Secweb-1.7.1/src/Secweb/ClearSiteData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.801219 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/
--rw-rw-rw-   0        0        0     6144 2023-06-11 14:16:25.000000 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py
--rw-rw-rw-   0        0        0      130 2021-07-11 12:29:16.000000 Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.806220 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/
--rw-rw-rw-   0        0        0     1686 2023-06-10 06:05:41.000000 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py
--rw-rw-rw-   0        0        0       74 2021-07-11 12:30:08.000000 Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.811220 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/
--rw-rw-rw-   0        0        0     1682 2023-06-10 05:46:33.000000 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py
--rw-rw-rw-   0        0        0       70 2021-07-11 12:30:45.000000 Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.815219 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/
--rw-rw-rw-   0        0        0     1677 2023-06-10 05:32:12.000000 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py
--rw-rw-rw-   0        0        0       74 2021-07-11 12:31:17.000000 Secweb-1.7.1/src/Secweb/CrossOriginResourcePolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.819218 Secweb-1.7.1/src/Secweb/ExpectCt/
--rw-rw-rw-   0        0        0     2210 2023-06-10 05:21:43.000000 Secweb-1.7.1/src/Secweb/ExpectCt/ExpectCtMiddleware.py
--rw-rw-rw-   0        0        0       42 2021-04-11 15:30:17.000000 Secweb-1.7.1/src/Secweb/ExpectCt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.823218 Secweb-1.7.1/src/Secweb/OriginAgentCluster/
--rw-rw-rw-   0        0        0     1146 2023-06-09 15:21:23.000000 Secweb-1.7.1/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py
--rw-rw-rw-   0        0        0       62 2021-04-11 15:30:42.000000 Secweb-1.7.1/src/Secweb/OriginAgentCluster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.831221 Secweb-1.7.1/src/Secweb/ReferrerPolicy/
--rw-rw-rw-   0        0        0     2345 2023-06-09 14:21:28.000000 Secweb-1.7.1/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py
--rw-rw-rw-   0        0        0       54 2021-04-11 15:31:16.000000 Secweb-1.7.1/src/Secweb/ReferrerPolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.841220 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/
--rw-rw-rw-   0        0        0     2155 2023-06-10 05:21:05.000000 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py
--rw-rw-rw-   0        0        0       51 2021-04-11 15:31:34.000000 Secweb-1.7.1/src/Secweb/StrictTransportSecurity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.848220 Secweb-1.7.1/src/Secweb/XContentTypeOptions/
--rw-rw-rw-   0        0        0     1162 2023-06-08 12:41:33.000000 Secweb-1.7.1/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py
--rw-rw-rw-   0        0        0       64 2021-04-11 15:31:57.000000 Secweb-1.7.1/src/Secweb/XContentTypeOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.853220 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/
--rw-rw-rw-   0        0        0     1553 2023-06-09 10:34:53.000000 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py
--rw-rw-rw-   0        0        0       64 2021-04-11 15:32:10.000000 Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.858219 Secweb-1.7.1/src/Secweb/XDownloadOptions/
--rw-rw-rw-   0        0        0     1136 2023-06-08 12:32:50.000000 Secweb-1.7.1/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py
--rw-rw-rw-   0        0        0       58 2021-04-11 15:32:26.000000 Secweb-1.7.1/src/Secweb/XDownloadOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.862222 Secweb-1.7.1/src/Secweb/XFrameOptions/
--rw-rw-rw-   0        0        0     1470 2023-06-09 10:32:42.000000 Secweb-1.7.1/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py
--rw-rw-rw-   0        0        0       45 2021-04-11 15:32:44.000000 Secweb-1.7.1/src/Secweb/XFrameOptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.866219 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/
--rw-rw-rw-   0        0        0     1735 2023-06-09 10:30:43.000000 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py
--rw-rw-rw-   0        0        0       84 2021-04-11 15:33:27.000000 Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/__init__.py
--rw-rw-rw-   0        0        0       25 2021-07-11 16:07:32.000000 Secweb-1.7.1/src/Secweb/__init__.py
--rw-rw-rw-   0        0        0     6764 2023-06-11 14:40:50.000000 Secweb-1.7.1/src/Secweb/index.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.871218 Secweb-1.7.1/src/Secweb/xXSSProtection/
--rw-rw-rw-   0        0        0       54 2021-04-11 15:33:44.000000 Secweb-1.7.1/src/Secweb/xXSSProtection/__init__.py
--rw-rw-rw-   0        0        0     1636 2023-06-11 04:52:15.000000 Secweb-1.7.1/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:19:55.786220 Secweb-1.7.1/src/Secweb.egg-info/
--rw-rw-rw-   0        0        0    18130 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1887 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 14:19:55.000000 Secweb-1.7.1/src/Secweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.344441 Secweb-1.7.2/
+-rw-rw-rw-   0        0        0    17154 2023-06-11 15:32:03.000000 Secweb-1.7.2/LICENSE
+-rw-rw-rw-   0        0        0    18130 2023-06-14 06:40:33.344441 Secweb-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17396 2023-06-11 15:31:47.000000 Secweb-1.7.2/README.md
+-rw-rw-rw-   0        0        0      800 2023-06-14 06:21:51.000000 Secweb-1.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:40:33.345440 Secweb-1.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.285206 Secweb-1.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.298441 Secweb-1.7.2/src/Secweb/
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.306441 Secweb-1.7.2/src/Secweb/CacheControl/
+-rw-rw-rw-   0        0        0     4261 2023-06-14 05:28:00.000000 Secweb-1.7.2/src/Secweb/CacheControl/CacheControlMiddleware.py
+-rw-rw-rw-   0        0        0       48 2022-04-09 06:01:04.000000 Secweb-1.7.2/src/Secweb/CacheControl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.308440 Secweb-1.7.2/src/Secweb/ClearSiteData/
+-rw-rw-rw-   0        0        0     3627 2023-06-14 05:27:41.000000 Secweb-1.7.2/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py
+-rw-rw-rw-   0        0        0       50 2022-04-09 06:01:25.000000 Secweb-1.7.2/src/Secweb/ClearSiteData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.310442 Secweb-1.7.2/src/Secweb/ContentSecurityPolicy/
+-rw-rw-rw-   0        0        0     5981 2023-06-14 05:27:06.000000 Secweb-1.7.2/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py
+-rw-rw-rw-   0        0        0      130 2021-07-11 12:29:16.000000 Secweb-1.7.2/src/Secweb/ContentSecurityPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.313441 Secweb-1.7.2/src/Secweb/CrossOriginEmbedderPolicy/
+-rw-rw-rw-   0        0        0     1562 2023-06-14 05:26:22.000000 Secweb-1.7.2/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       74 2021-07-11 12:30:08.000000 Secweb-1.7.2/src/Secweb/CrossOriginEmbedderPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.316442 Secweb-1.7.2/src/Secweb/CrossOriginOpenerPolicy/
+-rw-rw-rw-   0        0        0     1558 2023-06-14 05:26:04.000000 Secweb-1.7.2/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       70 2021-07-11 12:30:45.000000 Secweb-1.7.2/src/Secweb/CrossOriginOpenerPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.318444 Secweb-1.7.2/src/Secweb/CrossOriginResourcePolicy/
+-rw-rw-rw-   0        0        0     1553 2023-06-14 05:25:42.000000 Secweb-1.7.2/src/Secweb/CrossOriginResourcePolicy/CrossOriginResourcePolicyMiddleware.py
+-rw-rw-rw-   0        0        0       74 2021-07-11 12:31:17.000000 Secweb-1.7.2/src/Secweb/CrossOriginResourcePolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.321439 Secweb-1.7.2/src/Secweb/ExpectCt/
+-rw-rw-rw-   0        0        0     2073 2023-06-14 05:25:23.000000 Secweb-1.7.2/src/Secweb/ExpectCt/ExpectCtMiddleware.py
+-rw-rw-rw-   0        0        0       42 2021-04-11 15:30:17.000000 Secweb-1.7.2/src/Secweb/ExpectCt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.323440 Secweb-1.7.2/src/Secweb/OriginAgentCluster/
+-rw-rw-rw-   0        0        0     1038 2023-06-14 05:24:29.000000 Secweb-1.7.2/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py
+-rw-rw-rw-   0        0        0       62 2021-04-11 15:30:42.000000 Secweb-1.7.2/src/Secweb/OriginAgentCluster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.325440 Secweb-1.7.2/src/Secweb/ReferrerPolicy/
+-rw-rw-rw-   0        0        0     2209 2023-06-14 05:20:44.000000 Secweb-1.7.2/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py
+-rw-rw-rw-   0        0        0       54 2021-04-11 15:31:16.000000 Secweb-1.7.2/src/Secweb/ReferrerPolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.327440 Secweb-1.7.2/src/Secweb/StrictTransportSecurity/
+-rw-rw-rw-   0        0        0     2024 2023-06-14 05:23:12.000000 Secweb-1.7.2/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py
+-rw-rw-rw-   0        0        0       51 2021-04-11 15:31:34.000000 Secweb-1.7.2/src/Secweb/StrictTransportSecurity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.331443 Secweb-1.7.2/src/Secweb/XContentTypeOptions/
+-rw-rw-rw-   0        0        0     1054 2023-06-14 05:22:53.000000 Secweb-1.7.2/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       64 2021-04-11 15:31:57.000000 Secweb-1.7.2/src/Secweb/XContentTypeOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.333441 Secweb-1.7.2/src/Secweb/XDNSPrefetchControl/
+-rw-rw-rw-   0        0        0     1429 2023-06-14 05:22:36.000000 Secweb-1.7.2/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py
+-rw-rw-rw-   0        0        0       64 2021-04-11 15:32:10.000000 Secweb-1.7.2/src/Secweb/XDNSPrefetchControl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.336440 Secweb-1.7.2/src/Secweb/XDownloadOptions/
+-rw-rw-rw-   0        0        0     1028 2023-06-14 05:22:10.000000 Secweb-1.7.2/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       58 2021-04-11 15:32:26.000000 Secweb-1.7.2/src/Secweb/XDownloadOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.338439 Secweb-1.7.2/src/Secweb/XFrameOptions/
+-rw-rw-rw-   0        0        0     1346 2023-06-14 05:21:55.000000 Secweb-1.7.2/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py
+-rw-rw-rw-   0        0        0       45 2021-04-11 15:32:44.000000 Secweb-1.7.2/src/Secweb/XFrameOptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.340440 Secweb-1.7.2/src/Secweb/XPermittedCrossDomainPolicies/
+-rw-rw-rw-   0        0        0     1611 2023-06-14 05:21:33.000000 Secweb-1.7.2/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py
+-rw-rw-rw-   0        0        0       84 2021-04-11 15:33:27.000000 Secweb-1.7.2/src/Secweb/XPermittedCrossDomainPolicies/__init__.py
+-rw-rw-rw-   0        0        0       25 2021-07-11 16:07:32.000000 Secweb-1.7.2/src/Secweb/__init__.py
+-rw-rw-rw-   0        0        0     6641 2023-06-14 06:39:45.000000 Secweb-1.7.2/src/Secweb/index.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.342440 Secweb-1.7.2/src/Secweb/xXSSProtection/
+-rw-rw-rw-   0        0        0       54 2021-04-11 15:33:44.000000 Secweb-1.7.2/src/Secweb/xXSSProtection/__init__.py
+-rw-rw-rw-   0        0        0     1512 2023-06-14 05:21:09.000000 Secweb-1.7.2/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:40:33.303441 Secweb-1.7.2/src/Secweb.egg-info/
+-rw-rw-rw-   0        0        0    18130 2023-06-14 06:40:33.000000 Secweb-1.7.2/src/Secweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1887 2023-06-14 06:40:33.000000 Secweb-1.7.2/src/Secweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:40:33.000000 Secweb-1.7.2/src/Secweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 06:40:33.000000 Secweb-1.7.2/src/Secweb.egg-info/top_level.txt
```

### Comparing `Secweb-1.7.1/LICENSE` & `Secweb-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Secweb-1.7.1/PKG-INFO` & `Secweb-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Secweb
-Version: 1.7.1
+Version: 1.7.2
 Summary: Secweb is a pack of security middlewares for fastApi and starlette server it includes CSP, HSTS, and many more
 Author-email: Motagamwala Taha Arif Ali <tahaar5321@gmail.com>
 Project-URL: Homepage, https://github.com/tmotagam/Secweb
 Project-URL: Bug Tracker, https://github.com/tmotagam/Secweb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `Secweb-1.7.1/README.md` & `Secweb-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `Secweb-1.7.1/pyproject.toml` & `Secweb-1.7.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Secweb"
-version = "1.7.1"
+version = "1.7.2"
 authors = [ { name="Motagamwala Taha Arif Ali", email = "tahaar5321@gmail.com" }, ]
 description = "Secweb is a pack of security middlewares for fastApi and starlette server it includes CSP, HSTS, and many more"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `Secweb-1.7.1/src/Secweb/CacheControl/CacheControlMiddleware.py` & `Secweb-1.7.2/src/Secweb/CacheControl/CacheControlMiddleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class CacheControl:
     ''' CacheControl class sets Cache-Control header it takes one Parameter
 
     Example:
         app.add_middleware(CacheControl, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, int | bool] = {'max-age': 86400, 'private': True }):
+    def __init__(self, app, Option = {'max-age': 86400, 'private': True }):
         self.app = app
         self.policyString = ''
         if 'max-age' in Option and Option['max-age'] >= 0:
             self.policyString += f'max-age={str(Option["max-age"])}' if list(Option.keys()).__len__() == 1 else f'max-age={str(Option["max-age"])}, '
             Option.pop('max-age')
         if 's-maxage' in Option and Option['s-maxage'] >= 0:
             self.policyString += f's-maxage={str(Option["s-maxage"])}' if list(Option.keys()).__len__() == 1 else f's-maxage={str(Option["s-maxage"])}, '
@@ -54,19 +53,19 @@
             Option.pop('immutable')
         if 'stale-while-revalidate' in Option and Option['stale-while-revalidate'] > 0:
             self.policyString += f'stale-while-revalidate={str(Option["stale-while-revalidate"])}' if list(Option.keys()).__len__() == 1 else f'stale-while-revalidate={str(Option["stale-while-revalidate"])}, '
             Option.pop('stale-while-revalidate')
         if list(Option.keys()).__len__() != 0 :
             raise SyntaxError('Cache-Control has 12 options 1> "max-age" 2> "s-maxage" 3> "no-cache" 4> "no-store" 5> "no-transform" 6> "must-revalidate" 7> "proxy-revalidate" 8> "must-understand" 9> "private" 10> "public" 11> "immutable" 12> "stale-while-revalidate" ')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Cache_Control(message: Message):
+        async def set_Cache_Control(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Cache-Control', self.policyString)
 
             await send(message)
 
         await self.app(scope, receive, set_Cache_Control)
```

### Comparing `Secweb-1.7.1/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py` & `Secweb-1.7.2/src/Secweb/ClearSiteData/ClearSiteDataMiddleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 from starlette.convertors import CONVERTOR_TYPES
 from re import compile, escape
 
-def __path_regex_builder__(path: str):
+def __path_regex_builder__(path):
     is_host = not path.startswith("/")
 
     path_regex = "^"
     duplicated_params = set()
 
     idx = 0
     for match in compile("{([a-zA-Z_][a-zA-Z0-9_]*)(:[a-zA-Z_][a-zA-Z0-9_]*)?}").finditer(path):
@@ -49,15 +48,15 @@
         app.add_middleware(ClearSiteData, Option={}, Routes=[])
 
     Parameter:
 
     Option={} This is a dictionary
 
     Routes=[] This is an Array'''
-    def __init__(self, app: ASGIApp, Option: dict[str, bool] = {'cache': True, 'cookies': True, 'storage': True}, Routes: list[str] = []):
+    def __init__(self, app, Option = {'cache': True, 'cookies': True, 'storage': True}, Routes = []):
         self.app = app
         self.policyString = ''
         if Routes.__len__() == 0:
             raise SyntaxError('Cannot Set Clear-Site-Data header if the routes are empty')
         
         self.pathregex = [__path_regex_builder__(i) for i in Routes]
 
@@ -74,19 +73,19 @@
             if 'storage' in Option and Option['storage'] is True:
                 self.policyString += '"storage"'
                 Option.pop('storage')
 
         if list(Option.keys()).__len__() != 0 :
             raise SyntaxError('Clear-Site-Data has 4 options 1> "cache" 2> "cookies" 3> "storage" 4> "*"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
         
-        async def set_route(message: Message):
+        async def set_route(message):
             if message["type"] == "http.response.start":
                 for i in self.pathregex:
                     if i.match(scope["path"]):
                         headers = MutableHeaders(scope=message)
                         headers.append('Clear-Site-Data', self.policyString)
                         break
```

### Comparing `Secweb-1.7.1/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py` & `Secweb-1.7.2/src/Secweb/ContentSecurityPolicy/ContentSecurityPolicyMiddleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
 from secrets import token_urlsafe
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 nonce = None
 
 def Nonce_Processor(DEFAULT_ENTROPY=90):
     ''' This is the Nonce Processor module that will create the nonce for inline style and script
     It will be needed to call on the route which needs nonce for the inline script and css
@@ -35,23 +34,23 @@
     Parameters :
 
     Option={} This is a dictionary
 
     script_nonce=False This is the nonce flag for script
 
     style_nocne=True This is the nonce flag for style css'''
-    def __init__(self, app: ASGIApp, script_nonce: bool = False, style_nonce: bool = False, Option: dict[str, list[str]] = {'default-src': ["'self'"], 'base-uri': ["'self'"], 'block-all-mixed-content': [], 'font-src': ["'self'", 'https:', 'data:'], 'frame-ancestors': ["'self'"], 'img-src': ["'self'", 'data:'], "object-src": ["'none'"], "script-src": ["'self'"], "script-src-attr": ["'none'"], "style-src": ["'self'", "https:", "'unsafe-inline'"], "upgrade-insecure-requests": [], "require-trusted-types-for": ["'script'"]}):
+    def __init__(self, app, script_nonce: bool = False, style_nonce: bool = False, Option = {'default-src': ["'self'"], 'base-uri': ["'self'"], 'block-all-mixed-content': [], 'font-src': ["'self'", 'https:', 'data:'], 'frame-ancestors': ["'self'"], 'img-src': ["'self'", 'data:'], "object-src": ["'none'"], "script-src": ["'self'"], "script-src-attr": ["'none'"], "style-src": ["'self'", "https:", "'unsafe-inline'"], "upgrade-insecure-requests": [], "require-trusted-types-for": ["'script'"]}):
         self.app = app
         self.PolicyString = ''
         self.script_nonce = script_nonce
         self.style_nonce = style_nonce
         Policy = ['child-src', 'connect-src', 'default-src', 'font-src', 'frame-src', 'img-src', 'manifest-src', 'media-src', 'object-src', 'script-src', 'script-src-elem', 'script-src-attr', 'style-src', 'style-src-elem', 'style-src-attr', 'worker-src', 'base-uri', 'plugin-types', 'sandbox', 'form-action', 'frame-ancestors', 'navigate-to', 'report-uri', 'report-to', 'block-all-mixed-content', 'require-trusted-types-for', 'trusted-types', 'upgrade-insecure-requests']
         self.__PolicyCheck__(Option, Policy)
 
-    def __PolicyCheck__(self, Option: dict[str, list[str]], Policy: list[str]):
+    def __PolicyCheck__(self, Option, Policy):
         keys = list(Option.keys())
 
         if self.script_nonce is True:
             if keys.index('script-src') is None:
                 raise SyntaxError('script-src is compulsory for nonce')
 
         if self.style_nonce is True:
@@ -88,19 +87,19 @@
                         else:
                             self.PolicyString += '; '
                     else:
                         self.PolicyString += ' '
             else:
                 raise SyntaxError(f'The Policy { keys[i] } does not exists')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Content_Security_Policy(message: Message):
+        async def set_Content_Security_Policy(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 if self.script_nonce is True and self.style_nonce is True:
                     PS = self.PolicyString
                     headers.append('Content-Security-Policy', PS.format(script_nonce_value=nonce, style_nonce_value=nonce))
                 elif self.style_nonce is True:
                     PS = self.PolicyString
```

### Comparing `Secweb-1.7.1/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py` & `Secweb-1.7.2/src/Secweb/CrossOriginEmbedderPolicy/CrossOriginEmbedderPolicyMiddleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class CrossOriginEmbedderPolicy:
     ''' CrossOriginEmbedderPolicy class sets Cross-Origin-Embedder-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(CrossOriginEmbedderPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'Cross-Origin-Embedder-Policy': 'unsafe-none'}):
+    def __init__(self, app, Option = {'Cross-Origin-Embedder-Policy': 'unsafe-none'}):
         self.app = app
         self.Option = Option
         Policies = ['require-corp', 'unsafe-none', 'credentialless']
         if self.Option['Cross-Origin-Embedder-Policy'] not in Policies:
             raise SyntaxError('Cross-Origin-Embedder-Policy has 3 options 1> "unsafe-none" 2> "require-corp" 3> "credentialless"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Cross_Origin_Embedder_Policy(message: Message):
+        async def set_Cross_Origin_Embedder_Policy(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Cross-Origin-Embedder-Policy', self.Option['Cross-Origin-Embedder-Policy'])
 
             await send(message)
 
         await self.app(scope, receive, set_Cross_Origin_Embedder_Policy)
```

### Comparing `Secweb-1.7.1/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py` & `Secweb-1.7.2/src/Secweb/CrossOriginOpenerPolicy/CrossOriginOpenerPolicyMiddleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class CrossOriginOpenerPolicy:
     ''' CrossOriginOpenerPolicy class sets Cross-Origin-Opener-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(CrossOriginOpenerPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'Cross-Origin-Opener-Policy': 'unsafe-none'}):
+    def __init__(self, app, Option = {'Cross-Origin-Opener-Policy': 'unsafe-none'}):
         self.app = app
         self.Option = Option
         Policies = ['unsafe-none', 'same-origin-allow-popups', 'same-origin']
         if self.Option['Cross-Origin-Opener-Policy'] not in Policies:
             raise SyntaxError('Cross-Origin-Opener-Policy has 3 options 1> "unsafe-none" 2> "same-origin-allow-popups" 3> "same-origin"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Cross_Origin_Opener_Policy(message: Message):
+        async def set_Cross_Origin_Opener_Policy(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Cross-Origin-Opener-Policy', self.Option['Cross-Origin-Opener-Policy'])
 
             await send(message)
 
         await self.app(scope, receive, set_Cross_Origin_Opener_Policy)
```

### Comparing `Secweb-1.7.1/src/Secweb/ExpectCt/ExpectCtMiddleware.py` & `Secweb-1.7.2/src/Secweb/ExpectCt/ExpectCtMiddleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
 from warnings import warn
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class ExpectCt:
     ''' ExpectCt class takes only one parameter Option for setting the Expect-CT header (deprecated)
 
     Example :
         app.add_middleware(ExpectCt, Option={})
 
     Parameter :
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str | bool | int] = {'max-age': 123, 'enforce': False, 'report-uri': ''}):
+    def __init__(self, app, Option = {'max-age': 123, 'enforce': False, 'report-uri': ''}):
         self.app = app
         self.PolicyString = ''
         warn("Expect-CT Header is now deprecated by browsers and may be removed from the library in the upcoming versions", SyntaxWarning, 2)
         if 'max-age' in Option:
             if int(Option['max-age']) and int(Option['max-age']) > 0:
                 self.PolicyString += 'max-age=' + str(Option['max-age'])
             else:
@@ -32,19 +31,19 @@
 
             if 'report-uri' in Option and Option['report-uri'] != '':
                 self.PolicyString += ', report-uri=' + '"' + str(Option['report-uri']) + '"'
 
         else:
             raise SyntaxError('Expect-CT has 3 options 1> "max-age=<Age>" <- This is the compulsory option 2> "enforce" 3> "report-uri=<Your URI>"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Expect_CT(message: Message):
+        async def set_Expect_CT(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Expect-CT', self.PolicyString)
 
             await send(message)
 
         await self.app(scope, receive, set_Expect_CT)
```

### Comparing `Secweb-1.7.1/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py` & `Secweb-1.7.2/src/Secweb/OriginAgentCluster/OriginAgentClusterMiddleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class OriginAgentCluster:
     ''' OriginAgentCluster sets the Origin-Agent-Cluster header it takes no parameter
 
     Example :
         app.add_middleware(OriginAgentCluster)'''
-    def __init__(self, app: ASGIApp):
+    def __init__(self, app):
         self.app = app
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Origin_Agent_Cluster(message: Message):
+        async def set_Origin_Agent_Cluster(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Origin-Agent-Cluster', '?1')
 
             await send(message)
 
         await self.app(scope, receive, set_Origin_Agent_Cluster)
```

### Comparing `Secweb-1.7.1/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py` & `Secweb-1.7.2/src/Secweb/ReferrerPolicy/ReferrerPolicyMiddleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class ReferrerPolicy:
     ''' ReferrerPolicy class sets Referrer-Policy header it takes one Parameter
 
     Example:
         app.add_middleware(ReferrerPolicy, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str | list[str]] = {'Referrer-Policy': 'strict-origin-when-cross-origin'}):
+    def __init__(self, app, Option = {'Referrer-Policy': 'strict-origin-when-cross-origin'}):
         self.app = app
         Policies = ['no-referrer', 'no-referrer-when-downgrade', 'origin', 'origin-when-cross-origin', 'same-origin', 'strict-origin', 'strict-origin-when-cross-origin', 'unsafe-url']
         self.policystring = ''
         if Option['Referrer-Policy'] in Policies:
             self.policystring = Option['Referrer-Policy']
         elif len(Option['Referrer-Policy']) > 1:
             for option in Option['Referrer-Policy']:
                 if option not in Policies:
                     raise SyntaxError('Referrer-Policy has 8 options 1> "no-referrer" 2> "no-referrer-when-downgrade" 3> "origin" 4> "origin-when-cross-origin" 5> "same-origin" 6> "strict-origin" 7> "strict-origin-when-cross-origin" 8> "unsafe-url"')
             self.policystring = ', '.join(Option['Referrer-Policy'])
         else:
             raise SyntaxError('Referrer-Policy has 8 options 1> "no-referrer" 2> "no-referrer-when-downgrade" 3> "origin" 4> "origin-when-cross-origin" 5> "same-origin" 6> "strict-origin" 7> "strict-origin-when-cross-origin" 8> "unsafe-url"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Referrer_Policy(message: Message):
+        async def set_Referrer_Policy(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('Referrer-Policy', self.policystring)
 
             await send(message)
 
         await self.app(scope, receive, set_Referrer_Policy)
```

### Comparing `Secweb-1.7.1/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py` & `Secweb-1.7.2/src/Secweb/StrictTransportSecurity/StrictTransportSecurityMiddleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class HSTS:
     ''' HSTS class sets Strict-Transport-Security Header it takes one parameter
 
     Example :
         app.add_middleware(HSTS, Option={})
 
     Parameter :
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, int | bool] = {'max-age': 432000, 'includeSubDomains': True, 'preload': False}):
+    def __init__(self, app, Option = {'max-age': 432000, 'includeSubDomains': True, 'preload': False}):
         self.app = app
         self.PolicyString = ''
         if 'max-age' in Option:
             if int(Option['max-age']) and Option['max-age'] > 0:
                 self.PolicyString += 'max-age=' + str(Option['max-age'])
             else:
                 raise SyntaxError('max-age needs to be a positive integer')
@@ -33,19 +32,19 @@
 
             if 'preload' in Option and Option['preload'] is True:
                 self.PolicyString += '; preload'     
 
         else:
             raise SyntaxError('Strict-Transport-Security has 3 options 1> "max-age=<expire-time>" <- This is the compulsory option 2> "includeSubDomains" 3> "preload"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_Strict_Transport_Security(message: Message):
+        async def set_Strict_Transport_Security(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message) 
                 headers.append('Strict-Transport-Security', self.PolicyString)
 
             await send(message)
 
         await self.app(scope, receive, set_Strict_Transport_Security)
```

### Comparing `Secweb-1.7.1/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py` & `Secweb-1.7.2/src/Secweb/XContentTypeOptions/XContentTypeOptionsMiddleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class XContentTypeOptions:
     ''' XContentTypeOptions sets the X-Content-Type-Options header it takes no parameter
 
     Example :
         app.add_middleware(XContentTypeOptions)'''
-    def __init__(self, app: ASGIApp):
+    def __init__(self, app):
         self.app = app
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_Content_Type_Options(message: Message):
+        async def set_x_Content_Type_Options(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-Content-Type-Options', 'nosniff')
 
             await send(message)
 
         await self.app(scope, receive, set_x_Content_Type_Options)
```

### Comparing `Secweb-1.7.1/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py` & `Secweb-1.7.2/src/Secweb/XDNSPrefetchControl/XDNSPrefetchControlMiddleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class XDNSPrefetchControl:
     ''' XDNSPrefetchControl class sets X-DNS-Prefetch-Control header it takes one Parameter
 
     Example:
         app.add_middleware(XDNSPrefetchControl, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-DNS-Prefetch-Control': 'off'}):
+    def __init__(self, app, Option = {'X-DNS-Prefetch-Control': 'off'}):
         self.app = app
         self.Option = Option
         if self.Option['X-DNS-Prefetch-Control'] != 'on' and self.Option['X-DNS-Prefetch-Control'] != 'off':
             raise SyntaxError('X-DNS-Prefetch-Control has two values only 1> "on" 2> "off"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_DNS_Prefetch_Control(message: Message):
+        async def set_x_DNS_Prefetch_Control(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-DNS-Prefetch-Control', self.Option['X-DNS-Prefetch-Control'])
 
             await send(message)
 
         await self.app(scope, receive, set_x_DNS_Prefetch_Control)
```

### Comparing `Secweb-1.7.1/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py` & `Secweb-1.7.2/src/Secweb/XDownloadOptions/XDownloadOptionsMiddleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class XDownloadOptions:
     ''' XDownloadOptions sets the X-Download-Options header it takes no parameter
 
     Example :
         app.add_middleware(XDownloadOptions)'''
-    def __init__(self, app: ASGIApp):
+    def __init__(self, app):
         self.app = app
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_Download_Options(message: Message):
+        async def set_x_Download_Options(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-Download-Options', 'noopen')
 
             await send(message)
 
         await self.app(scope, receive, set_x_Download_Options)
```

### Comparing `Secweb-1.7.1/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py` & `Secweb-1.7.2/src/Secweb/XFrameOptions/XFrameOptionsMiddleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class XFrame:
     ''' XFrame class sets X-Frame-Options header it takes one Parameter
 
     Example:
         app.add_middleware(XFrame, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-Frame-Options': 'DENY'}):
+    def __init__(self, app, Option = {'X-Frame-Options': 'DENY'}):
         self.app = app
         self.Option = Option
         if self.Option['X-Frame-Options'] != 'SAMEORIGIN' and self.Option['X-Frame-Options'] != 'DENY':
             raise SyntaxError('X-Frame-Options has two values only 1> "DENY" 2> "SAMEORIGIN"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_Frame_Options(message: Message):
+        async def set_x_Frame_Options(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-Frame-Options', self.Option['X-Frame-Options'])
 
             await send(message)
 
         await self.app(scope, receive, set_x_Frame_Options)
```

### Comparing `Secweb-1.7.1/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py` & `Secweb-1.7.2/src/Secweb/XPermittedCrossDomainPolicies/XPermittedCrossDomainPoliciesMiddleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class XPermittedCrossDomainPolicies:
     ''' XPermittedCrossDomainPolicies class sets X-Permitted-Cross-Domain-Policies header it takes one Parameter
 
     Example:
         app.add_middleware(XPermittedCrossDomainPolicies, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-Permitted-Cross-Domain-Policies': 'none'}):
+    def __init__(self, app, Option = {'X-Permitted-Cross-Domain-Policies': 'none'}):
         self.app = app
         self.Option = Option
         Policies = ['none', 'master-only', 'by-content-type', 'all']
         if self.Option['X-Permitted-Cross-Domain-Policies'] not in Policies:
             raise SyntaxError('X-Permitted-Cross-Domain-Policies has four values 1> "none" 2> "master-only" 3> "by-content-type" 4> "all"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_Permitted_Cross_Domain_Policies(message: Message):
+        async def set_x_Permitted_Cross_Domain_Policies(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-Permitted-Cross-Domain-Policies', self.Option['X-Permitted-Cross-Domain-Policies'])
 
             await send(message)
 
         await self.app(scope, receive, set_x_Permitted_Cross_Domain_Policies)
```

### Comparing `Secweb-1.7.1/src/Secweb/index.py` & `Secweb-1.7.2/src/Secweb/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import ASGIApp
-
 from .XFrameOptions.XFrameOptionsMiddleware import XFrame
 from .CrossOriginEmbedderPolicy.CrossOriginEmbedderPolicyMiddleware import CrossOriginEmbedderPolicy
 from .CrossOriginOpenerPolicy.CrossOriginOpenerPolicyMiddleware import CrossOriginOpenerPolicy
 from .CrossOriginResourcePolicy.CrossOriginResourcePolicyMiddleware import CrossOriginResourcePolicy
 from .xXSSProtection.xXSSProtectionMiddleware import xXSSProtection
 from .StrictTransportSecurity.StrictTransportSecurityMiddleware import HSTS
 from .XPermittedCrossDomainPolicies.XPermittedCrossDomainPoliciesMiddleware import XPermittedCrossDomainPolicies
@@ -69,19 +67,19 @@
 
         'cacheControl' for Cache-Control
 
     This Values are for Option parameter"""
 
     def __init__(
         self,
-        app: ASGIApp,
-        Option: dict[str, dict[str, list[str] | str | bool | int]] = {},
-        Routes: list[str] = [],
-        script_nonce: bool = False,
-        style_nonce: bool = False,
+        app,
+        Option = {},
+        Routes = [],
+        script_nonce = False,
+        style_nonce = False,
     ) -> None:
         if not Option:
             app.add_middleware(XFrame)
             app.add_middleware(xXSSProtection)
             app.add_middleware(HSTS)
             app.add_middleware(XPermittedCrossDomainPolicies)
             app.add_middleware(XDownloadOptions)
```

### Comparing `Secweb-1.7.1/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py` & `Secweb-1.7.2/src/Secweb/xXSSProtection/xXSSProtectionMiddleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 '''  This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
   Copyright 2021-2023, Motagamwala Taha Arif Ali '''
 
-from starlette.types import Scope, Receive, Send, ASGIApp, Message
 from starlette.datastructures import MutableHeaders
 
 class xXSSProtection:
     ''' xXSSProtection class sets X-XSS-Protection header it takes one Parameter
 
     Example:
         app.add_middleware(xXSSProtection, Option={})
 
     Parameter:
 
     Option={} This is a dictionary'''
-    def __init__(self, app: ASGIApp, Option: dict[str, str] = {'X-XSS-Protection': '0'}):
+    def __init__(self, app, Option = {'X-XSS-Protection': '0'}):
         self.app = app
         self.Option = Option
         if self.Option['X-XSS-Protection'] != '0' and self.Option['X-XSS-Protection'] != '1' and self.Option['X-XSS-Protection'] != '1; mode=block' and '1; report=' not in self.Option['X-XSS-Protection']:
             raise SyntaxError('X-XSS-Protection has 4 options 1> "0" 2> "1" 3> "1; mode=block" 4> "1; report=<Your Reporting Uri>"')
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(self, scope, receive, send):
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
-        async def set_x_XSS_Protection(message: Message):
+        async def set_x_XSS_Protection(message):
             if message["type"] == "http.response.start":
                 headers = MutableHeaders(scope=message)
                 headers.append('X-XSS-Protection', self.Option['X-XSS-Protection'])
 
             await send(message)
 
         await self.app(scope, receive, set_x_XSS_Protection)
```

### Comparing `Secweb-1.7.1/src/Secweb.egg-info/PKG-INFO` & `Secweb-1.7.2/src/Secweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Secweb
-Version: 1.7.1
+Version: 1.7.2
 Summary: Secweb is a pack of security middlewares for fastApi and starlette server it includes CSP, HSTS, and many more
 Author-email: Motagamwala Taha Arif Ali <tahaar5321@gmail.com>
 Project-URL: Homepage, https://github.com/tmotagam/Secweb
 Project-URL: Bug Tracker, https://github.com/tmotagam/Secweb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `Secweb-1.7.1/src/Secweb.egg-info/SOURCES.txt` & `Secweb-1.7.2/src/Secweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

