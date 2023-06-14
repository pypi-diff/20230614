# Comparing `tmp/neon_phal_plugin_switches-0.0.4a0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_switches-0.0.4a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5535 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7650 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      878 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      697 b- defN 23-Jun-10 02:21 neon_phal_plugin_switches-0.0.4a0.dist-info/RECORD
-7 files, 11062 bytes uncompressed, 4263 bytes compressed:  61.5%
+Zip file size: 5534 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7650 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      884 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      697 b- defN 23-Jun-14 19:53 neon_phal_plugin_switches-0.0.4a1.dist-info/RECORD
+7 files, 11069 bytes uncompressed, 4262 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_switches/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/METADATA
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/WHEEL
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/top_level.txt
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_switches-0.0.4a0.dist-info/RECORD
+Filename: neon_phal_plugin_switches-0.0.4a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_phal_plugin_switches-0.0.4a0.dist-info/LICENSE.md` & `neon_phal_plugin_switches-0.0.4a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_switches-0.0.4a0.dist-info/METADATA` & `neon_phal_plugin_switches-0.0.4a1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-switches
-Version: 0.0.4a0
+Version: 0.0.4a1
 Summary: Hardware Switch Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-switches
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: sj201-interface (~=0.0.2)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
 Requires-Dist: ovos-utils (~=0.0.26)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 
 # PHAL Switches Plugin
 Enables switch inputs for volume, mute, and action button. Current implementation
@@ -21,8 +21,7 @@
 ## Default Pin Configuration
 | Pin | Connection    |
 |-----|---------------|
 | 22  | Volume Up     |
 | 23  | Volume Down   |
 | 24  | Action Button |
 | 25  | Mute Switch   |
-
```

## Comparing `neon_phal_plugin_switches-0.0.4a0.dist-info/RECORD` & `neon_phal_plugin_switches-0.0.4a1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 neon_phal_plugin_switches/__init__.py,sha256=SJhyq_ZXP9hn4sNCF1RqWwkr2L7nTVs5M4gqjOa5paw,7650
-neon_phal_plugin_switches-0.0.4a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_switches-0.0.4a0.dist-info/METADATA,sha256=v6ZRmHDbNgoPd7zauv994BQPPopELoXNlANdMuc3PnA,878
-neon_phal_plugin_switches-0.0.4a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_switches-0.0.4a0.dist-info/entry_points.txt,sha256=9fESMRlr8KEMPeXo1o_wu6aWIMoAanYHPDj6ELkvC8I,85
-neon_phal_plugin_switches-0.0.4a0.dist-info/top_level.txt,sha256=A8evCen-WsINGFm3FiXe9v9p8CfsVYsHd-2h_sd-ppg,26
-neon_phal_plugin_switches-0.0.4a0.dist-info/RECORD,,
+neon_phal_plugin_switches-0.0.4a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_switches-0.0.4a1.dist-info/METADATA,sha256=EIneMNe8q2ppGdWhTZxeUsoHP3CxEM5zv5cRf91kWn8,884
+neon_phal_plugin_switches-0.0.4a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_switches-0.0.4a1.dist-info/entry_points.txt,sha256=zoKKPfAmOevrv6Rtts2ypjje3i9pCrCm9tRt_oW-BBY,86
+neon_phal_plugin_switches-0.0.4a1.dist-info/top_level.txt,sha256=A8evCen-WsINGFm3FiXe9v9p8CfsVYsHd-2h_sd-ppg,26
+neon_phal_plugin_switches-0.0.4a1.dist-info/RECORD,,
```

