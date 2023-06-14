# Comparing `tmp/fluxgate_ctl-1.0.8-py3-none-any.whl.zip` & `tmp/fluxgate_ctl-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11271 bytes, number of entries: 9
+Zip file size: 11352 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-04 04:56 fluxgate_ctl/__init__.py
--rw-rw-r--  2.0 unx    20325 b- defN 23-Feb-10 18:49 fluxgate_ctl/__main__.py
+-rw-rw-r--  2.0 unx    20695 b- defN 23-Feb-10 18:57 fluxgate_ctl/__main__.py
 -rw-rw-r--  2.0 unx     7407 b- defN 23-Feb-04 05:32 fluxgate_ctl/discovery.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2757 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      753 b- defN 23-Feb-10 18:49 fluxgate_ctl-1.0.8.dist-info/RECORD
-9 files, 32481 bytes uncompressed, 9961 bytes compressed:  69.3%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2757 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      753 b- defN 23-Feb-10 18:57 fluxgate_ctl-1.0.9.dist-info/RECORD
+9 files, 32851 bytes uncompressed, 10042 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: fluxgate_ctl/__main__.py
 Comment: 
 
 Filename: fluxgate_ctl/discovery.py
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/LICENSE
+Filename: fluxgate_ctl-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/METADATA
+Filename: fluxgate_ctl-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/WHEEL
+Filename: fluxgate_ctl-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/entry_points.txt
+Filename: fluxgate_ctl-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/top_level.txt
+Filename: fluxgate_ctl-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fluxgate_ctl-1.0.8.dist-info/RECORD
+Filename: fluxgate_ctl-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fluxgate_ctl/__main__.py

```diff
@@ -290,14 +290,19 @@
                     flags,
                     mag_id,
                     mag_x,
                     mag_y,
                     mag_z,
                 ) = struct.unpack_from("<IIIIIIII", message[0], 0)
 
+                # Skip writing this if it isn't in the list
+                # Can happen right after ini file gets written to module
+                if(((1 << mag_id) & args.use_magnetometer) == 0):
+                    pass
+
                 volt_x = raw_to_voltage(mag_x)
                 volt_y = raw_to_voltage(mag_y)
                 volt_z = raw_to_voltage(mag_z)
 
                 # graph_data['ts'].append(time_sec + (time_nsec/1000000000))
                 graph_data[mag_id]["xs"].append(volt_x)
                 graph_data[mag_id]["ys"].append(volt_y)
@@ -593,14 +598,19 @@
                 calc_time = time_sec + (time_nsec / 1000000000)
 
                 if first_calc_time == 0:
                     first_calc_time = calc_time
 
                 delta_calc_time = calc_time - first_calc_time
 
+                # Skip writing this if it isn't in the list
+                # Can happen right after ini file gets written to module
+                if(((1 << mag_id) & args.use_magnetometer) == 0):
+                    pass
+
                 mag_count[mag_id] = mag_count[mag_id] + 1
 
                 # When the ADC is configured for bipolar operation, the output
                 # code is offset binary with a negative full-scale voltage resulting
                 # in a code of 000 … 000, a zero differential input voltage resulting in
                 # a code of 100 … 000, and a positive full-scale input voltage
                 # resulting in a code of 111 … 111. The output code for any
@@ -658,17 +668,15 @@
                 start_time = end_time
 
                 print(
                     "Rate "
                     + f"{(bit_count / delta / 1000000):.3f}"
                     + " mbit/s ["
                     + f"{int(msg_count / delta):d}"
-                    + " mag/s]"
-                    + " Delta: "
-                    + f"{delta_calc_time:.3f}",
+                    + " mag/s]",
                     end="\r",
                 )
 
                 bit_count = 0
                 msg_count = 0
                 first_calc_time = 0
```

## Comparing `fluxgate_ctl-1.0.8.dist-info/LICENSE` & `fluxgate_ctl-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fluxgate_ctl-1.0.8.dist-info/METADATA` & `fluxgate_ctl-1.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxgate-ctl
-Version: 1.0.8
+Version: 1.0.9
 Summary: fluxgate-ctl package for TUCAN
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

