# Comparing `tmp/fim_utils-1.5.0rc3.tar.gz` & `tmp/fim_utils-1.5.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.5.0rc3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fim_utils-1.5.0rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.5.0rc3.tar` & `fim_utils-1.5.0rc4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fim_utils-1.5.0rc3/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.0rc3/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.0rc3/MANIFEST.in
--rw-r--r--   0        0        0     7348 2023-06-03 17:33:55.104520 fim_utils-1.5.0rc3/README.md
--rw-r--r--   0        0        0      159 2023-06-02 22:05:34.391169 fim_utils-1.5.0rc3/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.0rc3/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.0rc3/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.0rc3/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.0rc3/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.0rc3/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fim_utils-1.5.0rc3/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.0rc3/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.0rc3/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.0rc3/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fim_utils-1.5.0rc3/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.0rc3/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fim_utils-1.5.0rc3/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21981 2023-06-02 21:31:39.454775 fim_utils-1.5.0rc3/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fim_utils-1.5.0rc3/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fim_utils-1.5.0rc3/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.0rc3/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fim_utils-1.5.0rc3/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.0rc3/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.0rc3/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.0rc3/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fim_utils-1.5.0rc3/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fim_utils-1.5.0rc3/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fim_utils-1.5.0rc3/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1717 2023-06-02 22:02:16.828125 fim_utils-1.5.0rc3/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fim_utils-1.5.0rc3/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fim_utils-1.5.0rc3/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fim_utils-1.5.0rc3/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0      950 2023-06-03 18:07:08.151748 fim_utils-1.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.0rc3/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.0rc3/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.0rc3/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.0rc3/test/ralph_test.py
--rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 fim_utils-1.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-02 21:51:15.709071 fim_utils-1.5.0rc4/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.0rc4/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.0rc4/MANIFEST.in
+-rw-r--r--   0        0        0     7348 2023-06-03 17:33:55.104520 fim_utils-1.5.0rc4/README.md
+-rw-r--r--   0        0        0      159 2023-06-03 19:34:00.632390 fim_utils-1.5.0rc4/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.0rc4/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.0rc4/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.0rc4/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.0rc4/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.0rc4/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19470 2023-01-20 02:29:04.877342 fim_utils-1.5.0rc4/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.0rc4/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.0rc4/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.0rc4/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3438 2022-10-26 01:51:00.891038 fim_utils-1.5.0rc4/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.0rc4/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-02 21:36:39.501897 fim_utils-1.5.0rc4/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21991 2023-06-03 19:29:49.863195 fim_utils-1.5.0rc4/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2505 2023-06-02 20:18:56.236739 fim_utils-1.5.0rc4/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1226 2023-06-02 20:19:05.598976 fim_utils-1.5.0rc4/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.0rc4/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-02 20:24:36.439237 fim_utils-1.5.0rc4/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.0rc4/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.0rc4/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.0rc4/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10867 2023-06-02 20:44:12.833883 fim_utils-1.5.0rc4/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:33:21.137112 fim_utils-1.5.0rc4/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2022-10-26 01:51:00.895483 fim_utils-1.5.0rc4/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-02 22:02:16.828125 fim_utils-1.5.0rc4/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-02 21:43:09.370334 fim_utils-1.5.0rc4/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5488 2023-06-02 21:42:49.420007 fim_utils-1.5.0rc4/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2015 2023-06-02 21:42:18.865192 fim_utils-1.5.0rc4/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0      950 2023-06-03 18:07:08.151748 fim_utils-1.5.0rc4/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.0rc4/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.0rc4/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.0rc4/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.0rc4/test/ralph_test.py
+-rw-r--r--   0        0        0     8031 1970-01-01 00:00:00.000000 fim_utils-1.5.0rc4/PKG-INFO
```

### Comparing `fim_utils-1.5.0rc3/.gitignore` & `fim_utils-1.5.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/LICENSE` & `fim_utils-1.5.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/README.md` & `fim_utils-1.5.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/al2s/arm.py` & `fim_utils-1.5.0rc4/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/al2s/cloud_cfg.py` & `fim_utils-1.5.0rc4/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/al2s/oess.py` & `fim_utils-1.5.0rc4/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/netam/arm.py` & `fim_utils-1.5.0rc4/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/netam/nso.py` & `fim_utils-1.5.0rc4/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/netam/sr_pce.py` & `fim_utils-1.5.0rc4/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/asset.py` & `fim_utils-1.5.0rc4/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.0rc4/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.0rc4/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.0rc4/fimutil/ralph/fim_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             units = 0
             labs = list()
             child_bdfs = list()
             child_numas = list()
             for pf_parent in v:
                 child_vfs = org.get_vfs_of_parent(pf_parent.fields['BDF'])
                 macs, bdfs, vlans, numas = __convert_vf_list_to_interface_labels(child_vfs)
-                labs.append(Labels(mac=macs, vlan=vlans))
+                labs.append(Labels(mac=macs, vlan=vlans, bdf=bdfs))
                 child_bdfs.extend(bdfs)
                 child_numas.extend(numas)
                 units += len(child_vfs)
             slot = v[0].fields['Slot']
             model = v[0].fields['Model']
             descr = v[0].fields['Description']
             interface_node_ids = list(map(mac_to_node_id, parent_macs))
```

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/fpga.py` & `fim_utils-1.5.0rc4/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/gpu.py` & `fim_utils-1.5.0rc4/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/model.py` & `fim_utils-1.5.0rc4/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/nvme.py` & `fim_utils-1.5.0rc4/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.0rc4/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/site.py` & `fim_utils-1.5.0rc4/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/storage.py` & `fim_utils-1.5.0rc4/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/ralph/worker_node.py` & `fim_utils-1.5.0rc4/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/utilities/generate_instance_flavors.py` & `fim_utils-1.5.0rc4/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/utilities/scan_net.py` & `fim_utils-1.5.0rc4/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/utilities/scan_oess.py` & `fim_utils-1.5.0rc4/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/utilities/scan_site.py` & `fim_utils-1.5.0rc4/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/fimutil/utilities/scan_worker.py` & `fim_utils-1.5.0rc4/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/pyproject.toml` & `fim_utils-1.5.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/setup.py` & `fim_utils-1.5.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/test/netam_test.py` & `fim_utils-1.5.0rc4/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.0rc3/PKG-INFO` & `fim_utils-1.5.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.5.0rc3
+Version: 1.5.0rc4
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

