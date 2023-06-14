# Comparing `tmp/basic_math_operations-1.0.163.tar.gz` & `tmp/basic_math_operations-1.0.164.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_math_operations-1.0.163.tar", last modified: Fri Jun  9 12:28:03 2023, max compression
+gzip compressed data, was "basic_math_operations-1.0.164.tar", last modified: Wed Jun 14 15:06:52 2023, max compression
```

## Comparing `basic_math_operations-1.0.163.tar` & `basic_math_operations-1.0.164.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/basic_math_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/basic_math_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:28:03.847288 basic_math_operations-1.0.163/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)    75064 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-09 12:27:42.000000 basic_math_operations-1.0.163/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 12:28:03.000000 basic_math_operations-1.0.163/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/basic_math_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/basic_math_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.571944 basic_math_operations-1.0.164/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:52.575944 basic_math_operations-1.0.164/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)    75528 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-14 15:06:25.000000 basic_math_operations-1.0.164/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:06:52.000000 basic_math_operations-1.0.164/src/python-module/version.txt
```

### Comparing `basic_math_operations-1.0.163/LICENSE` & `basic_math_operations-1.0.164/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.163/README.md` & `basic_math_operations-1.0.164/README.md`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.163/setup.py` & `basic_math_operations-1.0.164/setup.py`

 * *Files identical despite different names*

### Comparing `basic_math_operations-1.0.163/src/python-module/libbasic_math_operations.a` & `basic_math_operations-1.0.164/src/python-module/libbasic_math_operations.a`

 * *Files 1% similar despite different names*

#### file list

```diff
@@ -2,26 +2,26 @@
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 basic_math_operations.c.o
 ?rw-r--r--   0        0        0    28944 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
 ?rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 strlen_asm.asm.o
 ?rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
 ?rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 add_whole.asm.o
 ?rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 add_whole_same_length.asm.o
-?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 add.c.o
+?rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 add.c.o
 ?rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 subtract_whole.asm.o
 ?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 subtract_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 subtractp.c.o
-?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 subtract.c.o
+?rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 subtract.c.o
 ?rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 _multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
-?rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 multiply.c.o
+?rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 multiply.c.o
 ?rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
-?rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
+?rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
 ?rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
-?rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 divide.c.o
+?rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 divide.c.o
 ?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
 ?rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 addp.c.o
 ?rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 remove_zeroes.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 increment_whole.c.o
```

#### add.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1080 (bytes into file)
+  Start of section headers:          1120 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x438:
+There are 13 section headers, starting at offset 0x460:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 0000fb 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000308 0000a8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 00013b 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 00013b 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00013b 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000167 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000168 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000188 000068 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 0003b0 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0001f0 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0002c8 00003b 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 0003c8 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 00012b 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000330 0000a8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 00016b 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 00016b 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000197 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000198 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001b8 000060 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 0003d8 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000218 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0002f0 00003b 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 0003f0 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 9 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS add.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   251 FUNC    GLOBAL DEFAULT    1 add
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
-     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND addp
+     3: 0000000000000000   299 FUNC    GLOBAL DEFAULT    1 add
+     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND addp
+     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtractp
```

##### readelf --wide --relocs {}

```diff
@@ -1,14 +1,14 @@
 
-Relocation section '.rela.text' at offset 0x308 contains 7 entries:
+Relocation section '.rela.text' at offset 0x330 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000054  0000000500000004 R_X86_64_PLT32         0000000000000000 addp - 4
-0000000000000081  0000000500000004 R_X86_64_PLT32         0000000000000000 addp - 4
-0000000000000089  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-000000000000009e  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000000bb  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
-00000000000000e3  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
-000000000000003d  0000000400000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+0000000000000059  0000000400000004 R_X86_64_PLT32         0000000000000000 addp - 4
+00000000000000b1  0000000400000004 R_X86_64_PLT32         0000000000000000 addp - 4
+00000000000000b9  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+00000000000000ce  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000000eb  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
+0000000000000113  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
+0000000000000079  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x3b0 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x3d8 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,55 +9,48 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..00000000000000fb
+00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..000000000000012b
   DW_CFA_advance_loc: 13 to 000000000000000d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_advance_loc: 4 to 0000000000000011
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_advance_loc: 4 to 0000000000000015
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc: 33 to 0000000000000036
+  DW_CFA_advance_loc: 31 to 0000000000000034
   DW_CFA_remember_state
-  DW_CFA_restore: r3 (rbx)
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 4 to 000000000000003a
-  DW_CFA_restore: r6 (rbp)
+  DW_CFA_advance_loc: 1 to 0000000000000035
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000003c
-  DW_CFA_restore: r12 (r12)
+  DW_CFA_advance_loc: 2 to 0000000000000037
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 12 to 0000000000000048
+  DW_CFA_advance_loc: 9 to 0000000000000040
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 1 to 0000000000000049
-  DW_CFA_remember_state
-  DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 000000000000004a
-  DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000004c
-  DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 0000000000000050
-  DW_CFA_restore_state
-  DW_CFA_advance_loc: 24 to 0000000000000068
-  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 50 to 0000000000000072
   DW_CFA_restore: r3 (rbx)
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 4 to 0000000000000076
   DW_CFA_restore: r6 (rbp)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000000078
   DW_CFA_restore: r12 (r12)
-  DW_CFA_advance_loc: 8 to 0000000000000070
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 16 to 0000000000000088
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+  DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,88 +4,102 @@
 Disassembly of section .text:
 
 0000000000000000 <add>:
 add():
 	endbr64
 	movzbl (%rdi),%eax
 	test   %al,%al
-	je     68 <add+0x68>
+	je     80 <add+0x80>
 	push   %r12
 	mov    %rdx,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	movzbl (%rsi),%edx
 	test   %dl,%dl
-	je     48 <add+0x48>
+	je     33 <add+0x33>
 	mov    %rdi,%rbx
-	cmp    $0x2d,%al
-	je     70 <add+0x70>
+	cmp    $0x75,%al
+	jne    40 <add+0x40>
+	cmpb   $0x0,0x1(%rdi)
+	jne    40 <add+0x40>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	ret
+	nopl   0x0(%rax,%rax,1)
+	cmpb   $0x75,0x0(%rbp)
+	je     88 <add+0x88>
 	cmp    $0x2d,%dl
-	jne    50 <add+0x50>
+	je     64 <add+0x64>
+	cmp    $0x2d,%al
+	je     a0 <add+0xa0>
+	mov    %r12,%rdx
+	mov    %rbp,%rsi
+	mov    %rbx,%rdi
+	call   5d <add+0x5d>
+ R_X86_64_PLT32	addp-0x4
+	movzbl (%rbx),%eax
+	movzbl 0x0(%rbp),%edx
 	cmp    $0x2d,%al
-	je     70 <add+0x70>
+	je     a0 <add+0xa0>
 	cmp    $0x2d,%dl
