# Comparing `tmp/ibm-cloud-networking-services-0.8.0.tar.gz` & `tmp/ibm-cloud-networking-services-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-cloud-networking-services-0.8.0.tar", last modified: Tue Aug 17 07:18:29 2021, max compression
+gzip compressed data, was "dist/ibm-cloud-networking-services-0.9.0.tar", last modified: Mon Aug 30 22:18:48 2021, max compression
```

## Comparing `ibm-cloud-networking-services-0.8.0.tar` & `ibm-cloud-networking-services-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9613 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8588 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9613 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-17 07:09:54.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2334 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-17 07:18:29.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/
--rw-rw-r--   0 travis    (2000) travis    (2000)    37458 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39687 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/security_events_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117553 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/transit_gateway_apis_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39584 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/user_agent_blocking_rules_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22652 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_events_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92873 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/ssl_certificate_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11475 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_zones_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32006 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/custom_pages_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   305357 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zones_settings_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10767 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/permitted_networks_for_dns_zones_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50763 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/caching_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29258 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rule_groups_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17557 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_record_bulk_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43876 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/page_rule_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2471 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9245 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/cis_ip_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35606 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_records_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44540 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/range_applications_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   276113 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_svcs_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62764 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/resource_records_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28269 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rule_packages_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87236 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_rate_limits_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35995 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_monitor_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99325 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancers_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40533 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_lockdown_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18847 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/firewall_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11856 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46205 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_firewall_access_rules_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2699 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37298 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rules_api_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13018 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/routing_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36575 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zones_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   220083 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/direct_link_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42222 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_pools_v0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63706 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/direct_link_provider_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46130 2021-08-17 07:09:23.000000 ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/firewall_access_rules_v1.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9613 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8588 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      215 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9613 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-30 22:01:51.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2334 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-30 22:18:48.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37458 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39687 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/security_events_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117553 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/transit_gateway_apis_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39584 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/user_agent_blocking_rules_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22652 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_events_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92873 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/ssl_certificate_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11475 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_zones_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32006 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/custom_pages_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   305357 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zones_settings_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10767 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/permitted_networks_for_dns_zones_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50763 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/caching_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29258 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rule_groups_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17557 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_record_bulk_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43876 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/page_rule_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2471 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9245 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/cis_ip_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35606 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_records_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44540 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/range_applications_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   276113 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_svcs_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62764 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/resource_records_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28269 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rule_packages_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87236 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_rate_limits_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35995 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_monitor_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99325 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancers_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40533 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_lockdown_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18847 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/firewall_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11856 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46205 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_firewall_access_rules_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2699 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37298 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rules_api_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13018 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/routing_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36575 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zones_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   227808 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/direct_link_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42222 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_pools_v0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63706 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/direct_link_provider_v2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46130 2021-08-30 22:01:18.000000 ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/firewall_access_rules_v1.py
```

### Comparing `ibm-cloud-networking-services-0.8.0/PKG-INFO` & `ibm-cloud-networking-services-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-cloud-networking-services
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client library for IBM Cloud Networking Services
 Home-page: https://github.com/IBM/networking-python-sdk
 Author: IBM
 Author-email: devexdev@us.ibm.com
 License: Apache 2.0
 Keywords: ibm_cloud_networking_services
 Platform: UNKNOWN
