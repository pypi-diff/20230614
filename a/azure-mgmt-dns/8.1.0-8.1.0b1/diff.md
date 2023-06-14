# Comparing `tmp/azure-mgmt-dns-8.1.0.zip` & `tmp/azure-mgmt-dns-8.1.0b1.zip`

## zipinfo {}

```diff
@@ -1,153 +1,122 @@
-Zip file size: 230263 bytes, number of entries: 151
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/
--rw-rw-r--  2.0 unx     2116 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/README.md
--rw-rw-r--  2.0 unx     2845 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/setup.py
--rw-rw-r--  2.0 unx      614 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/_meta.json
--rw-rw-r--  2.0 unx       38 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/setup.cfg
--rw-rw-r--  2.0 unx     7394 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/CHANGELOG.md
--rw-rw-r--  2.0 unx      209 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/MANIFEST.in
--rw-rw-r--  2.0 unx    10402 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/PKG-INFO
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/LICENSE
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/tests/recordings/
--rw-rw-r--  2.0 unx     2801 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/tests/conftest.py
--rw-rw-r--  2.0 unx     8830 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/tests/test_mgmt_dns.py
--rw-rw-r--  2.0 unx    35653 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      124 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     6019 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx    10402 b- defN 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/
--rw-rw-r--  2.0 unx       65 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/
--rw-rw-r--  2.0 unx      360 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/models.py
--rw-rw-r--  2.0 unx    78854 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/_serialization.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/py.typed
--rw-rw-r--  2.0 unx      713 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/__init__.py
--rw-rw-r--  2.0 unx     9800 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/_dns_management_client.py
--rw-rw-r--  2.0 unx      345 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/_version.py
--rw-rw-r--  2.0 unx     3221 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_vendor.py
--rw-rw-r--  2.0 unx      897 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_patch.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_version.py
--rw-rw-r--  2.0 unx     3489 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_configuration.py
--rw-rw-r--  2.0 unx    42836 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py
--rw-rw-r--  2.0 unx    56318 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py
--rw-rw-r--  2.0 unx     4542 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py
--rw-rw-r--  2.0 unx     3537 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx    34180 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    43424 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py
--rw-rw-r--  2.0 unx    31627 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx     1961 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py
--rw-rw-r--  2.0 unx      952 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_vendor.py
--rw-rw-r--  2.0 unx      897 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_patch.py
--rw-rw-r--  2.0 unx     4340 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_dns_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_version.py
--rw-rw-r--  2.0 unx     3473 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_configuration.py
--rw-rw-r--  2.0 unx    34256 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_patch.py
--rw-rw-r--  2.0 unx    49213 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_patch.py
--rw-rw-r--  2.0 unx     4480 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py
--rw-rw-r--  2.0 unx     3521 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_configuration.py
--rw-rw-r--  2.0 unx    27319 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    38008 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py
--rw-rw-r--  2.0 unx    32234 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     2081 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_patch.py
--rw-rw-r--  2.0 unx     3016 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py
--rw-rw-r--  2.0 unx      558 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/__init__.py
--rw-rw-r--  2.0 unx     9993 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_dns_management_client.py
--rw-rw-r--  2.0 unx     3285 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_configuration.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_vendor.py
--rw-rw-r--  2.0 unx      897 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_patch.py
--rw-rw-r--  2.0 unx     5153 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_dns_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_version.py
--rw-rw-r--  2.0 unx     3489 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_configuration.py
--rw-rw-r--  2.0 unx    43023 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_zones_operations.py
--rw-rw-r--  2.0 unx     8786 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dns_resource_reference_operations.py
--rw-rw-r--  2.0 unx    27953 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dnssec_configs_operations.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_patch.py
--rw-rw-r--  2.0 unx    56526 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_record_sets_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_patch.py
--rw-rw-r--  2.0 unx     5306 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_dns_management_client.py
--rw-rw-r--  2.0 unx     3537 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx    34367 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_zones_operations.py
--rw-rw-r--  2.0 unx     7529 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dns_resource_reference_operations.py
--rw-rw-r--  2.0 unx    22299 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dnssec_configs_operations.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    43632 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_record_sets_operations.py
--rw-rw-r--  2.0 unx    56075 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx     2746 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_patch.py
--rw-rw-r--  2.0 unx     1239 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_dns_management_client_enums.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/
--rw-rw-r--  2.0 unx     1302 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_vendor.py
--rw-rw-r--  2.0 unx      897 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_patch.py
--rw-rw-r--  2.0 unx     4795 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_dns_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_version.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_configuration.py
--rw-rw-r--  2.0 unx    41776 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py
--rw-rw-r--  2.0 unx     8686 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_patch.py
--rw-rw-r--  2.0 unx    54976 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-14 01:49 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_patch.py
--rw-rw-r--  2.0 unx     4939 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_dns_management_client.py
--rw-rw-r--  2.0 unx     3588 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_configuration.py
--rw-rw-r--  2.0 unx    33489 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_zones_operations.py
--rw-rw-r--  2.0 unx     7451 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_dns_resource_reference_operations.py
--rw-rw-r--  2.0 unx      980 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    42566 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_record_sets_operations.py
--rw-rw-r--  2.0 unx    33746 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     2145 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_patch.py
--rw-rw-r--  2.0 unx      952 b- defN 23-Jun-14 01:48 azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_dns_management_client_enums.py
-151 files, 1224490 bytes uncompressed, 198859 bytes compressed:  83.8%
+Zip file size: 175398 bytes, number of entries: 120
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/tests/
+-rw-rw-r--  2.0 unx     2812 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/setup.py
+-rw-rw-r--  2.0 unx     2087 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/README.md
+-rw-rw-r--  2.0 unx    10015 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx     7047 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/LICENSE
+-rw-rw-r--  2.0 unx      209 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx       38 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/setup.cfg
+-rw-rw-r--  2.0 unx      614 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/_meta.json
+-rw-rw-r--  2.0 unx      116 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    10015 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     4409 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/dependency_links.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/
+-rw-rw-r--  2.0 unx       65 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/
+-rw-rw-r--  2.0 unx     7811 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_dns_management_client.py
+-rw-rw-r--  2.0 unx      495 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_version.py
+-rw-rw-r--  2.0 unx    78842 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_serialization.py
+-rw-rw-r--  2.0 unx      713 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/__init__.py
+-rw-rw-r--  2.0 unx      360 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/models.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/py.typed
+-rw-rw-r--  2.0 unx     3221 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_configuration.py
+-rw-rw-r--  2.0 unx     7967 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_dns_management_client.py
+-rw-rw-r--  2.0 unx      558 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/__init__.py
+-rw-rw-r--  2.0 unx     3285 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_configuration.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/
+-rw-rw-r--  2.0 unx     4712 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_dns_management_client.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_version.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_patch.py
+-rw-rw-r--  2.0 unx      897 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_vendor.py
+-rw-rw-r--  2.0 unx     3789 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_configuration.py
+-rw-rw-r--  2.0 unx    33746 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx      952 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_dns_management_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_patch.py
+-rw-rw-r--  2.0 unx     2145 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/
+-rw-rw-r--  2.0 unx     4851 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_dns_management_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_patch.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     3837 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx    42460 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx     7535 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_dns_resource_reference_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    33413 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_zones_operations.py
+-rw-rw-r--  2.0 unx    54996 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx     8788 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_patch.py
+-rw-rw-r--  2.0 unx      980 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/__init__.py
+-rw-rw-r--  2.0 unx    41808 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/
+-rw-rw-r--  2.0 unx     4295 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_version.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_patch.py
+-rw-rw-r--  2.0 unx      897 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_vendor.py
+-rw-rw-r--  2.0 unx     3746 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_configuration.py
+-rw-rw-r--  2.0 unx    31627 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py
+-rw-rw-r--  2.0 unx      952 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py
+-rw-rw-r--  2.0 unx     1961 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/
+-rw-rw-r--  2.0 unx     4430 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py
+-rw-rw-r--  2.0 unx    43374 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    34160 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py
+-rw-rw-r--  2.0 unx    56548 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py
+-rw-rw-r--  2.0 unx    43056 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/
+-rw-rw-r--  2.0 unx     4271 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_dns_management_client.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_version.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_patch.py
+-rw-rw-r--  2.0 unx      897 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/__init__.py
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_vendor.py
+-rw-rw-r--  2.0 unx     3722 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_configuration.py
+-rw-rw-r--  2.0 unx    32210 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     2985 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_patch.py
+-rw-rw-r--  2.0 unx     2081 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/
+-rw-rw-r--  2.0 unx     4406 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_patch.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     3770 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx    37935 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    27276 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py
+-rw-rw-r--  2.0 unx    49248 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_patch.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/__init__.py
+-rw-rw-r--  2.0 unx    34303 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-13 05:57 azure-mgmt-dns-8.1.0b1/tests/recordings/
+-rw-rw-r--  2.0 unx     2801 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/tests/conftest.py
+-rw-rw-r--  2.0 unx     8830 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/tests/test_mgmt_dns.py
+-rw-rw-r--  2.0 unx    35674 b- defN 23-Feb-13 05:56 azure-mgmt-dns-8.1.0b1/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json
+120 files, 888454 bytes uncompressed, 150764 bytes compressed:  83.0%
```

## zipnote {}

```diff
@@ -1,454 +1,361 @@
-Filename: azure-mgmt-dns-8.1.0/
+Filename: azure-mgmt-dns-8.1.0b1/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/tests/
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/
+Filename: azure-mgmt-dns-8.1.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/
+Filename: azure-mgmt-dns-8.1.0b1/tests/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/README.md
+Filename: azure-mgmt-dns-8.1.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/setup.py
+Filename: azure-mgmt-dns-8.1.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/_meta.json
+Filename: azure-mgmt-dns-8.1.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/setup.cfg
+Filename: azure-mgmt-dns-8.1.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/CHANGELOG.md
+Filename: azure-mgmt-dns-8.1.0b1/LICENSE
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/MANIFEST.in
+Filename: azure-mgmt-dns-8.1.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/PKG-INFO
+Filename: azure-mgmt-dns-8.1.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/LICENSE
+Filename: azure-mgmt-dns-8.1.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/tests/recordings/
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/tests/conftest.py
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/tests/test_mgmt_dns.py
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/not-zip-safe
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/top_level.txt
+Filename: azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/requires.txt
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/dependency_links.txt
+Filename: azure-mgmt-dns-8.1.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/SOURCES.txt
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/PKG-INFO
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_version.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_serialization.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/models.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/models.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/py.typed
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/_serialization.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/py.typed
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/_version.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_version.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_vendor.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_version.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_dns_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_dns_resource_reference_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_vendor.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_version.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_version.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_models_py3.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_version.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_vendor.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_vendor.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_version.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dns_resource_reference_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dnssec_configs_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_dns_management_client.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_configuration.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_zones_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_patch.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dns_resource_reference_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dnssec_configs_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/__init__.py
+Filename: azure-mgmt-dns-8.1.0b1/tests/recordings/
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_patch.py
+Filename: azure-mgmt-dns-8.1.0b1/tests/conftest.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_record_sets_operations.py
+Filename: azure-mgmt-dns-8.1.0b1/tests/test_mgmt_dns.py
 Comment: 
 
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_models_py3.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_dns_management_client_enums.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_vendor.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_dns_management_client.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_version.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/_configuration.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_dns_management_client.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/_configuration.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_zones_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_dns_resource_reference_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/_record_sets_operations.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_models_py3.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/__init__.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_patch.py
-Comment: 
-
-Filename: azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_dns_management_client_enums.py
+Filename: azure-mgmt-dns-8.1.0b1/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-dns-8.1.0/README.md` & `azure-mgmt-dns-8.1.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,16 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DnsManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-Code samples for this package can be found at:
-- [Search DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
-- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+Code samples for this package can be found at [DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
```

## Comparing `azure-mgmt-dns-8.1.0/setup.py` & `azure-mgmt-dns-8.1.0b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 #!/usr/bin/env python
 
-# -------------------------------------------------------------------------
+#-------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
-# --------------------------------------------------------------------------
+#--------------------------------------------------------------------------
 
 import re
 import os.path
 from io import open
 from setuptools import find_packages, setup
 
 # Change the PACKAGE_NAME only to change folder and different name
 PACKAGE_NAME = "azure-mgmt-dns"
 PACKAGE_PPRINT_NAME = "DNS Management"
 
 # a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace("-", "/")
+package_folder_path = PACKAGE_NAME.replace('-', '/')
 # a-b-c => a.b.c
-namespace_name = PACKAGE_NAME.replace("-", ".")
+namespace_name = PACKAGE_NAME.replace('-', '.')
 
 # Version extraction inspired from 'requests'
-with open(
-    os.path.join(package_folder_path, "version.py")
-    if os.path.exists(os.path.join(package_folder_path, "version.py"))
-    else os.path.join(package_folder_path, "_version.py"),
-    "r",
-) as fd:
-    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
+with open(os.path.join(package_folder_path, 'version.py')
+          if os.path.exists(os.path.join(package_folder_path, 'version.py'))
+          else os.path.join(package_folder_path, '_version.py'), 'r') as fd:
+    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
+                        fd.read(), re.MULTILINE).group(1)
 
 if not version:
-    raise RuntimeError("Cannot find version information")
+    raise RuntimeError('Cannot find version information')
 
-with open("README.md", encoding="utf-8") as f:
+with open('README.md', encoding='utf-8') as f:
     readme = f.read()
-with open("CHANGELOG.md", encoding="utf-8") as f:
+with open('CHANGELOG.md', encoding='utf-8') as f:
     changelog = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=version,