-	je     d8 <add+0xd8>
+	je     108 <add+0x108>
 	pop    %rbx
 	mov    %r12,%rdi
 	pop    %rbp
 	pop    %r12
-	jmp    41 <add+0x41>
+	jmp    7d <add+0x7d>
  R_X86_64_PLT32	remove_zeroes-0x4
-	nopl   0x0(%rax)
-	pop    %rbx
-	pop    %rbp
-	pop    %r12
-	ret
 	nopl   (%rax)
-	mov    %r12,%rdx
-	call   58 <add+0x58>
- R_X86_64_PLT32	addp-0x4
-	movzbl (%rbx),%eax
-	movzbl 0x0(%rbp),%edx
-	jmp    28 <add+0x28>
-	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
+	cmpb   $0x0,0x1(%rbp)
+	jne    46 <add+0x46>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	jmp    33 <add+0x33>
+	nopw   0x0(%rax,%rax,1)
 	cmp    $0x2d,%dl
-	jne    b0 <add+0xb0>
+	jne    e0 <add+0xe0>
 	mov    %r12,%rdx
 	lea    0x1(%rbp),%rsi
 	lea    0x1(%rbx),%rdi
-	call   85 <add+0x85>
+	call   b5 <add+0xb5>
  R_X86_64_PLT32	addp-0x4
 	mov    %r12,%rdi
-	call   8d <add+0x8d>
+	call   bd <add+0xbd>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rax,%rdx
 	test   %rax,%rax
-	je     a2 <add+0xa2>
+	je     d2 <add+0xd2>
 	lea    0x1(%r12),%rdi
 	mov    %r12,%rsi
-	call   a2 <add+0xa2>
+	call   d2 <add+0xd2>
  R_X86_64_PLT32	memmove-0x4
 	movb   $0x2d,(%r12)
-	jmp    35 <add+0x35>
+	jmp    71 <add+0x71>
 	nopl   0x0(%rax)
 	lea    0x1(%rbx),%rsi
 	mov    %r12,%rdx
 	mov    %rbp,%rdi
-	call   bf <add+0xbf>
+	call   ef <add+0xef>
  R_X86_64_PLT32	subtractp-0x4
 	cmpb   $0x2d,(%rbx)
-	jne    f2 <add+0xf2>
+	jne    122 <add+0x122>
 	movzbl 0x0(%rbp),%eax
 	cmp    $0x2d,%al
-	jne    35 <add+0x35>
-	jmp    75 <add+0x75>
+	jne    71 <add+0x71>
+	jmp    a5 <add+0xa5>
 	nopw   0x0(%rax,%rax,1)
 	lea    0x1(%rbp),%rsi
 	mov    %r12,%rdx
 	mov    %rbx,%rdi
-	call   e7 <add+0xe7>
+	call   117 <add+0x117>
  R_X86_64_PLT32	subtractp-0x4
 	cmpb   $0x2d,(%rbx)
-	jne    35 <add+0x35>
-	jmp    c4 <add+0xc4>
+	jne    71 <add+0x71>
+	jmp    f4 <add+0xf4>
 	movzbl 0x0(%rbp),%edx
-	jmp    2c <add+0x2c>
+	jmp    68 <add+0x68>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,10 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
-  0x00000020 00000000 fb000000 004d0e10 8c02440e .........M....D.
-  0x00000030 18860344 0e208304 610ac30e 1844c60e ...D. ..a....D..
-  0x00000040 1042cc0e 084c0b41 0a0e1841 0e10420e .B...L.A...A..B.
-  0x00000050 08440b58 0e08c3c6 cc480e20 83048603 .D.X.....H. ....
-  0x00000060 8c020000 00000000                   ........
+  0x00000010 1b0c0708 90010000 44000000 1c000000 ........D.......
+  0x00000020 00000000 2b010000 004d0e10 8c02440e ....+....M....D.
+  0x00000030 18860344 0e208304 5f0a0e18 410e1042 ...D. .._...A..B
+  0x00000040 0e08490b 72c30e18 44c60e10 42cc0e08 ..I.r...D...B...
+  0x00000050 500e2083 0486038c 02000000 00000000 P. .............
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,7 +1,7 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00616464 2e630061 64640072 656d6f76 .add.c.add.remov
-  0x00000010 655f7a65 726f6573 00616464 70007374 e_zeroes.addp.st
+  0x00000000 00616464 2e630061 64640061 64647000 .add.c.add.addp.
+  0x00000010 72656d6f 76655f7a 65726f65 73007374 remove_zeroes.st
   0x00000020 726c656e 5f61736d 006d656d 6d6f7665 rlen_asm.memmove
   0x00000030 00737562 74726163 747000            .subtractp.