@@ -28,15 +28,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 [![PyPI](https://img.shields.io/pypi/v/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/ibm-cloud-networking-services)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![codecov](https://codecov.io/gh/IBM/networking-python-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/IBM/networking-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Networking Services Python SDK Version 0.8.0
+# IBM Cloud Networking Services Python SDK Version 0.9.0
 
 Python client library to interact with various [IBM Cloud Networking Service APIs](https://cloud.ibm.com/apidocs?category=network).
 
 ## Table of Contents
 
 <!--
   The TOC below is generated using the `markdown-toc` node package.
@@ -121,21 +121,21 @@
 - Python 3.6 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-cloud-networking-services==0.8.0"
+pip install --upgrade "ibm-cloud-networking-services==0.9.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-cloud-networking-servies==0.8.0"
+easy_install --upgrade "ibm-cloud-networking-servies==0.9.0"
 ```
 
 ## Using the SDK
 
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 ## Questions
```

### Comparing `ibm-cloud-networking-services-0.8.0/README.md` & `ibm-cloud-networking-services-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 [![PyPI](https://img.shields.io/pypi/v/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/ibm-cloud-networking-services)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![codecov](https://codecov.io/gh/IBM/networking-python-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/IBM/networking-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Networking Services Python SDK Version 0.8.0
+# IBM Cloud Networking Services Python SDK Version 0.9.0
 
 Python client library to interact with various [IBM Cloud Networking Service APIs](https://cloud.ibm.com/apidocs?category=network).
 
 ## Table of Contents
 
 <!--
   The TOC below is generated using the `markdown-toc` node package.
@@ -96,21 +96,21 @@
 - Python 3.6 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-cloud-networking-services==0.8.0"
+pip install --upgrade "ibm-cloud-networking-services==0.9.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-cloud-networking-servies==0.8.0"
+easy_install --upgrade "ibm-cloud-networking-servies==0.9.0"
 ```
 
 ## Using the SDK
 
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 ## Questions
```

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/PKG-INFO` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-cloud-networking-services
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client library for IBM Cloud Networking Services
 Home-page: https://github.com/IBM/networking-python-sdk
 Author: IBM
 Author-email: devexdev@us.ibm.com
 License: Apache 2.0
 Keywords: ibm_cloud_networking_services
 Platform: UNKNOWN
@@ -28,15 +28,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 [![PyPI](https://img.shields.io/pypi/v/ibm-cloud-networking-services)](https://pypi.org/project/ibm-cloud-networking-services/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/ibm-cloud-networking-services)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![codecov](https://codecov.io/gh/IBM/networking-python-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/IBM/networking-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
-# IBM Cloud Networking Services Python SDK Version 0.8.0
+# IBM Cloud Networking Services Python SDK Version 0.9.0
 
 Python client library to interact with various [IBM Cloud Networking Service APIs](https://cloud.ibm.com/apidocs?category=network).
 
 ## Table of Contents
 
 <!--
   The TOC below is generated using the `markdown-toc` node package.
@@ -121,21 +121,21 @@
 - Python 3.6 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-cloud-networking-services==0.8.0"
+pip install --upgrade "ibm-cloud-networking-services==0.9.0"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-cloud-networking-servies==0.8.0"
+easy_install --upgrade "ibm-cloud-networking-servies==0.9.0"
 ```
 
 ## Using the SDK
 
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/master/README.md)
 
 ## Questions
```

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services.egg-info/SOURCES.txt` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/LICENSE` & `ibm-cloud-networking-services-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/setup.py` & `ibm-cloud-networking-services-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 PACKAGE_NAME = 'ibm_cloud_networking_services'
 PACKAGE_DESC = 'Python client library for IBM Cloud Networking Services'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/security_events_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/security_events_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/transit_gateway_apis_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/transit_gateway_apis_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/user_agent_blocking_rules_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/user_agent_blocking_rules_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_events_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_events_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/ssl_certificate_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/ssl_certificate_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_zones_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_zones_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/custom_pages_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/custom_pages_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zones_settings_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zones_settings_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/permitted_networks_for_dns_zones_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/permitted_networks_for_dns_zones_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/caching_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/caching_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rule_groups_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rule_groups_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_record_bulk_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_record_bulk_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/page_rule_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/page_rule_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/common.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/common.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/cis_ip_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/cis_ip_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_records_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_records_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/range_applications_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/range_applications_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/dns_svcs_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/dns_svcs_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/resource_records_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/resource_records_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rule_packages_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rule_packages_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_rate_limits_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_rate_limits_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_monitor_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_monitor_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancers_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancers_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_lockdown_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_lockdown_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/firewall_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/firewall_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zone_firewall_access_rules_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zone_firewall_access_rules_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/__init__.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/waf_rules_api_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/waf_rules_api_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/routing_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/routing_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/zones_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/zones_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/direct_link_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/direct_link_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,15 @@
         return response
 
 
     def update_gateway(self,
         id: str,
         *,
         authentication_key: 'GatewayPatchTemplateAuthenticationKey' = None,
+        connection_mode: str = None,
         global_: bool = None,
         loa_reject_reason: str = None,
         macsec_config: 'GatewayMacsecConfigPatchTemplate' = None,
         metered: bool = None,
         name: str = None,
         operational_status: str = None,
         speed_mbps: int = None,
@@ -279,14 +280,20 @@
 
         :param str id: Direct Link gateway identifier.
         :param GatewayPatchTemplateAuthenticationKey authentication_key: (optional)
                The identity of the standard key to use for BGP MD5 authentication key.
                The key material that you provide must be base64 encoded and original
                string must be maximum 126 ASCII characters in length.
                To clear the optional `authentication_key` field patch its crn to `""`.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param bool global_: (optional) Gateways with global routing (`true`) can
                connect to networks outside of their associated region.
         :param str loa_reject_reason: (optional) Use this field during LOA
                rejection to provide the reason for the rejection.
                Only allowed for type=dedicated gateways.
         :param GatewayMacsecConfigPatchTemplate macsec_config: (optional) MACsec
                configuration information.  When patching any macsec_config fields, no
@@ -322,14 +329,15 @@
 
         params = {
             'version': self.version
         }
 
         data = {
             'authentication_key': authentication_key,
+            'connection_mode': connection_mode,
             'global': global_,
             'loa_reject_reason': loa_reject_reason,
             'macsec_config': macsec_config,
             'metered': metered,
             'name': name,
             'operational_status': operational_status,
             'speed_mbps': speed_mbps
@@ -354,14 +362,15 @@
 
 
     def create_gateway_action(self,
         id: str,
         action: str,
         *,
         authentication_key: 'GatewayActionTemplateAuthenticationKey' = None,
+        connection_mode: str = None,
         global_: bool = None,
         metered: bool = None,
         resource_group: 'ResourceGroupIdentity' = None,
         updates: List[object] = None,
         **kwargs
     ) -> DetailedResponse:
         """
@@ -375,14 +384,20 @@
         :param str action: Action request.
         :param GatewayActionTemplateAuthenticationKey authentication_key:
                (optional) The identity of the standard key to use for BGP MD5
                authentication key.
                The key material that you provide must be base64 encoded and original
                string must be maximum 126 ASCII characters in length.
                To clear the optional `authentication_key` field patch its crn to `""`.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param bool global_: (optional) Required for create_gateway_approve
                requests to select the gateway's routing option.  Gateways with global
                routing (`true`) can connect to networks outside of their associated
                region.
         :param bool metered: (optional) Required for create_gateway_approve
                requests to select the gateway's metered billing option.  When `true`
                gateway usage is billed per gigabyte.  When `false` there is no per
@@ -418,14 +433,15 @@
         params = {
             'version': self.version
         }
 
         data = {
             'action': action,
             'authentication_key': authentication_key,
+            'connection_mode': connection_mode,
             'global': global_,
             'metered': metered,
             'resource_group': resource_group,
             'updates': updates
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
@@ -1281,14 +1297,19 @@
     :attr str carrier_name: (optional) Carrier name.  Only set for type=dedicated
           gateways.
     :attr GatewayChangeRequest change_request: (optional) Changes pending approval
           for provider managed Direct Link Connect gateways.
     :attr str completion_notice_reject_reason: (optional) Reason for completion
           notice rejection.  Only included on type=dedicated gateways with a rejected
           completion notice.
+    :attr str connection_mode: (optional) Type of services this Gateway is attached
+          to. Mode transit means this Gateway will be attached to Transit Gateway Service
+          and direct means this Gateway will be attached to vpc or classic connection. The
+          list of enumerated values for this property may expand in the future. Code and
+          processes using this field  must tolerate unexpected values.
     :attr datetime created_at: The date and time resource was created.
     :attr str crn: The CRN (Cloud Resource Name) of this gateway.
     :attr str cross_connect_router: (optional) Cross connect router.  Only included
           on type=dedicated gateways.
     :attr str customer_name: (optional) Customer name.  Only set for type=dedicated
           gateways.
     :attr bool global_: Gateways with global routing (`true`) can connect to
@@ -1342,14 +1363,15 @@
                  bgp_cer_cidr: str = None,
                  bgp_ibm_asn: int = None,
                  bgp_ibm_cidr: str = None,
                  bgp_status: str = None,
                  carrier_name: str = None,
                  change_request: 'GatewayChangeRequest' = None,
                  completion_notice_reject_reason: str = None,
+                 connection_mode: str = None,
                  cross_connect_router: str = None,
                  customer_name: str = None,
                  link_status: str = None,
                  macsec_config: 'GatewayMacsecConfig' = None,
                  port: 'GatewayPort' = None,
                  provider_api_managed: bool = None,
                  resource_group: 'ResourceGroupReference' = None,
@@ -1396,14 +1418,20 @@
         :param str carrier_name: (optional) Carrier name.  Only set for
                type=dedicated gateways.
         :param GatewayChangeRequest change_request: (optional) Changes pending
                approval for provider managed Direct Link Connect gateways.
         :param str completion_notice_reject_reason: (optional) Reason for
                completion notice rejection.  Only included on type=dedicated gateways with
                a rejected completion notice.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param str cross_connect_router: (optional) Cross connect router.  Only
                included on type=dedicated gateways.
         :param str customer_name: (optional) Customer name.  Only set for
                type=dedicated gateways.
         :param str link_status: (optional) Gateway link status.  Only included on
                type=dedicated gateways. The list of enumerated values for this property
                may expand in the future. Code and processes using this field  must
@@ -1425,14 +1453,15 @@
         self.bgp_cer_cidr = bgp_cer_cidr
         self.bgp_ibm_asn = bgp_ibm_asn
         self.bgp_ibm_cidr = bgp_ibm_cidr
         self.bgp_status = bgp_status
         self.carrier_name = carrier_name
         self.change_request = change_request
         self.completion_notice_reject_reason = completion_notice_reject_reason
+        self.connection_mode = connection_mode
         self.created_at = created_at
         self.crn = crn
         self.cross_connect_router = cross_connect_router
         self.customer_name = customer_name
         self.global_ = global_
         self.id = id
         self.link_status = link_status
@@ -1471,14 +1500,16 @@
             args['bgp_status'] = _dict.get('bgp_status')
         if 'carrier_name' in _dict:
             args['carrier_name'] = _dict.get('carrier_name')
         if 'change_request' in _dict:
             args['change_request'] = _dict.get('change_request')
         if 'completion_notice_reject_reason' in _dict:
             args['completion_notice_reject_reason'] = _dict.get('completion_notice_reject_reason')
+        if 'connection_mode' in _dict:
+            args['connection_mode'] = _dict.get('connection_mode')
         if 'created_at' in _dict:
             args['created_at'] = string_to_datetime(_dict.get('created_at'))
         else:
             raise ValueError('Required property \'created_at\' not present in Gateway JSON')
         if 'crn' in _dict:
             args['crn'] = _dict.get('crn')
         else:
@@ -1561,14 +1592,16 @@
             _dict['bgp_status'] = self.bgp_status
         if hasattr(self, 'carrier_name') and self.carrier_name is not None:
             _dict['carrier_name'] = self.carrier_name
         if hasattr(self, 'change_request') and self.change_request is not None:
             _dict['change_request'] = self.change_request
         if hasattr(self, 'completion_notice_reject_reason') and self.completion_notice_reject_reason is not None:
             _dict['completion_notice_reject_reason'] = self.completion_notice_reject_reason
+        if hasattr(self, 'connection_mode') and self.connection_mode is not None:
+            _dict['connection_mode'] = self.connection_mode
         if hasattr(self, 'created_at') and self.created_at is not None:
             _dict['created_at'] = datetime_to_string(self.created_at)
         if hasattr(self, 'crn') and self.crn is not None:
             _dict['crn'] = self.crn
         if hasattr(self, 'cross_connect_router') and self.cross_connect_router is not None:
             _dict['cross_connect_router'] = self.cross_connect_router
         if hasattr(self, 'customer_name') and self.customer_name is not None:
@@ -1630,14 +1663,26 @@
         """
         ACTIVE = "active"
         CONNECT = "connect"
         ESTABLISHED = "established"
         IDLE = "idle"
 
 
+    class ConnectionModeEnum(Enum):
+        """
+        Type of services this Gateway is attached to. Mode transit means this Gateway will
+        be attached to Transit Gateway Service and direct means this Gateway will be
+        attached to vpc or classic connection. The list of enumerated values for this
+        property may expand in the future. Code and processes using this field  must
+        tolerate unexpected values.
+        """
+        DIRECT = "direct"
+        TRANSIT = "transit"
+
+
     class LinkStatusEnum(Enum):
         """
         Gateway link status.  Only included on type=dedicated gateways. The list of
         enumerated values for this property may expand in the future. Code and processes
         using this field  must tolerate unexpected values.
         """
         DOWN = "down"
@@ -3088,14 +3133,19 @@
     :attr str bgp_ibm_cidr: (optional) BGP IBM CIDR.
           For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
           automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
           For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR, the
           value must reside in one of "10.254.0.0/16", "172.16.0.0/12", "192.168.0.0/16",
           "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr and bgp_ibm_cidr must
           have matching network and subnet mask values.
+    :attr str connection_mode: (optional) Type of services this Gateway is attached
+          to. Mode transit means this Gateway will be attached to Transit Gateway Service
+          and direct means this Gateway will be attached to vpc or classic connection. The
+          list of enumerated values for this property may expand in the future. Code and
+          processes using this field  must tolerate unexpected values.
     :attr bool global_: Gateways with global routing (`true`) can connect to
           networks outside their associated region.
     :attr bool metered: Metered billing option.  When `true` gateway usage is billed
           per gigabyte.  When `false` there is no per gigabyte usage charge, instead a
           flat rate is charged for the gateway.
     :attr str name: The unique user-defined name for this gateway.
     :attr ResourceGroupIdentity resource_group: (optional) Resource group for this
@@ -3113,14 +3163,15 @@
                  speed_mbps: int,
                  type: str,
                  *,
                  authentication_key: 'GatewayTemplateAuthenticationKey' = None,
                  bgp_base_cidr: str = None,
                  bgp_cer_cidr: str = None,
                  bgp_ibm_cidr: str = None,
+                 connection_mode: str = None,
                  resource_group: 'ResourceGroupIdentity' = None) -> None:
         """
         Initialize a GatewayTemplate object.
 
         :param int bgp_asn: BGP ASN.
         :param bool global_: Gateways with global routing (`true`) can connect to
                networks outside their associated region.
@@ -3151,23 +3202,41 @@
         :param str bgp_ibm_cidr: (optional) BGP IBM CIDR.
                For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
                automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
                For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR,
                the value must reside in one of "10.254.0.0/16", "172.16.0.0/12",
                "192.168.0.0/16", "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr
                and bgp_ibm_cidr must have matching network and subnet mask values.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param ResourceGroupIdentity resource_group: (optional) Resource group for
                this resource. If unspecified, the account's [default resource
                group](https://cloud.ibm.com/apidocs/resource-manager#introduction) is
                used.
         """
         msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
                   ", ".join(['GatewayTemplateGatewayTypeDedicatedTemplate', 'GatewayTemplateGatewayTypeConnectTemplate']))
         raise Exception(msg)
 
+    class ConnectionModeEnum(Enum):
+        """
+        Type of services this Gateway is attached to. Mode transit means this Gateway will
+        be attached to Transit Gateway Service and direct means this Gateway will be
+        attached to vpc or classic connection. The list of enumerated values for this
+        property may expand in the future. Code and processes using this field  must
+        tolerate unexpected values.
+        """
+        DIRECT = "direct"
+        TRANSIT = "transit"
+
+
     class TypeEnum(Enum):
         """
         Offering type.
         """
         CONNECT = "connect"
         DEDICATED = "dedicated"
 
@@ -4694,14 +4763,19 @@
     :attr str bgp_ibm_cidr: (optional) BGP IBM CIDR.
           For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
           automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
           For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR, the
           value must reside in one of "10.254.0.0/16", "172.16.0.0/12", "192.168.0.0/16",
           "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr and bgp_ibm_cidr must
           have matching network and subnet mask values.
+    :attr str connection_mode: (optional) Type of services this Gateway is attached
+          to. Mode transit means this Gateway will be attached to Transit Gateway Service
+          and direct means this Gateway will be attached to vpc or classic connection. The
+          list of enumerated values for this property may expand in the future. Code and
+          processes using this field  must tolerate unexpected values.
     :attr bool global_: Gateways with global routing (`true`) can connect to
           networks outside their associated region.
     :attr bool metered: Metered billing option.  When `true` gateway usage is billed
           per gigabyte.  When `false` there is no per gigabyte usage charge, instead a
           flat rate is charged for the gateway.
     :attr str name: The unique user-defined name for this gateway.
     :attr ResourceGroupIdentity resource_group: (optional) Resource group for this
@@ -4721,14 +4795,15 @@
                  type: str,
                  port: 'GatewayPortIdentity',
                  *,
                  authentication_key: 'GatewayTemplateGatewayTypeConnectTemplateAuthenticationKey' = None,
                  bgp_base_cidr: str = None,
                  bgp_cer_cidr: str = None,
                  bgp_ibm_cidr: str = None,
+                 connection_mode: str = None,
                  resource_group: 'ResourceGroupIdentity' = None) -> None:
         """
         Initialize a GatewayTemplateGatewayTypeConnectTemplate object.
 
         :param int bgp_asn: BGP ASN.
         :param bool global_: Gateways with global routing (`true`) can connect to
                networks outside their associated region.
@@ -4762,25 +4837,32 @@
         :param str bgp_ibm_cidr: (optional) BGP IBM CIDR.
                For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
                automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
                For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR,
                the value must reside in one of "10.254.0.0/16", "172.16.0.0/12",
                "192.168.0.0/16", "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr
                and bgp_ibm_cidr must have matching network and subnet mask values.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param ResourceGroupIdentity resource_group: (optional) Resource group for
                this resource. If unspecified, the account's [default resource
                group](https://cloud.ibm.com/apidocs/resource-manager#introduction) is
                used.
         """
         # pylint: disable=super-init-not-called
         self.authentication_key = authentication_key
         self.bgp_asn = bgp_asn
         self.bgp_base_cidr = bgp_base_cidr
         self.bgp_cer_cidr = bgp_cer_cidr
         self.bgp_ibm_cidr = bgp_ibm_cidr
+        self.connection_mode = connection_mode
         self.global_ = global_
         self.metered = metered
         self.name = name
         self.resource_group = resource_group
         self.speed_mbps = speed_mbps
         self.type = type
         self.port = port
@@ -4797,14 +4879,16 @@
             raise ValueError('Required property \'bgp_asn\' not present in GatewayTemplateGatewayTypeConnectTemplate JSON')
         if 'bgp_base_cidr' in _dict:
             args['bgp_base_cidr'] = _dict.get('bgp_base_cidr')
         if 'bgp_cer_cidr' in _dict:
             args['bgp_cer_cidr'] = _dict.get('bgp_cer_cidr')
         if 'bgp_ibm_cidr' in _dict:
             args['bgp_ibm_cidr'] = _dict.get('bgp_ibm_cidr')
+        if 'connection_mode' in _dict:
+            args['connection_mode'] = _dict.get('connection_mode')
         if 'global' in _dict:
             args['global_'] = _dict.get('global')
         else:
             raise ValueError('Required property \'global\' not present in GatewayTemplateGatewayTypeConnectTemplate JSON')
         if 'metered' in _dict:
             args['metered'] = _dict.get('metered')
         else:
@@ -4843,14 +4927,16 @@
             _dict['bgp_asn'] = self.bgp_asn
         if hasattr(self, 'bgp_base_cidr') and self.bgp_base_cidr is not None:
             _dict['bgp_base_cidr'] = self.bgp_base_cidr
         if hasattr(self, 'bgp_cer_cidr') and self.bgp_cer_cidr is not None:
             _dict['bgp_cer_cidr'] = self.bgp_cer_cidr
         if hasattr(self, 'bgp_ibm_cidr') and self.bgp_ibm_cidr is not None:
             _dict['bgp_ibm_cidr'] = self.bgp_ibm_cidr
+        if hasattr(self, 'connection_mode') and self.connection_mode is not None:
+            _dict['connection_mode'] = self.connection_mode
         if hasattr(self, 'global_') and self.global_ is not None:
             _dict['global'] = self.global_
         if hasattr(self, 'metered') and self.metered is not None:
             _dict['metered'] = self.metered
         if hasattr(self, 'name') and self.name is not None:
             _dict['name'] = self.name
         if hasattr(self, 'resource_group') and self.resource_group is not None:
@@ -4877,14 +4963,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'GatewayTemplateGatewayTypeConnectTemplate') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
+    class ConnectionModeEnum(Enum):
+        """
+        Type of services this Gateway is attached to. Mode transit means this Gateway will
+        be attached to Transit Gateway Service and direct means this Gateway will be
+        attached to vpc or classic connection. The list of enumerated values for this
+        property may expand in the future. Code and processes using this field  must
+        tolerate unexpected values.
+        """
+        DIRECT = "direct"
+        TRANSIT = "transit"
+
+
     class TypeEnum(Enum):
         """
         Offering type.
         """
         CONNECT = "connect"
         DEDICATED = "dedicated"
 
@@ -4916,14 +5014,19 @@
     :attr str bgp_ibm_cidr: (optional) BGP IBM CIDR.
           For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
           automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
           For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR, the
           value must reside in one of "10.254.0.0/16", "172.16.0.0/12", "192.168.0.0/16",
           "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr and bgp_ibm_cidr must
           have matching network and subnet mask values.
+    :attr str connection_mode: (optional) Type of services this Gateway is attached
+          to. Mode transit means this Gateway will be attached to Transit Gateway Service
+          and direct means this Gateway will be attached to vpc or classic connection. The
+          list of enumerated values for this property may expand in the future. Code and
+          processes using this field  must tolerate unexpected values.
     :attr bool global_: Gateways with global routing (`true`) can connect to
           networks outside their associated region.
     :attr bool metered: Metered billing option.  When `true` gateway usage is billed
           per gigabyte.  When `false` there is no per gigabyte usage charge, instead a
           flat rate is charged for the gateway.
     :attr str name: The unique user-defined name for this gateway.
     :attr ResourceGroupIdentity resource_group: (optional) Resource group for this
@@ -4951,14 +5054,15 @@
                  customer_name: str,
                  location_name: str,
                  *,
                  authentication_key: 'GatewayTemplateGatewayTypeDedicatedTemplateAuthenticationKey' = None,
                  bgp_base_cidr: str = None,
                  bgp_cer_cidr: str = None,
                  bgp_ibm_cidr: str = None,
+                 connection_mode: str = None,
                  resource_group: 'ResourceGroupIdentity' = None,
                  macsec_config: 'GatewayMacsecConfigTemplate' = None) -> None:
         """
         Initialize a GatewayTemplateGatewayTypeDedicatedTemplate object.
 
         :param int bgp_asn: BGP ASN.
         :param bool global_: Gateways with global routing (`true`) can connect to
@@ -4995,27 +5099,34 @@
         :param str bgp_ibm_cidr: (optional) BGP IBM CIDR.
                For auto IP assignment, omit bgp_cer_cidr and bgp_ibm_cidr.  IBM will
                automatically select values for bgp_cer_cidr and bgp_ibm_cidr.
                For explicit IP assignment set a valid bgp_cer_cidr and bgp_ibm_cidr CIDR,
                the value must reside in one of "10.254.0.0/16", "172.16.0.0/12",
                "192.168.0.0/16", "169.254.0.0/16" or an owned public CIDR.  bgp_cer_cidr
                and bgp_ibm_cidr must have matching network and subnet mask values.
+        :param str connection_mode: (optional) Type of services this Gateway is
+               attached to. Mode transit means this Gateway will be attached to Transit
+               Gateway Service and direct means this Gateway will be attached to vpc or
+               classic connection. The list of enumerated values for this property may
+               expand in the future. Code and processes using this field  must tolerate
+               unexpected values.
         :param ResourceGroupIdentity resource_group: (optional) Resource group for
                this resource. If unspecified, the account's [default resource
                group](https://cloud.ibm.com/apidocs/resource-manager#introduction) is
                used.
         :param GatewayMacsecConfigTemplate macsec_config: (optional) MACsec
                configuration information.  Contact IBM support for access to MACsec.
         """
         # pylint: disable=super-init-not-called
         self.authentication_key = authentication_key
         self.bgp_asn = bgp_asn
         self.bgp_base_cidr = bgp_base_cidr
         self.bgp_cer_cidr = bgp_cer_cidr
         self.bgp_ibm_cidr = bgp_ibm_cidr