-    description="Microsoft Azure {} Client Library for Python".format(PACKAGE_PPRINT_NAME),
-    long_description=readme + "\n\n" + changelog,
-    long_description_content_type="text/markdown",
-    license="MIT License",
-    author="Microsoft Corporation",
-    author_email="azpysdkhelp@microsoft.com",
-    url="https://github.com/Azure/azure-sdk-for-python",
+    description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
+    long_description=readme + '\n\n' + changelog,
+    long_description_content_type='text/markdown',
+    license='MIT License',
+    author='Microsoft Corporation',
+    author_email='azpysdkhelp@microsoft.com',
+    url='https://github.com/Azure/azure-sdk-for-python',
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
+        'Development Status :: 4 - Beta',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
-    packages=find_packages(
-        exclude=[
-            "tests",
-            # Exclude packages that will be covered by PEP420 or nspkg
-            "azure",
-            "azure.mgmt",
-        ]
-    ),
+    packages=find_packages(exclude=[
+        'tests',
+        # Exclude packages that will be covered by PEP420 or nspkg
+        'azure',
+        'azure.mgmt',
+    ]),
     include_package_data=True,
     package_data={
-        "pytyped": ["py.typed"],
+        'pytyped': ['py.typed'],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
+        "msrest>=0.7.1",
         "azure-common~=1.1",
         "azure-mgmt-core>=1.3.2,<2.0.0",
         "typing-extensions>=4.3.0; python_version<'3.8.0'",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.7"
 )
```

## Comparing `azure-mgmt-dns-8.1.0/_meta.json` & `azure-mgmt-dns-8.1.0b1/_meta.json`

 * *Files 8% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7777777777777777%*

 * *Differences: {"'autorest_command'": "'autorest specification/dns/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.4.0 --use=@autorest/modelerfour@4.24.3 '*

 * *                       "--version=3.9.2 --version-tolerant=False'",*

 * * "'commit'": "'c4eb7d4facbb9312f435df8c8ffe5061bfb02890'",*

 * * "'use'": "{insert: [(0 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.2",
-    "autorest_command": "autorest specification/dns/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.6.0 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
-    "commit": "e2b5f9323c4214408969a6e953b4075cfdc693b6",
+    "autorest_command": "autorest specification/dns/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.4.0 --use=@autorest/modelerfour@4.24.3 --version=3.9.2 --version-tolerant=False",
+    "commit": "c4eb7d4facbb9312f435df8c8ffe5061bfb02890",
     "readme": "specification/dns/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.6.0",
+        "@autorest/python@6.4.0",
         "@autorest/modelerfour@4.24.3"
     ]
 }
```

## Comparing `azure-mgmt-dns-8.1.0/CHANGELOG.md` & `azure-mgmt-dns-8.1.0b1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,9 @@
 # Release History
 
-## 8.1.0 (2023-06-14)
-
-### Features Added
-
-  - Added operation group DnssecConfigsOperations
-  - Model RecordSet has a new parameter ds_records
-  - Model RecordSet has a new parameter naptr_records
-  - Model RecordSet has a new parameter tlsa_records
-  - Model Zone has a new parameter signing_keys
-  - Model Zone has a new parameter system_data
-
 ## 8.1.0b1 (2023-02-10)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-dns-8.1.0/PKG-INFO` & `azure-mgmt-dns-8.1.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-dns
-Version: 8.1.0
+Version: 8.1.0b1
 Summary: Microsoft Azure DNS Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -64,17 +64,16 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DnsManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-Code samples for this package can be found at:
-- [Search DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
-- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+Code samples for this package can be found at [DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -85,25 +84,14 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-dns%2FREADME.png)
 
 
 # Release History
 
-## 8.1.0 (2023-06-14)
-
-### Features Added
-
-  - Added operation group DnssecConfigsOperations
-  - Model RecordSet has a new parameter ds_records
-  - Model RecordSet has a new parameter naptr_records
-  - Model RecordSet has a new parameter tlsa_records
-  - Model Zone has a new parameter signing_keys
-  - Model Zone has a new parameter system_data
-
 ## 8.1.0b1 (2023-02-10)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-dns-8.1.0/LICENSE` & `azure-mgmt-dns-8.1.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/tests/conftest.py` & `azure-mgmt-dns-8.1.0b1/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/tests/test_mgmt_dns.py` & `azure-mgmt-dns-8.1.0b1/tests/test_mgmt_dns.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json` & `azure-mgmt-dns-8.1.0b1/tests/recordings/test_mgmt_dns.pyTestMgmtDnstest_public_zone.json`

 * *Files 7% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9938258765044479%*

 * *Differences: {"'Entries'": "{0: {'RequestHeaders': {'User-Agent': 'azsdk-python-identity/1.13.0b3 Python/3.8.16 "*

 * *              '(Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) '*

 * *              "VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0'}, 'ResponseHeaders': "*

 * *              "{'Date': 'Fri, 10 Feb 2023 08:09:02 GMT', 'x-ms-ests-server': '2.1.14601.9 - NCUS "*

 * *              "ProdSlices'}}, 1: {'RequestHeaders': {'User-Agent': 'azsdk-python-identity/1.13.0b3 "*

 * *              'Python/3.8.16 (Linux-5.15.0-1031-azu […]*

```diff
@@ -2,15 +2,15 @@
     "Entries": [
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "*/*",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-identity/1.14.0b2 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-identity/1.13.0b3 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://login.microsoftonline.com/00000000-0000-0000-0000-000000000000/v2.0/.well-known/openid-configuration",
             "ResponseBody": {
                 "authorization_endpoint": "https://login.microsoftonline.com/00000000-0000-0000-0000-000000000000/oauth2/v2.0/authorize",
                 "claims_supported": [
                     "sub",
@@ -79,32 +79,32 @@
             },
             "ResponseHeaders": {
                 "Access-Control-Allow-Methods": "GET, OPTIONS",
                 "Access-Control-Allow-Origin": "*",
                 "Cache-Control": "max-age=86400, private",
                 "Content-Length": "1753",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:36 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:02 GMT",
                 "P3P": "CP=\"DSP CUR OTPi IND OTRi ONL FIN\"",
                 "Set-Cookie": "[set-cookie;]",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-XSS-Protection": "0",
-                "x-ms-ests-server": "2.1.15620.8 - EUS ProdSlices"
+                "x-ms-ests-server": "2.1.14601.9 - NCUS ProdSlices"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Cookie": "cookie;",
-                "User-Agent": "azsdk-python-identity/1.14.0b2 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-identity/1.13.0b3 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://login.microsoftonline.com/common/discovery/instance?api-version=1.1&authorization_endpoint=https://login.microsoftonline.com/common/oauth2/authorize",
             "ResponseBody": {
                 "api-version": "1.1",
                 "metadata": [
                     {
@@ -152,41 +152,41 @@
             },
             "ResponseHeaders": {
                 "Access-Control-Allow-Methods": "GET, OPTIONS",
                 "Access-Control-Allow-Origin": "*",
                 "Cache-Control": "max-age=86400, private",
                 "Content-Length": "945",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:36 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:02 GMT",
                 "P3P": "CP=\"DSP CUR OTPi IND OTRi ONL FIN\"",
                 "Set-Cookie": "[set-cookie;]",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-XSS-Protection": "0",
-                "x-ms-ests-server": "2.1.15482.18 - NCUS ProdSlices"
+                "x-ms-ests-server": "2.1.14601.8 - SCUS ProdSlices"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": "client_id=00000000-0000-0000-0000-000000000000&grant_type=client_credentials&client_info=1&client_secret=00000000-0000-0000-0000-000000000000&claims=%7B%22access_token%22%3A+%7B%22xms_cc%22%3A+%7B%22values%22%3A+%5B%22CP1%22%5D%7D%7D%7D&scope=https%3A%2F%2Fmanagement.azure.com%2F.default",
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "288",
                 "Content-Type": "application/x-www-form-urlencoded",
                 "Cookie": "cookie;",
-                "User-Agent": "azsdk-python-identity/1.14.0b2 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0",
-                "client-request-id": "73e10d31-80b7-4b62-a447-3411476959f4",
+                "User-Agent": "azsdk-python-identity/1.13.0b3 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0",
+                "client-request-id": "0bf74bd6-cc01-4558-94ac-b10fb54af9d8",
                 "x-client-cpu": "x64",
                 "x-client-current-telemetry": "4|730,0|",
                 "x-client-last-telemetry": "4|0|||",
                 "x-client-os": "linux",
                 "x-client-sku": "MSAL.Python",
-                "x-client-ver": "1.22.0",
+                "x-client-ver": "1.21.0",
                 "x-ms-lib-capability": "retry-after, h429"
             },
             "RequestMethod": "POST",
             "RequestUri": "https://login.microsoftonline.com/00000000-0000-0000-0000-000000000000/oauth2/v2.0/token",
             "ResponseBody": {
                 "access_token": "access_token",
                 "expires_in": 86399,
@@ -194,25 +194,25 @@
                 "refresh_in": 43199,
                 "token_type": "Bearer"
             },
             "ResponseHeaders": {
                 "Cache-Control": "no-store, no-cache",
                 "Content-Length": "114",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:36 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:03 GMT",
                 "Expires": "-1",
                 "P3P": "CP=\"DSP CUR OTPi IND OTRi ONL FIN\"",
                 "Pragma": "no-cache",
                 "Set-Cookie": "[set-cookie;]",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-XSS-Protection": "0",
-                "client-request-id": "73e10d31-80b7-4b62-a447-3411476959f4",
+                "client-request-id": "0bf74bd6-cc01-4558-94ac-b10fb54af9d8",
                 "x-ms-clitelem": "1,0,0,,",
-                "x-ms-ests-server": "2.1.15620.8 - SCUS ProdSlices"
+                "x-ms-ests-server": "2.1.14601.9 - SCUS ProdSlices"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": {
                 "location": "global",
                 "properties": {
@@ -221,20 +221,20 @@
             },
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "60",
                 "Content-Type": "application/json",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "PUT",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e?api-version=2018-05-01",
             "ResponseBody": {
-                "etag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                "etag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                 "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e",
                 "location": "global",
                 "name": "pydns.comcec6214e",
                 "properties": {
                     "maxNumberOfRecordSets": 10000,
                     "maxNumberOfRecordsPerRecordSet": null,
                     "nameServers": [
@@ -249,38 +249,38 @@
                 "tags": {},
                 "type": "Microsoft.Network/dnszones"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Length": "526",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:42 GMT",
-                "ETag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                "Date": "Fri, 10 Feb 2023 08:09:08 GMT",
+                "ETag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "fd6b09aa-cca1-4c62-bfd2-51161a11b872",
+                "x-ms-correlation-request-id": "3743de26-295b-47e7-b48c-c776c2e1a69e",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "11999",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094042Z:fd6b09aa-cca1-4c62-bfd2-51161a11b872"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080908Z:3743de26-295b-47e7-b48c-c776c2e1a69e"
             },
             "StatusCode": 201
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e?api-version=2018-05-01",
             "ResponseBody": {
-                "etag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                "etag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                 "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e",
                 "location": "global",
                 "name": "pydns.comcec6214e",
                 "properties": {
                     "maxNumberOfRecordSets": 10000,
                     "maxNumberOfRecordsPerRecordSet": null,
                     "nameServers": [
@@ -295,42 +295,42 @@
                 "tags": {},
                 "type": "Microsoft.Network/dnszones"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:42 GMT",
-                "ETag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                "Date": "Fri, 10 Feb 2023 08:09:08 GMT",
+                "ETag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "7fc7264c-60ae-4cbc-b783-17682c213517",
+                "x-ms-correlation-request-id": "228d9ee3-1ce6-4cef-8e49-fa7aa192eb32",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "499",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094042Z:7fc7264c-60ae-4cbc-b783-17682c213517"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080908Z:228d9ee3-1ce6-4cef-8e49-fa7aa192eb32"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones?api-version=2018-05-01",
             "ResponseBody": {
                 "value": [
                     {
-                        "etag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                        "etag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e",
                         "location": "global",
                         "name": "pydns.comcec6214e",
                         "properties": {
                             "maxNumberOfRecordSets": 10000,
                             "maxNumberOfRecordsPerRecordSet": null,
                             "nameServers": [
@@ -347,42 +347,42 @@
                     }
                 ]
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:42 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:08 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "4ee4662d-3ac4-48dd-810d-0ab7cee8a9bc",
+                "x-ms-correlation-request-id": "7794e8f4-bc35-4e25-917b-f0fe7b9037ba",
                 "x-ms-ratelimit-remaining-subscription-resource-entities-read": "59999",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "498",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094042Z:4ee4662d-3ac4-48dd-810d-0ab7cee8a9bc"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080908Z:7794e8f4-bc35-4e25-917b-f0fe7b9037ba"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.Network/dnszones?api-version=2018-05-01",
             "ResponseBody": {
                 "value": [
                     {
-                        "etag": "0f5f3990-c333-4114-8793-4ef0c9d5381b",
+                        "etag": "cae4c818-319e-4294-8d48-be5a7a210ddd",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e",
                         "location": "global",
                         "name": "pydns.comcec6214e",
                         "properties": {
                             "maxNumberOfRecordSets": 10000,
                             "maxNumberOfRecordsPerRecordSet": null,
                             "nameServers": [
@@ -399,25 +399,25 @@
                     }
                 ]
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:42 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:08 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "79de49d3-774c-4071-b756-aa3935fe691e",
+                "x-ms-correlation-request-id": "875aa9cc-6dea-4f7e-9cdc-3c371b0b8053",
                 "x-ms-ratelimit-remaining-subscription-resource-entities-read": "59998",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "497",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094042Z:79de49d3-774c-4071-b756-aa3935fe691e"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080909Z:875aa9cc-6dea-4f7e-9cdc-3c371b0b8053"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": {
                 "properties": {
                     "ARecords": [
@@ -430,20 +430,20 @@
             },
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "70",
                 "Content-Type": "application/json",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "PUT",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/A/record_setcec6214e?api-version=2018-05-01",
             "ResponseBody": {
-                "etag": "cc5b4959-0407-4862-9816-628a11b4fa53",
+                "etag": "e3daadc5-7ca8-49ac-aace-576ffee6de60",
                 "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/A/record_setcec6214e",
                 "name": "record_setcec6214e",
                 "properties": {
                     "ARecords": [
                         {
                             "ipv4Address": "1.2.3.4"
                         }
@@ -455,23 +455,23 @@
                 },
                 "type": "Microsoft.Network/dnszones/A"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Length": "447",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:43 GMT",
-                "ETag": "cc5b4959-0407-4862-9816-628a11b4fa53",
+                "Date": "Fri, 10 Feb 2023 08:09:09 GMT",
+                "ETag": "e3daadc5-7ca8-49ac-aace-576ffee6de60",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "e97d223d-1cb7-4b68-9ae4-f0600d764ad5",
+                "x-ms-correlation-request-id": "4ece4744-fa1d-4fb3-b3cc-5bbb82a2f09e",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "11999",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094043Z:e97d223d-1cb7-4b68-9ae4-f0600d764ad5"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080909Z:4ece4744-fa1d-4fb3-b3cc-5bbb82a2f09e"
             },
             "StatusCode": 201
         },
         {
             "RequestBody": {
                 "properties": {
                     "ARecords": [
@@ -487,20 +487,20 @@
             },
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "98",
                 "Content-Type": "application/json",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "PATCH",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/A/record_setcec6214e?api-version=2018-05-01",
             "ResponseBody": {
-                "etag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                "etag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                 "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/A/record_setcec6214e",
                 "name": "record_setcec6214e",
                 "properties": {
                     "ARecords": [
                         {
                             "ipv4Address": "1.2.3.4"
                         },
@@ -515,40 +515,40 @@
                 },
                 "type": "Microsoft.Network/dnszones/A"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:43 GMT",
-                "ETag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                "Date": "Fri, 10 Feb 2023 08:09:09 GMT",
+                "ETag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "db4519d7-c1ad-4ddc-9a32-b9b8346f60a9",
+                "x-ms-correlation-request-id": "2175920f-8aa2-4318-91c8-7d915c6c7017",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "11998",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094043Z:db4519d7-c1ad-4ddc-9a32-b9b8346f60a9"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080910Z:2175920f-8aa2-4318-91c8-7d915c6c7017"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/A/record_setcec6214e?api-version=2018-05-01",
             "ResponseBody": {
-                "etag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                "etag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                 "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/A/record_setcec6214e",
                 "name": "record_setcec6214e",
                 "properties": {
                     "ARecords": [
                         {
                             "ipv4Address": "1.2.3.4"
                         },
@@ -563,42 +563,42 @@
                 },
                 "type": "Microsoft.Network/dnszones/A"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:43 GMT",
-                "ETag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                "Date": "Fri, 10 Feb 2023 08:09:10 GMT",
+                "ETag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "f87e0738-1a4b-45bb-b49c-56fba0281dfd",
+                "x-ms-correlation-request-id": "97d1106b-413a-4fbd-ace5-4c590a76780a",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "499",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094043Z:f87e0738-1a4b-45bb-b49c-56fba0281dfd"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080910Z:97d1106b-413a-4fbd-ace5-4c590a76780a"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/A?api-version=2018-05-01",
             "ResponseBody": {
                 "value": [
                     {
-                        "etag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                        "etag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/A/record_setcec6214e",
                         "name": "record_setcec6214e",
                         "properties": {
                             "ARecords": [
                                 {
                                     "ipv4Address": "1.2.3.4"
                                 },
@@ -615,42 +615,42 @@
                     }
                 ]
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:44 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:10 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "655aea6b-2678-4ccb-a9aa-8c5d06264a05",
+                "x-ms-correlation-request-id": "464ec7d3-f1ab-4bfd-bb7b-7f77f7817cdf",
                 "x-ms-ratelimit-remaining-subscription-resource-entities-read": "59999",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "498",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094044Z:655aea6b-2678-4ccb-a9aa-8c5d06264a05"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080910Z:464ec7d3-f1ab-4bfd-bb7b-7f77f7817cdf"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/recordsets?api-version=2018-05-01",
             "ResponseBody": {
                 "value": [
                     {
-                        "etag": "4f3ac8da-2d8e-4fcc-a84b-7f8da02092e5",
+                        "etag": "13585b96-95a0-4b02-802c-c116715127a3",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/NS/@",
                         "name": "@",
                         "properties": {
                             "NSRecords": [
                                 {
                                     "nsdname": "ns1-36.azure-dns.com."
                                 },
@@ -668,15 +668,15 @@
                             "fqdn": "pydns.comcec6214e.",
                             "provisioningState": "Succeeded",
                             "targetResource": {}
                         },
                         "type": "Microsoft.Network/dnszones/NS"
                     },
                     {
-                        "etag": "c32d5ed1-d4b0-4663-b7ad-0b4aee9b78ee",
+                        "etag": "41b6bf9f-f07c-4ff0-bc17-e0d41c8a208d",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/SOA/@",
                         "name": "@",
                         "properties": {
                             "SOARecord": {
                                 "email": "azuredns-hostmaster.microsoft.com",
                                 "expireTime": 2419200,
                                 "host": "ns1-36.azure-dns.com.",
@@ -689,15 +689,15 @@
                             "fqdn": "pydns.comcec6214e.",
                             "provisioningState": "Succeeded",
                             "targetResource": {}
                         },
                         "type": "Microsoft.Network/dnszones/SOA"
                     },
                     {
-                        "etag": "d8ef43ef-2ee3-4d6c-9050-18fdff3f72c5",
+                        "etag": "2de66656-6a01-4cd8-aef5-38f973c4ab52",
                         "id": "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnszones/pydns.comcec6214e/A/record_setcec6214e",
                         "name": "record_setcec6214e",
                         "properties": {
                             "ARecords": [
                                 {
                                     "ipv4Address": "1.2.3.4"
                                 },
@@ -714,109 +714,109 @@
                     }
                 ]
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:44 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:10 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "a1ebf558-1fc7-466a-82d3-20323473f854",
+                "x-ms-correlation-request-id": "4399b1af-a6af-41d7-bf25-4b148565886d",
                 "x-ms-ratelimit-remaining-subscription-resource-entities-read": "59997",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "499",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094044Z:a1ebf558-1fc7-466a-82d3-20323473f854"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080910Z:4399b1af-a6af-41d7-bf25-4b148565886d"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "0",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "DELETE",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e/A/record_setcec6214e?api-version=2018-05-01",
             "ResponseBody": null,
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Length": "0",
-                "Date": "Tue, 13 Jun 2023 09:40:44 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:11 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "78406cd4-8ff8-44c3-8e5f-061ad627f5be",
+                "x-ms-correlation-request-id": "c27aa8e8-7706-479e-a66d-6cd869e21f12",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "11999",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094044Z:78406cd4-8ff8-44c3-8e5f-061ad627f5be"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080911Z:c27aa8e8-7706-479e-a66d-6cd869e21f12"
             },
             "StatusCode": 200
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 "Content-Length": "0",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "DELETE",
             "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsZones/pydns.comcec6214e?api-version=2018-05-01",
             "ResponseBody": null,
             "ResponseHeaders": {
-                "Azure-AsyncOperation": "https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationStatuses/00000000-0000-0000-0000-000000000024;1131565;pydns.comcec6214e;Regular?api-version=2018-05-01",
+                "Azure-AsyncOperation": "https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationStatuses/00000000-0000-0000-0000-000000000024;926653;pydns.comcec6214e;Regular?api-version=2018-05-01",
                 "Cache-Control": "private",
                 "Content-Length": "0",
-                "Date": "Tue, 13 Jun 2023 09:40:48 GMT",
-                "Location": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationResults/00000000-0000-0000-0000-000000000024;1131565;pydns.comcec6214e;Regular?api-version=2018-05-01",
+                "Date": "Fri, 10 Feb 2023 08:09:15 GMT",
+                "Location": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationResults/00000000-0000-0000-0000-000000000024;926653;pydns.comcec6214e;Regular?api-version=2018-05-01",
                 "Retry-After": "3",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "cae6f1f8-5355-4d8b-8e73-f240a77793d5",
+                "x-ms-correlation-request-id": "5ba79871-950e-496e-acc8-4b93211edc6c",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "11999",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094049Z:cae6f1f8-5355-4d8b-8e73-f240a77793d5"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080915Z:5ba79871-950e-496e-acc8-4b93211edc6c"
             },
             "StatusCode": 202
         },
         {
             "RequestBody": null,
             "RequestHeaders": {
                 "Accept": "*/*",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
-                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0 Python/3.8.16 (Linux-5.15.0-1038-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
+                "User-Agent": "azsdk-python-azure-mgmt-dns/8.1.0b1 Python/3.8.16 (Linux-5.15.0-1031-azure-x86_64-with-glibc2.2.5) VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2500_0"
             },
             "RequestMethod": "GET",
-            "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationStatuses/00000000-0000-0000-0000-000000000024;1131565;pydns.comcec6214e;Regular?api-version=2018-05-01",
+            "RequestUri": "https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/cec6214e/providers/Microsoft.Network/dnsOperationStatuses/00000000-0000-0000-0000-000000000024;926653;pydns.comcec6214e;Regular?api-version=2018-05-01",
             "ResponseBody": {
                 "status": "Succeeded"
             },
             "ResponseHeaders": {
                 "Cache-Control": "private",
                 "Content-Encoding": "gzip",
                 "Content-Type": "application/json; charset=utf-8",
-                "Date": "Tue, 13 Jun 2023 09:40:48 GMT",
+                "Date": "Fri, 10 Feb 2023 08:09:15 GMT",
                 "Server": "Microsoft-IIS/10.0",
                 "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
                 "Transfer-Encoding": "chunked",
                 "Vary": "Accept-Encoding",
                 "X-Content-Type-Options": "nosniff",
                 "X-Powered-By": "ASP.NET",
-                "x-ms-correlation-request-id": "9baff9d3-88cb-4455-a389-47fc795ad66f",
+                "x-ms-correlation-request-id": "acc14af8-4979-4eb7-a668-111a8726f2c2",
                 "x-ms-ratelimit-remaining-subscription-resource-requests": "499",
-                "x-ms-routing-request-id": "EASTUS2:20230613T094049Z:9baff9d3-88cb-4455-a389-47fc795ad66f"
+                "x-ms-routing-request-id": "EASTUS2:20230210T080915Z:acc14af8-4979-4eb7-a668-111a8726f2c2"
             },
             "StatusCode": 200
         }
     ],
     "Variables": {}
 }
```

## Comparing `azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/SOURCES.txt` & `azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -80,40 +80,14 @@
 azure/mgmt/dns/v2018_05_01/models/_models_py3.py
 azure/mgmt/dns/v2018_05_01/models/_patch.py
 azure/mgmt/dns/v2018_05_01/operations/__init__.py
 azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py
 azure/mgmt/dns/v2018_05_01/operations/_patch.py
 azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py
 azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py
-azure/mgmt/dns/v2023_07_01_preview/__init__.py
-azure/mgmt/dns/v2023_07_01_preview/_configuration.py
-azure/mgmt/dns/v2023_07_01_preview/_dns_management_client.py
-azure/mgmt/dns/v2023_07_01_preview/_patch.py
-azure/mgmt/dns/v2023_07_01_preview/_vendor.py
-azure/mgmt/dns/v2023_07_01_preview/_version.py
-azure/mgmt/dns/v2023_07_01_preview/aio/__init__.py
-azure/mgmt/dns/v2023_07_01_preview/aio/_configuration.py
-azure/mgmt/dns/v2023_07_01_preview/aio/_dns_management_client.py
-azure/mgmt/dns/v2023_07_01_preview/aio/_patch.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/__init__.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dns_resource_reference_operations.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dnssec_configs_operations.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/_patch.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/_record_sets_operations.py
-azure/mgmt/dns/v2023_07_01_preview/aio/operations/_zones_operations.py
-azure/mgmt/dns/v2023_07_01_preview/models/__init__.py
-azure/mgmt/dns/v2023_07_01_preview/models/_dns_management_client_enums.py
-azure/mgmt/dns/v2023_07_01_preview/models/_models_py3.py
-azure/mgmt/dns/v2023_07_01_preview/models/_patch.py
-azure/mgmt/dns/v2023_07_01_preview/operations/__init__.py
-azure/mgmt/dns/v2023_07_01_preview/operations/_dns_resource_reference_operations.py
-azure/mgmt/dns/v2023_07_01_preview/operations/_dnssec_configs_operations.py
-azure/mgmt/dns/v2023_07_01_preview/operations/_patch.py
-azure/mgmt/dns/v2023_07_01_preview/operations/_record_sets_operations.py
-azure/mgmt/dns/v2023_07_01_preview/operations/_zones_operations.py
 azure_mgmt_dns.egg-info/PKG-INFO
 azure_mgmt_dns.egg-info/SOURCES.txt
 azure_mgmt_dns.egg-info/dependency_links.txt
 azure_mgmt_dns.egg-info/not-zip-safe
 azure_mgmt_dns.egg-info/requires.txt
 azure_mgmt_dns.egg-info/top_level.txt
 tests/conftest.py
```

## Comparing `azure-mgmt-dns-8.1.0/azure_mgmt_dns.egg-info/PKG-INFO` & `azure-mgmt-dns-8.1.0b1/azure_mgmt_dns.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-dns
-Version: 8.1.0
+Version: 8.1.0b1
 Summary: Microsoft Azure DNS Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -64,17 +64,16 @@
 
 sub_id = os.getenv("AZURE_SUBSCRIPTION_ID")
 client = DnsManagementClient(credential=DefaultAzureCredential(), subscription_id=sub_id)
 ```
 
 ## Examples
 
-Code samples for this package can be found at:
-- [Search DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com
-- [Azure Python Mgmt SDK Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
+
+Code samples for this package can be found at [DNS Management](https://docs.microsoft.com/samples/browse/?languages=python&term=Getting%20started%20-%20Managing&terms=Getting%20started%20-%20Managing) on docs.microsoft.com and [Samples Repo](https://aka.ms/azsdk/python/mgmt/samples)
 
 
 ## Troubleshooting
 
 ## Next steps
 
 ## Provide Feedback
@@ -85,25 +84,14 @@
 
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-dns%2FREADME.png)
 
 
 # Release History
 
-## 8.1.0 (2023-06-14)
-
-### Features Added
-
-  - Added operation group DnssecConfigsOperations
-  - Model RecordSet has a new parameter ds_records
-  - Model RecordSet has a new parameter naptr_records
-  - Model RecordSet has a new parameter tlsa_records
-  - Model Zone has a new parameter signing_keys
-  - Model Zone has a new parameter system_data
-
 ## 8.1.0b1 (2023-02-10)
 
 ### Other Changes
 
   - Added generated samples in github repo
   - Drop support for python<3.7.0
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/_serialization.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                                xml_name = "{}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -1269,15 +1269,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+        xml_name = "{}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1293,15 +1293,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+        xml_name = "{}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_dns_management_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -67,16 +67,14 @@
         credential: "TokenCredential",
         subscription_id: str,
         api_version: Optional[str]=None,
         base_url: str = "https://management.azure.com",
         profile: KnownProfiles=KnownProfiles.default,
         **kwargs: Any
     ):
-        if api_version:
-            kwargs.setdefault('api_version', api_version)
         self._config = DnsManagementClientConfiguration(credential, subscription_id, **kwargs)
         self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
         super(DnsManagementClient, self).__init__(
             api_version=api_version,
             profile=profile
         )
 
@@ -87,106 +85,79 @@
     @classmethod
     def models(cls, api_version=DEFAULT_API_VERSION):
         """Module depends on the API version:
 
            * 2016-04-01: :mod:`v2016_04_01.models<azure.mgmt.dns.v2016_04_01.models>`
            * 2018-03-01-preview: :mod:`v2018_03_01_preview.models<azure.mgmt.dns.v2018_03_01_preview.models>`
            * 2018-05-01: :mod:`v2018_05_01.models<azure.mgmt.dns.v2018_05_01.models>`
-           * 2023-07-01-preview: :mod:`v2023_07_01_preview.models<azure.mgmt.dns.v2023_07_01_preview.models>`
         """
         if api_version == '2016-04-01':
             from .v2016_04_01 import models
             return models
         elif api_version == '2018-03-01-preview':
             from .v2018_03_01_preview import models
             return models
         elif api_version == '2018-05-01':
             from .v2018_05_01 import models
             return models
-        elif api_version == '2023-07-01-preview':
-            from .v2023_07_01_preview import models
-            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def dns_resource_reference(self):
         """Instance depends on the API version:
 
            * 2018-05-01: :class:`DnsResourceReferenceOperations<azure.mgmt.dns.v2018_05_01.operations.DnsResourceReferenceOperations>`
-           * 2023-07-01-preview: :class:`DnsResourceReferenceOperations<azure.mgmt.dns.v2023_07_01_preview.operations.DnsResourceReferenceOperations>`
         """
         api_version = self._get_api_version('dns_resource_reference')
         if api_version == '2018-05-01':
             from .v2018_05_01.operations import DnsResourceReferenceOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from .v2023_07_01_preview.operations import DnsResourceReferenceOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'dns_resource_reference'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
-
-    @property
-    def dnssec_configs(self):
-        """Instance depends on the API version:
-
-           * 2023-07-01-preview: :class:`DnssecConfigsOperations<azure.mgmt.dns.v2023_07_01_preview.operations.DnssecConfigsOperations>`
-        """
-        api_version = self._get_api_version('dnssec_configs')
-        if api_version == '2023-07-01-preview':
-            from .v2023_07_01_preview.operations import DnssecConfigsOperations as OperationClass
-        else:
-            raise ValueError("API version {} does not have operation group 'dnssec_configs'".format(api_version))
-        self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def record_sets(self):
         """Instance depends on the API version:
 
            * 2016-04-01: :class:`RecordSetsOperations<azure.mgmt.dns.v2016_04_01.operations.RecordSetsOperations>`
            * 2018-03-01-preview: :class:`RecordSetsOperations<azure.mgmt.dns.v2018_03_01_preview.operations.RecordSetsOperations>`
            * 2018-05-01: :class:`RecordSetsOperations<azure.mgmt.dns.v2018_05_01.operations.RecordSetsOperations>`
-           * 2023-07-01-preview: :class:`RecordSetsOperations<azure.mgmt.dns.v2023_07_01_preview.operations.RecordSetsOperations>`
         """
         api_version = self._get_api_version('record_sets')
         if api_version == '2016-04-01':
             from .v2016_04_01.operations import RecordSetsOperations as OperationClass
         elif api_version == '2018-03-01-preview':
             from .v2018_03_01_preview.operations import RecordSetsOperations as OperationClass
         elif api_version == '2018-05-01':
             from .v2018_05_01.operations import RecordSetsOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from .v2023_07_01_preview.operations import RecordSetsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'record_sets'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def zones(self):
         """Instance depends on the API version:
 
            * 2016-04-01: :class:`ZonesOperations<azure.mgmt.dns.v2016_04_01.operations.ZonesOperations>`
            * 2018-03-01-preview: :class:`ZonesOperations<azure.mgmt.dns.v2018_03_01_preview.operations.ZonesOperations>`
            * 2018-05-01: :class:`ZonesOperations<azure.mgmt.dns.v2018_05_01.operations.ZonesOperations>`
-           * 2023-07-01-preview: :class:`ZonesOperations<azure.mgmt.dns.v2023_07_01_preview.operations.ZonesOperations>`
         """
         api_version = self._get_api_version('zones')
         if api_version == '2016-04-01':
             from .v2016_04_01.operations import ZonesOperations as OperationClass
         elif api_version == '2018-03-01-preview':
             from .v2018_03_01_preview.operations import ZonesOperations as OperationClass
         elif api_version == '2018-05-01':
             from .v2018_05_01.operations import ZonesOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from .v2023_07_01_preview.operations import ZonesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'zones'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     def close(self):
         self._client.close()
     def __enter__(self):
         self._client.__enter__()
         return self
     def __exit__(self, *exc_details):
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_vendor.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_dns_management_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClient:  # pylint: disable=client-accepts-api-version-keyword
     """The DNS Management Client.
 
     :ivar record_sets: RecordSetsOperations operations
-    :vartype record_sets: azure.mgmt.dns.v2018_03_01_preview.operations.RecordSetsOperations
+    :vartype record_sets: azure.mgmt.dns.v2016_04_01.operations.RecordSetsOperations
     :ivar zones: ZonesOperations operations
-    :vartype zones: azure.mgmt.dns.v2018_03_01_preview.operations.ZonesOperations
+    :vartype zones: azure.mgmt.dns.v2016_04_01.operations.ZonesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2018-03-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2016-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -48,26 +48,22 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2018-03-01-preview"
-        )
-        self.zones = ZonesOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2018-03-01-preview"
-        )
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :keyword api_version: Api Version. Default value is "2018-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop("api_version", "2018-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +58,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_zones_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,14 +28,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -47,29 +51,27 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -87,28 +89,26 @@
 
 def build_delete_request(
     resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -120,28 +120,26 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, zone_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -153,29 +151,27 @@
 
 def build_update_request(
     resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -191,27 +187,25 @@
 
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
@@ -223,21 +217,21 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(subscription_id: str, *, top: Optional[int] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones")
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
@@ -251,27 +245,26 @@
 
 class ZonesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2018_03_01_preview.DnsManagementClient`'s
+        :class:`~azure.mgmt.dns.v2018_05_01.DnsManagementClient`'s
         :attr:`zones` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: _models.Zone,
@@ -279,34 +272,33 @@
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.Zone:
         """Creates or updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
@@ -316,16 +308,15 @@
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.Zone:
         """Creates or updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
         :type parameters: IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
@@ -335,15 +326,15 @@
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
@@ -351,58 +342,55 @@
         parameters: Union[_models.Zone, IO],
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         **kwargs: Any
     ) -> _models.Zone:
         """Creates or updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a Zone type
          or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.Zone or IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -416,17 +404,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -456,17 +443,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
@@ -474,17 +459,16 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -499,16 +483,15 @@
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, zone_name: str, if_match: Optional[str] = None, **kwargs: Any
     ) -> LROPoller[None]:
         """Deletes a DNS zone. WARNING: All DNS records in the zone will also be deleted. This operation
         cannot be undone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param if_match: The etag of the DNS zone. Omit this value to always delete the current zone.
          Specify the last-seen etag value to prevent accidentally deleting any concurrent changes.
          Default value is None.
         :type if_match: str
@@ -523,17 +506,15 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
@@ -570,55 +551,51 @@
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
     @distributed_trace
     def get(self, resource_group_name: str, zone_name: str, **kwargs: Any) -> _models.Zone:
         """Gets a DNS zone. Retrieves the zone properties, but not the record sets within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -643,31 +620,30 @@
         if_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.Zone:
         """Updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the Update operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.ZoneUpdate
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.ZoneUpdate
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
@@ -676,86 +652,82 @@
         if_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.Zone:
         """Updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the Update operation. Required.
         :type parameters: IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: Union[_models.ZoneUpdate, IO],
         if_match: Optional[str] = None,
         **kwargs: Any
     ) -> _models.Zone:
         """Updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the Update operation. Is either a ZoneUpdate type or
          a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.ZoneUpdate or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.ZoneUpdate or IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ZoneUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -768,17 +740,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -796,31 +767,28 @@
 
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, top: Optional[int] = None, **kwargs: Any
     ) -> Iterable["_models.Zone"]:
         """Lists the DNS zones within a resource group.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_05_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -866,17 +834,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -893,23 +860,21 @@
         """Lists the DNS zones in all resource groups in a subscription.
 
         :param top: The maximum number of DNS zones to return. If not specified, returns up to 100
          zones. Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_05_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -954,17 +919,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_record_sets_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,14 +26,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -46,15 +50,17 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