```

#### subtract.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1056 (bytes into file)
+  Start of section headers:          1128 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x420:
+There are 13 section headers, starting at offset 0x468:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 0000df 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 0002f0 0000a8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 00011f 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 00011f 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00011f 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00014b 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000150 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000170 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000398 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0001d0 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0002a8 000045 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 0003b0 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 00012b 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000338 0000a8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 00016b 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 00016b 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000197 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000198 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001b8 000060 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 0003e0 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000218 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0002f0 000045 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 0003f8 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 9 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS subtract.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   223 FUNC    GLOBAL DEFAULT    1 subtract
+     3: 0000000000000000   299 FUNC    GLOBAL DEFAULT    1 subtract
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtractp
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND addp
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,14 +1,14 @@
 
-Relocation section '.rela.text' at offset 0x2f0 contains 7 entries:
+Relocation section '.rela.text' at offset 0x338 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000039  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
-000000000000004c  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
-0000000000000083  0000000600000004 R_X86_64_PLT32         0000000000000000 addp - 4
-000000000000008b  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000a0  0000000800000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+0000000000000059  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
+00000000000000b1  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
 00000000000000cb  0000000600000004 R_X86_64_PLT32         0000000000000000 addp - 4
-0000000000000068  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+00000000000000d3  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+00000000000000e8  0000000800000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+0000000000000113  0000000600000004 R_X86_64_PLT32         0000000000000000 addp - 4
+0000000000000079  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x398 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x3e0 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,43 +9,43 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..00000000000000df
+00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..000000000000012b
   DW_CFA_advance_loc: 13 to 000000000000000d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_advance_loc: 4 to 0000000000000011
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_advance_loc: 4 to 0000000000000015
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
-  DW_CFA_advance_loc: 44 to 0000000000000041
+  DW_CFA_advance_loc: 31 to 0000000000000034
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 0000000000000042
+  DW_CFA_advance_loc: 1 to 0000000000000035
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000044
+  DW_CFA_advance_loc: 2 to 0000000000000037
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 0000000000000048
+  DW_CFA_advance_loc: 9 to 0000000000000040
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 25 to 0000000000000061
+  DW_CFA_advance_loc: 50 to 0000000000000072
   DW_CFA_restore: r3 (rbx)
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 4 to 0000000000000065
+  DW_CFA_advance_loc: 4 to 0000000000000076
   DW_CFA_restore: r6 (rbp)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000067
+  DW_CFA_advance_loc: 2 to 0000000000000078
   DW_CFA_restore: r12 (r12)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 17 to 0000000000000078
+  DW_CFA_advance_loc: 16 to 0000000000000088
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-32
   DW_CFA_offset: r6 (rbp) at cfa-24
   DW_CFA_offset: r12 (r12) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,86 +4,102 @@
 Disassembly of section .text:
 
 0000000000000000 <subtract>:
 subtract():
 	endbr64
 	movzbl (%rdi),%eax
 	test   %al,%al
-	je     70 <subtract+0x70>
+	je     80 <subtract+0x80>
 	push   %r12
 	mov    %rdx,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	movzbl (%rsi),%edx
 	test   %dl,%dl
-	je     40 <subtract+0x40>
+	je     33 <subtract+0x33>
 	mov    %rdi,%rbx
-	cmp    $0x2d,%dl
-	je     57 <subtract+0x57>
-	cmp    $0x2d,%al
-	jne    48 <subtract+0x48>
-	cmp    $0x2d,%dl
-	jne    78 <subtract+0x78>
-	lea    0x1(%rbx),%rsi
-	lea    0x1(%rbp),%rdi
-	mov    %r12,%rdx
-	call   3d <subtract+0x3d>
- R_X86_64_PLT32	subtractp-0x4
-	jmp    60 <subtract+0x60>
-	nop
+	cmp    $0x75,%al
+	jne    40 <subtract+0x40>
+	cmpb   $0x0,0x1(%rdi)
+	jne    40 <subtract+0x40>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
-	nopl   (%rax)
+	nopl   0x0(%rax,%rax,1)
+	cmpb   $0x75,0x0(%rbp)
+	je     88 <subtract+0x88>
+	cmp    $0x2d,%dl
+	je     64 <subtract+0x64>
+	cmp    $0x2d,%al
+	je     a0 <subtract+0xa0>
 	mov    %r12,%rdx
-	call   50 <subtract+0x50>
+	mov    %rbp,%rsi
+	mov    %rbx,%rdi
+	call   5d <subtract+0x5d>
  R_X86_64_PLT32	subtractp-0x4
 	movzbl (%rbx),%eax
 	movzbl 0x0(%rbp),%edx
 	cmp    $0x2d,%al
-	je     28 <subtract+0x28>
+	je     a0 <subtract+0xa0>
 	cmp    $0x2d,%dl
-	je     c0 <subtract+0xc0>
+	je     108 <subtract+0x108>
 	pop    %rbx
 	mov    %r12,%rdi
 	pop    %rbp
 	pop    %r12
-	jmp    6c <subtract+0x6c>
+	jmp    7d <subtract+0x7d>
  R_X86_64_PLT32	remove_zeroes-0x4
-	nopl   0x0(%rax)
+	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
+	cmpb   $0x0,0x1(%rbp)
+	jne    46 <subtract+0x46>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	jmp    33 <subtract+0x33>
+	nopw   0x0(%rax,%rax,1)
+	cmp    $0x2d,%dl
+	jne    c0 <subtract+0xc0>
+	lea    0x1(%rbx),%rsi
+	lea    0x1(%rbp),%rdi
+	mov    %r12,%rdx
+	call   b5 <subtract+0xb5>
+ R_X86_64_PLT32	subtractp-0x4
+	jmp    71 <subtract+0x71>
+	nopw   0x0(%rax,%rax,1)
 	mov    %r12,%rdx
 	lea    0x1(%rbx),%rdi
 	mov    %rbp,%rsi
-	call   87 <subtract+0x87>
+	call   cf <subtract+0xcf>
  R_X86_64_PLT32	addp-0x4
 	mov    %r12,%rdi
-	call   8f <subtract+0x8f>
+	call   d7 <subtract+0xd7>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rax,%rdx
 	test   %rax,%rax
-	je     a4 <subtract+0xa4>
+	je     ec <subtract+0xec>
 	lea    0x1(%r12),%rdi
 	mov    %r12,%rsi
-	call   a4 <subtract+0xa4>
+	call   ec <subtract+0xec>
  R_X86_64_PLT32	memmove-0x4
 	movb   $0x2d,(%r12)
 	cmpb   $0x2d,(%rbx)
-	jne    d6 <subtract+0xd6>
+	jne    122 <subtract+0x122>
 	movzbl 0x0(%rbp),%eax
 	cmp    $0x2d,%al
-	jne    60 <subtract+0x60>
-	jmp    2d <subtract+0x2d>
-	nopl   0x0(%rax,%rax,1)
+	jne    71 <subtract+0x71>
+	jmp    a5 <subtract+0xa5>
+	nopl   0x0(%rax)
 	lea    0x1(%rbp),%rsi
 	mov    %r12,%rdx
 	mov    %rbx,%rdi
-	call   cf <subtract+0xcf>
+	call   117 <subtract+0x117>
  R_X86_64_PLT32	addp-0x4
 	cmpb   $0x2d,(%rbx)
-	jne    60 <subtract+0x60>
-	jmp    ae <subtract+0xae>
+	jne    71 <subtract+0x71>
+	jmp    f6 <subtract+0xf6>
 	movzbl 0x0(%rbp),%edx
-	jmp    5b <subtract+0x5b>
+	jmp    68 <subtract+0x68>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 44000000 1c000000 ........D.......
-  0x00000020 00000000 df000000 004d0e10 8c02440e .........M....D.
-  0x00000030 18860344 0e208304 6c0a0e18 410e1042 ...D. ..l...A..B
-  0x00000040 0e08440b 59c30e18 44c60e10 42cc0e08 ..D.Y...D...B...
-  0x00000050 510e2083 0486038c 02000000 00000000 Q. .............
+  0x00000020 00000000 2b010000 004d0e10 8c02440e ....+....M....D.
+  0x00000030 18860344 0e208304 5f0a0e18 410e1042 ...D. .._...A..B
+  0x00000040 0e08490b 72c30e18 44c60e10 42cc0e08 ..I.r...D...B...
+  0x00000050 500e2083 0486038c 02000000 00000000 P. .............
```

#### multiply.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1184 (bytes into file)
+  Start of section headers:          1200 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x4a0:
+There are 13 section headers, starting at offset 0x4b0:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 000133 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000340 0000d8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000173 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000173 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000173 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00019f 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000080 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000418 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000240 0000c0 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000300 000040 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000430 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000153 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000350 0000d8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000193 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000193 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000193 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001bf 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0001c0 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001e0 000070 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000428 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000250 0000c0 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000310 000040 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000440 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,11 +1,11 @@
 
 Symbol table '.symtab' contains 8 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS multiply.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   307 FUNC    GLOBAL DEFAULT    1 multiply
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
-     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiplyp
+     3: 0000000000000000   339 FUNC    GLOBAL DEFAULT    1 multiply
+     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiplyp
+     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,16 +1,16 @@
 