+        self.connection_mode = connection_mode
         self.global_ = global_
         self.metered = metered
         self.name = name
         self.resource_group = resource_group
         self.speed_mbps = speed_mbps
         self.type = type
         self.carrier_name = carrier_name
@@ -5036,14 +5147,16 @@
             raise ValueError('Required property \'bgp_asn\' not present in GatewayTemplateGatewayTypeDedicatedTemplate JSON')
         if 'bgp_base_cidr' in _dict:
             args['bgp_base_cidr'] = _dict.get('bgp_base_cidr')
         if 'bgp_cer_cidr' in _dict:
             args['bgp_cer_cidr'] = _dict.get('bgp_cer_cidr')
         if 'bgp_ibm_cidr' in _dict:
             args['bgp_ibm_cidr'] = _dict.get('bgp_ibm_cidr')
+        if 'connection_mode' in _dict:
+            args['connection_mode'] = _dict.get('connection_mode')
         if 'global' in _dict:
             args['global_'] = _dict.get('global')
         else:
             raise ValueError('Required property \'global\' not present in GatewayTemplateGatewayTypeDedicatedTemplate JSON')
         if 'metered' in _dict:
             args['metered'] = _dict.get('metered')
         else:
@@ -5096,14 +5209,16 @@
             _dict['bgp_asn'] = self.bgp_asn
         if hasattr(self, 'bgp_base_cidr') and self.bgp_base_cidr is not None:
             _dict['bgp_base_cidr'] = self.bgp_base_cidr
         if hasattr(self, 'bgp_cer_cidr') and self.bgp_cer_cidr is not None:
             _dict['bgp_cer_cidr'] = self.bgp_cer_cidr
         if hasattr(self, 'bgp_ibm_cidr') and self.bgp_ibm_cidr is not None:
             _dict['bgp_ibm_cidr'] = self.bgp_ibm_cidr
