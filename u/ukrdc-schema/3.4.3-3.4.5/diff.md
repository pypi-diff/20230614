# Comparing `tmp/ukrdc_schema-3.4.3-py3-none-any.whl.zip` & `tmp/ukrdc_schema-3.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 254207 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-14 09:25 ukrdc_schema/__init__.py
--rw-r--r--  2.0 unx   245322 b- defN 23-Jun-14 09:25 ukrdc_schema/pv_2_0_schema.py
--rw-r--r--  2.0 unx  2996304 b- defN 23-Jun-14 09:25 ukrdc_schema/rrtf_schema.py
--rw-r--r--  2.0 unx  1146641 b- defN 23-Jun-14 09:25 ukrdc_schema/ukrdc_schema.py
--rw-r--r--  2.0 unx     1058 b- defN 23-Jun-14 09:25 ukrdc_schema/transforms/RR_XML_to_TXT.xsl
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-14 09:25 ukrdc_schema-3.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 09:25 ukrdc_schema-3.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-14 09:25 ukrdc_schema-3.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      757 b- defN 23-Jun-14 09:25 ukrdc_schema-3.4.3.dist-info/RECORD
-9 files, 4390454 bytes uncompressed, 252907 bytes compressed:  94.2%
+Zip file size: 254206 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-14 10:52 ukrdc_schema/__init__.py
+-rw-r--r--  2.0 unx   245322 b- defN 23-Jun-14 10:53 ukrdc_schema/pv_2_0_schema.py
+-rw-r--r--  2.0 unx  2996304 b- defN 23-Jun-14 10:53 ukrdc_schema/rrtf_schema.py
+-rw-r--r--  2.0 unx  1146641 b- defN 23-Jun-14 10:53 ukrdc_schema/ukrdc_schema.py
+-rw-r--r--  2.0 unx     1058 b- defN 23-Jun-14 10:52 ukrdc_schema/transforms/RR_XML_to_TXT.xsl
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-14 10:53 ukrdc_schema-3.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 10:53 ukrdc_schema-3.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-14 10:53 ukrdc_schema-3.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      757 b- defN 23-Jun-14 10:53 ukrdc_schema-3.4.5.dist-info/RECORD
+9 files, 4390454 bytes uncompressed, 252906 bytes compressed:  94.2%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: ukrdc_schema/ukrdc_schema.py
 Comment: 
 
 Filename: ukrdc_schema/transforms/RR_XML_to_TXT.xsl
 Comment: 
 
-Filename: ukrdc_schema-3.4.3.dist-info/METADATA
+Filename: ukrdc_schema-3.4.5.dist-info/METADATA
 Comment: 
 
-Filename: ukrdc_schema-3.4.3.dist-info/WHEEL
+Filename: ukrdc_schema-3.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: ukrdc_schema-3.4.3.dist-info/top_level.txt
+Filename: ukrdc_schema-3.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ukrdc_schema-3.4.3.dist-info/RECORD
+Filename: ukrdc_schema-3.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ukrdc_schema/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "3.4.3"
+__version__ = "3.4.5"
```

## ukrdc_schema/pv_2_0_schema.py

```diff
@@ -1,24 +1,24 @@
 # ./pyxb_build/ukrdc_schema/pv_2_0_schema.py
 # -*- coding: utf-8 -*-
 # PyXB bindings for NM:e92452c8d3e28a9e27abfc9994d2007779e7f4c9
-# Generated 2023-06-14 09:25:51.014313 by PyXB version 1.2.6 using Python 3.9.17.final.0
+# Generated 2023-06-14 10:53:09.718623 by PyXB version 1.2.6 using Python 3.9.16.final.0
 # Namespace AbsentNamespace0
 
 from __future__ import unicode_literals
 import pyxb
 import pyxb.binding
 import pyxb.binding.saxer
 import io
 import pyxb.utils.utility
 import pyxb.utils.domutils
 import sys
 import pyxb.utils.six as _six
 # Unique identifier for bindings created at the same time
-_GenerationUID = pyxb.utils.utility.UniqueIdentifier('urn:uuid:7415a41a-0a95-11ee-bb5c-b3667bb196e6')
+_GenerationUID = pyxb.utils.utility.UniqueIdentifier('urn:uuid:a693aef8-0aa1-11ee-9731-fbb9b58e295a')
 
 # Version of PyXB used to generate the bindings
 _PyXBVersion = '1.2.6'
 # Generated bindings are not compatible across PyXB versions
 if pyxb.__version__ != _PyXBVersion:
     raise pyxb.PyXBVersionError(_PyXBVersion)