-Relocation section '.rela.text' at offset 0x340 contains 9 entries:
+Relocation section '.rela.text' at offset 0x350 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000064  0000000500000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
-0000000000000097  0000000500000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
-000000000000009f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000b4  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000000db  0000000500000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
-00000000000000e3  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000f8  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-000000000000011b  0000000500000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
-0000000000000049  0000000400000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+0000000000000068  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
+00000000000000c3  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
+00000000000000cb  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+00000000000000e0  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+0000000000000103  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
+000000000000010b  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+0000000000000120  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000013b  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
+000000000000008a  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x418 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x428 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,71 +9,56 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000064 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000133
-  DW_CFA_advance_loc: 13 to 000000000000000d
+00000018 0000000000000054 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000153
+  DW_CFA_advance_loc: 17 to 0000000000000011
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000000f
+  DW_CFA_advance_loc: 2 to 0000000000000013
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 4 to 0000000000000013
+  DW_CFA_advance_loc: 4 to 0000000000000017
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 1 to 0000000000000014
+  DW_CFA_advance_loc: 1 to 0000000000000018
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 000000000000001b
+  DW_CFA_advance_loc: 7 to 000000000000001f
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 36 to 000000000000003f
+  DW_CFA_advance_loc: 34 to 0000000000000041
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 0000000000000043
-  DW_CFA_restore: r3 (rbx)
+  DW_CFA_advance_loc: 1 to 0000000000000042
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000000044
-  DW_CFA_restore: r6 (rbp)
+  DW_CFA_advance_loc: 1 to 0000000000000043
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000046
-  DW_CFA_restore: r12 (r12)
+  DW_CFA_advance_loc: 2 to 0000000000000045
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000048
-  DW_CFA_restore: r13 (r13)
+  DW_CFA_advance_loc: 2 to 0000000000000047
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000050
+  DW_CFA_advance_loc: 9 to 0000000000000050
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 4 to 0000000000000054
-  DW_CFA_remember_state
+  DW_CFA_advance_loc: 48 to 0000000000000080
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000000055
-  DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000000056
-  DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000058
-  DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000005a
-  DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 0000000000000060
-  DW_CFA_restore_state
-  DW_CFA_advance_loc: 24 to 0000000000000078
-  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 4 to 0000000000000084
   DW_CFA_restore: r3 (rbx)
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 0000000000000085
   DW_CFA_restore: r6 (rbp)
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000000087
   DW_CFA_restore: r12 (r12)
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000000089
   DW_CFA_restore: r13 (r13)
-  DW_CFA_advance_loc: 8 to 0000000000000080
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 15 to 0000000000000098
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-40
   DW_CFA_offset: r6 (rbp) at cfa-32
   DW_CFA_offset: r12 (r12) at cfa-24
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
```

##### strings --all --bytes=8 {}

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 multiply.c
 multiply
-remove_zeroes
 multiplyp
+remove_zeroes
 strlen_asm
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,104 +4,118 @@
 Disassembly of section .text:
 
 0000000000000000 <multiply>:
 multiply():
 	endbr64
 	movzbl (%rdi),%eax
 	test   %al,%al
-	je     78 <multiply+0x78>
+	je     90 <multiply+0x90>
 	push   %r13
 	push   %r12
 	mov    %rdx,%r12
 	push   %rbp
 	push   %rbx
 	mov    %rsi,%rbx
 	sub    $0x8,%rsp
 	movzbl (%rsi),%edx
 	test   %dl,%dl
-	je     50 <multiply+0x50>
+	je     3d <multiply+0x3d>
 	mov    %rdi,%rbp
-	cmp    $0x2d,%al
-	je     80 <multiply+0x80>
-	cmp    $0x2d,%dl
-	jne    60 <multiply+0x60>
-	cmp    $0x2d,%al
-	je     80 <multiply+0x80>
-	cmp    $0x2d,%dl
-	je     d0 <multiply+0xd0>
-	add    $0x8,%rsp
-	mov    %r12,%rdi
-	pop    %rbx
-	pop    %rbp
-	pop    %r12
-	pop    %r13
-	jmp    4d <multiply+0x4d>
- R_X86_64_PLT32	remove_zeroes-0x4
-	nopl   (%rax)
+	cmp    $0x75,%al
+	jne    50 <multiply+0x50>
+	cmpb   $0x0,0x1(%rdi)
+	jne    50 <multiply+0x50>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	nopl   0x0(%rax,%rax,1)
+	cmpb   $0x75,(%rbx)
+	je     98 <multiply+0x98>
+	cmp    $0x2d,%dl
+	je     73 <multiply+0x73>
+	cmp    $0x2d,%al
+	je     b0 <multiply+0xb0>
 	mov    %r12,%rdx
-	call   68 <multiply+0x68>
+	mov    %rbx,%rsi
+	mov    %rbp,%rdi
+	call   6c <multiply+0x6c>
  R_X86_64_PLT32	multiplyp-0x4
 	movzbl 0x0(%rbp),%eax
 	movzbl (%rbx),%edx
-	jmp    2e <multiply+0x2e>
-	nopl   0x0(%rax)
+	cmp    $0x2d,%al
+	je     b0 <multiply+0xb0>
+	cmp    $0x2d,%dl
+	je     f8 <multiply+0xf8>
+	add    $0x8,%rsp
+	mov    %r12,%rdi
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	jmp    8e <multiply+0x8e>
+ R_X86_64_PLT32	remove_zeroes-0x4
+	xchg   %ax,%ax
 	ret
 	nopl   0x0(%rax)
+	cmpb   $0x0,0x1(%rbx)
+	jne    55 <multiply+0x55>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	jmp    3d <multiply+0x3d>
+	nopw   0x0(%rax,%rax,1)
 	lea    0x1(%rbp),%r13
 	cmp    $0x2d,%dl
-	je     110 <multiply+0x110>
+	je     130 <multiply+0x130>
 	mov    %r12,%rdx
 	mov    %rbx,%rsi
 	mov    %r13,%rdi
-	call   9b <multiply+0x9b>
+	call   c7 <multiply+0xc7>
  R_X86_64_PLT32	multiplyp-0x4
 	mov    %r12,%rdi
-	call   a3 <multiply+0xa3>
+	call   cf <multiply+0xcf>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rax,%rdx
 	test   %rax,%rax
-	je     b8 <multiply+0xb8>
+	je     e4 <multiply+0xe4>
 	lea    0x1(%r12),%rdi
 	mov    %r12,%rsi
-	call   b8 <multiply+0xb8>
+	call   e4 <multiply+0xe4>
  R_X86_64_PLT32	memmove-0x4
 	movb   $0x2d,(%r12)
 	cmpb   $0x2d,0x0(%rbp)
-	je     3b <multiply+0x3b>
+	je     7c <multiply+0x7c>
 	movzbl (%rbx),%edx
-	jmp    32 <multiply+0x32>
-	nop
+	jmp    77 <multiply+0x77>
+	nopl   0x0(%rax)
 	mov    %r12,%rdx
 	lea    0x1(%rbx),%rsi
 	mov    %rbp,%rdi
-	call   df <multiply+0xdf>
+	call   107 <multiply+0x107>
  R_X86_64_PLT32	multiplyp-0x4
 	mov    %r12,%rdi
-	call   e7 <multiply+0xe7>
+	call   10f <multiply+0x10f>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rax,%rdx
 	test   %rax,%rax
-	je     fc <multiply+0xfc>
+	je     124 <multiply+0x124>
 	lea    0x1(%r12),%rdi
 	mov    %r12,%rsi
-	call   fc <multiply+0xfc>
+	call   124 <multiply+0x124>
  R_X86_64_PLT32	memmove-0x4
 	movb   $0x2d,(%r12)
-	jmp    3b <multiply+0x3b>
-	cs nopw 0x0(%rax,%rax,1)
+	jmp    7c <multiply+0x7c>
+	xchg   %ax,%ax
 	lea    0x1(%rbx),%rsi
 	mov    %r12,%rdx
 	mov    %r13,%rdi
-	call   11f <multiply+0x11f>
+	call   13f <multiply+0x13f>
  R_X86_64_PLT32	multiplyp-0x4
 	cmpb   $0x2d,0x0(%rbp)
-	jne    c7 <multiply+0xc7>
+	jne    ef <multiply+0xef>
 	cmpb   $0x2d,(%rbx)
-	je     3b <multiply+0x3b>
-	jmp    8d <multiply+0x8d>
+	je     7c <multiply+0x7c>
+	jmp    b9 <multiply+0xb9>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,12 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 64000000 1c000000 ........d.......
-  0x00000020 00000000 33010000 004d0e10 8d02420e ....3....M....B.
+  0x00000010 1b0c0708 90010000 54000000 1c000000 ........T.......
+  0x00000020 00000000 53010000 00510e10 8d02420e ....S....Q....B.
   0x00000030 188c0344 0e208604 410e2883 05470e30 ...D. ..A.(..G.0
-  0x00000040 640a0e28 44c30e20 41c60e18 42cc0e10 d..(D.. A...B...
-  0x00000050 42cd0e08 480b440a 0e28410e 20410e18 B...H.D..(A. A..
-  0x00000060 420e1042 0e08460b 580e08c3 c6cccd48 B..B..F.X......H
-  0x00000070 0e308305 86048c03 8d020000 00000000 .0..............
+  0x00000040 620a0e28 410e2041 0e18420e 10420e08 b..(A. A..B..B..
+  0x00000050 490b700e 2844c30e 2041c60e 1842cc0e I.p.(D.. A...B..
+  0x00000060 1042cd0e 084f0e30 83058604 8c038d02 .B...O.0........
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,7 +1,7 @@
 
 Hex dump of section '.strtab':
   0x00000000 006d756c 7469706c 792e6300 6d756c74 .multiply.c.mult
-  0x00000010 69706c79 0072656d 6f76655f 7a65726f iply.remove_zero
-  0x00000020 6573006d 756c7469 706c7970 00737472 es.multiplyp.str
+  0x00000010 69706c79 006d756c 7469706c 79700072 iply.multiplyp.r
+  0x00000020 656d6f76 655f7a65 726f6573 00737472 emove_zeroes.str
   0x00000030 6c656e5f 61736d00 6d656d6d 6f766500 len_asm.memmove.
```