+        if hasattr(self, 'connection_mode') and self.connection_mode is not None:
+            _dict['connection_mode'] = self.connection_mode
         if hasattr(self, 'global_') and self.global_ is not None:
             _dict['global'] = self.global_
         if hasattr(self, 'metered') and self.metered is not None:
             _dict['metered'] = self.metered
         if hasattr(self, 'name') and self.name is not None:
             _dict['name'] = self.name
         if hasattr(self, 'resource_group') and self.resource_group is not None:
@@ -5138,14 +5253,26 @@
             return False
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'GatewayTemplateGatewayTypeDedicatedTemplate') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
+    class ConnectionModeEnum(Enum):
+        """
+        Type of services this Gateway is attached to. Mode transit means this Gateway will
+        be attached to Transit Gateway Service and direct means this Gateway will be
+        attached to vpc or classic connection. The list of enumerated values for this
+        property may expand in the future. Code and processes using this field  must
+        tolerate unexpected values.
+        """
+        DIRECT = "direct"
+        TRANSIT = "transit"
+
+
     class TypeEnum(Enum):
         """
         Offering type.
         """
         CONNECT = "connect"
         DEDICATED = "dedicated"
```

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/global_load_balancer_pools_v0.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/global_load_balancer_pools_v0.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/direct_link_provider_v2.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/direct_link_provider_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-networking-services-0.8.0/ibm_cloud_networking_services/firewall_access_rules_v1.py` & `ibm-cloud-networking-services-0.9.0/ibm_cloud_networking_services/firewall_access_rules_v1.py`

 * *Files identical despite different names*