```

## ukrdc_schema/rrtf_schema.py

```diff
@@ -1,24 +1,24 @@
 # ./pyxb_build/ukrdc_schema/rrtf_schema.py
 # -*- coding: utf-8 -*-
 # PyXB bindings for NM:e92452c8d3e28a9e27abfc9994d2007779e7f4c9
-# Generated 2023-06-14 09:25:52.836346 by PyXB version 1.2.6 using Python 3.9.17.final.0
+# Generated 2023-06-14 10:53:11.667390 by PyXB version 1.2.6 using Python 3.9.16.final.0
 # Namespace AbsentNamespace0
 
 from __future__ import unicode_literals
 import pyxb
 import pyxb.binding
 import pyxb.binding.saxer
 import io
 import pyxb.utils.utility
 import pyxb.utils.domutils
 import sys
 import pyxb.utils.six as _six
 # Unique identifier for bindings created at the same time
-_GenerationUID = pyxb.utils.utility.UniqueIdentifier('urn:uuid:74f17846-0a95-11ee-bb5c-b3667bb196e6')
+_GenerationUID = pyxb.utils.utility.UniqueIdentifier('urn:uuid:a7839a1c-0aa1-11ee-9731-fbb9b58e295a')
 
 # Version of PyXB used to generate the bindings
 _PyXBVersion = '1.2.6'
 # Generated bindings are not compatible across PyXB versions
 if pyxb.__version__ != _PyXBVersion:
     raise pyxb.PyXBVersionError(_PyXBVersion)
```

## ukrdc_schema/ukrdc_schema.py

```diff
@@ -3,19 +3,19 @@
 00000020: 635f 7363 6865 6d61 2e70 790a 2320 2d2a  c_schema.py.# -*
 00000030: 2d20 636f 6469 6e67 3a20 7574 662d 3820  - coding: utf-8 
 00000040: 2d2a 2d0a 2320 5079 5842 2062 696e 6469  -*-.# PyXB bindi
 00000050: 6e67 7320 666f 7220 4e4d 3a62 3238 3334  ngs for NM:b2834
 00000060: 3836 6364 3166 3965 3766 6231 6130 3732  86cd1f9e7fb1a072
 00000070: 3461 3433 3363 3166 3037 3037 3730 6630  4a433c1f070770f0
 00000080: 3836 390a 2320 4765 6e65 7261 7465 6420  869.# Generated 
-00000090: 3230 3233 2d30 362d 3134 2030 393a 3235  2023-06-14 09:25
-000000a0: 3a35 312e 3834 3635 3638 2062 7920 5079  :51.846568 by Py
+00000090: 3230 3233 2d30 362d 3134 2031 303a 3533  2023-06-14 10:53
+000000a0: 3a31 302e 3539 3135 3631 2062 7920 5079  :10.591561 by Py
 000000b0: 5842 2076 6572 7369 6f6e 2031 2e32 2e36  XB version 1.2.6
 000000c0: 2075 7369 6e67 2050 7974 686f 6e20 332e   using Python 3.
-000000d0: 392e 3137 2e66 696e 616c 2e30 0a23 204e  9.17.final.0.# N
+000000d0: 392e 3136 2e66 696e 616c 2e30 0a23 204e  9.16.final.0.# N
 000000e0: 616d 6573 7061 6365 2068 7474 703a 2f2f  amespace http://
 000000f0: 7777 772e 7269 7867 2e6f 7267 2e75 6b2f  www.rixg.org.uk/
 00000100: 0a0a 6672 6f6d 205f 5f66 7574 7572 655f  ..from __future_
 00000110: 5f20 696d 706f 7274 2075 6e69 636f 6465  _ import unicode
 00000120: 5f6c 6974 6572 616c 730a 696d 706f 7274  _literals.import
 00000130: 2070 7978 620a 696d 706f 7274 2070 7978   pyxb.import pyx
 00000140: 622e 6269 6e64 696e 670a 696d 706f 7274  b.binding.import
