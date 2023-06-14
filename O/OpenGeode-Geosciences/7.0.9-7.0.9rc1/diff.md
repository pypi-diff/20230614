# Comparing `tmp/OpenGeode_Geosciences-7.0.9-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-7.0.9rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 526334 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      199 b- defN 23-Jun-02 09:07 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Jun-02 09:07 opengeode_geosciences/explicit.py
--rw-rw-rw-  2.0 fat     1239 b- defN 23-Jun-02 09:07 opengeode_geosciences/implicit.py
--rw-rw-rw-  2.0 fat   559616 b- defN 23-Jun-02 09:09 opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll
--rw-rw-rw-  2.0 fat   408064 b- defN 23-Jun-02 09:09 opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll
--rw-rw-rw-  2.0 fat   389120 b- defN 23-Jun-02 09:09 opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   336896 b- defN 23-Jun-02 09:09 opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3233 b- defN 23-Jun-02 09:09 OpenGeode_Geosciences-7.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-02 09:09 OpenGeode_Geosciences-7.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-02 09:09 OpenGeode_Geosciences-7.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1136 b- defN 23-Jun-02 09:09 OpenGeode_Geosciences-7.0.9.dist-info/RECORD
-11 files, 1700864 bytes uncompressed, 524358 bytes compressed:  69.2%
+Zip file size: 526358 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      199 b- defN 23-May-30 18:50 opengeode_geosciences/__init__.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-May-30 18:50 opengeode_geosciences/explicit.py
+-rw-rw-rw-  2.0 fat     1239 b- defN 23-May-30 18:50 opengeode_geosciences/implicit.py
+-rw-rw-rw-  2.0 fat   559616 b- defN 23-May-30 18:52 opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll
+-rw-rw-rw-  2.0 fat   408064 b- defN 23-May-30 18:52 opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll
+-rw-rw-rw-  2.0 fat   389120 b- defN 23-May-30 18:52 opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   336896 b- defN 23-May-30 18:52 opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3239 b- defN 23-May-30 18:52 OpenGeode_Geosciences-7.0.9rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-30 18:52 OpenGeode_Geosciences-7.0.9rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-May-30 18:52 OpenGeode_Geosciences-7.0.9rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1148 b- defN 23-May-30 18:52 OpenGeode_Geosciences-7.0.9rc1.dist-info/RECORD
+11 files, 1700882 bytes uncompressed, 524358 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd
 Comment: 
 
 Filename: opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.9.dist-info/METADATA
+Filename: OpenGeode_Geosciences-7.0.9rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.9.dist-info/WHEEL
+Filename: OpenGeode_Geosciences-7.0.9rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.9.dist-info/top_level.txt
+Filename: OpenGeode_Geosciences-7.0.9rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Geosciences-7.0.9.dist-info/RECORD
+Filename: OpenGeode_Geosciences-7.0.9rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800440ac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun  2 09:08:19 2023
+Time/Date		Tue May 30 18:51:49 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000045400
 SizeOfInitializedData	0000000000043200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000440ac
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0008d000
 SizeOfHeaders		00000400
-CheckSum		00091b98
+CheckSum		00094415
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -101730,16 +101730,17 @@
    18004a958:	movsxd 0x74(%rcx),%esp
    18004a95b:	imul   $0x5ba00000,0x6e(%rdi),%ebp
    18004a962:	or     %al,0x1(%rax)
    18004a968:	rex pop %rsp
    18004a96a:	or     %al,0x1(%rax)
    18004a970:	add    %al,(%rax)
    18004a972:	add    %al,(%rax)
-   18004a974:	xorl   $0x0,0x6479(%rcx)
-   18004a97b:	add    %cl,0x3c000000(%rip)        # 0x1bc04a981
+   18004a974:	vpcmpeqd 0x0(%rax,%rax,1),%ymm7,%ymm12
+   18004a97a:	add    %al,(%rax)
+   18004a97c:	or     $0x3c000000,%eax
    18004a981:	add    (%rax),%eax
    18004a983:	add    %ch,%al
    18004a985:	xor    %al,0x518e800(%rip)        # 0x1851d918b
    18004a98b:	add    %al,(%rax)
    18004a98d:	add    %al,(%rax)
    18004a98f:	add    %bh,(%rax)
    18004a991:	add    %eax,(%rax)
