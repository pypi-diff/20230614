# Comparing `tmp/cdktf-proxmox-0.0.98.tar.gz` & `tmp/cdktf-proxmox-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-proxmox-0.0.98.tar", last modified: Sun Jun  4 00:34:38 2023, max compression
+gzip compressed data, was "cdktf-proxmox-0.0.99.tar", last modified: Mon Jun  5 00:31:52 2023, max compression
```

## Comparing `cdktf-proxmox-0.0.98.tar` & `cdktf-proxmox-0.0.99.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.853662 cdktf-proxmox-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.857662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   472462 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.98.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40294 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpools/
--rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvms/
--rw-r--r--   0 runner    (1001) docker     (123)    38851 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bonds/
--rw-r--r--   0 runner    (1001) docker     (123)    53915 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bridges/
--rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40607 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/
--rw-r--r--   0 runner    (1001) docker     (123)    41455 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvms/
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_nfs/
--rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_zfs/
--rw-r--r--   0 runner    (1001) docker     (123)    40422 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)    49186 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_resource_pools/
--rw-r--r--   0 runner    (1001) docker     (123)    48933 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_template/
--rw-r--r--   0 runner    (1001) docker     (123)    95525 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_templates/
--rw-r--r--   0 runner    (1001) docker     (123)   117070 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_virtual_machines/
--rw-r--r--   0 runner    (1001) docker     (123)   120407 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_pools/
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40435 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm/
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool/
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    25096 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.865662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bond/
--rw-r--r--   0 runner    (1001) docker     (123)    56269 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)    52889 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/nfs_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/nfs_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/resource_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    34782 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/resource_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   413855 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.869662 cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-06-04 00:34:21.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:34:38.861662 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-04 00:34:38.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-04 00:34:38.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:34:38.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 00:34:38.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 00:34:38.000000 cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.112079 cdktf-proxmox-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-05 00:31:52.112079 cdktf-proxmox-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 00:31:52.112079 cdktf-proxmox-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.100079 cdktf-proxmox-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   472457 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.99.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40294 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpools/
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvms/
+-rw-r--r--   0 runner    (1001) docker     (123)    38851 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)    53915 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40607 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/
+-rw-r--r--   0 runner    (1001) docker     (123)    41455 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvms/
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_nfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_zfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    40422 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    49186 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_resource_pools/
+-rw-r--r--   0 runner    (1001) docker     (123)    48933 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    95525 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   117070 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_virtual_machines/
+-rw-r--r--   0 runner    (1001) docker     (123)   120407 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_pools/
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40435 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm/
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool/
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    25096 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bond/
+-rw-r--r--   0 runner    (1001) docker     (123)    56269 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)    52889 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/nfs_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/nfs_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/resource_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    34782 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/resource_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.108080 cdktf-proxmox-0.0.99/src/cdktf_proxmox/virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   413855 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.112079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.112079 cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-06-05 00:31:37.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:31:52.104079 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-05 00:31:52.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-05 00:31:52.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:31:52.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 00:31:52.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 00:31:52.000000 cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/top_level.txt
```

### Comparing `cdktf-proxmox-0.0.98/LICENSE` & `cdktf-proxmox-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/PKG-INFO` & `cdktf-proxmox-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-proxmox
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends generated constructs from the Proxmox Terraform provider
 Home-page: https://github.com/awlsring/cdktf-proxmox.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-proxmox.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-proxmox-0.0.98/README.md` & `cdktf-proxmox-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/setup.py` & `cdktf-proxmox-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-proxmox",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "A package that vends generated constructs from the Proxmox Terraform provider",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-proxmox.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -52,15 +52,15 @@
         "cdktf_proxmox.resource_pool",
         "cdktf_proxmox.virtual_machine",
         "cdktf_proxmox.zfs_pool",
         "cdktf_proxmox.zfs_storage_class"
     ],
     "package_data": {
         "cdktf_proxmox._jsii": [
-            "cdktf-proxmox@0.0.98.jsii.tgz"
+            "cdktf-proxmox@0.0.99.jsii.tgz"
         ],
         "cdktf_proxmox": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_lvms/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_lvms/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_nodes/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_template/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_templates/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_storage_class/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bond/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bond/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/network_bridge/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/network_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/nfs_storage_class/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/nfs_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/provider/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/resource_pool/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/resource_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/virtual_machine/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/virtual_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_pool/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox/zfs_storage_class/__init__.py` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox/zfs_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/PKG-INFO` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-proxmox
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends generated constructs from the Proxmox Terraform provider
 Home-page: https://github.com/awlsring/cdktf-proxmox.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-proxmox.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-proxmox-0.0.98/src/cdktf_proxmox.egg-info/SOURCES.txt` & `cdktf-proxmox-0.0.99/src/cdktf_proxmox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_proxmox/py.typed
 src/cdktf_proxmox.egg-info/PKG-INFO
 src/cdktf_proxmox.egg-info/SOURCES.txt
 src/cdktf_proxmox.egg-info/dependency_links.txt
 src/cdktf_proxmox.egg-info/requires.txt
 src/cdktf_proxmox.egg-info/top_level.txt
 src/cdktf_proxmox/_jsii/__init__.py
-src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.98.jsii.tgz
+src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.99.jsii.tgz
 src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
 src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
 src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
 src/cdktf_proxmox/data_proxmox_lvms/__init__.py
 src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
 src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
 src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
```