@@ -30,17 +30,17 @@
 000001d0: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
 000001e0: 666f 7220 6269 6e64 696e 6773 2063 7265  for bindings cre
 000001f0: 6174 6564 2061 7420 7468 6520 7361 6d65  ated at the same
 00000200: 2074 696d 650a 5f47 656e 6572 6174 696f   time._Generatio
 00000210: 6e55 4944 203d 2070 7978 622e 7574 696c  nUID = pyxb.util
 00000220: 732e 7574 696c 6974 792e 556e 6971 7565  s.utility.Unique
 00000230: 4964 656e 7469 6669 6572 2827 7572 6e3a  Identifier('urn:
-00000240: 7575 6964 3a37 3434 3466 3538 612d 3061  uuid:7444f58a-0a
-00000250: 3935 2d31 3165 652d 6262 3563 2d62 3336  95-11ee-bb5c-b36
-00000260: 3637 6262 3139 3665 3627 290a 0a23 2056  67bb196e6')..# V
+00000240: 7575 6964 3a61 3663 3962 6166 322d 3061  uuid:a6c9baf2-0a
+00000250: 6131 2d31 3165 652d 3937 3331 2d66 6262  a1-11ee-9731-fbb
+00000260: 3962 3538 6532 3935 6127 290a 0a23 2056  9b58e295a')..# V
 00000270: 6572 7369 6f6e 206f 6620 5079 5842 2075  ersion of PyXB u
 00000280: 7365 6420 746f 2067 656e 6572 6174 6520  sed to generate 
 00000290: 7468 6520 6269 6e64 696e 6773 0a5f 5079  the bindings._Py
 000002a0: 5842 5665 7273 696f 6e20 3d20 2731 2e32  XBVersion = '1.2
 000002b0: 2e36 270a 2320 4765 6e65 7261 7465 6420  .6'.# Generated 
 000002c0: 6269 6e64 696e 6773 2061 7265 206e 6f74  bindings are not
 000002d0: 2063 6f6d 7061 7469 626c 6520 6163 726f   compatible acro
```

## Comparing `ukrdc_schema-3.4.3.dist-info/RECORD` & `ukrdc_schema-3.4.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ukrdc_schema/__init__.py,sha256=HNo38i3AlfMCqVm-f3x3A2HRkN7m8KamIgg-jxq1h-k,22
-ukrdc_schema/pv_2_0_schema.py,sha256=kR2wwfMSoS_iDf9UFFglH9Dmvru6LmEw6YT-xzlPSjY,245322
-ukrdc_schema/rrtf_schema.py,sha256=Lz4MgaS_DrrzGUJp11pOvWLOK3D7Aq_YZQL3n4Zs-pQ,2996304
-ukrdc_schema/ukrdc_schema.py,sha256=zv91rJUjOnWCcawOaK-hI32tzbORSmK1twxF0kuvdIs,1146641
+ukrdc_schema/__init__.py,sha256=E2FJaHa69ObEhb_Ady32kJ21mdDdNGE9JWFVsC8L_qE,22
+ukrdc_schema/pv_2_0_schema.py,sha256=6ELy8piSQvfQbNyEnBUjX1myUi-dYpngbfw9XNdEe0s,245322
+ukrdc_schema/rrtf_schema.py,sha256=Pd6k8vZPAks0IGXSPOsyL2CSFl0iehyJOjnXbEVjWwM,2996304
+ukrdc_schema/ukrdc_schema.py,sha256=t85LTl5ihbE5IOESNjpl4v_XbHPfGmsA0APcjdQn190,1146641
 ukrdc_schema/transforms/RR_XML_to_TXT.xsl,sha256=Y0icUxt4Cff1aujzzZACpKTvCoakdkuOnTbHH4NBo2M,1058
-ukrdc_schema-3.4.3.dist-info/METADATA,sha256=F3XiWEU6JPyqpUP-hKA8di3toBeNA-Nl6I9s0lMGRDE,245
-ukrdc_schema-3.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ukrdc_schema-3.4.3.dist-info/top_level.txt,sha256=7zNwKN28GdUNcaMLL8jwxBIhSdaLx8spLjOyIn1wdx4,13
-ukrdc_schema-3.4.3.dist-info/RECORD,,
+ukrdc_schema-3.4.5.dist-info/METADATA,sha256=v_SU_Mrbc2lb5ypXqmU_KKrRT38pjRld-DKmxfzv_cg,245
+ukrdc_schema-3.4.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ukrdc_schema-3.4.5.dist-info/top_level.txt,sha256=7zNwKN28GdUNcaMLL8jwxBIhSdaLx8spLjOyIn1wdx4,13
+ukrdc_schema-3.4.5.dist-info/RECORD,,
```