```

## opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018003c420
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun  2 09:08:50 2023
+Time/Date		Tue May 30 18:52:21 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000003e600
 SizeOfInitializedData	0000000000025000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000003c420
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00068000
 SizeOfHeaders		00000400
-CheckSum		000661cf
+CheckSum		00068a4e
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -91579,28 +91579,29 @@
    180043716:	add    %al,(%rax)
    180043718:	xor    %dl,(%rbx)
    18004371a:	(bad)
    18004371b:	addb   $0x0,(%rcx)
    18004371e:	add    %al,(%rax)
    180043720:	add    %al,(%rax)
    180043722:	add    %al,(%rax)
-   180043724:	movabs %al,0xd000000006479b1
-   18004372d:	add    %al,(%rax)
-   18004372f:	add    %bh,(%rbx,%rax,1)
-   180043732:	add    %al,(%rax)
-   180043734:	test   %eax,%fs:(%rax,%rax,1)
-   180043738:	outsl  %fs:(%rsi),(%dx)
-   18004373a:	add    $0x0,%al
-   18004373c:	add    %al,(%rax)
-   18004373e:	add    %al,(%rax)
-   180043740:	cmp    %al,(%rcx)
+   180043724:	in     $0x45,%eax
+   180043726:	jbe    0x18004378c
+   180043728:	add    %al,(%rax)
+   18004372a:	add    %al,(%rax)
+   18004372c:	or     $0x3c000000,%eax
+   180043731:	add    (%rax),%eax
+   180043733:	add    %ah,0x4(%rbp,%rax,4)
+   180043737:	add    %ah,0x4(%rdi,%rbp,2)
+   18004373b:	add    %al,(%rax)
+   18004373d:	add    %al,(%rax)
+   18004373f:	add    %bh,(%rax)
+   180043741:	add    %eax,(%rax)
 	...
-   180043796:	add    %al,(%rax)
-   180043798:	cmp    %dl,%al
-   18004379a:	add    $0x180,%eax
+   180043797:	add    %bh,(%rax)
+   180043799:	rolb   0x180(%rip)        # 0x18004391f
 	...
    1800437af:	add    %bh,(%rax)
    1800437b1:	(bad)
    1800437b3:	addb   $0x0,(%rcx)
    1800437b6:	add    %al,(%rax)
    1800437b8:	rex.W (bad)
    1800437bb:	addb   $0x0,(%rcx)
```

## Comparing `OpenGeode_Geosciences-7.0.9.dist-info/METADATA` & `OpenGeode_Geosciences-7.0.9rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Geosciences
-Version: 7.0.9
+Version: 7.0.9rc1
 Summary: OpenGeode module for Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.1.10)
+Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
 
 <h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.0.9 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 7.0.9rc1 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown Requires-Dist: opengeode-core (==14.*,>=14.1.10)
+markdown Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

## Comparing `OpenGeode_Geosciences-7.0.9.dist-info/RECORD` & `OpenGeode_Geosciences-7.0.9rc1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 opengeode_geosciences/__init__.py,sha256=w7_ys_rdYFV6X9-DHDK4aHD3C7a7YbuiKhXh-gdoyq0,199
 opengeode_geosciences/explicit.py,sha256=uSrCUigVUNQlZUlZGI6tLpCACmWLqC3zJdI9V9p2L9w,1239
 opengeode_geosciences/implicit.py,sha256=1h6T21wYBxmNpkFTsSbPw-sFx79T_iZGANQRnwCtmho,1239
-opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll,sha256=ZhtC_ScVguKTJoaA-V4Vg_QmACt93NG7fC9B_Sw5og8,559616
-opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll,sha256=wcrt8_bEkqvTRZ-z_1hPiQnM0XeoPusyKKAirnwyRBc,408064
-opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd,sha256=th6-FScx8f9ktORex9sQfTVwNciBEqSl9p5Emh_MdT8,389120
-opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd,sha256=s74xVA5dzBrlnnFgbTGVHIRzMatVf_eyc1sZfIFmWkI,336896
-OpenGeode_Geosciences-7.0.9.dist-info/METADATA,sha256=uAFmJuUuwVhfOAz4deplLFQsBYyFKYpJXeOtQoXL5MQ,3233
-OpenGeode_Geosciences-7.0.9.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Geosciences-7.0.9.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
-OpenGeode_Geosciences-7.0.9.dist-info/RECORD,,
+opengeode_geosciences/bin/OpenGeode-Geosciences_explicit.dll,sha256=_Wg7sWOAJNb3OBIymFAh_OtUWcDw_miktnVHcTST2Vo,559616
+opengeode_geosciences/bin/OpenGeode-Geosciences_implicit.dll,sha256=fLZllSU5drVE2RlV-HB3ulko9x1Meiawb4R5FgMWh8w,408064
+opengeode_geosciences/bin/opengeode_geosciences_py_explicit.cp39-win_amd64.pyd,sha256=sARdwYMn9rimZFujNIse1o5SBio754xqHPPLjWkQQsI,389120
+opengeode_geosciences/bin/opengeode_geosciences_py_implicit.cp39-win_amd64.pyd,sha256=s1COyyWEJsj7HOba-bNSHxadic2PYwILt8qcrpq-zG0,336896
+OpenGeode_Geosciences-7.0.9rc1.dist-info/METADATA,sha256=qKCnIZOqTaHH5wSeDnfSZDq_PvkvTvVdiFYphUFBY1E,3239
+OpenGeode_Geosciences-7.0.9rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_Geosciences-7.0.9rc1.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
+OpenGeode_Geosciences-7.0.9rc1.dist-info/RECORD,,
```

