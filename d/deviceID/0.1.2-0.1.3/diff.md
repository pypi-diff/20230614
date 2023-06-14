# Comparing `tmp/deviceID-0.1.2.tar.gz` & `tmp/deviceID-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deviceID-0.1.2.tar", last modified: Wed Jun 14 14:26:34 2023, max compression
+gzip compressed data, was "deviceID-0.1.3.tar", last modified: Wed Jun 14 14:31:04 2023, max compression
```

## Comparing `deviceID-0.1.2.tar` & `deviceID-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:26:34.889823 deviceID-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-14 14:26:34.889823 deviceID-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:26:34.885823 deviceID-0.1.2/deviceID/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.2/deviceID/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5164 2023-06-14 14:26:03.000000 deviceID-0.1.2/deviceID/deviceID.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:26:34.885823 deviceID-0.1.2/deviceID.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      161 2023-06-14 14:26:34.000000 deviceID-0.1.2/deviceID.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      211 2023-06-14 14:26:34.000000 deviceID-0.1.2/deviceID.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-06-14 14:26:34.000000 deviceID-0.1.2/deviceID.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-06-14 14:26:34.000000 deviceID-0.1.2/deviceID.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 14:26:34.889823 deviceID-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      347 2023-06-14 14:26:26.000000 deviceID-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:26:34.889823 deviceID-0.1.2/tests/
--rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.2/tests/test_deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-14 14:31:04.092250 deviceID-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:10.000000 deviceID-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/deviceID/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-14 07:31:55.000000 deviceID-0.1.3/deviceID/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5172 2023-06-14 14:27:46.000000 deviceID-0.1.3/deviceID/deviceID.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/deviceID.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      161 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      211 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-06-14 14:31:04.000000 deviceID-0.1.3/deviceID.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 14:31:04.092250 deviceID-0.1.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      347 2023-06-14 14:31:00.000000 deviceID-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 14:31:04.092250 deviceID-0.1.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-06-14 08:04:52.000000 deviceID-0.1.3/tests/test_deviceID.py
```

### Comparing `deviceID-0.1.2/deviceID/deviceID.py` & `deviceID-0.1.3/deviceID/deviceID.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,11 +131,11 @@
             if 'Location:' in data:
               if ('SystemBoard' in data.split('Location:')[1]):
                 isSystemMemory = True
     return xxhash.xxh64(';'.join(disks) + ';'.join(memory_devices) + ';' + ecc + ',' + max_memory + ',' + memory_num + ';' + processor_serial + ';' + processor_id + ';' + processor_manufacturer + ';' + processor_family + ';' + processor_version + ';' + processor_socket + ';' + processor_cores + ';' + processor_threads + ';' + motherboard_id + ';' + motherboard_name + ';' + motherboard_manufacturer).hexdigest()
   elif platform == "darwin":
     print('os x')
   elif platform == "win32":
-  import wmi
-  c = wmi.WMI()
-  hddSerialNumber = c.Win32_PhysicalMedia()[0].wmi_property('SerialNumber').value.strip()
-  print(hddSerialNumber)
+    import wmi
+    c = wmi.WMI()
+    hddSerialNumber = c.Win32_PhysicalMedia()[0].wmi_property('SerialNumber').value.strip()
+    print(hddSerialNumber)
```

