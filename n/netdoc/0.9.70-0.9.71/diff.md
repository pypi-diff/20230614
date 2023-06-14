# Comparing `tmp/netdoc-0.9.70.tar.gz` & `tmp/netdoc-0.9.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.70.tar", last modified: Fri May 26 13:54:47 2023, max compression
+gzip compressed data, was "netdoc-0.9.71.tar", last modified: Fri May 26 14:13:45 2023, max compression
```

## Comparing `netdoc-0.9.70.tar` & `netdoc-0.9.71.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 13:54:45.000000 netdoc-0.9.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 13:54:45.000000 netdoc-0.9.70/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 13:54:47.074940 netdoc-0.9.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-26 13:54:45.000000 netdoc-0.9.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc/discoverers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_ios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/netmiko_hp_comware.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/discoverers/netmiko_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/ingestors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/0007_discoverylog_supported.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/nornir_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/reports/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/reports/NetDoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/arptableentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/cable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/devicerole.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/devicetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/discoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/discoverylog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/macaddresstableentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/routetableentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/schemas/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/scripts/NetDoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.054940 netdoc-0.9.70/netdoc/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc/static/netdoc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.066940 netdoc-0.9.70/netdoc/static/netdoc/css/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/css/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/css/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   220164 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/css/vis-network.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.070940 netdoc-0.9.70/netdoc/static/netdoc/img/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/access-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/backup.png
--rw-r--r--   0 runner    (1001) docker     (123)    28633 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/circuit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/core-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/distribution-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/firewall.png
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/internal-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/non-racked-devices.png
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/power-feed.png
--rw-r--r--   0 runner    (1001) docker     (123)    18685 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/power-panel.png
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/power-units.png
--rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/provider-networks.png
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/router.png
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/server.png
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/storage.png
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/unknown.png
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/wan-network.png
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/img/wireless-ap.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.070940 netdoc-0.9.70/netdoc/static/netdoc/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/diagram.js
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/netdoc.js
--rw-r--r--   0 runner    (1001) docker     (123)   702066 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/vis-network.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1930592 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/netdoc/templates/netdoc/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/arptableentry.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/netdoc/templates/netdoc/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/buttons/discover.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/buttons/export.html
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/credential.html
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/diagram.html
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/discoverable.html
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/discoverable_discover.html
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/discoverable_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/discoverylog.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/netdoc/templates/netdoc/htmx/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/htmx/discover_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templates/netdoc/macaddresstableentry.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/netdoc/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/templatetags/netdoc_buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.074940 netdoc-0.9.70/netdoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/topologies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-05-26 13:54:45.000000 netdoc-0.9.70/netdoc/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:54:47.058940 netdoc-0.9.70/netdoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 13:54:47.000000 netdoc-0.9.70/netdoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 13:54:46.000000 netdoc-0.9.70/netdoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 13:54:47.074940 netdoc-0.9.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-26 13:54:46.000000 netdoc-0.9.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 14:13:43.000000 netdoc-0.9.71/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 14:13:43.000000 netdoc-0.9.71/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 14:13:45.081743 netdoc-0.9.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-26 14:13:43.000000 netdoc-0.9.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.065743 netdoc-0.9.71/netdoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 14:13:44.000000 netdoc-0.9.71/netdoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.065743 netdoc-0.9.71/netdoc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.065743 netdoc-0.9.71/netdoc/discoverers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/netmiko_hp_comware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/discoverers/netmiko_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.069743 netdoc-0.9.71/netdoc/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.073743 netdoc-0.9.71/netdoc/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/0007_discoverylog_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/nornir_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.073743 netdoc-0.9.71/netdoc/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/reports/NetDoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.073743 netdoc-0.9.71/netdoc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/arptableentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/cable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/devicerole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/devicetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/discoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/discoverylog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/macaddresstableentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/routetableentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/schemas/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.073743 netdoc-0.9.71/netdoc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/scripts/NetDoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.061743 netdoc-0.9.71/netdoc/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.061743 netdoc-0.9.71/netdoc/static/netdoc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.073743 netdoc-0.9.71/netdoc/static/netdoc/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/css/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/css/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   220164 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/css/vis-network.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.077743 netdoc-0.9.71/netdoc/static/netdoc/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/access-switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/backup.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28633 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/circuit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/core-switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/distribution-switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/firewall.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/internal-switch.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/power-feed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18685 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/power-panel.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/power-units.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/provider-networks.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/router.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/server.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/storage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/unknown.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/wan-network.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/img/wireless-ap.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.077743 netdoc-0.9.71/netdoc/static/netdoc/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/diagram.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/netdoc.js
+-rw-r--r--   0 runner    (1001) docker     (123)   702066 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/vis-network.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1930592 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.061743 netdoc-0.9.71/netdoc/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/netdoc/templates/netdoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/arptableentry.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/netdoc/templates/netdoc/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/buttons/discover.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/buttons/export.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/credential.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/diagram.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/discoverable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/discoverable_discover.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/discoverable_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/discoverylog.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/netdoc/templates/netdoc/htmx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templates/netdoc/macaddresstableentry.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/netdoc/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/templatetags/netdoc_buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.081743 netdoc-0.9.71/netdoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/topologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-05-26 14:13:43.000000 netdoc-0.9.71/netdoc/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:13:45.065743 netdoc-0.9.71/netdoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 14:13:45.000000 netdoc-0.9.71/netdoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 14:13:45.081743 netdoc-0.9.71/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-26 14:13:44.000000 netdoc-0.9.71/setup.py
```

### Comparing `netdoc-0.9.70/LICENSE` & `netdoc-0.9.71/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/README.md` & `netdoc-0.9.71/README.md`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/__init__.py` & `netdoc-0.9.71/netdoc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class NetdocConfig(PluginConfig):
     """Configuration class."""
 
     name = "netdoc"
     verbose_name = "NetDoc"
     description = "Automatic Network Documentation plugin for NetBox"
-    version = "0.9.70"
+    version = "0.9.71"
     author = "Andrea Dainese"
     author_email = "andrea@adainese.it"
     base_url = "netdoc"
     required_settings = ["NTC_TEMPLATES_DIR"]
     default_settings = {
         "MAX_INGESTED_LOGS": 50,
         "NTC_TEMPLATES_DIR": "/opt/ntc-templates/ntc_templates/templates",
```

