# Comparing `tmp/fim_utils-1.5.0rc4.tar.gz` & `tmp/fim_utils-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.5.0rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fim_utils-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.5.0rc4.tar` & `fim_utils-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fim_utils-1.5.0rc4/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.0rc4/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.0rc4/MANIFEST.in
--rw-r--r--   0        0        0     7348 2023-06-03 17:33:55.104520 fim_utils-1.5.0rc4/README.md
--rw-r--r--   0        0        0      159 2023-06-03 19:34:00.632390 fim_utils-1.5.0rc4/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.0rc4/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.0rc4/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.0rc4/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.0rc4/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.0rc4/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fim_utils-1.5.0rc4/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.0rc4/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.0rc4/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.0rc4/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fim_utils-1.5.0rc4/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.0rc4/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fim_utils-1.5.0rc4/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21991 2023-06-03 19:29:49.863195 fim_utils-1.5.0rc4/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fim_utils-1.5.0rc4/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fim_utils-1.5.0rc4/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.0rc4/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fim_utils-1.5.0rc4/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.0rc4/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.0rc4/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.0rc4/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fim_utils-1.5.0rc4/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fim_utils-1.5.0rc4/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fim_utils-1.5.0rc4/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1717 2023-06-02 22:02:16.828125 fim_utils-1.5.0rc4/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fim_utils-1.5.0rc4/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fim_utils-1.5.0rc4/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fim_utils-1.5.0rc4/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0      950 2023-06-03 18:07:08.151748 fim_utils-1.5.0rc4/pyproject.toml
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.0rc4/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.0rc4/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.0rc4/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.0rc4/test/ralph_test.py
--rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 fim_utils-1.5.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.1/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.1/MANIFEST.in
+-rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.1/README.md
+-rw-r--r--   0        0        0      156 2023-06-14 19:27:11.590636 fim_utils-1.5.1/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.1/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.1/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.1/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.1/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.1/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.1/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.1/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.1/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.1/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3456 2023-06-14 19:22:11.396659 fim_utils-1.5.1/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.1/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.1/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.1/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2505 2023-06-14 13:08:12.066017 fim_utils-1.5.1/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1226 2023-06-14 13:08:12.066616 fim_utils-1.5.1/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.1/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.1/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.1/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.1/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.1/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10922 2023-06-14 19:23:06.279493 fim_utils-1.5.1/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.1/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.1/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.1/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.1/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5488 2023-06-14 13:08:12.069995 fim_utils-1.5.1/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2015 2023-06-14 13:08:12.070557 fim_utils-1.5.1/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.1/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.1/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.1/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.1/test/ralph_test.py
+-rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.1/PKG-INFO
```

### Comparing `fim_utils-1.5.0rc4/.gitignore` & `fim_utils-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/LICENSE` & `fim_utils-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/README.md` & `fim_utils-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/al2s/arm.py` & `fim_utils-1.5.1/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/al2s/cloud_cfg.py` & `fim_utils-1.5.1/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/al2s/oess.py` & `fim_utils-1.5.1/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/netam/arm.py` & `fim_utils-1.5.1/fimutil/netam/arm.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         # add AL2S abstract switch node and ns
         al2s_node = self.topology.add_node(name='AL2S', site='AL2S',
                                            node_id='node+AL2S', ntype=f.NodeType.Switch,  stitch_node=True,
                                            capacities=f.Capacities(unit=1))
         al2s_l2_ns = al2s_node.add_network_service(name=al2s_node.name + '-ns', layer=f.Layer.L2,  stitch_node=True,
                                                    node_id=al2s_node.node_id + '-ns', nstype=f.ServiceType.MPLS)
-
+        regexVlanPort = re.compile(r'\/\d+/\d+\/\d+\.\d+$')
         # add site nodes
         for node in nodes:
             # add switch node
             node_name = node['name']
             # TODO: get model name from NSO
             model_name = 'NCS 55A1-36H'
             # TODO: get official site name from Ralph (or in switch description string) ?
@@ -161,30 +161,34 @@
                     port_mac = port['phys-address']
                     port_nid = f"port+{node_name}:{port_name}"
                     speed_gbps = int(int(port['speed']) / 1000000000)
                     # add capabilities
                     port_caps = f.Capacities(bw=speed_gbps)
                     # add labels (vlan ??)
                     port_labs = f.Labels(local_name=port_name, mac=port_mac)