#### divide_whole_with_remainder.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1104 (bytes into file)
+  Start of section headers:          1288 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x450:
+There are 13 section headers, starting at offset 0x508:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 0000b0 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 0002f0 0000d8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 0000f0 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 0000f0 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000f0 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00011c 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000120 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000140 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 0003c8 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0001a0 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000278 000071 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 0003e0 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000149 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 0003a8 0000d8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000189 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000189 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000189 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001b5 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0001b8 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001d8 000080 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000480 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000258 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000330 000071 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000498 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,12 +1,12 @@
 
 Symbol table '.symtab' contains 9 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS divide_whole_with_remainder.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   176 FUNC    GLOBAL DEFAULT    1 divide_whole_with_remainder
+     3: 0000000000000000   329 FUNC    GLOBAL DEFAULT    1 divide_whole_with_remainder
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _divide_whole_with_remainder
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_leading_zeroes_inplace
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
```

##### readelf --wide --relocs {}

```diff
@@ -1,16 +1,16 @@
 
-Relocation section '.rela.text' at offset 0x2f0 contains 9 entries:
+Relocation section '.rela.text' at offset 0x3a8 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000001f  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-000000000000002a  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-0000000000000037  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-000000000000004e  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000067  0000000600000004 R_X86_64_PLT32         0000000000000000 _divide_whole_with_remainder - 4
-0000000000000072  0000000700000004 R_X86_64_PLT32         0000000000000000 remove_leading_zeroes_inplace - 4
-000000000000007a  0000000700000004 R_X86_64_PLT32         0000000000000000 remove_leading_zeroes_inplace - 4
-0000000000000091  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000ac  0000000800000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000074  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+000000000000007f  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+000000000000008c  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+00000000000000a3  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000000bc  0000000600000004 R_X86_64_PLT32         0000000000000000 _divide_whole_with_remainder - 4
+00000000000000c7  0000000700000004 R_X86_64_PLT32         0000000000000000 remove_leading_zeroes_inplace - 4
+00000000000000cf  0000000700000004 R_X86_64_PLT32         0000000000000000 remove_leading_zeroes_inplace - 4
+00000000000000e9  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+0000000000000104  0000000800000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x3c8 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x480 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,43 +9,68 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..00000000000000b0
+00000018 0000000000000064 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000149
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 5 to 000000000000000b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000000010
+  DW_CFA_advance_loc: 2 to 000000000000000d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000000012
+  DW_CFA_advance_loc: 5 to 0000000000000012
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_advance_loc: 4 to 0000000000000016
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 4 to 000000000000001a
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_advance_loc: 4 to 000000000000001e
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 128 to 000000000000009e
+  DW_CFA_advance_loc: 35 to 0000000000000041
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000000a2
+  DW_CFA_advance_loc: 1 to 0000000000000042
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000000a3
+  DW_CFA_advance_loc: 1 to 0000000000000043
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000000a5
+  DW_CFA_advance_loc: 2 to 0000000000000045
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000000a7
+  DW_CFA_advance_loc: 2 to 0000000000000047
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000000a9
+  DW_CFA_advance_loc: 2 to 0000000000000049
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000000ab
+  DW_CFA_advance_loc: 2 to 000000000000004b
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 5 to 0000000000000050
+  DW_CFA_restore_state
+  DW_CFA_advance_loc1: 166 to 00000000000000f6
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 4 to 00000000000000fa
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 00000000000000fb
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 2 to 00000000000000fd
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 00000000000000ff
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000000101
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000000103
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 13 to 0000000000000110
+  DW_CFA_restore_state
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,9 @@
 []A\A]A^A_
