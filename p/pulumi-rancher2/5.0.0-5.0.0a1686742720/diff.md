# Comparing `tmp/pulumi_rancher2-5.0.0.tar.gz` & `tmp/pulumi_rancher2-5.0.0a1686742720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-5.0.0.tar", last modified: Wed Jun 14 13:29:52 2023, max compression
+gzip compressed data, was "pulumi_rancher2-5.0.0a1686742720.tar", last modified: Wed Jun 14 11:44:51 2023, max compression
```

## Comparing `pulumi_rancher2-5.0.0.tar` & `pulumi_rancher2-5.0.0a1686742720.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1287410 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)   141124 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41552 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)  1602259 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:29:52.677234 pulumi_rancher2-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-14 13:29:52.000000 pulumi_rancher2-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1287410 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141124 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41552 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1602259 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:44:51.471551 pulumi_rancher2-5.0.0a1686742720/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 11:44:51.000000 pulumi_rancher2-5.0.0a1686742720/setup.py
```

### Comparing `pulumi_rancher2-5.0.0/PKG-INFO` & `pulumi_rancher2-5.0.0a1686742720/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 5.0.0
+Version: 5.0.0a1686742720
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.0.0/README.md` & `pulumi_rancher2-5.0.0a1686742720/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/__init__.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/active_directory.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/app.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/catalog.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/certificate.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alter_group.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_alter_rule.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/feature.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_app.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_alter_rule.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_project.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_role_tempalte.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/get_user.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/global_role.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/namespace.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/node_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/notifier.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/outputs.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/project.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/provider.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/registry.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/role_tempalte.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/role_template.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/secret.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/setting.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/token.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2/user.py` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rancher2
-Version: 5.0.0
+Version: 5.0.0a1686742720
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.0.0/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-5.0.0a1686742720/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.0.0/setup.py` & `pulumi_rancher2-5.0.0a1686742720/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.0.0"
-PLUGIN_VERSION = "5.0.0"
+VERSION = "5.0.0a1686742720"
+PLUGIN_VERSION = "5.0.0-alpha.1686742720+75dbe1d1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rancher2', PLUGIN_VERSION])
         except OSError as error:
```

