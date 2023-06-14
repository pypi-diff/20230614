# Comparing `tmp/esp-secure-cert-tool-1.0.0.tar.gz` & `tmp/esp-secure-cert-tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-secure-cert-tool-1.0.0.tar", last modified: Fri Jun  9 05:54:30 2023, max compression
+gzip compressed data, was "dist/esp-secure-cert-tool-1.0.1.tar", last modified: Wed Jun 14 04:29:54 2023, max compression
```

## Comparing `esp-secure-cert-tool-1.0.0.tar` & `esp-secure-cert-tool-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    15564 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/configure_esp_secure_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/configure_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/custflash_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/efuse_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/esp_secure_cert_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/nvs_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    14937 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert/tlv_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:54:30.000000 esp-secure-cert-tool-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-09 05:54:17.000000 esp-secure-cert-tool-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15836 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/configure_esp_secure_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/configure_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/custflash_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/efuse_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/esp_secure_cert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/nvs_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert/tlv_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:29:54.000000 esp-secure-cert-tool-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-14 04:29:44.000000 esp-secure-cert-tool-1.0.1/setup.py
```

### Comparing `esp-secure-cert-tool-1.0.0/LICENSE` & `esp-secure-cert-tool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/PKG-INFO` & `esp-secure-cert-tool-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-1.0.0/README.md` & `esp-secure-cert-tool-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/configure_esp_secure_cert.py` & `esp-secure-cert-tool-1.0.1/configure_esp_secure_cert.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,15 +336,19 @@
                 tlv_priv_key.efuse_key_id = args.efuse_key_id
                 priv_key_len = int(args.priv_key_algo[1], 10)
                 tlv_priv_key.priv_key_len = priv_key_len
                 tlv_format.generate_partition_ds(tlv_priv_key,
                                                  args.device_cert,
                                                  ca_cert, idf_target,
                                                  bin_filename)
-
+        else:
+            tlv_format.generate_partition_no_ds(tlv_priv_key,
+                                                args.device_cert,
+                                                ca_cert, idf_target,
+                                                bin_filename)
     elif args.sec_cert_type == 'cust_flash':
         if args.configure_ds is not False:
             custflash_format.generate_partition_ds(c, iv, args.efuse_key_id,
                                                    key_size, args.device_cert,
                                                    ca_cert, idf_target,
                                                    bin_filename)
         else:
```

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/configure_ds.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/configure_ds.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/custflash_format.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/custflash_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/efuse_helper.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/efuse_helper.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/esp_secure_cert_helper.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/esp_secure_cert_helper.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/nvs_format.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/nvs_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert/tlv_format.py` & `esp-secure-cert-tool-1.0.1/esp_secure_cert/tlv_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,18 +292,17 @@
     else:
         raise ValueError('Invalid key type')
 
 
 # @info
 #       This function generates the cust_flash partition of
 #       the encrypted private key parameters when DS is disabled.
-def generate_partition_no_ds(device_cert,
-                             ca_cert,
-                             priv_key: tlv_priv_key_t,
-                             idf_target, op_file):
+def generate_partition_no_ds(priv_key: tlv_priv_key_t,
+                             device_cert, ca_cert, idf_target,
+                             op_file):
     # cust_flash partition is of size 0x2000 i.e. 8192 bytes
     tlv_data_length = 0
     with open(op_file, 'wb') as output_file:
         partition_size = 0x2000
         output_file_data = bytearray(b'\xff' * partition_size)
         cur_offset = 0
         dev_cert_data = load_certificate(device_cert)
```

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/PKG-INFO` & `esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-1.0.0/esp_secure_cert_tool.egg-info/SOURCES.txt` & `esp-secure-cert-tool-1.0.1/esp_secure_cert_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-1.0.0/setup.py` & `esp-secure-cert-tool-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-secure-cert-tool "
         "documentation for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 long_description = """
 ====================
 esp-secure-cert-tool
 ====================
 The python utility helps to configure and provision the device with
 PKI credentials to generate the esp_secure_cert partition.
```