+[]A\A]A^A_
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 divide_whole_with_remainder.c
 strlen_asm
 _divide_whole_with_remainder
 remove_leading_zeroes_inplace
 .shstrtab
 .rela.text
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5,66 +5,106 @@
 
 0000000000000000 <divide_whole_with_remainder>:
 divide_whole_with_remainder():
 	endbr64
 	push   %r15
 	mov    %rdi,%r15
 	push   %r14
-	mov    %rdx,%r14
 	push   %r13
+	mov    %rdx,%r13
 	push   %r12
 	mov    %rcx,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	sub    $0x8,%rsp
-	call   23 <divide_whole_with_remainder+0x23>
+	cmpb   $0x75,(%rdi)
+	jne    50 <divide_whole_with_remainder+0x50>
+	cmpb   $0x0,0x1(%rdi)
+	jne    50 <divide_whole_with_remainder+0x50>
+	mov    $0x75,%eax
+	mov    $0x75,%edx
+	mov    %ax,0x0(%r13)
+	mov    %dx,(%r12)
+	add    $0x8,%rsp
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+	nopl   0x0(%rax)
+	movzbl 0x0(%rbp),%eax
+	cmp    $0x75,%eax
+	je     110 <divide_whole_with_remainder+0x110>
+	cmp    $0x30,%eax
+	je     120 <divide_whole_with_remainder+0x120>
+	cmpb   $0x2d,0x0(%rbp)
+	je     130 <divide_whole_with_remainder+0x130>
+	mov    %r15,%rdi
+	call   78 <divide_whole_with_remainder+0x78>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rbp,%rdi
 	mov    %rax,%rbx
-	call   2e <divide_whole_with_remainder+0x2e>
+	call   83 <divide_whole_with_remainder+0x83>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rbp,%rdi
 	lea    0x2(%rbx,%rax,1),%rbx
-	call   3b <divide_whole_with_remainder+0x3b>
+	call   90 <divide_whole_with_remainder+0x90>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    $0x1,%esi
 	lea    (%rax,%rax,4),%rdx
 	lea    (%rbx,%rbx,4),%rax
 	lea    0x17(%rax,%rdx,2),%rdi
-	call   52 <divide_whole_with_remainder+0x52>
+	call   a7 <divide_whole_with_remainder+0xa7>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rbx,%rcx
 	mov    %rbp,%rsi
-	mov    %r14,%rdx
+	mov    %r13,%rdx
 	mov    %rax,%r8
 	mov    %r15,%rdi
-	mov    %rax,%r13
+	mov    %rax,%r14
 	xor    %ebx,%ebx
-	call   6b <divide_whole_with_remainder+0x6b>
+	call   c0 <divide_whole_with_remainder+0xc0>
  R_X86_64_PLT32	_divide_whole_with_remainder-0x4
-	mov    %r14,%rdi
+	mov    %r13,%rdi
 	mov    %rax,%rbp
-	call   76 <divide_whole_with_remainder+0x76>
+	call   cb <divide_whole_with_remainder+0xcb>
  R_X86_64_PLT32	remove_leading_zeroes_inplace-0x4
 	mov    %rbp,%rdi
-	call   7e <divide_whole_with_remainder+0x7e>
+	call   d3 <divide_whole_with_remainder+0xd3>
  R_X86_64_PLT32	remove_leading_zeroes_inplace-0x4
-	jmp    8d <divide_whole_with_remainder+0x8d>
+	jmp    e5 <divide_whole_with_remainder+0xe5>
+	nopl   (%rax)
 	movzbl 0x0(%rbp,%rbx,1),%eax
 	mov    %al,(%r12,%rbx,1)
 	add    $0x1,%rbx
 	mov    %rbp,%rdi
-	call   95 <divide_whole_with_remainder+0x95>
+	call   ed <divide_whole_with_remainder+0xed>
  R_X86_64_PLT32	strlen_asm-0x4
 	cmp    %rbx,%rax
-	ja     80 <divide_whole_with_remainder+0x80>
+	ja     d8 <divide_whole_with_remainder+0xd8>
 	add    $0x8,%rsp
-	mov    %r13,%rdi
+	mov    %r14,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    b0 <divide_whole_with_remainder+0xb0>
+	jmp    108 <divide_whole_with_remainder+0x108>
  R_X86_64_PLT32	free-0x4
