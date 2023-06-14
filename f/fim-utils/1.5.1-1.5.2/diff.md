# Comparing `tmp/fim_utils-1.5.1.tar.gz` & `tmp/fim_utils-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fim_utils-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.5.1.tar` & `fim_utils-1.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.1/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.1/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.1/MANIFEST.in
--rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.1/README.md
--rw-r--r--   0        0        0      156 2023-06-14 19:27:11.590636 fim_utils-1.5.1/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.1/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.1/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.1/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.1/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.1/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.1/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.1/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.1/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.1/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-14 19:22:11.396659 fim_utils-1.5.1/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.1/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.1/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.1/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2505 2023-06-14 13:08:12.066017 fim_utils-1.5.1/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1226 2023-06-14 13:08:12.066616 fim_utils-1.5.1/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.1/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.1/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.1/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.1/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.1/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10922 2023-06-14 19:23:06.279493 fim_utils-1.5.1/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.1/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.1/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.1/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.1/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5488 2023-06-14 13:08:12.069995 fim_utils-1.5.1/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2015 2023-06-14 13:08:12.070557 fim_utils-1.5.1/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.1/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.1/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.1/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.1/test/ralph_test.py
--rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.2/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.2/README.md
+-rw-r--r--   0        0        0      156 2023-06-14 19:58:07.843935 fim_utils-1.5.2/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.2/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.2/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.2/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.2/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.2/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.2/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.2/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.2/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.2/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3456 2023-06-14 19:22:11.396659 fim_utils-1.5.2/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.2/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.2/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.2/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2023-06-14 19:54:12.053408 fim_utils-1.5.2/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1304 2023-06-14 19:54:22.381741 fim_utils-1.5.2/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.2/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.2/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.2/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.2/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.2/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10922 2023-06-14 19:23:06.279493 fim_utils-1.5.2/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.2/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.2/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.2/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.2/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5594 2023-06-14 19:50:45.471475 fim_utils-1.5.2/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2023-06-14 19:57:09.799801 fim_utils-1.5.2/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.2/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.2/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.2/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.2/test/ralph_test.py
+-rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.2/PKG-INFO
```

### Comparing `fim_utils-1.5.1/.gitignore` & `fim_utils-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/LICENSE` & `fim_utils-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/README.md` & `fim_utils-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/al2s/arm.py` & `fim_utils-1.5.2/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/al2s/cloud_cfg.py` & `fim_utils-1.5.2/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/al2s/oess.py` & `fim_utils-1.5.2/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/netam/arm.py` & `fim_utils-1.5.2/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/netam/nso.py` & `fim_utils-1.5.2/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/netam/sr_pce.py` & `fim_utils-1.5.2/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/asset.py` & `fim_utils-1.5.2/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.2/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.2/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.2/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/fpga.py` & `fim_utils-1.5.2/fimutil/ralph/fpga.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         ret = list()
         fpga_index = 1
         for field in custom_fields:
             for fpga_model in FPGA_MODELS:
                 try:
                     ports = []
                     if fpga_model in custom_fields[field]:
+                        logging.debug(f'Detected FPGA {fpga_model}')
                         model = fpga_model
                         description = custom_fields[field]
                         bdf = custom_fields[field + '_pci_id']
                         # -1 means unknown
                         numa = custom_fields.get(field + '_numa_node', '-1')
                         sn = custom_fields[f'fpga{fpga_index}_sn']
                         usb_id = custom_fields[f'fpga{fpga_index}_usb_device_id']
```

### Comparing `fim_utils-1.5.1/fimutil/ralph/gpu.py` & `fim_utils-1.5.2/fimutil/ralph/gpu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Any
 from dataclasses import dataclass
 
 import pyjq
+import logging
 
 GPU_MODELS = ['Quadro RTX 6000/8000', 'Tesla T4', 'A40', 'A30 PCIe']
 
 
 @dataclass(frozen=True)
 class GPU:
     """
@@ -25,14 +26,15 @@
         of GPU objects (which can be empty).
         """
         custom_fields = pyjq.one('.custom_fields', node_raw_json)
         ret = list()
         for field in custom_fields:
             for gpu_model in GPU_MODELS:
                 if gpu_model in custom_fields[field]:
+                    logging.debug(f'Detected GPU {gpu_model}')
                     model = gpu_model
                     description = custom_fields[field]
                     bdf = custom_fields[field + '_pci_id']
                     # -1 means unknown
                     numa = custom_fields.get(field + '_numa_node', '-1')
                     ret.append(GPU(model, description, bdf, numa))
         return ret
```

### Comparing `fim_utils-1.5.1/fimutil/ralph/model.py` & `fim_utils-1.5.2/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/nvme.py` & `fim_utils-1.5.2/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.2/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/site.py` & `fim_utils-1.5.2/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/storage.py` & `fim_utils-1.5.2/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/ralph/worker_node.py` & `fim_utils-1.5.2/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/utilities/generate_instance_flavors.py` & `fim_utils-1.5.2/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/utilities/scan_net.py` & `fim_utils-1.5.2/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/utilities/scan_oess.py` & `fim_utils-1.5.2/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/fimutil/utilities/scan_site.py` & `fim_utils-1.5.2/fimutil/utilities/scan_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
     args = parser.parse_args()
 
     if args.debug is None:
         logging.basicConfig(level=logging.INFO)
     elif args.debug >= 1:
         logging.basicConfig(level=logging.DEBUG)
+        # silence urllib
+        logging.getLogger('urllib3.connectionpool').setLevel(level=logging.INFO)
 
     if args.site is None:
         print('You must specify the site name', file=sys.stderr)
         sys.exit(-1)
 
     args.site = args.site.upper()
```

### Comparing `fim_utils-1.5.1/fimutil/utilities/scan_worker.py` & `fim_utils-1.5.2/fimutil/utilities/scan_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
     args = parser.parse_args()
 
     if args.debug is None:
         logging.basicConfig(level=logging.INFO)
     elif args.debug >= 1:
         logging.basicConfig(level=logging.DEBUG)
+        # silence urllib
+        logging.getLogger('urllib3.connectionpool').setLevel(level=logging.INFO)
 
     if args.worker is None:
         print('You must specify the worker', file=sys.stderr)
         sys.exit(-1)
 
     if args.base_uri is None:
         print('You must specify the base URL (typically https://hostname/api/data-center-assets/',
```

### Comparing `fim_utils-1.5.1/pyproject.toml` & `fim_utils-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/setup.py` & `fim_utils-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/test/netam_test.py` & `fim_utils-1.5.2/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.1/PKG-INFO` & `fim_utils-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.5.1
+Version: 1.5.2
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

