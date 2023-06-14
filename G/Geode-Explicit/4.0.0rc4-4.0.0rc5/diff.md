# Comparing `tmp/Geode_Explicit-4.0.0rc4-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.0.0rc5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2242421 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-May-31 12:03 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-31 12:03 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-May-31 12:03 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2246144 b- defN 23-May-31 12:03 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    47616 b- defN 23-May-31 12:03 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2065408 b- defN 23-May-31 12:03 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-May-31 12:03 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-May-31 12:03 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2401 b- defN 23-May-31 12:03 Geode_Explicit-4.0.0rc4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 12:03 Geode_Explicit-4.0.0rc4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-31 12:03 Geode_Explicit-4.0.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 23-May-31 12:03 Geode_Explicit-4.0.0rc4.dist-info/RECORD
-12 files, 4658952 bytes uncompressed, 2240497 bytes compressed:  51.9%
+Zip file size: 2242417 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-May-31 15:57 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-31 15:57 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-May-31 15:57 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  2246144 b- defN 23-May-31 15:57 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    47616 b- defN 23-May-31 15:57 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  2065408 b- defN 23-May-31 15:57 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-May-31 15:57 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-May-31 15:57 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2401 b- defN 23-May-31 15:57 Geode_Explicit-4.0.0rc5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-31 15:57 Geode_Explicit-4.0.0rc5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-31 15:57 Geode_Explicit-4.0.0rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 23-May-31 15:57 Geode_Explicit-4.0.0rc5.dist-info/RECORD
+12 files, 4658952 bytes uncompressed, 2240493 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc4.dist-info/METADATA
+Filename: Geode_Explicit-4.0.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc4.dist-info/WHEEL
+Filename: Geode_Explicit-4.0.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc4.dist-info/top_level.txt
+Filename: Geode_Explicit-4.0.0rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc4.dist-info/RECORD
+Filename: Geode_Explicit-4.0.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180186d8c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 31 12:03:37 2023
+Time/Date		Wed May 31 15:57:45 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000189800
 SizeOfInitializedData	000000000009aa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000186d8c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0022b000
 SizeOfHeaders		00000400
-CheckSum		00226f33
+CheckSum		0022dcf3
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -666946,16 +666946,15 @@
    1801f2938:	(bad)
    1801f293d:	insb   (%dx),%es:(%rdi)
    1801f293e:	insb   (%dx),%es:(%rdi)
    1801f293f:	outsl  %ds:(%rsi),(%dx)
    1801f2940:	movsxd 0x74(%rcx),%esp
    1801f2943:	imul   $0x0,0x6e(%rdi),%ebp
    1801f294a:	add    %al,(%rax)
-   1801f294c:	cltd
-   1801f294d:	(bad)
+   1801f294c:	jns    0x1801f29bc
    1801f294e:	ja     0x1801f29b4
    1801f2950:	add    %al,(%rax)
    1801f2952:	add    %al,(%rax)
    1801f2954:	or     $0x60000000,%eax
    1801f2959:	add    (%rax),%eax
    1801f295b:	add    %ah,(%rax)
    1801f295d:	rex.WB (bad)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180006a6c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 31 12:03:24 2023
+Time/Date		Wed May 31 15:57:29 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000006a00
 SizeOfInitializedData	0000000000004c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000006a6c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00010000
 SizeOfHeaders		00000400
-CheckSum		00011f7b
+CheckSum		00018d35
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -10112,19 +10112,16 @@
    1800086a0:	movsxd 0x74(%rcx),%esp
    1800086a3:	imul   $0xc1800000,0x6e(%rdi),%ebp
    1800086aa:	add    %al,0x1(%rax)
    1800086b0:	and    %al,%dl
    1800086b2:	add    %al,0x1(%rax)
    1800086b8:	add    %al,(%rax)
    1800086ba:	add    %al,(%rax)
-   1800086bc:	mov    %?,(%rdi)
-   1800086be:	ja     0x180008724
-   1800086c0:	add    %al,(%rax)
-   1800086c2:	add    %al,(%rax)
-   1800086c4:	or     $0xec000000,%eax
+   1800086bc:	imul   $0x64,0x77(%rsi),%ebp
+   1800086c3:	add    %cl,-0x14000000(%rip)        # 0x16c0086c9
    1800086c9:	add    (%rax),%al
    1800086cb:	add    %bl,-0x74(%rax)
    1800086ce:	add    %al,(%rax)
    1800086d0:	pop    %rax
    1800086d1:	jp     0x1800086d3
 	...
    1800086df:	add    %bh,(%rax)
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180165320
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 31 12:03:24 2023
+Time/Date		Wed May 31 15:57:32 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000166e00
 SizeOfInitializedData	0000000000091200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000165320
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		001ff000
 SizeOfHeaders		00000400
-CheckSum		00201faf
+CheckSum		001f8d70
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -622336,15 +622336,16 @@
    1801cee78:	(bad)
    1801cee7d:	insb   (%dx),%es:(%rdi)
    1801cee7e:	insb   (%dx),%es:(%rdi)
    1801cee7f:	outsl  %ds:(%rsi),(%dx)
    1801cee80:	movsxd 0x74(%rcx),%esp
    1801cee83:	imul   $0x0,0x6e(%rdi),%ebp
    1801cee8a:	add    %al,(%rax)
-   1801cee8c:	mov    %?,(%rdi)
+   1801cee8c:	insb   (%dx),%es:(%rdi)
+   1801cee8d:	outsb  %ds:(%rsi),(%dx)
    1801cee8e:	ja     0x1801ceef4
    1801cee90:	add    %al,(%rax)
    1801cee92:	add    %al,(%rax)
    1801cee94:	or     $0x60000000,%eax
    1801cee99:	add    (%rax),%eax
    1801cee9b:	add    %ch,(%rdx,%rcx,1)
    1801cee9e:	sbb    $0x1cfc2c00,%eax
```

## Comparing `Geode_Explicit-4.0.0rc4.dist-info/METADATA` & `Geode_Explicit-4.0.0rc5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.0.0rc4
+Version: 4.0.0rc5
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: geode-background (==7.*,>=7.2.0rc2)
-Requires-Dist: geode-common (==26.*,>=26.0.0rc1)
+Requires-Dist: geode-common (==26.*,>=26.0.0rc2)
 Requires-Dist: geode-conversion (==5.*,>=5.0.6rc1)
 Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
 Requires-Dist: opengeode-geosciences (==7.*,>=7.0.9rc1)
 Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3)
 Requires-Dist: opengeode-inspector (==3.*,>=3.0.6rc1)
 Requires-Dist: opengeode-io (==6.*,>=6.0.6)
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.0rc4 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.0rc5 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.2.0rc2)
-Requires-Dist: geode-common (==26.*,>=26.0.0rc1) Requires-Dist: geode-
+Requires-Dist: geode-common (==26.*,>=26.0.0rc2) Requires-Dist: geode-
 conversion (==5.*,>=5.0.6rc1) Requires-Dist: opengeode-core
 (==14.*,>=14.1.10rc5) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.9rc1)
 Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3) Requires-Dist:
 opengeode-inspector (==3.*,>=3.0.6rc1) Requires-Dist: opengeode-io
 (==6.*,>=6.0.6)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
```