+	nopl   0x0(%rax,%rax,1)
+	cmpb   $0x0,0x1(%rbp)
+	je     29 <divide_whole_with_remainder+0x29>
+	jmp    5d <divide_whole_with_remainder+0x5d>
+	nop
+	cmpb   $0x0,0x1(%rbp)
+	je     29 <divide_whole_with_remainder+0x29>
+	jmp    66 <divide_whole_with_remainder+0x66>
+	nop
+	cmpb   $0x30,0x1(%rbp)
+	jne    70 <divide_whole_with_remainder+0x70>
+	cmpb   $0x0,0x2(%rbp)
+	je     29 <divide_whole_with_remainder+0x29>
+	jmp    70 <divide_whole_with_remainder+0x70>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,10 +1,12 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 44000000 1c000000 ........D.......
-  0x00000020 00000000 b0000000 00460e10 8f02450e .........F....E.
-  0x00000030 188e0345 0e208d04 420e288c 05440e30 ...E. ..B.(..D.0
-  0x00000040 8606440e 38830744 0e400280 0e38440e ..D.8..D.@...8D.
+  0x00000010 1b0c0708 90010000 64000000 1c000000 ........d.......
+  0x00000020 00000000 49010000 00460e10 8f02450e ....I....F....E.
+  0x00000030 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
+  0x00000040 8606440e 38830744 0e40630a 0e38410e ..D.8..D.@c..8A.
   0x00000050 30410e28 420e2042 0e18420e 10420e08 0A.(B. B..B..B..
+  0x00000060 450b02a6 0a0e3844 0e30410e 28420e20 E.....8D.0A.(B. 
+  0x00000070 420e1842 0e10420e 084d0b00 00000000 B..B..B..M......
```

#### divide.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1192 (bytes into file)
+  Start of section headers:          1344 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x4a8:
+There are 13 section headers, starting at offset 0x540:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 000136 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000348 0000d8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000176 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000176 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000176 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001a2 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 0001a8 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0001c8 000080 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000420 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000248 0000c0 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000308 00003a 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000438 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 0001d0 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 0003e0 0000d8 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000210 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000210 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000210 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00023c 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000240 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000260 000080 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 0004b8 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 0002e0 0000c0 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0003a0 00003a 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 0004d0 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,11 +1,11 @@
 
 Symbol table '.symtab' contains 8 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS divide.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   310 FUNC    GLOBAL DEFAULT    1 divide
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
-     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND dividep
-     6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
-     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
+     3: 0000000000000000   464 FUNC    GLOBAL DEFAULT    1 divide
+     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND dividep
+     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
+     6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
+     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
```

##### readelf --wide --relocs {}

```diff
@@ -1,16 +1,16 @@
 
-Relocation section '.rela.text' at offset 0x348 contains 9 entries:
+Relocation section '.rela.text' at offset 0x3e0 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000064  0000000500000004 R_X86_64_PLT32         0000000000000000 dividep - 4
-000000000000009a  0000000500000004 R_X86_64_PLT32         0000000000000000 dividep - 4
-00000000000000a2  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000b6  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000000e6  0000000500000004 R_X86_64_PLT32         0000000000000000 dividep - 4
-00000000000000ee  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-0000000000000102  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-000000000000011e  0000000500000004 R_X86_64_PLT32         0000000000000000 dividep - 4
-0000000000000048  0000000400000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
+00000000000000a1  0000000400000004 R_X86_64_PLT32         0000000000000000 dividep - 4
+00000000000000a9  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+00000000000000c8  0000000600000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000012f  0000000400000004 R_X86_64_PLT32         0000000000000000 dividep - 4
+000000000000017b  0000000400000004 R_X86_64_PLT32         0000000000000000 dividep - 4
+0000000000000183  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+0000000000000198  0000000600000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000001b3  0000000400000004 R_X86_64_PLT32         0000000000000000 dividep - 4
+000000000000015a  0000000700000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x420 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x4b8 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,69 +9,69 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000064 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000136
-  DW_CFA_advance_loc: 13 to 000000000000000d
+00000018 0000000000000064 0000001c FDE cie=00000000 pc=0000000000000000..00000000000001d0
+  DW_CFA_advance_loc: 17 to 0000000000000011
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000000f
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000000013
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 0000000000000014
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_advance_loc: 4 to 0000000000000017
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 0000000000000015
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000000018
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000016
-  DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc: 39 to 000000000000003d
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_advance_loc: 7 to 000000000000001f
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc: 34 to 0000000000000041
   DW_CFA_remember_state
-  DW_CFA_restore: r3 (rbx)
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 0000000000000041
-  DW_CFA_restore: r6 (rbp)
+  DW_CFA_advance_loc: 1 to 0000000000000042
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000043
-  DW_CFA_restore: r12 (r12)
+  DW_CFA_advance_loc: 1 to 0000000000000043
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 2 to 0000000000000045
-  DW_CFA_restore: r13 (r13)
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 2 to 0000000000000047
-  DW_CFA_restore: r14 (r14)
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 9 to 0000000000000050
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 1 to 0000000000000051
+  DW_CFA_advance_loc1: 152 to 00000000000000e8
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_restore: r3 (rbx)
+  DW_CFA_restore: r6 (rbp)
+  DW_CFA_restore: r12 (r12)
+  DW_CFA_restore: r13 (r13)
+  DW_CFA_advance_loc: 8 to 00000000000000f0
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc1: 96 to 0000000000000150
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 1 to 0000000000000052
+  DW_CFA_advance_loc: 4 to 0000000000000154
+  DW_CFA_restore: r3 (rbx)
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000000054
+  DW_CFA_advance_loc: 1 to 0000000000000155
+  DW_CFA_restore: r6 (rbp)
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000000056
+  DW_CFA_advance_loc: 2 to 0000000000000157
+  DW_CFA_restore: r12 (r12)
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000058
+  DW_CFA_advance_loc: 2 to 0000000000000159
+  DW_CFA_restore: r13 (r13)
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000000060
+  DW_CFA_advance_loc: 7 to 0000000000000160
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 24 to 0000000000000078
-  DW_CFA_def_cfa_offset: 8
-  DW_CFA_restore: r3 (rbx)
-  DW_CFA_restore: r6 (rbp)
-  DW_CFA_restore: r12 (r12)
-  DW_CFA_restore: r13 (r13)
-  DW_CFA_restore: r14 (r14)
-  DW_CFA_advance_loc: 8 to 0000000000000080
-  DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
```

##### strings --all --bytes=8 {}

```diff
@@ -1,11 +1,10 @@
-[]A\A]A^
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 divide.c
-remove_zeroes
 strlen_asm
+remove_zeroes
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,107 +4,140 @@
 Disassembly of section .text:
 
 0000000000000000 <divide>:
 divide():
 	endbr64
 	movzbl (%rdi),%eax
 	test   %al,%al
-	je     78 <divide+0x78>
-	push   %r14
+	je     e8 <divide+0xe8>
 	push   %r13
-	mov    %rdx,%r13
 	push   %r12
+	mov    %rdx,%r12
 	push   %rbp
 	push   %rbx
-	movzbl (%rsi),%edx
 	mov    %rsi,%rbx
+	sub    $0x18,%rsp
+	movzbl (%rsi),%edx
 	test   %dl,%dl
-	je     50 <divide+0x50>
+	je     3d <divide+0x3d>
 	mov    %rdi,%rbp
-	mov    %rcx,%r12
-	cmp    $0x2d,%al
-	je     80 <divide+0x80>
-	cmp    $0x2d,%dl
-	jne    60 <divide+0x60>
-	cmp    $0x2d,%al
-	je     80 <divide+0x80>
-	cmp    $0x2d,%dl
-	je     d8 <divide+0xd8>
+	cmp    $0x75,%al
+	jne    50 <divide+0x50>
+	cmpb   $0x0,0x1(%rdi)
+	jne    50 <divide+0x50>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	add    $0x18,%rsp
 	pop    %rbx
-	mov    %r13,%rdi
 	pop    %rbp
 	pop    %r12
 	pop    %r13
-	pop    %r14
-	jmp    4c <divide+0x4c>
- R_X86_64_PLT32	remove_zeroes-0x4
-	nopl   0x0(%rax)
-	pop    %rbx
-	pop    %rbp
-	pop    %r12
-	pop    %r13
-	pop    %r14
 	ret
-	nopl   0x0(%rax)
-	mov    %r13,%rdx
-	call   68 <divide+0x68>
- R_X86_64_PLT32	dividep-0x4
-	movzbl 0x0(%rbp),%eax
-	movzbl (%rbx),%edx
-	jmp    2f <divide+0x2f>
-	nopl   0x0(%rax)
-	ret
-	nopl   0x0(%rax)
-	lea    0x1(%rbp),%r14
-	cmp    $0x2d,%dl
+	nopl   0x0(%rax,%rax,1)
+	movzbl (%rbx),%esi
+	cmp    $0x75,%esi
+	je     f0 <divide+0xf0>
+	cmp    $0x30,%esi
 	je     110 <divide+0x110>
-	mov    %r13,%rdx
-	mov    %r12,%rcx
+	cmpb   $0x2d,(%rbx)
+	jne    74 <divide+0x74>
+	cmpb   $0x30,0x1(%rbx)
+	je     160 <divide+0x160>
+	cmp    $0x2d,%dl
+	je     13f <divide+0x13f>
+	cmp    $0x2d,%al
+	jne    120 <divide+0x120>
+	lea    0x1(%rbp),%r13
+	cmp    $0x2d,%dl
+	je     1a3 <divide+0x1a3>
+	mov    %r12,%rdx
 	mov    %rbx,%rsi
-	mov    %r14,%rdi
-	call   9e <divide+0x9e>
- R_X86_64_PLT32	dividep-0x4
 	mov    %r13,%rdi
-	call   a6 <divide+0xa6>
+	mov    %rcx,0x8(%rsp)
+	call   a5 <divide+0xa5>
+ R_X86_64_PLT32	dividep-0x4
+	mov    %r12,%rdi
+	call   ad <divide+0xad>
  R_X86_64_PLT32	strlen_asm-0x4
-	mov    %rax,%rdx
+	mov    0x8(%rsp),%rcx
 	test   %rax,%rax
-	je     ba <divide+0xba>
-	lea    0x1(%r13),%rdi
-	mov    %r13,%rsi
-	call   ba <divide+0xba>
+	mov    %rax,%rdx
+	je     d1 <divide+0xd1>
+	lea    0x1(%r12),%rdi
+	mov    %r12,%rsi
+	mov    %rcx,0x8(%rsp)
+	call   cc <divide+0xcc>
  R_X86_64_PLT32	memmove-0x4
-	movb   $0x2d,0x0(%r13)
+	mov    0x8(%rsp),%rcx
+	movb   $0x2d,(%r12)
 	cmpb   $0x2d,0x0(%rbp)
-	je     3c <divide+0x3c>
+	je     14c <divide+0x14c>
 	movzbl (%rbx),%edx
-	jmp    33 <divide+0x33>
+	jmp    147 <divide+0x147>
 	nopl   0x0(%rax)
-	mov    %r13,%rdx
+	ret
+	nopl   0x0(%rax)
+	cmpb   $0x0,0x1(%rbx)
+	jne    5c <divide+0x5c>
+	mov    $0x75,%eax
+	mov    %ax,(%r12)
+	jmp    3d <divide+0x3d>
+	nopl   0x0(%rax)
+	cmpb   $0x0,0x1(%rbx)
+	je     33 <divide+0x33>
+	jmp    65 <divide+0x65>
+	nop
+	mov    %r12,%rdx
+	mov    %rbx,%rsi
+	mov    %rbp,%rdi
+	mov    %rcx,0x8(%rsp)
+	call   133 <divide+0x133>
+ R_X86_64_PLT32	dividep-0x4
+	movzbl 0x0(%rbp),%eax
+	movzbl (%rbx),%edx
+	mov    0x8(%rsp),%rcx
+	cmp    $0x2d,%al
+	je     85 <divide+0x85>
+	cmp    $0x2d,%dl
+	je     170 <divide+0x170>
+	add    $0x18,%rsp
+	mov    %r12,%rdi
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	jmp    15e <divide+0x15e>
+ R_X86_64_PLT32	remove_zeroes-0x4
+	xchg   %ax,%ax
+	cmpb   $0x0,0x2(%rbx)
+	je     33 <divide+0x33>
+	jmp    74 <divide+0x74>
+	nop
+	mov    %r12,%rdx
 	lea    0x1(%rbx),%rsi
-	mov    %r12,%rcx
 	mov    %rbp,%rdi
-	call   ea <divide+0xea>
+	call   17f <divide+0x17f>
  R_X86_64_PLT32	dividep-0x4
-	mov    %r13,%rdi
-	call   f2 <divide+0xf2>
+	mov    %r12,%rdi
+	call   187 <divide+0x187>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    %rax,%rdx
 	test   %rax,%rax
-	je     106 <divide+0x106>
-	lea    0x1(%r13),%rdi
-	mov    %r13,%rsi
-	call   106 <divide+0x106>
+	je     19c <divide+0x19c>
+	lea    0x1(%r12),%rdi
+	mov    %r12,%rsi
+	call   19c <divide+0x19c>
  R_X86_64_PLT32	memmove-0x4
-	movb   $0x2d,0x0(%r13)
-	jmp    3c <divide+0x3c>
+	movb   $0x2d,(%r12)
+	jmp    14c <divide+0x14c>
 	lea    0x1(%rbx),%rsi
-	mov    %r12,%rcx
-	mov    %r13,%rdx
-	mov    %r14,%rdi
-	call   122 <divide+0x122>
+	mov    %r12,%rdx
+	mov    %r13,%rdi
+	mov    %rcx,0x8(%rsp)
+	call   1b7 <divide+0x1b7>
  R_X86_64_PLT32	dividep-0x4
 	cmpb   $0x2d,0x0(%rbp)
-	jne    c9 <divide+0xc9>
+	mov    0x8(%rsp),%rcx
+	jne    dc <divide+0xdc>
 	cmpb   $0x2d,(%rbx)
-	je     3c <divide+0x3c>
-	jmp    8d <divide+0x8d>
+	je     14c <divide+0x14c>
+	jmp    92 <divide+0x92>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,12 +1,12 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 64000000 1c000000 ........d.......
-  0x00000020 00000000 36010000 004d0e10 8e02420e ....6....M....B.
-  0x00000030 188d0345 0e208c04 410e2886 05410e30 ...E. ..A.(..A.0
-  0x00000040 8306670a c30e2844 c60e2042 cc0e1842 ..g...(D.. B...B
-  0x00000050 cd0e1042 ce0e0849 0b410a0e 28410e20 ...B...I.A..(A. 
-  0x00000060 420e1842 0e10420e 08480b58 0e08c3c6 B..B..B..H.X....
-  0x00000070 cccdce48 0e308306 86058c04 8d038e02 ...H.0..........
+  0x00000020 00000000 d0010000 00510e10 8d02420e .........Q....B.
+  0x00000030 188c0344 0e208604 410e2883 05470e40 ...D. ..A.(..G.@
+  0x00000040 620a0e28 410e2041 0e18420e 10420e08 b..(A. A..B..B..
+  0x00000050 490b0298 0e08c3c6 cccd480e 40830586 I.........H.@...
+  0x00000060 048c038d 0202600a 0e2844c3 0e2041c6 ......`..(D.. A.
+  0x00000070 0e1842cc 0e1042cd 0e08470b 00000000 ..B...B...G.....
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,7 +1,7 @@
 
 Hex dump of section '.strtab':
   0x00000000 00646976 6964652e 63006469 76696465 .divide.c.divide
-  0x00000010 0072656d 6f76655f 7a65726f 65730064 .remove_zeroes.d
-  0x00000020 69766964 65700073 74726c65 6e5f6173 ividep.strlen_as
-  0x00000030 6d006d65 6d6d6f76 6500              m.memmove.
+  0x00000010 00646976 69646570 00737472 6c656e5f .dividep.strlen_
+  0x00000020 61736d00 6d656d6d 6f766500 72656d6f asm.memmove.remo
+  0x00000030 76655f7a 65726f65 7300              ve_zeroes.
```

### Comparing `basic_math_operations-1.0.163/src/python-module/module.c` & `basic_math_operations-1.0.164/src/python-module/module.c`

 * *Files identical despite different names*