@@ -96,15 +102,17 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
@@ -147,15 +155,17 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
@@ -191,15 +201,17 @@
     record_type: Union[str, _models.RecordType],
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
@@ -235,15 +247,17 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}",
     )  # pylint: disable=line-too-long
@@ -279,15 +293,17 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/recordsets",
     )  # pylint: disable=line-too-long
@@ -322,15 +338,17 @@
     top: Optional[int] = None,
     record_set_name_suffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2018-03-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/all",
     )  # pylint: disable=line-too-long
@@ -371,15 +389,14 @@
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def update(
         self,
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
@@ -505,24 +522,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -537,17 +554,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -706,24 +722,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -739,17 +755,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -809,16 +824,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
@@ -829,17 +844,16 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -885,16 +899,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
@@ -904,17 +918,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -961,16 +974,16 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1020,17 +1033,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1069,16 +1081,16 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1127,17 +1139,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1176,16 +1187,16 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1234,17 +1245,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_dns_management_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,26 +48,22 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2018-03-01-preview"
-        )
-        self.zones = ZonesOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2018-03-01-preview"
-        )
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
@@ -25,22 +31,22 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2018-03-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2016-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2018-03-01-preview")
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", "2016-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_zones_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -36,14 +36,18 @@
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_request,
     build_update_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ZonesOperations:
     """
     .. warning::
@@ -58,15 +62,14 @@
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: _models.Zone,
@@ -180,24 +183,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -211,17 +214,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -251,16 +253,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
@@ -269,17 +271,16 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -318,16 +319,16 @@
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
@@ -386,16 +387,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
@@ -403,17 +404,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -533,24 +533,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ZoneUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -563,17 +563,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -606,16 +605,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -662,17 +661,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -696,16 +694,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -751,17 +749,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_record_sets_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,14 +35,18 @@
     build_get_request,
     build_list_all_by_dns_zone_request,
     build_list_by_dns_zone_request,
     build_list_by_type_request,
     build_update_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class RecordSetsOperations:
     """
     .. warning::
@@ -57,15 +61,14 @@
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
@@ -191,24 +194,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -223,17 +226,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -392,24 +394,24 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -425,17 +427,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -495,16 +496,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
@@ -515,17 +516,16 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -571,16 +571,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
@@ -590,17 +590,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -648,16 +647,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -707,17 +706,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -757,16 +755,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -815,17 +813,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -865,16 +862,16 @@
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2018-03-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -923,17 +920,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_dns_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_vendor.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_dns_management_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClient:  # pylint: disable=client-accepts-api-version-keyword
     """The DNS Management Client.
 
     :ivar record_sets: RecordSetsOperations operations
-    :vartype record_sets: azure.mgmt.dns.v2016_04_01.operations.RecordSetsOperations
+    :vartype record_sets: azure.mgmt.dns.v2018_03_01_preview.operations.RecordSetsOperations
     :ivar zones: ZonesOperations operations
-    :vartype zones: azure.mgmt.dns.v2016_04_01.operations.ZonesOperations
+    :vartype zones: azure.mgmt.dns.v2018_03_01_preview.operations.ZonesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2016-04-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-03-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -48,24 +48,22 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2016-04-01"
-        )
-        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize, "2016-04-01")
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
@@ -32,15 +38,15 @@
     :keyword api_version: Api Version. Default value is "2016-04-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2016-04-01")
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", "2016-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_zones_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,14 +28,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -47,15 +51,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
@@ -87,15 +91,15 @@
 
 def build_delete_request(
     resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
@@ -120,15 +124,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, zone_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
@@ -153,15 +157,15 @@
 
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones",
     )  # pylint: disable=line-too-long
@@ -185,15 +189,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(subscription_id: str, *, top: Optional[int] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -225,15 +229,14 @@
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: _models.Zone,
@@ -347,22 +350,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -376,17 +379,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -416,15 +418,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[Optional[_models.ZoneDeleteResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
@@ -432,17 +434,16 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -488,15 +489,15 @@
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.dns.v2016_04_01.models.ZoneDeleteResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneDeleteResult] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(
                 resource_group_name=resource_group_name,
@@ -556,32 +557,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -613,15 +613,15 @@
         :return: An iterator like instance of either Zone or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2016_04_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -667,17 +667,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -700,15 +699,15 @@
         :return: An iterator like instance of either Zone or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2016_04_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -753,17 +752,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_record_sets_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,14 +26,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -46,15 +50,15 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
@@ -96,15 +100,15 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
@@ -147,15 +151,15 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
@@ -191,15 +195,15 @@
     record_type: Union[str, _models.RecordType],
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
@@ -235,15 +239,15 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}",
     )  # pylint: disable=line-too-long
@@ -279,15 +283,15 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
+    api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/recordsets",
     )  # pylint: disable=line-too-long
@@ -328,15 +332,14 @@
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def update(
         self,
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
@@ -462,22 +465,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -492,17 +495,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -661,22 +663,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -692,17 +694,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -762,15 +763,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -780,17 +781,16 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -836,15 +836,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -853,17 +853,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -910,15 +909,15 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2016_04_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -967,17 +966,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1016,15 +1014,15 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2016_04_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1072,17 +1070,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_dns_management_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,24 +48,22 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2016-04-01"
-        )
-        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize, "2016-04-01")
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2016-04-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-03-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2016-04-01")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop("api_version", "2018-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +58,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_zones_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -35,14 +35,18 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ZonesOperations:
     """
     .. warning::