### Comparing `netdoc-0.9.70/netdoc/api/serializers.py` & `netdoc-0.9.71/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/api/urls.py` & `netdoc-0.9.71/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/api/views.py` & `netdoc-0.9.71/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.71/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.71/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.71/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/filtersets.py` & `netdoc-0.9.71/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/forms.py` & `netdoc-0.9.71/netdoc/forms.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.71/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/migrations/0001_initial.py` & `netdoc-0.9.71/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.71/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.71/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.71/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.71/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/models.py` & `netdoc-0.9.71/netdoc/models.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/navigation.py` & `netdoc-0.9.71/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/nornir_inventory.py` & `netdoc-0.9.71/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/reports/NetDoc.py` & `netdoc-0.9.71/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/arptableentry.py` & `netdoc-0.9.71/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/cable.py` & `netdoc-0.9.71/netdoc/schemas/cable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/credential.py` & `netdoc-0.9.71/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/device.py` & `netdoc-0.9.71/netdoc/schemas/device.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/devicerole.py` & `netdoc-0.9.71/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/devicetype.py` & `netdoc-0.9.71/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/discoverable.py` & `netdoc-0.9.71/netdoc/schemas/discoverable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/discoverylog.py` & `netdoc-0.9.71/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/interface.py` & `netdoc-0.9.71/netdoc/schemas/interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/ipaddress.py` & `netdoc-0.9.71/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.71/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/manufacturer.py` & `netdoc-0.9.71/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/prefix.py` & `netdoc-0.9.71/netdoc/schemas/prefix.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/routetableentry.py` & `netdoc-0.9.71/netdoc/schemas/routetableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/site.py` & `netdoc-0.9.71/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/vlan.py` & `netdoc-0.9.71/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/schemas/vrf.py` & `netdoc-0.9.71/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/scripts/NetDoc.py` & `netdoc-0.9.71/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.71/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.71/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.71/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.71/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.71/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.71/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.71/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.71/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.71/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/tables.py` & `netdoc-0.9.71/netdoc/tables.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/tasks.py` & `netdoc-0.9.71/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.71/netdoc/templates/netdoc/arptableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.71/netdoc/templates/netdoc/credential.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.71/netdoc/templates/netdoc/diagram.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.71/netdoc/templates/netdoc/discoverable.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.71/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.71/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.71/netdoc/templates/netdoc/discoverable_list.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.71/netdoc/templates/netdoc/discoverylog.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.71/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.71/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.71/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.71/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/tests/test.py` & `netdoc-0.9.71/netdoc/tests/test.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/topologies.py` & `netdoc-0.9.71/netdoc/topologies.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/urls.py` & `netdoc-0.9.71/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/utils.py` & `netdoc-0.9.71/netdoc/utils.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc/views.py` & `netdoc-0.9.71/netdoc/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.71/netdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.70/setup.py` & `netdoc-0.9.71/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.70"
+__version__ = "0.9.71"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
```