+                    if 'ietf-ip:ipv6' in port and 'address' in port['ietf-ip:ipv6']:
+                        for ipv6_addr in port['ietf-ip:ipv6']['address']:
+                            ipv6_addr_ip = ipv6_addr['ip']
+                            ipv6_addr_prefix_len = ipv6_addr['prefix-length']
+                            port_labs = f.Labels().update(port_labs, local_name=port_name, ipv6=ipv6_addr_ip)
+                            # only take the first
+                            break
+                    elif regexVlanPort.search(port_name):  # skip if no ipv6 address (it's a slice vlan port)
+                        continue
                     if 'ietf-ip:ipv4' in port and 'address' in port['ietf-ip:ipv4']:
                         for ipv4_addr in port['ietf-ip:ipv4']['address']:
                             ipv4_addr_ip = ipv4_addr['ip']
                             ipv4_addr_mask = ipv4_addr['netmask']
                             port_labs = f.Labels().update(port_labs, local_name=port_name, ipv4=ipv4_addr_ip)
                             port_ipv4net_map[port_nid] = {"site": site_name, "port": port_name,
                                 "ip": ipv4_addr_ip, "netmask": ipv4_addr_mask}
                             # only take the first
                             break
-                    if 'ietf-ip:ipv6' in port and 'address' in port['ietf-ip:ipv6']:
-                        for ipv6_addr in port['ietf-ip:ipv6']['address']:
-                            ipv6_addr_ip = ipv6_addr['ip']
-                            ipv6_addr_prefix_len = ipv6_addr['prefix-length']
-                            port_labs = f.Labels().update(port_labs, local_name=port_name, ipv6=ipv6_addr_ip)
-                            # only take the first
-                            break
+                    elif regexVlanPort.search(port_name):  # skip if no ipv4 address (it's a slice vlan port)
+                        continue
                     sp = l2_ns.add_interface(name=port_name, itype=f.InterfaceType.TrunkPort,
                                              node_id=port_nid, labels=port_labs,
                                              capacities=port_caps)
                     if port_nid in port_ipv4net_map:
                         port_ipv4net_map[port_nid]["interface"] = sp
                     # add external facility stitching links
                     # refer to port_name as stitch_port
```

### Comparing `fim_utils-1.5.0rc4/fimutil/netam/nso.py` & `fim_utils-1.5.1/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/netam/sr_pce.py` & `fim_utils-1.5.1/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/asset.py` & `fim_utils-1.5.1/fimutil/ralph/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Ethernet = auto()
     EthernetCardPF = auto()
     EthernetCardVF = auto()
     Model = auto()
     Storage = auto()
     DPSwitch = auto()
     Abstract = auto()
+    FPGA = auto()
 
     def __str__(self):
         return self.name
 
 
 class RalphAsset(ABC):
     """
```

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.1/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.1/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.1/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/fpga.py` & `fim_utils-1.5.1/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/gpu.py` & `fim_utils-1.5.1/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/model.py` & `fim_utils-1.5.1/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/nvme.py` & `fim_utils-1.5.1/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.1/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/site.py` & `fim_utils-1.5.1/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/storage.py` & `fim_utils-1.5.1/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/ralph/worker_node.py` & `fim_utils-1.5.1/fimutil/ralph/worker_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             if comp.__dict__.get('type') and comp.type != RalphAssetType.EthernetCardVF:
                 d = comp.fields.copy()
                 d['Type'] = str(comp.type)
                 comps.append(d)
             elif not comp.__dict__.get('type'):
                 # GPU or FPGA
                 d = comp.__dict__.copy()
-                d['Type'] = str(RalphAssetType.GPU)
+                d['Type'] = str(RalphAssetType.GPU) if isinstance(comp, GPU) else str(RalphAssetType.FPGA)
                 comps.append(d)
         ret['Components'] = comps
         return ret
 
     def get_dp_ports(self):
         """
         Return a list of names of DP switch ports this node is connected to
```

### Comparing `fim_utils-1.5.0rc4/fimutil/utilities/generate_instance_flavors.py` & `fim_utils-1.5.1/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/utilities/scan_net.py` & `fim_utils-1.5.1/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/utilities/scan_oess.py` & `fim_utils-1.5.1/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/utilities/scan_site.py` & `fim_utils-1.5.1/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/fimutil/utilities/scan_worker.py` & `fim_utils-1.5.1/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/pyproject.toml` & `fim_utils-1.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.8"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fim-utils"
-authors = [{name = "Ilya Baldin", email = "ibaldin@renci.org"}, {name = "Xi Yang", email="xiyang@es.net"}]
+authors = [{name = "Ilya Baldin", email = "ibaldin@renci.org"}, {name = "Xi Yang", email="xiyang@es.net"}, {name="Hussamuddin Nasir", email="nasir@netlab.uky.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License",
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent"]
 dynamic = ["version", "description"]
 requires-python = '>=3.9'
```

### Comparing `fim_utils-1.5.0rc4/setup.py` & `fim_utils-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/test/netam_test.py` & `fim_utils-1.5.1/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc4/PKG-INFO` & `fim_utils-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.5.0rc4
+Version: 1.5.1
 Summary: This is a package of Information Model utilitied for FABRIC
-Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>
+Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Dist: fabric_fim >= 1.5.0
 Requires-Dist: pyjq == 2.6.0
```