@@ -57,15 +61,14 @@
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: _models.Zone,
@@ -179,22 +182,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -208,17 +211,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -248,15 +250,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[Optional[_models.ZoneDeleteResult]] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
@@ -264,17 +266,16 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -320,15 +321,15 @@
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.dns.v2016_04_01.models.ZoneDeleteResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneDeleteResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(
                 resource_group_name=resource_group_name,
@@ -388,32 +389,31 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -445,15 +445,15 @@
         :return: An iterator like instance of either Zone or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2016_04_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -499,17 +499,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -532,15 +531,15 @@
         :return: An iterator like instance of either Zone or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2016_04_01.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -585,17 +584,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_record_sets_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -34,14 +34,18 @@
     build_delete_request,
     build_get_request,
     build_list_by_dns_zone_request,
     build_list_by_type_request,
     build_update_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class RecordSetsOperations:
     """
     .. warning::
@@ -56,15 +60,14 @@
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
@@ -190,22 +193,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -220,17 +223,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -389,22 +391,22 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -420,17 +422,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -490,15 +491,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -508,17 +509,16 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -564,15 +564,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -581,17 +581,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -638,15 +637,15 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2016_04_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -695,17 +694,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -744,15 +742,15 @@
         :return: An iterator like instance of either RecordSet or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2016_04_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._api_version or "2016-04-01"))
+        api_version: Literal["2016-04-01"] = kwargs.pop("api_version", _params.pop("api-version", "2016-04-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -800,17 +798,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_models_py3.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,15 +726,15 @@
      "MultipleChoices", "Ambiguous", "MovedPermanently", "Moved", "Found", "Redirect", "SeeOther",
      "RedirectMethod", "NotModified", "UseProxy", "Unused", "TemporaryRedirect", "RedirectKeepVerb",
      "BadRequest", "Unauthorized", "PaymentRequired", "Forbidden", "NotFound", "MethodNotAllowed",
      "NotAcceptable", "ProxyAuthenticationRequired", "RequestTimeout", "Conflict", "Gone",
      "LengthRequired", "PreconditionFailed", "RequestEntityTooLarge", "RequestUriTooLong",
      "UnsupportedMediaType", "RequestedRangeNotSatisfiable", "ExpectationFailed", "UpgradeRequired",
      "InternalServerError", "NotImplemented", "BadGateway", "ServiceUnavailable", "GatewayTimeout",
-     "HttpVersionNotSupported", and "Continue".
+     and "HttpVersionNotSupported".
     :vartype status_code: str or ~azure.mgmt.dns.v2016_04_01.models.HttpStatusCode
     :ivar request_id:
     :vartype request_id: str
     """
 
     _attribute_map = {
         "azure_async_operation": {"key": "azureAsyncOperation", "type": "str"},
@@ -763,15 +763,15 @@
          "MultipleChoices", "Ambiguous", "MovedPermanently", "Moved", "Found", "Redirect", "SeeOther",
          "RedirectMethod", "NotModified", "UseProxy", "Unused", "TemporaryRedirect", "RedirectKeepVerb",
          "BadRequest", "Unauthorized", "PaymentRequired", "Forbidden", "NotFound", "MethodNotAllowed",
          "NotAcceptable", "ProxyAuthenticationRequired", "RequestTimeout", "Conflict", "Gone",
          "LengthRequired", "PreconditionFailed", "RequestEntityTooLarge", "RequestUriTooLong",
          "UnsupportedMediaType", "RequestedRangeNotSatisfiable", "ExpectationFailed", "UpgradeRequired",
          "InternalServerError", "NotImplemented", "BadGateway", "ServiceUnavailable", "GatewayTimeout",
-         "HttpVersionNotSupported", and "Continue".
+         and "HttpVersionNotSupported".
         :paramtype status_code: str or ~azure.mgmt.dns.v2016_04_01.models.HttpStatusCode
         :keyword request_id:
         :paramtype request_id: str
         """
         super().__init__(**kwargs)
         self.azure_async_operation = azure_async_operation
         self.status = status
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_dns_management_client_enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     UPGRADE_REQUIRED = "UpgradeRequired"
     INTERNAL_SERVER_ERROR = "InternalServerError"
     NOT_IMPLEMENTED = "NotImplemented"
     BAD_GATEWAY = "BadGateway"
     SERVICE_UNAVAILABLE = "ServiceUnavailable"
     GATEWAY_TIMEOUT = "GatewayTimeout"
     HTTP_VERSION_NOT_SUPPORTED = "HttpVersionNotSupported"
-    CONTINUE_ENUM = "Continue"
 
 
 class OperationStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """OperationStatus."""
 
     IN_PROGRESS = "InProgress"
     SUCCEEDED = "Succeeded"
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_dns_management_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,16 +67,14 @@
         credential: "AsyncTokenCredential",
         subscription_id: str,
         api_version: Optional[str] = None,
         base_url: str = "https://management.azure.com",
         profile: KnownProfiles = KnownProfiles.default,
         **kwargs: Any
     ) -> None:
-        if api_version:
-            kwargs.setdefault('api_version', api_version)
         self._config = DnsManagementClientConfiguration(credential, subscription_id, **kwargs)
         self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
         super(DnsManagementClient, self).__init__(
             api_version=api_version,
             profile=profile
         )
 
@@ -87,106 +85,79 @@
     @classmethod
     def models(cls, api_version=DEFAULT_API_VERSION):
         """Module depends on the API version:
 
            * 2016-04-01: :mod:`v2016_04_01.models<azure.mgmt.dns.v2016_04_01.models>`
            * 2018-03-01-preview: :mod:`v2018_03_01_preview.models<azure.mgmt.dns.v2018_03_01_preview.models>`
            * 2018-05-01: :mod:`v2018_05_01.models<azure.mgmt.dns.v2018_05_01.models>`
-           * 2023-07-01-preview: :mod:`v2023_07_01_preview.models<azure.mgmt.dns.v2023_07_01_preview.models>`
         """
         if api_version == '2016-04-01':
             from ..v2016_04_01 import models
             return models
         elif api_version == '2018-03-01-preview':
             from ..v2018_03_01_preview import models
             return models
         elif api_version == '2018-05-01':
             from ..v2018_05_01 import models
             return models
-        elif api_version == '2023-07-01-preview':
-            from ..v2023_07_01_preview import models
-            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def dns_resource_reference(self):
         """Instance depends on the API version:
 
            * 2018-05-01: :class:`DnsResourceReferenceOperations<azure.mgmt.dns.v2018_05_01.aio.operations.DnsResourceReferenceOperations>`
-           * 2023-07-01-preview: :class:`DnsResourceReferenceOperations<azure.mgmt.dns.v2023_07_01_preview.aio.operations.DnsResourceReferenceOperations>`
         """
         api_version = self._get_api_version('dns_resource_reference')
         if api_version == '2018-05-01':
             from ..v2018_05_01.aio.operations import DnsResourceReferenceOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from ..v2023_07_01_preview.aio.operations import DnsResourceReferenceOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'dns_resource_reference'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
-
-    @property
-    def dnssec_configs(self):
-        """Instance depends on the API version:
-
-           * 2023-07-01-preview: :class:`DnssecConfigsOperations<azure.mgmt.dns.v2023_07_01_preview.aio.operations.DnssecConfigsOperations>`
-        """
-        api_version = self._get_api_version('dnssec_configs')
-        if api_version == '2023-07-01-preview':
-            from ..v2023_07_01_preview.aio.operations import DnssecConfigsOperations as OperationClass
-        else:
-            raise ValueError("API version {} does not have operation group 'dnssec_configs'".format(api_version))
-        self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def record_sets(self):
         """Instance depends on the API version:
 
            * 2016-04-01: :class:`RecordSetsOperations<azure.mgmt.dns.v2016_04_01.aio.operations.RecordSetsOperations>`
            * 2018-03-01-preview: :class:`RecordSetsOperations<azure.mgmt.dns.v2018_03_01_preview.aio.operations.RecordSetsOperations>`
            * 2018-05-01: :class:`RecordSetsOperations<azure.mgmt.dns.v2018_05_01.aio.operations.RecordSetsOperations>`
-           * 2023-07-01-preview: :class:`RecordSetsOperations<azure.mgmt.dns.v2023_07_01_preview.aio.operations.RecordSetsOperations>`
         """
         api_version = self._get_api_version('record_sets')
         if api_version == '2016-04-01':
             from ..v2016_04_01.aio.operations import RecordSetsOperations as OperationClass
         elif api_version == '2018-03-01-preview':
             from ..v2018_03_01_preview.aio.operations import RecordSetsOperations as OperationClass
         elif api_version == '2018-05-01':
             from ..v2018_05_01.aio.operations import RecordSetsOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from ..v2023_07_01_preview.aio.operations import RecordSetsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'record_sets'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def zones(self):
         """Instance depends on the API version:
 
            * 2016-04-01: :class:`ZonesOperations<azure.mgmt.dns.v2016_04_01.aio.operations.ZonesOperations>`
            * 2018-03-01-preview: :class:`ZonesOperations<azure.mgmt.dns.v2018_03_01_preview.aio.operations.ZonesOperations>`
            * 2018-05-01: :class:`ZonesOperations<azure.mgmt.dns.v2018_05_01.aio.operations.ZonesOperations>`
-           * 2023-07-01-preview: :class:`ZonesOperations<azure.mgmt.dns.v2023_07_01_preview.aio.operations.ZonesOperations>`
         """
         api_version = self._get_api_version('zones')
         if api_version == '2016-04-01':
             from ..v2016_04_01.aio.operations import ZonesOperations as OperationClass
         elif api_version == '2018-03-01-preview':
             from ..v2018_03_01_preview.aio.operations import ZonesOperations as OperationClass
         elif api_version == '2018-05-01':
             from ..v2018_05_01.aio.operations import ZonesOperations as OperationClass
-        elif api_version == '2023-07-01-preview':
-            from ..v2023_07_01_preview.aio.operations import ZonesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'zones'".format(api_version))
         self._config.api_version = api_version
-        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)), api_version)
+        return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     async def close(self):
         await self._client.close()
     async def __aenter__(self):
         await self._client.__aenter__()
         return self
     async def __aexit__(self, *exc_details):
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/aio/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_vendor.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_dns_management_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,40 @@
 
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
 
 from . import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import DnsManagementClientConfiguration
-from .operations import DnsResourceReferenceOperations, DnssecConfigsOperations, RecordSetsOperations, ZonesOperations
+from .operations import DnsResourceReferenceOperations, RecordSetsOperations, ZonesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClient:  # pylint: disable=client-accepts-api-version-keyword
     """The DNS Management Client.
 
-    :ivar dnssec_configs: DnssecConfigsOperations operations
-    :vartype dnssec_configs: azure.mgmt.dns.v2023_07_01_preview.operations.DnssecConfigsOperations
     :ivar record_sets: RecordSetsOperations operations
-    :vartype record_sets: azure.mgmt.dns.v2023_07_01_preview.operations.RecordSetsOperations
+    :vartype record_sets: azure.mgmt.dns.v2018_05_01.operations.RecordSetsOperations
     :ivar zones: ZonesOperations operations
-    :vartype zones: azure.mgmt.dns.v2023_07_01_preview.operations.ZonesOperations
+    :vartype zones: azure.mgmt.dns.v2018_05_01.operations.ZonesOperations
     :ivar dns_resource_reference: DnsResourceReferenceOperations operations
     :vartype dns_resource_reference:
-     azure.mgmt.dns.v2023_07_01_preview.operations.DnsResourceReferenceOperations
+     azure.mgmt.dns.v2018_05_01.operations.DnsResourceReferenceOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: Specifies the Azure subscription ID, which uniquely identifies the
+     Microsoft Azure subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-07-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-05-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -53,31 +52,24 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.dnssec_configs = DnssecConfigsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
-        self.zones = ZonesOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.dns_resource_reference = DnsResourceReferenceOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
+            self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,45 +2,52 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: Specifies the Azure subscription ID, which uniquely identifies the
+     Microsoft Azure subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-07-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-05-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-07-01-preview")
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", "2018-05-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +59,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/operations/_zones_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -28,14 +28,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -47,15 +51,17 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
@@ -87,15 +93,17 @@
 
 def build_delete_request(
     resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
@@ -120,15 +128,17 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, zone_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
     )  # pylint: disable=line-too-long
@@ -153,15 +163,17 @@
 
 def build_update_request(
     resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}",
@@ -191,15 +203,17 @@
 
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, top: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones",
     )  # pylint: disable=line-too-long
@@ -223,15 +237,17 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(subscription_id: str, *, top: Optional[int] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2018-03-01-preview")
+    )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -251,27 +267,26 @@
 
 class ZonesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.DnsManagementClient`'s
+        :class:`~azure.mgmt.dns.v2018_03_01_preview.DnsManagementClient`'s
         :attr:`zones` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
         parameters: _models.Zone,
@@ -285,28 +300,28 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
@@ -335,15 +350,15 @@
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
@@ -358,51 +373,51 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a Zone type
          or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone or IO
+        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone or IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
          an existing zone. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -416,17 +431,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -456,16 +470,16 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
@@ -474,31 +488,26 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
         "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
     @distributed_trace
     def begin_delete(
@@ -527,16 +536,16 @@
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
@@ -581,30 +590,30 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
@@ -612,17 +621,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -653,25 +661,25 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the Update operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.ZoneUpdate
+        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.ZoneUpdate
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
@@ -696,15 +704,15 @@
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
@@ -718,48 +726,48 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param parameters: Parameters supplied to the Update operation. Is either a ZoneUpdate type or
          a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.ZoneUpdate or IO
+        :type parameters: ~azure.mgmt.dns.v2018_03_01_preview.models.ZoneUpdate or IO
         :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
          zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :rtype: ~azure.mgmt.dns.v2018_03_01_preview.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "ZoneUpdate")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -772,17 +780,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -808,22 +815,22 @@
          Required.
         :type resource_group_name: str
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.Zone]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -870,17 +877,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -897,22 +903,22 @@
         """Lists the DNS zones in all resource groups in a subscription.
 
         :param top: The maximum number of DNS zones to return. If not specified, returns up to 100
          zones. Default value is None.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.Zone]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_03_01_preview.models.Zone]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-03-01-preview"] = kwargs.pop(
+            "api_version", _params.pop("api-version", "2018-03-01-preview")
         )
         cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -958,17 +964,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dns_resource_reference_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_dns_resource_reference_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,35 +24,39 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_by_target_resources_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Network/getDnsResourceReference"
     )
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -66,42 +70,41 @@
 
 class DnsResourceReferenceOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.DnsManagementClient`'s
+        :class:`~azure.mgmt.dns.v2018_05_01.DnsManagementClient`'s
         :attr:`dns_resource_reference` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def get_by_target_resources(
         self, parameters: _models.DnsResourceReferenceRequest, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
         """Returns the DNS records specified by the referencing targetResourceIds.
 
         :param parameters: Properties for dns resource reference request. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceRequest
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def get_by_target_resources(
         self, parameters: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
@@ -110,56 +113,54 @@
         :param parameters: Properties for dns resource reference request. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def get_by_target_resources(
         self, parameters: Union[_models.DnsResourceReferenceRequest, IO], **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
         """Returns the DNS records specified by the referencing targetResourceIds.
 
         :param parameters: Properties for dns resource reference request. Is either a
          DnsResourceReferenceRequest type or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceRequest or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DnsResourceReferenceResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "DnsResourceReferenceRequest")
 
         request = build_get_by_target_resources_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -169,17 +170,16 @@
             template_url=self.get_by_target_resources.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_dnssec_configs_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_zones_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,375 +2,261 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar, Union, cast
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.arm_polling import ARMPolling
+from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from .. import models as _models
-from ..._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._zones_operations import (
+    build_create_or_update_request,
+    build_delete_request,
+    build_get_request,
+    build_list_by_resource_group_request,
+    build_list_request,
+    build_update_request,
+)
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_create_or_update_request(
-    resource_group_name: str,
-    zone_name: str,
-    subscription_id: str,
-    *,
-    if_match: Optional[str] = None,
-    if_none_match: Optional[str] = None,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if if_match is not None:
-        _headers["If-Match"] = _SERIALIZER.header("if_match", if_match, "str")
-    if if_none_match is not None:
-        _headers["If-None-Match"] = _SERIALIZER.header("if_none_match", if_none_match, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_delete_request(
-    resource_group_name: str, zone_name: str, subscription_id: str, *, if_match: Optional[str] = None, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if if_match is not None:
-        _headers["If-Match"] = _SERIALIZER.header("if_match", if_match, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_get_request(resource_group_name: str, zone_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_list_by_dns_zone_request(
-    resource_group_name: str, zone_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-    }
-
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class DnssecConfigsOperations:
+class ZonesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.DnsManagementClient`'s
-        :attr:`dnssec_configs` attribute.
+        :class:`~azure.mgmt.dns.v2018_05_01.aio.DnsManagementClient`'s
+        :attr:`zones` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
-    def _create_or_update_initial(
+    @overload
+    async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
+        parameters: _models.Zone,
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.DnssecConfig:
+    ) -> _models.Zone:
+        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
+         an existing zone. Other values will be ignored. Default value is None.
+        :type if_none_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_or_update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        parameters: IO,
+        if_match: Optional[str] = None,
+        if_none_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Zone:
+        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
+        :type parameters: IO
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
+         an existing zone. Other values will be ignored. Default value is None.
+        :type if_none_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_or_update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        parameters: Union[_models.Zone, IO],
+        if_match: Optional[str] = None,
+        if_none_match: Optional[str] = None,
+        **kwargs: Any
+    ) -> _models.Zone:
+        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a Zone type
+         or a IO type. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.Zone or IO
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
+         an existing zone. Other values will be ignored. Default value is None.
+        :type if_none_match: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.DnssecConfig] = kwargs.pop("cls", None)
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(parameters, (IO, bytes)):
+            _content = parameters
+        else:
+            _json = self._serialize.body(parameters, "Zone")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
             if_none_match=if_none_match,
             api_version=api_version,
-            template_url=self._create_or_update_initial.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("DnssecConfig", pipeline_response)
+            deserialized = self._deserialize("Zone", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("DnssecConfig", pipeline_response)
+            deserialized = self._deserialize("Zone", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default"
-    }
-
-    @distributed_trace
-    def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        zone_name: str,
-        if_match: Optional[str] = None,
-        if_none_match: Optional[str] = None,
-        **kwargs: Any
-    ) -> LROPoller[_models.DnssecConfig]:
-        """Creates or updates the DNSSEC configuration on a DNS zone.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
-        :type zone_name: str
-        :param if_match: The etag of the DNSSEC configuration. Omit this value to always overwrite the
-         DNSSEC configuration. Specify the last-seen etag value to prevent accidentally overwriting any
-         concurrent changes. Default value is None.
-        :type if_match: str
-        :param if_none_match: Set to '*' to allow this DNSSEC configuration to be created, but to
-         prevent updating existing DNSSEC configuration. Other values will be ignored. Default value is
-         None.
-        :type if_none_match: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DnssecConfig or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.dns.v2023_07_01_preview.models.DnssecConfig]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.DnssecConfig] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = self._create_or_update_initial(
-                resource_group_name=resource_group_name,
-                zone_name=zone_name,
-                if_match=if_match,
-                if_none_match=if_none_match,
-                api_version=api_version,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("DnssecConfig", pipeline_response)
-            if cls:
-                return cls(pipeline_response, deserialized, {})
-            return deserialized
-
-        if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
-        elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return LROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default"
+    create_or_update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
-    def _delete_initial(  # pylint: disable=inconsistent-return-statements
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, zone_name: str, if_match: Optional[str] = None, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
@@ -378,75 +264,68 @@
             template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
-    @distributed_trace
-    def begin_delete(
+    @distributed_trace_async
+    async def begin_delete(
         self, resource_group_name: str, zone_name: str, if_match: Optional[str] = None, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Deletes the DNSSEC configuration on a DNS zone. This operation cannot be undone.
+    ) -> AsyncLROPoller[None]:
+        """Deletes a DNS zone. WARNING: All DNS records in the zone will also be deleted. This operation
+        cannot be undone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
-        :param if_match: The etag of this DNSSEC configuration. Omit this value to always delete the
-         DNSSEC configuration. Specify the last-seen etag value to prevent accidentally deleting any
-         concurrent changes. Default value is None.
+        :param if_match: The etag of the DNS zone. Omit this value to always delete the current zone.
+         Specify the last-seen etag value to prevent accidentally deleting any concurrent changes.
+         Default value is None.
         :type if_match: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
+         this operation to not poll, or pass in your own initialized polling object for a personal
+         polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
          Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._delete_initial(  # type: ignore
+            raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 zone_name=zone_name,
                 if_match=if_match,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
@@ -455,137 +334,285 @@
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
                 return cls(pipeline_response, None, {})
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
-    @distributed_trace
-    def get(self, resource_group_name: str, zone_name: str, **kwargs: Any) -> _models.DnssecConfig:
-        """Gets the DNSSEC configuration.
+    @distributed_trace_async
+    async def get(self, resource_group_name: str, zone_name: str, **kwargs: Any) -> _models.Zone:
+        """Gets a DNS zone. Retrieves the zone properties, but not the record sets within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: DnssecConfig or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnssecConfig
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.DnssecConfig] = kwargs.pop("cls", None)
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("DnssecConfig", pipeline_response)
+        deserialized = self._deserialize("Zone", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs/default"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
     }
 
-    @distributed_trace
-    def list_by_dns_zone(
-        self, resource_group_name: str, zone_name: str, **kwargs: Any
-    ) -> Iterable["_models.DnssecConfig"]:
-        """Lists the DNSSEC configurations in a DNS zone.
+    @overload
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        parameters: _models.ZoneUpdate,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Zone:
+        """Updates a DNS zone. Does not modify DNS records within the zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
+        :param parameters: Parameters supplied to the Update operation. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.ZoneUpdate
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either DnssecConfig or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.DnssecConfig]
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
+
+    @overload
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        parameters: IO,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.Zone:
+        """Updates a DNS zone. Does not modify DNS records within the zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param parameters: Parameters supplied to the Update operation. Required.
+        :type parameters: IO
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        parameters: Union[_models.ZoneUpdate, IO],
+        if_match: Optional[str] = None,
+        **kwargs: Any
+    ) -> _models.Zone:
+        """Updates a DNS zone. Does not modify DNS records within the zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param parameters: Parameters supplied to the Update operation. Is either a ZoneUpdate type or
+         a IO type. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.ZoneUpdate or IO
+        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
+         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: Zone or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.Zone
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(parameters, (IO, bytes)):
+            _content = parameters
+        else:
+            _json = self._serialize.body(parameters, "ZoneUpdate")
+
+        request = build_update_request(
+            resource_group_name=resource_group_name,
+            zone_name=zone_name,
+            subscription_id=self._config.subscription_id,
+            if_match=if_match,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self.update.metadata["url"],
+            headers=_headers,
+            params=_params,
         )
-        cls: ClsType[_models.DnssecConfigListResult] = kwargs.pop("cls", None)
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("Zone", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
+    }
+
+    @distributed_trace
+    def list_by_resource_group(
+        self, resource_group_name: str, top: Optional[int] = None, **kwargs: Any
+    ) -> AsyncIterable["_models.Zone"]:
+        """Lists the DNS zones within a resource group.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param top: The maximum number of record sets to return. If not specified, returns up to 100
+         record sets. Default value is None.
+        :type top: int
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: An iterator like instance of either Zone or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_05_01.models.Zone]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_dns_zone_request(
+                request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
-                    zone_name=zone_name,
                     subscription_id=self._config.subscription_id,
+                    top=top,
                     api_version=api_version,
-                    template_url=self.list_by_dns_zone.metadata["url"],
+                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -602,34 +629,116 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("DnssecConfigListResult", pipeline_response)
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ZoneListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
+        async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(get_next, extract_data)
+        return AsyncItemPaged(get_next, extract_data)
 
-    list_by_dns_zone.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/dnssecConfigs"
+    list_by_resource_group.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones"
     }
+
+    @distributed_trace
+    def list(self, top: Optional[int] = None, **kwargs: Any) -> AsyncIterable["_models.Zone"]:
+        """Lists the DNS zones in all resource groups in a subscription.
+
+        :param top: The maximum number of DNS zones to return. If not specified, returns up to 100
+         zones. Default value is None.
+        :type top: int
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: An iterator like instance of either Zone or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_05_01.models.Zone]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    top=top,
+                    api_version=api_version,
+                    template_url=self.list.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ZoneListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones"}
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/operations/_record_sets_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/_record_sets_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,14 +26,18 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from ..._serialization import Serializer
 from .._vendor import _convert_request, _format_url_section
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -46,33 +50,31 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
         "relativeRecordSetName": _SERIALIZER.url(
             "relative_record_set_name", relative_record_set_name, "str", skip_quote=True
         ),
         "recordType": _SERIALIZER.url("record_type", record_type, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -96,33 +98,31 @@
     if_match: Optional[str] = None,
     if_none_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
         "relativeRecordSetName": _SERIALIZER.url(
             "relative_record_set_name", relative_record_set_name, "str", skip_quote=True
         ),
         "recordType": _SERIALIZER.url("record_type", record_type, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -147,32 +147,30 @@
     *,
     if_match: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
         "relativeRecordSetName": _SERIALIZER.url(
             "relative_record_set_name", relative_record_set_name, "str", skip_quote=True
         ),
         "recordType": _SERIALIZER.url("record_type", record_type, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -191,32 +189,30 @@
     record_type: Union[str, _models.RecordType],
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
         "relativeRecordSetName": _SERIALIZER.url(
             "relative_record_set_name", relative_record_set_name, "str", skip_quote=True
         ),
         "recordType": _SERIALIZER.url("record_type", record_type, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -235,29 +231,27 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
         "recordType": _SERIALIZER.url("record_type", record_type, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
@@ -279,28 +273,26 @@
     top: Optional[int] = None,
     recordsetnamesuffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/recordsets",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
@@ -322,28 +314,26 @@
     top: Optional[int] = None,
     record_set_name_suffix: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-07-01-preview"))
+    api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/all",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
         "zoneName": _SERIALIZER.url("zone_name", zone_name, "str"),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     if top is not None:
         _params["$top"] = _SERIALIZER.query("top", top, "int")
@@ -359,27 +349,26 @@
 
 class RecordSetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.DnsManagementClient`'s
+        :class:`~azure.mgmt.dns.v2018_05_01.DnsManagementClient`'s
         :attr:`record_sets` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     def update(
         self,
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
@@ -388,37 +377,36 @@
         if_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RecordSet:
         """Updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
         :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the Update operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
@@ -429,37 +417,36 @@
         if_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RecordSet:
         """Updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
         :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the Update operation. Required.
         :type parameters: IO
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
@@ -468,61 +455,58 @@
         record_type: Union[str, _models.RecordType],
         parameters: Union[_models.RecordSet, IO],
         if_match: Optional[str] = None,
         **kwargs: Any
     ) -> _models.RecordSet:
         """Updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
         :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the Update operation. Is either a RecordSet type or a
          IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet or IO
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -537,17 +521,16 @@
             template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -573,43 +556,42 @@
         parameters: _models.RecordSet,
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RecordSet:
-        """Creates or updates a record set within a DNS zone. Record sets of type SOA can be updated but
-        not created (they are created when the DNS zone is created).
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
-        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
          updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
@@ -619,43 +601,42 @@
         parameters: IO,
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.RecordSet:
-        """Creates or updates a record set within a DNS zone. Record sets of type SOA can be updated but
-        not created (they are created when the DNS zone is created).
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
-        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
         :type parameters: IO
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
          updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
@@ -663,67 +644,64 @@
         relative_record_set_name: str,
         record_type: Union[str, _models.RecordType],
         parameters: Union[_models.RecordSet, IO],
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         **kwargs: Any
     ) -> _models.RecordSet:
-        """Creates or updates a record set within a DNS zone. Record sets of type SOA can be updated but
-        not created (they are created when the DNS zone is created).
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
-        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a RecordSet
          type or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet or IO
         :param if_match: The etag of the record set. Omit this value to always overwrite the current
          record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
         :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
          updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
@@ -739,17 +717,16 @@
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -775,28 +752,27 @@
         resource_group_name: str,
         zone_name: str,
         relative_record_set_name: str,
         record_type: Union[str, _models.RecordType],
         if_match: Optional[str] = None,
         **kwargs: Any
     ) -> None:
-        """Deletes a record set from a DNS zone. This operation cannot be undone. Record sets of type SOA
-        cannot be deleted (they are deleted when the DNS zone is deleted).
+        """Deletes a record set from a DNS zone. This operation cannot be undone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
-        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA cannot
+         be deleted (they are deleted when the DNS zone is deleted). Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param if_match: The etag of the record set. Omit this value to always delete the current
          record set. Specify the last-seen etag value to prevent accidentally deleting any concurrent
          changes. Default value is None.
         :type if_match: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
@@ -809,17 +785,15 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -829,17 +803,16 @@
             template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -858,44 +831,41 @@
         zone_name: str,
         relative_record_set_name: str,
         record_type: Union[str, _models.RecordType],
         **kwargs: Any
     ) -> _models.RecordSet:
         """Gets a record set.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
         :type relative_record_set_name: str
         :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RecordSet or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
             relative_record_set_name=relative_record_set_name,
             record_type=record_type,
@@ -904,17 +874,16 @@
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -938,40 +907,37 @@
         record_type: Union[str, _models.RecordType],
         top: Optional[int] = None,
         recordsetnamesuffix: Optional[str] = None,
         **kwargs: Any
     ) -> Iterable["_models.RecordSet"]:
         """Lists the record sets of a specified type in a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
-        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
-         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", "TXT", "TLSA", "DS", and "NAPTR". Required.
-        :type record_type: str or ~azure.mgmt.dns.v2023_07_01_preview.models.RecordType
+        :param record_type: The type of record sets to enumerate. Known values are: "A", "AAAA", "CAA",
+         "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
         :param recordsetnamesuffix: The suffix label of the record set name that has to be used to
          filter the record set enumerations. If this parameter is specified, Enumeration will return
          only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
         :type recordsetnamesuffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either RecordSet or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1020,17 +986,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1049,37 +1014,34 @@
         zone_name: str,
         top: Optional[int] = None,
         recordsetnamesuffix: Optional[str] = None,
         **kwargs: Any
     ) -> Iterable["_models.RecordSet"]:
         """Lists all record sets in a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
         :param recordsetnamesuffix: The suffix label of the record set name that has to be used to
          filter the record set enumerations. If this parameter is specified, Enumeration will return
          only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
         :type recordsetnamesuffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either RecordSet or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1127,17 +1089,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
@@ -1156,37 +1117,34 @@
         zone_name: str,
         top: Optional[int] = None,
         record_set_name_suffix: Optional[str] = None,
         **kwargs: Any
     ) -> Iterable["_models.RecordSet"]:
         """Lists all record sets in a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
         :param record_set_name_suffix: The suffix label of the record set name that has to be used to
          filter the record set enumerations. If this parameter is specified, Enumeration will return
          only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
         :type record_set_name_suffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either RecordSet or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.RecordSet]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1234,17 +1192,16 @@
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_dns_management_client.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/_dns_management_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,42 +11,40 @@
 
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
 
 from .. import models as _models
 from ..._serialization import Deserializer, Serializer
 from ._configuration import DnsManagementClientConfiguration
-from .operations import DnsResourceReferenceOperations, DnssecConfigsOperations, RecordSetsOperations, ZonesOperations
+from .operations import DnsResourceReferenceOperations, RecordSetsOperations, ZonesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class DnsManagementClient:  # pylint: disable=client-accepts-api-version-keyword
     """The DNS Management Client.
 
-    :ivar dnssec_configs: DnssecConfigsOperations operations
-    :vartype dnssec_configs:
-     azure.mgmt.dns.v2023_07_01_preview.aio.operations.DnssecConfigsOperations
     :ivar record_sets: RecordSetsOperations operations
-    :vartype record_sets: azure.mgmt.dns.v2023_07_01_preview.aio.operations.RecordSetsOperations
+    :vartype record_sets: azure.mgmt.dns.v2018_05_01.aio.operations.RecordSetsOperations
     :ivar zones: ZonesOperations operations
-    :vartype zones: azure.mgmt.dns.v2023_07_01_preview.aio.operations.ZonesOperations
+    :vartype zones: azure.mgmt.dns.v2018_05_01.aio.operations.ZonesOperations
     :ivar dns_resource_reference: DnsResourceReferenceOperations operations
     :vartype dns_resource_reference:
-     azure.mgmt.dns.v2023_07_01_preview.aio.operations.DnsResourceReferenceOperations
+     azure.mgmt.dns.v2018_05_01.aio.operations.DnsResourceReferenceOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :param subscription_id: Specifies the Azure subscription ID, which uniquely identifies the
+     Microsoft Azure subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-07-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-05-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -54,31 +52,24 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = DnsManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._client = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
-        self.dnssec_configs = DnssecConfigsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
-        self.record_sets = RecordSetsOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
-        self.zones = ZonesOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
-        )
+        self.record_sets = RecordSetsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.zones = ZonesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.dns_resource_reference = DnsResourceReferenceOperations(
-            self._client, self._config, self._serialize, self._deserialize, "2023-07-01-preview"
+            self._client, self._config, self._serialize, self._deserialize
         )
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/_configuration.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,45 +2,52 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+import sys
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class DnsManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
     """Configuration for DnsManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: The ID of the target subscription. Required.
+    :type credential: ~azure.core.credentials.TokenCredential
+    :param subscription_id: Specifies the Azure subscription ID, which uniquely identifies the
+     Microsoft Azure subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-07-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2018-05-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
         super(DnsManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-07-01-preview")
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", "2018-05-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,15 +59,15 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_zones_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_record_sets_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,644 +2,767 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._zones_operations import (
+from ...operations._record_sets_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
-    build_list_by_resource_group_request,
-    build_list_request,
+    build_list_all_by_dns_zone_request,
+    build_list_by_dns_zone_request,
+    build_list_by_type_request,
     build_update_request,
 )
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class ZonesOperations:
+class RecordSetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.aio.DnsManagementClient`'s
-        :attr:`zones` attribute.
+        :class:`~azure.mgmt.dns.v2018_05_01.aio.DnsManagementClient`'s
+        :attr:`record_sets` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
+
+    @overload
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        parameters: _models.RecordSet,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.RecordSet:
+        """Updates a record set within a DNS zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param parameters: Parameters supplied to the Update operation. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        parameters: IO,
+        if_match: Optional[str] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.RecordSet:
+        """Updates a record set within a DNS zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param parameters: Parameters supplied to the Update operation. Required.
+        :type parameters: IO
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def update(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        parameters: Union[_models.RecordSet, IO],
+        if_match: Optional[str] = None,
+        **kwargs: Any
+    ) -> _models.RecordSet:
+        """Updates a record set within a DNS zone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param parameters: Parameters supplied to the Update operation. Is either a RecordSet type or a
+         IO type. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet or IO
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
+         Default value is None.
+        :paramtype content_type: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(parameters, (IO, bytes)):
+            _content = parameters
+        else:
+            _json = self._serialize.body(parameters, "RecordSet")
+
+        request = build_update_request(
+            resource_group_name=resource_group_name,
+            zone_name=zone_name,
+            relative_record_set_name=relative_record_set_name,
+            record_type=record_type,
+            subscription_id=self._config.subscription_id,
+            if_match=if_match,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            template_url=self.update.metadata["url"],
+            headers=_headers,
+            params=_params,
+        )
+        request = _convert_request(request)
+        request.url = self._client.format_url(request.url)
+
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=False, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("RecordSet", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    update.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}"
+    }
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
-        parameters: _models.Zone,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        parameters: _models.RecordSet,
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Zone:
-        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+    ) -> _models.RecordSet:
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
-        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
-         an existing zone. Other values will be ignored. Default value is None.
+        :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
+         updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
         parameters: IO,
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Zone:
-        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+    ) -> _models.RecordSet:
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :param parameters: Parameters supplied to the CreateOrUpdate operation. Required.
         :type parameters: IO
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
-        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
-         an existing zone. Other values will be ignored. Default value is None.
+        :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
+         updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         zone_name: str,
-        parameters: Union[_models.Zone, IO],
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        parameters: Union[_models.RecordSet, IO],
         if_match: Optional[str] = None,
         if_none_match: Optional[str] = None,
         **kwargs: Any
-    ) -> _models.Zone:
-        """Creates or updates a DNS zone. Does not modify DNS records within the zone.
+    ) -> _models.RecordSet:
+        """Creates or updates a record set within a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
-        :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a Zone type
-         or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone or IO
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA can be
+         updated but not created (they are created when the DNS zone is created). Known values are: "A",
+         "AAAA", "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param parameters: Parameters supplied to the CreateOrUpdate operation. Is either a RecordSet
+         type or a IO type. Required.
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.RecordSet or IO
+        :param if_match: The etag of the record set. Omit this value to always overwrite the current
+         record set. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
          changes. Default value is None.
         :type if_match: str
-        :param if_none_match: Set to '*' to allow a new DNS zone to be created, but to prevent updating
-         an existing zone. Other values will be ignored. Default value is None.
+        :param if_none_match: Set to '*' to allow a new record set to be created, but to prevent
+         updating an existing record set. Other values will be ignored. Default value is None.
         :type if_none_match: str
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
+        cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
-            _json = self._serialize.body(parameters, "Zone")
+            _json = self._serialize.body(parameters, "RecordSet")
 
         request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
+            relative_record_set_name=relative_record_set_name,
+            record_type=record_type,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
             if_none_match=if_none_match,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
             template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("Zone", pipeline_response)
+            deserialized = self._deserialize("RecordSet", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("Zone", pipeline_response)
+            deserialized = self._deserialize("RecordSet", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}"
     }
 
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, zone_name: str, if_match: Optional[str] = None, **kwargs: Any
+    @distributed_trace_async
+    async def delete(  # pylint: disable=inconsistent-return-statements
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        if_match: Optional[str] = None,
+        **kwargs: Any
     ) -> None:
+        """Deletes a record set from a DNS zone. This operation cannot be undone.
+
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
+         Required.
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Record sets of type SOA cannot
+         be deleted (they are deleted when the DNS zone is deleted). Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param if_match: The etag of the record set. Omit this value to always delete the current
+         record set. Specify the last-seen etag value to prevent accidentally deleting any concurrent
+         changes. Default value is None.
+        :type if_match: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_delete_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
+            relative_record_set_name=relative_record_set_name,
+            record_type=record_type,
             subscription_id=self._config.subscription_id,
             if_match=if_match,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
+            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
         if cls:
-            return cls(pipeline_response, None, response_headers)
+            return cls(pipeline_response, None, {})
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
+    delete.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}"
     }
 
     @distributed_trace_async
-    async def begin_delete(
-        self, resource_group_name: str, zone_name: str, if_match: Optional[str] = None, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
-        """Deletes a DNS zone. WARNING: All DNS records in the zone will also be deleted. This operation
-        cannot be undone.
+    async def get(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        relative_record_set_name: str,
+        record_type: Union[str, _models.RecordType],
+        **kwargs: Any
+    ) -> _models.RecordSet:
+        """Gets a record set.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
-        :param if_match: The etag of the DNS zone. Omit this value to always delete the current zone.
-         Specify the last-seen etag value to prevent accidentally deleting any concurrent changes.
-         Default value is None.
-        :type if_match: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
-                resource_group_name=resource_group_name,
-                zone_name=zone_name,
-                if_match=if_match,
-                api_version=api_version,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
-            if cls:
-                return cls(pipeline_response, None, {})
-
-        if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
-        elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return AsyncLROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
-    }
-
-    @distributed_trace_async
-    async def get(self, resource_group_name: str, zone_name: str, **kwargs: Any) -> _models.Zone:
-        """Gets a DNS zone. Retrieves the zone properties, but not the record sets within the zone.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
+        :param relative_record_set_name: The name of the record set, relative to the name of the zone.
          Required.
-        :type resource_group_name: str
-        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
-        :type zone_name: str
+        :type relative_record_set_name: str
+        :param record_type: The type of DNS record in this record set. Known values are: "A", "AAAA",
+         "CAA", "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :return: RecordSet or the result of cls(response)
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.RecordSet
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.RecordSet] = kwargs.pop("cls", None)
 
         request = build_get_request(
             resource_group_name=resource_group_name,
             zone_name=zone_name,
+            relative_record_set_name=relative_record_set_name,
+            record_type=record_type,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("Zone", pipeline_response)
+        deserialized = self._deserialize("RecordSet", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}/{relativeRecordSetName}"
     }
 
-    @overload
-    async def update(
-        self,
-        resource_group_name: str,
-        zone_name: str,
-        parameters: _models.ZoneUpdate,
-        if_match: Optional[str] = None,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.Zone:
-        """Updates a DNS zone. Does not modify DNS records within the zone.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
-        :type zone_name: str
-        :param parameters: Parameters supplied to the Update operation. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.ZoneUpdate
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
-         changes. Default value is None.
-        :type if_match: str
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def update(
+    @distributed_trace
+    def list_by_type(
         self,
         resource_group_name: str,
         zone_name: str,
-        parameters: IO,
-        if_match: Optional[str] = None,
-        *,
-        content_type: str = "application/json",
+        record_type: Union[str, _models.RecordType],
+        top: Optional[int] = None,
+        recordsetnamesuffix: Optional[str] = None,
         **kwargs: Any
-    ) -> _models.Zone:
-        """Updates a DNS zone. Does not modify DNS records within the zone.
+    ) -> AsyncIterable["_models.RecordSet"]:
+        """Lists the record sets of a specified type in a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
         :param zone_name: The name of the DNS zone (without a terminating dot). Required.
         :type zone_name: str
-        :param parameters: Parameters supplied to the Update operation. Required.
-        :type parameters: IO
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
-         changes. Default value is None.
-        :type if_match: str
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
+        :param record_type: The type of record sets to enumerate. Known values are: "A", "AAAA", "CAA",
+         "CNAME", "MX", "NS", "PTR", "SOA", "SRV", and "TXT". Required.
+        :type record_type: str or ~azure.mgmt.dns.v2018_05_01.models.RecordType
+        :param top: The maximum number of record sets to return. If not specified, returns up to 100
+         record sets. Default value is None.
+        :type top: int
+        :param recordsetnamesuffix: The suffix label of the record set name that has to be used to
+         filter the record set enumerations. If this parameter is specified, Enumeration will return
+         only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
+        :type recordsetnamesuffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
+        :return: An iterator like instance of either RecordSet or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    @distributed_trace_async
-    async def update(
-        self,
-        resource_group_name: str,
-        zone_name: str,
-        parameters: Union[_models.ZoneUpdate, IO],
-        if_match: Optional[str] = None,
-        **kwargs: Any
-    ) -> _models.Zone:
-        """Updates a DNS zone. Does not modify DNS records within the zone.
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
-        :type zone_name: str
-        :param parameters: Parameters supplied to the Update operation. Is either a ZoneUpdate type or
-         a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.ZoneUpdate or IO
-        :param if_match: The etag of the DNS zone. Omit this value to always overwrite the current
-         zone. Specify the last-seen etag value to prevent accidentally overwriting any concurrent
-         changes. Default value is None.
-        :type if_match: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Zone or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.Zone
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Zone] = kwargs.pop("cls", None)
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(parameters, (IOBase, bytes)):
-            _content = parameters
-        else:
-            _json = self._serialize.body(parameters, "ZoneUpdate")
+                request = build_list_by_type_request(
+                    resource_group_name=resource_group_name,
+                    zone_name=zone_name,
+                    record_type=record_type,
+                    subscription_id=self._config.subscription_id,
+                    top=top,
+                    recordsetnamesuffix=recordsetnamesuffix,
+                    api_version=api_version,
+                    template_url=self.list_by_type.metadata["url"],
+                    headers=_headers,
+                    params=_params,
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
 
-        request = build_update_request(
-            resource_group_name=resource_group_name,
-            zone_name=zone_name,
-            subscription_id=self._config.subscription_id,
-            if_match=if_match,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.update.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                request = _convert_request(request)
+                request.url = self._client.format_url(request.url)
+                request.method = "GET"
+            return request
 
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("RecordSetListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        response = pipeline_response.http_response
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
 
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=False, **kwargs
+            )
+            response = pipeline_response.http_response
 
-        deserialized = self._deserialize("Zone", pipeline_response)
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+            return pipeline_response
 
-        return deserialized
+        return AsyncItemPaged(get_next, extract_data)
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}"
+    list_by_type.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/{recordType}"
     }
 
     @distributed_trace
-    def list_by_resource_group(
-        self, resource_group_name: str, top: Optional[int] = None, **kwargs: Any
-    ) -> AsyncIterable["_models.Zone"]:
-        """Lists the DNS zones within a resource group.
+    def list_by_dns_zone(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        top: Optional[int] = None,
+        recordsetnamesuffix: Optional[str] = None,
+        **kwargs: Any
+    ) -> AsyncIterable["_models.RecordSet"]:
+        """Lists all record sets in a DNS zone.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
         :param top: The maximum number of record sets to return. If not specified, returns up to 100
          record sets. Default value is None.
         :type top: int
+        :param recordsetnamesuffix: The suffix label of the record set name that has to be used to
+         filter the record set enumerations. If this parameter is specified, Enumeration will return
+         only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
+        :type recordsetnamesuffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.Zone]
+        :return: An iterator like instance of either RecordSet or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                request = build_list_by_dns_zone_request(
                     resource_group_name=resource_group_name,
+                    zone_name=zone_name,
                     subscription_id=self._config.subscription_id,
                     top=top,
+                    recordsetnamesuffix=recordsetnamesuffix,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
+                    template_url=self.list_by_dns_zone.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -657,78 +780,92 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ZoneListResult", pipeline_response)
+            deserialized = self._deserialize("RecordSetListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones"
+    list_by_dns_zone.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/recordsets"
     }
 
     @distributed_trace
-    def list(self, top: Optional[int] = None, **kwargs: Any) -> AsyncIterable["_models.Zone"]:
-        """Lists the DNS zones in all resource groups in a subscription.
+    def list_all_by_dns_zone(
+        self,
+        resource_group_name: str,
+        zone_name: str,
+        top: Optional[int] = None,
+        record_set_name_suffix: Optional[str] = None,
+        **kwargs: Any
+    ) -> AsyncIterable["_models.RecordSet"]:
+        """Lists all record sets in a DNS zone.
 
-        :param top: The maximum number of DNS zones to return. If not specified, returns up to 100
-         zones. Default value is None.
+        :param resource_group_name: The name of the resource group. Required.
+        :type resource_group_name: str
+        :param zone_name: The name of the DNS zone (without a terminating dot). Required.
+        :type zone_name: str
+        :param top: The maximum number of record sets to return. If not specified, returns up to 100
+         record sets. Default value is None.
         :type top: int
+        :param record_set_name_suffix: The suffix label of the record set name that has to be used to
+         filter the record set enumerations. If this parameter is specified, Enumeration will return
+         only records that end with .:code:`<recordSetNameSuffix>`. Default value is None.
+        :type record_set_name_suffix: str
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Zone or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2023_07_01_preview.models.Zone]
+        :return: An iterator like instance of either RecordSet or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.dns.v2018_05_01.models.RecordSet]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
-        cls: ClsType[_models.ZoneListResult] = kwargs.pop("cls", None)
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
+        cls: ClsType[_models.RecordSetListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                request = build_list_all_by_dns_zone_request(
+                    resource_group_name=resource_group_name,
+                    zone_name=zone_name,
                     subscription_id=self._config.subscription_id,
                     top=top,
+                    record_set_name_suffix=record_set_name_suffix,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
+                    template_url=self.list_all_by_dns_zone.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
 
             else:
@@ -746,31 +883,32 @@
                 )
                 request = _convert_request(request)
                 request.url = self._client.format_url(request.url)
                 request.method = "GET"
             return request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ZoneListResult", pipeline_response)
+            deserialized = self._deserialize("RecordSetListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                request, stream=False, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Network/dnszones"}
+    list_all_by_dns_zone.metadata = {
+        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/dnsZones/{zoneName}/all"
+    }
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_dns_resource_reference_operations.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/_dns_resource_reference_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
+import sys
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -24,52 +24,55 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._dns_resource_reference_operations import build_get_by_target_resources_request
 
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DnsResourceReferenceOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.dns.v2023_07_01_preview.aio.DnsManagementClient`'s
+        :class:`~azure.mgmt.dns.v2018_05_01.aio.DnsManagementClient`'s
         :attr:`dns_resource_reference` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        self._api_version = input_args.pop(0) if input_args else kwargs.pop("api_version")
 
     @overload
     async def get_by_target_resources(
         self, parameters: _models.DnsResourceReferenceRequest, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
         """Returns the DNS records specified by the referencing targetResourceIds.
 
         :param parameters: Properties for dns resource reference request. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceRequest
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def get_by_target_resources(
         self, parameters: IO, *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
@@ -78,56 +81,54 @@
         :param parameters: Properties for dns resource reference request. Required.
         :type parameters: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def get_by_target_resources(
         self, parameters: Union[_models.DnsResourceReferenceRequest, IO], **kwargs: Any
     ) -> _models.DnsResourceReferenceResult:
         """Returns the DNS records specified by the referencing targetResourceIds.
 
         :param parameters: Properties for dns resource reference request. Is either a
          DnsResourceReferenceRequest type or a IO type. Required.
-        :type parameters: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceRequest or IO
+        :type parameters: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceRequest or IO
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DnsResourceReferenceResult or the result of cls(response)
-        :rtype: ~azure.mgmt.dns.v2023_07_01_preview.models.DnsResourceReferenceResult
+        :rtype: ~azure.mgmt.dns.v2018_05_01.models.DnsResourceReferenceResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        api_version: str = kwargs.pop(
-            "api_version", _params.pop("api-version", self._api_version or "2023-07-01-preview")
-        )
+        api_version: Literal["2018-05-01"] = kwargs.pop("api_version", _params.pop("api-version", "2018-05-01"))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DnsResourceReferenceResult] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
+        if isinstance(parameters, (IO, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "DnsResourceReferenceRequest")
 
         request = build_get_by_target_resources_request(
             subscription_id=self._config.subscription_id,
             api_version=api_version,
@@ -137,17 +138,16 @@
             template_url=self.get_by_target_resources.metadata["url"],
             headers=_headers,
             params=_params,
         )
         request = _convert_request(request)
         request.url = self._client.format_url(request.url)
 
-        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            request, stream=False, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/aio/operations/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,79 +7,59 @@
 # --------------------------------------------------------------------------
 
 from ._models_py3 import ARecord
 from ._models_py3 import AaaaRecord
 from ._models_py3 import CaaRecord
 from ._models_py3 import CloudErrorBody
 from ._models_py3 import CnameRecord
-from ._models_py3 import DelegationSignerInfo
-from ._models_py3 import Digest
 from ._models_py3 import DnsResourceReference
 from ._models_py3 import DnsResourceReferenceRequest
 from ._models_py3 import DnsResourceReferenceResult
-from ._models_py3 import DnssecConfig
-from ._models_py3 import DnssecConfigListResult
-from ._models_py3 import DsRecord
 from ._models_py3 import MxRecord
-from ._models_py3 import NaptrRecord
 from ._models_py3 import NsRecord
 from ._models_py3 import PtrRecord
 from ._models_py3 import RecordSet
 from ._models_py3 import RecordSetListResult
 from ._models_py3 import RecordSetUpdateParameters
 from ._models_py3 import Resource
-from ._models_py3 import SigningKey
 from ._models_py3 import SoaRecord
 from ._models_py3 import SrvRecord
 from ._models_py3 import SubResource
-from ._models_py3 import SystemData
-from ._models_py3 import TlsaRecord
 from ._models_py3 import TxtRecord
 from ._models_py3 import Zone
 from ._models_py3 import ZoneListResult
 from ._models_py3 import ZoneUpdate
 
-from ._dns_management_client_enums import CreatedByType
 from ._dns_management_client_enums import RecordType
 from ._dns_management_client_enums import ZoneType
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ARecord",
     "AaaaRecord",
     "CaaRecord",
     "CloudErrorBody",
     "CnameRecord",
-    "DelegationSignerInfo",
-    "Digest",
     "DnsResourceReference",
     "DnsResourceReferenceRequest",
     "DnsResourceReferenceResult",
-    "DnssecConfig",
-    "DnssecConfigListResult",
-    "DsRecord",
     "MxRecord",
-    "NaptrRecord",
     "NsRecord",
     "PtrRecord",
     "RecordSet",
     "RecordSetListResult",
     "RecordSetUpdateParameters",
     "Resource",
-    "SigningKey",
     "SoaRecord",
     "SrvRecord",
     "SubResource",
-    "SystemData",
-    "TlsaRecord",
     "TxtRecord",
     "Zone",
     "ZoneListResult",
     "ZoneUpdate",
-    "CreatedByType",
     "RecordType",
     "ZoneType",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_patch.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2016_04_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2023_07_01_preview/models/_dns_management_client_enums.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_03_01_preview/models/_dns_management_client_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,39 +6,27 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
-class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The type of identity that created the resource."""
-
-    USER = "User"
-    APPLICATION = "Application"
-    MANAGED_IDENTITY = "ManagedIdentity"
-    KEY = "Key"
-
-
 class RecordType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """RecordType."""
 
     A = "A"
     AAAA = "AAAA"
     CAA = "CAA"
     CNAME = "CNAME"
     MX = "MX"
     NS = "NS"
     PTR = "PTR"
     SOA = "SOA"
     SRV = "SRV"
     TXT = "TXT"
-    TLSA = "TLSA"
-    DS = "DS"
-    NAPTR = "NAPTR"
 
 
 class ZoneType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of this DNS zone (Public or Private)."""
 
     PUBLIC = "Public"
     PRIVATE = "Private"
```

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/aio/operations/__init__.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-dns-8.1.0/azure/mgmt/dns/v2018_05_01/models/_models_py3.py` & `azure-mgmt-dns-8.1.0b1/azure/mgmt/dns/v2018_05_01/models/_models_py3.py`

 * *Files identical despite different names*

