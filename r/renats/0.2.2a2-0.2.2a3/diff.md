# Comparing `tmp/renats-0.2.2a2.tar.gz` & `tmp/renats-0.2.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renats-0.2.2a2.tar", max compression
+gzip compressed data, was "renats-0.2.2a3.tar", max compression
```

## Comparing `renats-0.2.2a2.tar` & `renats-0.2.2a3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a2/README.md
--rw-r--r--   0        0        0      431 2023-06-13 13:46:33.268272 renats-0.2.2a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/__init__.py
--rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/__init__.py
--rw-r--r--   0        0        0      242 2023-06-13 13:17:27.752054 renats-0.2.2a2/renats/client/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1467 2023-06-13 13:28:47.718277 renats-0.2.2a2/renats/client/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     5403 2023-06-13 13:18:15.172206 renats-0.2.2a2/renats/client/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      588 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/client/__pycache__/message.cpython-310.pyc
--rw-r--r--   0        0        0     1107 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/client/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     2399 2023-06-13 13:18:15.192206 renats-0.2.2a2/renats/client/__pycache__/subscription.cpython-310.pyc
--rw-r--r--   0        0        0      912 2023-06-13 13:46:24.528236 renats-0.2.2a2/renats/client/base.py
--rw-r--r--   0        0        0     6372 2023-06-13 13:46:37.700290 renats-0.2.2a2/renats/client/client.py
--rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/handler.py
--rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/message.py
--rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/parser.py
--rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/subscription.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/connection/__init__.py
--rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a2/renats/connection/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1693 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/connection/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2003 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/connection/__pycache__/tcp.cpython-310.pyc
--rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/connection/base.py
--rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/connection/connection.py
--rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/connection/tcp.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/protocol/__init__.py
--rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a2/renats/protocol/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      925 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/__pycache__/protocol.cpython-310.pyc
--rw-r--r--   0        0        0     2335 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/protocol/messages/__init__.py
--rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a2/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a2/renats/protocol/messages/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      863 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
--rw-r--r--   0        0        0     1926 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
--rw-r--r--   0        0        0     2341 2023-06-13 13:09:10.690155 renats-0.2.2a2/renats/protocol/messages/__pycache__/service.cpython-310.pyc
--rw-r--r--   0        0        0     1650 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
--rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a2/renats/protocol/messages/base.py
--rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/msg.py
--rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/pub.py
--rw-r--r--   0        0        0     1702 2023-06-13 13:46:24.528236 renats-0.2.2a2/renats/protocol/messages/service.py
--rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/sub.py
--rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/protocol.py
--rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/utils.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a2/PKG-INFO
+-rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a3/README.md
+-rw-r--r--   0        0        0      431 2023-06-13 15:42:45.664444 renats-0.2.2a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a3/renats/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/client/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-13 13:17:27.752054 renats-0.2.2a3/renats/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1458 2023-06-13 15:33:03.896793 renats-0.2.2a3/renats/client/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     5403 2023-06-13 15:42:56.804519 renats-0.2.2a3/renats/client/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      588 2023-06-13 13:28:47.722277 renats-0.2.2a3/renats/client/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0        0        0     1154 2023-06-13 15:42:56.808519 renats-0.2.2a3/renats/client/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2023-06-13 13:18:15.192206 renats-0.2.2a3/renats/client/__pycache__/subscription.cpython-310.pyc
+-rw-r--r--   0        0        0      912 2023-06-13 13:46:24.528236 renats-0.2.2a3/renats/client/base.py
+-rw-r--r--   0        0        0     6372 2023-06-13 15:42:38.160393 renats-0.2.2a3/renats/client/client.py
+-rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/client/handler.py
+-rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/client/message.py
+-rw-r--r--   0        0        0      988 2023-06-13 15:42:21.864283 renats-0.2.2a3/renats/client/parser.py
+-rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/client/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a3/renats/connection/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a3/renats/connection/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1693 2023-06-13 13:17:27.772054 renats-0.2.2a3/renats/connection/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2003 2023-06-13 13:28:47.722277 renats-0.2.2a3/renats/connection/__pycache__/tcp.cpython-310.pyc
+-rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/connection/base.py
+-rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a3/renats/connection/connection.py
+-rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/connection/tcp.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a3/renats/protocol/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a3/renats/protocol/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-06-13 13:17:27.772054 renats-0.2.2a3/renats/protocol/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      925 2023-06-13 13:28:47.722277 renats-0.2.2a3/renats/protocol/__pycache__/protocol.cpython-310.pyc
+-rw-r--r--   0        0        0     2335 2023-06-13 13:17:27.772054 renats-0.2.2a3/renats/protocol/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a3/renats/protocol/messages/__init__.py
+-rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a3/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a3/renats/protocol/messages/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      863 2023-06-13 13:17:27.772054 renats-0.2.2a3/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     1926 2023-06-13 13:28:47.722277 renats-0.2.2a3/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
+-rw-r--r--   0        0        0     2341 2023-06-13 15:23:36.274460 renats-0.2.2a3/renats/protocol/messages/__pycache__/service.cpython-310.pyc
+-rw-r--r--   0        0        0     1650 2023-06-13 13:28:47.722277 renats-0.2.2a3/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
+-rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a3/renats/protocol/messages/base.py
+-rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/messages/msg.py
+-rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/messages/pub.py
+-rw-r--r--   0        0        0     1702 2023-06-13 13:46:24.528236 renats-0.2.2a3/renats/protocol/messages/service.py
+-rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/messages/sub.py
+-rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/protocol.py
+-rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a3/renats/protocol/utils.py
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a3/PKG-INFO
```

### Comparing `renats-0.2.2a2/README.md` & `renats-0.2.2a3/README.md`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/client/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a3/renats/client/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 13:28:46 2023 UTC, .py size: 925 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-00000000: 6f0d 0d0a 0000 0000 0e6f 8864 9d03 0000  o........o.d....
+00000000: 6f0d 0d0a 0000 0000 3073 8864 9003 0000  o.......0s.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
-00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6404 6c09 6d0a 5a0a 0100 650b 650c 650c  d.l.m.Z...e.e.e.
+00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6404  ..d.d.l.m.Z...d.
+00000060: 6405 6c09 6d0a 5a0a 0100 650b 650c 650c  d.l.m.Z...e.e.e.
 00000070: 6602 1900 5a0d 6505 650a 6701 6506 6602  f...Z.e.e.g.e.f.
-00000080: 1900 5a0e 6504 6405 6406 6407 8d02 5a0f  ..Z.e.d.d.d...Z.
-00000090: 4700 6408 6409 8400 6409 6501 8303 5a10  G.d.d...d.e...Z.
-000000a0: 640a 5300 290b e900 0000 0029 02da 0341  d.S.)......)...A
+00000080: 1900 5a0e 6504 6406 6407 6408 8d02 5a0f  ..Z.e.d.d.d...Z.
+00000090: 4700 6409 640a 8400 640a 6501 8303 5a10  G.d.d...d.e...Z.
+000000a0: 640b 5300 290c e900 0000 0029 02da 0341  d.S.)......)...A
 000000b0: 4243 da0e 6162 7374 7261 6374 6d65 7468  BC..abstractmeth
 000000c0: 6f64 2903 da07 5479 7065 5661 72da 0843  od)...TypeVar..C
 000000d0: 616c 6c61 626c 65da 0341 6e79 2901 da04  allable..Any)...
-000000e0: 5365 6c66 2901 da07 4d65 7373 6167 65da  Self)...Message.
-000000f0: 1053 7562 7363 7269 7074 696f 6e54 7970  .SubscriptionTyp
-00000100: 65da 0c53 7562 7363 7269 7074 696f 6e29  e..Subscription)
-00000110: 01da 0562 6f75 6e64 6300 0000 0000 0000  ...boundc.......
-00000120: 0000 0000 0000 0000 000a 0000 0040 0000  .............@..
-00000130: 0073 8000 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
-00000140: 6401 6504 6504 6505 6506 6602 1900 1900  d.e.e.e.e.f.....
-00000150: 6402 6507 6604 6403 6404 8404 8301 5a08  d.e.f.d.d.....Z.
-00000160: 6503 6415 6407 6505 6408 6509 6409 6505  e.d.d.e.d.e.d.e.
-00000170: 640a 650a 6608 640b 640c 8405 8301 5a0b  d.e.f.d.d.....Z.
-00000180: 6503 6407 6505 640d 650c 6402 650d 6606  e.d.e.d.e.d.e.f.
-00000190: 640e 640f 8404 8301 5a0e 6503 6416 6411  d.d.....Z.e.d.d.
-000001a0: 6505 6412 6506 6604 6413 6414 8405 8301  e.d.e.f.d.d.....
-000001b0: 5a0f 6406 5300 2917 da04 4e41 5453 da07  Z.d.S.)...NATS..
-000001c0: 7365 7276 6572 73da 0672 6574 7572 6e63  servers..returnc
-000001d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000001e0: 0100 0000 c300 0000 f308 0000 0081 0174  ...............t
-000001f0: 0083 0082 01a9 014e a901 da13 4e6f 7449  .......N....NotI
-00000200: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
-00000210: 02da 0473 656c 6672 0d00 0000 a900 7214  ...selfr......r.
-00000220: 0000 00fa 412f 686f 6d65 2f72 6573 7069  ....A/home/respi
-00000230: 7265 6e73 2f68 616e 6469 6365 652f 6465  rens/handicee/de
-00000240: 7665 6c6f 702f 7765 622f 5265 4e41 5453  velop/web/ReNATS
-00000250: 2f72 656e 6174 732f 636c 6965 6e74 2f62  /renats/client/b
-00000260: 6173 652e 7079 da07 636f 6e6e 6563 740e  ase.py..connect.
-00000270: 0000 00f3 0400 0000 0280 0602 7a0c 4e41  ............z.NA
-00000280: 5453 2e63 6f6e 6e65 6374 f300 0000 004e  TS.connect.....N
-00000290: da07 7375 626a 6563 74da 0770 6179 6c6f  ..subject..paylo
-000002a0: 6164 da0d 7265 706c 795f 7375 626a 6563  ad..reply_subjec
-000002b0: 74da 0768 6561 6465 7273 6305 0000 0000  t..headersc.....
-000002c0: 0000 0000 0000 0005 0000 0001 0000 00c3  ................
-000002d0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-000002e0: 0000 2905 7213 0000 0072 1900 0000 721a  ..).r....r....r.
-000002f0: 0000 0072 1b00 0000 721c 0000 0072 1400  ...r....r....r..
-00000300: 0000 7214 0000 0072 1500 0000 da07 7075  ..r....r......pu
-00000310: 626c 6973 6812 0000 0072 1700 0000 7a0c  blish....r....z.
-00000320: 4e41 5453 2e70 7562 6c69 7368 da08 6361  NATS.publish..ca
-00000330: 6c6c 6261 636b 6303 0000 0000 0000 0000  llbackc.........
-00000340: 0000 0003 0000 0001 0000 00c3 0000 0072  ...............r
-00000350: 0f00 0000 7210 0000 0072 1100 0000 2903  ....r....r....).
-00000360: 7213 0000 0072 1900 0000 721e 0000 0072  r....r....r....r
-00000370: 1400 0000 7214 0000 0072 1500 0000 da09  ....r....r......
-00000380: 7375 6273 6372 6962 6516 0000 0072 1700  subscribe....r..
-00000390: 0000 7a0e 4e41 5453 2e73 7562 7363 7269  ..z.NATS.subscri
-000003a0: 6265 7201 0000 00da 0f73 7562 7363 7269  ber......subscri
-000003b0: 7074 696f 6e5f 6964 da0d 6d65 7373 6167  ption_id..messag
-000003c0: 6573 5f6c 6566 7463 0300 0000 0000 0000  es_leftc........
-000003d0: 0000 0000 0300 0000 0100 0000 c300 0000  ................
-000003e0: 720f 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
-000003f0: 0372 1300 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000400: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000410: 0b75 6e73 7562 7363 7269 6265 1a00 0000  .unsubscribe....
-00000420: 7217 0000 007a 104e 4154 532e 756e 7375  r....z.NATS.unsu
-00000430: 6273 6372 6962 6529 0372 1800 0000 4e4e  bscribe).r....NN
-00000440: 2901 7201 0000 0029 10da 085f 5f6e 616d  ).r....)...__nam
-00000450: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000460: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0300  .__qualname__r..
-00000470: 0000 da05 7475 706c 65da 0373 7472 da03  ....tuple..str..
-00000480: 696e 7472 0700 0000 7216 0000 00da 0562  intr....r......b
-00000490: 7974 6573 da0b 4865 6164 6572 7354 7970  ytes..HeadersTyp
-000004a0: 6572 1d00 0000 da18 5375 6273 6372 6970  er......Subscrip
-000004b0: 7469 6f6e 4361 6c6c 6261 636b 5479 7065  tionCallbackType
-000004c0: 7209 0000 0072 1f00 0000 7222 0000 0072  r....r....r"...r
-000004d0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000004e0: 0000 0072 0c00 0000 0d00 0000 7312 0000  ...r........s...
-000004f0: 0008 0002 0120 0102 031e 0102 0318 0102  ..... ..........
-00000500: 031a 0172 0c00 0000 4e29 11da 0361 6263  ...r....N)...abc
-00000510: 7202 0000 0072 0300 0000 da06 7479 7069  r....r......typi
-00000520: 6e67 7204 0000 0072 0500 0000 7206 0000  ngr....r....r...
-00000530: 00da 1174 7970 696e 675f 6578 7465 6e73  ...typing_extens
-00000540: 696f 6e73 7207 0000 00da 1572 656e 6174  ionsr......renat
-00000550: 732e 636c 6965 6e74 2e6d 6573 7361 6765  s.client.message
-00000560: 7208 0000 00da 0464 6963 7472 2700 0000  r......dictr'...
-00000570: 722a 0000 0072 2b00 0000 7209 0000 0072  r*...r+...r....r
-00000580: 0c00 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
-00000590: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
-000005a0: 653e 0100 0000 7310 0000 0010 0014 010c  e>....s.........
-000005b0: 020c 020c 020e 010c 0114 03              ...........
+000000e0: 5365 6c66 e901 0000 0029 01da 074d 6573  Self.....)...Mes
+000000f0: 7361 6765 da10 5375 6273 6372 6970 7469  sage..Subscripti
+00000100: 6f6e 5479 7065 da0c 5375 6273 6372 6970  onType..Subscrip
+00000110: 7469 6f6e 2901 da05 626f 756e 6463 0000  tion)...boundc..
+00000120: 0000 0000 0000 0000 0000 0000 0000 0a00  ................
+00000130: 0000 4000 0000 7380 0000 0065 005a 0164  ..@...s....e.Z.d
+00000140: 005a 0265 0364 0165 0465 0465 0565 0666  .Z.e.d.e.e.e.e.f
+00000150: 0219 0019 0064 0265 0766 0464 0364 0484  .....d.e.f.d.d..
+00000160: 0483 015a 0865 0364 1564 0765 0564 0865  ...Z.e.d.d.e.d.e
+00000170: 0964 0965 0564 0a65 0a66 0864 0b64 0c84  .d.e.d.e.f.d.d..
+00000180: 0583 015a 0b65 0364 0765 0564 0d65 0c64  ...Z.e.d.e.d.e.d
+00000190: 0265 0d66 0664 0e64 0f84 0483 015a 0e65  .e.f.d.d.....Z.e
+000001a0: 0364 1664 1165 0564 1265 0666 0464 1364  .d.d.e.d.e.f.d.d
+000001b0: 1484 0583 015a 0f64 0653 0029 17da 044e  .....Z.d.S.)...N
+000001c0: 4154 53da 0773 6572 7665 7273 da06 7265  ATS..servers..re
+000001d0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+000001e0: 0002 0000 0001 0000 00c3 0000 00f3 0800  ................
+000001f0: 0000 8101 7400 8300 8201 a901 4ea9 01da  ....t.......N...
+00000200: 134e 6f74 496d 706c 656d 656e 7465 6445  .NotImplementedE
+00000210: 7272 6f72 2902 da04 7365 6c66 720e 0000  rror)...selfr...
+00000220: 00a9 0072 1500 0000 fa41 2f68 6f6d 652f  ...r.....A/home/
+00000230: 7265 7370 6972 656e 732f 6861 6e64 6963  respirens/handic
+00000240: 6565 2f64 6576 656c 6f70 2f77 6562 2f52  ee/develop/web/R
+00000250: 654e 4154 532f 7265 6e61 7473 2f63 6c69  eNATS/renats/cli
+00000260: 656e 742f 6261 7365 2e70 79da 0763 6f6e  ent/base.py..con
+00000270: 6e65 6374 0e00 0000 f304 0000 0002 8006  nect............
+00000280: 027a 0c4e 4154 532e 636f 6e6e 6563 74f3  .z.NATS.connect.
+00000290: 0000 0000 4eda 0773 7562 6a65 6374 da07  ....N..subject..
+000002a0: 7061 796c 6f61 64da 0d72 6570 6c79 5f73  payload..reply_s
+000002b0: 7562 6a65 6374 da07 6865 6164 6572 7363  ubject..headersc
+000002c0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+000002d0: 0100 0000 c300 0000 7210 0000 0072 1100  ........r....r..
+000002e0: 0000 7212 0000 0029 0572 1400 0000 721a  ..r....).r....r.
+000002f0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00000300: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000310: 00da 0770 7562 6c69 7368 1200 0000 7218  ...publish....r.
+00000320: 0000 007a 0c4e 4154 532e 7075 626c 6973  ...z.NATS.publis
+00000330: 68da 0863 616c 6c62 6163 6b63 0300 0000  h..callbackc....
+00000340: 0000 0000 0000 0000 0300 0000 0100 0000  ................
+00000350: c300 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
+00000360: 0000 0029 0372 1400 0000 721a 0000 0072  ...).r....r....r
+00000370: 1f00 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000380: 0000 00da 0973 7562 7363 7269 6265 1600  .....subscribe..
+00000390: 0000 7218 0000 007a 0e4e 4154 532e 7375  ..r....z.NATS.su
+000003a0: 6273 6372 6962 6572 0100 0000 da0f 7375  bscriber......su
+000003b0: 6273 6372 6970 7469 6f6e 5f69 64da 0d6d  bscription_id..m
+000003c0: 6573 7361 6765 735f 6c65 6674 6303 0000  essages_leftc...
+000003d0: 0000 0000 0000 0000 0003 0000 0001 0000  ................
+000003e0: 00c3 0000 0072 1000 0000 7211 0000 0072  .....r....r....r
+000003f0: 1200 0000 2903 7214 0000 0072 2100 0000  ....).r....r!...
+00000400: 7222 0000 0072 1500 0000 7215 0000 0072  r"...r....r....r
+00000410: 1600 0000 da0b 756e 7375 6273 6372 6962  ......unsubscrib
+00000420: 651a 0000 0072 1800 0000 7a10 4e41 5453  e....r....z.NATS
+00000430: 2e75 6e73 7562 7363 7269 6265 2903 7219  .unsubscribe).r.
+00000440: 0000 004e 4e29 0172 0100 0000 2910 da08  ...NN).r....)...
+00000450: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000460: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000470: 5f5f 7203 0000 00da 0574 7570 6c65 da03  __r......tuple..
+00000480: 7374 72da 0369 6e74 7207 0000 0072 1700  str..intr....r..
+00000490: 0000 da05 6279 7465 73da 0b48 6561 6465  ....bytes..Heade
+000004a0: 7273 5479 7065 721e 0000 00da 1853 7562  rsTyper......Sub
+000004b0: 7363 7269 7074 696f 6e43 616c 6c62 6163  scriptionCallbac
+000004c0: 6b54 7970 6572 0a00 0000 7220 0000 0072  kTyper....r ...r
+000004d0: 2300 0000 7215 0000 0072 1500 0000 7215  #...r....r....r.
+000004e0: 0000 0072 1600 0000 720d 0000 000d 0000  ...r....r.......
+000004f0: 0073 1200 0000 0800 0201 2001 0203 1e01  .s........ .....
+00000500: 0203 1801 0203 1a01 720d 0000 004e 2911  ........r....N).
+00000510: da03 6162 6372 0200 0000 7203 0000 00da  ..abcr....r.....
+00000520: 0674 7970 696e 6772 0400 0000 7205 0000  .typingr....r...
+00000530: 0072 0600 0000 da11 7479 7069 6e67 5f65  .r......typing_e
+00000540: 7874 656e 7369 6f6e 7372 0700 0000 da07  xtensionsr......
+00000550: 6d65 7373 6167 6572 0900 0000 da04 6469  messager......di
+00000560: 6374 7228 0000 0072 2b00 0000 722c 0000  ctr(...r+...r,..
+00000570: 0072 0a00 0000 720d 0000 0072 1500 0000  .r....r....r....
+00000580: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000590: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
+000005a0: 0000 1000 1401 0c02 0c02 0c02 0e01 0c01  ................
+000005b0: 1403                                     ..
```

### Comparing `renats-0.2.2a2/renats/client/__pycache__/client.cpython-310.pyc` & `renats-0.2.2a3/renats/client/__pycache__/client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 13:18:08 2023 UTC, .py size: 6372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 906c 8864 e418 0000  o........l.d....
+00000000: 6f0d 0d0a 0000 0000 6e8e 8864 e418 0000  o.......n..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6201 0000 5500  .....@...sb...U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c00 6d02 5a02 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c03 6d04 5a04 0100 6400 6401 6c05 5a06  l.m.Z...d.d.l.Z.
 00000060: 6400 6404 6c07 6d08 5a08 0100 6405 6406  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 0100 6405 6407 6c0b 6d0c  l.m.Z...d.d.l.m.
@@ -48,15 +48,15 @@
 000002f0: 6250 726f 746f 636f 6c4d 6573 7361 6765  bProtocolMessage
 00000300: da1a 4445 4641 554c 545f 434f 4e4e 4543  ..DEFAULT_CONNEC
 00000310: 5449 4f4e 5f54 494d 454f 5554 da1c 4445  TION_TIMEOUT..DE
 00000320: 4641 554c 545f 494e 464f 5f57 4149 5449  FAULT_INFO_WAITI
 00000330: 4e47 5f54 494d 454f 5554 da07 7079 7468  NG_TIMEOUT..pyth
 00000340: 6f6e 33da 0f43 4c49 454e 545f 4c41 4e47  on3..CLIENT_LANG
 00000350: 5541 4745 7a0d 302e 322e 322d 616c 7068  UAGEz.0.2.2-alph
-00000360: 612d 31da 0e43 4c49 454e 545f 5645 5253  a-1..CLIENT_VERS
+00000360: 612d 33da 0e43 4c49 454e 545f 5645 5253  a-3..CLIENT_VERS
 00000370: 494f 4e46 da19 434c 4945 4e54 5f43 4f4e  IONF..CLIENT_CON
 00000380: 4e45 4354 494f 4e5f 5645 5242 4f53 4554  NECTION_VERBOSET
 00000390: da1a 434c 4945 4e54 5f43 4f4e 4e45 4354  ..CLIENT_CONNECT
 000003a0: 494f 4e5f 5045 4441 4e54 4943 da16 434c  ION_PEDANTIC..CL
 000003b0: 4945 4e54 5f53 5550 504f 5254 5f48 4541  IENT_SUPPORT_HEA
 000003c0: 4445 5253 6300 0000 0000 0000 0000 0000  DERSc...........
 000003d0: 0000 0000 0009 0000 0040 0000 0073 d800  .........@...s..
```

### Comparing `renats-0.2.2a2/renats/client/__pycache__/message.cpython-310.pyc` & `renats-0.2.2a3/renats/client/__pycache__/message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/client/__pycache__/subscription.cpython-310.pyc` & `renats-0.2.2a3/renats/client/__pycache__/subscription.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/client/base.py` & `renats-0.2.2a3/renats/client/base.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/client/client.py` & `renats-0.2.2a3/renats/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ..protocol.messages.service import InfoProtocolMessage, ConnectProtocolMessage
 from ..protocol.messages.sub import SubProtocolMessage, UnsubProtocolMessage
 
 DEFAULT_CONNECTION_TIMEOUT: Final[float] = 2
 DEFAULT_INFO_WAITING_TIMEOUT: Final[float] = 2
 
 CLIENT_LANGUAGE: Final[str] = "python3"
-CLIENT_VERSION: Final[str] = "0.2.2-alpha-2"
+CLIENT_VERSION: Final[str] = "0.2.2-alpha-3"
 
 CLIENT_CONNECTION_VERBOSE: Final[bool] = False
 CLIENT_CONNECTION_PEDANTIC: Final[bool] = True
 CLIENT_SUPPORT_HEADERS: Final[bool] = False
 
 
 class NATSClient(NATS):
```

### Comparing `renats-0.2.2a2/renats/client/handler.py` & `renats-0.2.2a3/renats/client/handler.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/client/parser.py` & `renats-0.2.2a3/renats/client/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 
 async def parse_msg(head: bytes, connection: Connection) -> MsgProtocolMessage:
     match = re.match(MSG_HEAD_PATTERN, head)
     if match is None:
         raise InvalidProtocolMessage(head)
     subject, sid, _, reply_to, payload_length = match.groups()
-    payload = await connection.readexactly(int(payload_length) + utils.CRLF_SIZE)
+    payload = (await connection.readexactly(int(payload_length) + utils.CRLF_SIZE)).removesuffix(b"\r\n")
     return MsgProtocolMessage(
-        subject=subject,
-        sid=sid,
-        reply_to=reply_to,
+        subject=subject.decode(),
+        sid=sid.decode(),
+        reply_to=reply_to.decode(),
         payload_length=int(payload_length),
         payload=payload
     )
 
 
 async def parse_hmsg(head: bytes, connection: Connection) -> HMsgProtocolMessage:
     raise NotImplementedError()
```

### Comparing `renats-0.2.2a2/renats/client/subscription.py` & `renats-0.2.2a3/renats/client/subscription.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/connection/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a3/renats/connection/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/connection/__pycache__/tcp.cpython-310.pyc` & `renats-0.2.2a3/renats/connection/__pycache__/tcp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/connection/base.py` & `renats-0.2.2a3/renats/connection/base.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/connection/tcp.py` & `renats-0.2.2a3/renats/connection/tcp.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/__pycache__/exceptions.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/__pycache__/protocol.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/__pycache__/protocol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/__pycache__/utils.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/exceptions.py` & `renats-0.2.2a3/renats/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/messages/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/__pycache__/msg.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/messages/__pycache__/msg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/__pycache__/pub.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/messages/__pycache__/pub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/__pycache__/service.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/messages/__pycache__/service.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 12:43:42 2023 UTC, .py size: 1702 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7e64 8864 a606 0000  o.......~d.d....
+00000000: 6f0d 0d0a 0000 0000 3073 8864 a606 0000  o.......0s.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6500  d.l.m.Z.m.Z...e.
 00000050: a005 6403 a101 5a06 4700 6404 6405 8400  ..d...Z.G.d.d...
 00000060: 6405 6503 8303 5a07 4700 6406 6407 8400  d.e...Z.G.d.d...
 00000070: 6407 6503 6408 6409 8d04 5a08 6401 5300  d.e.d.d...Z.d.S.
```

### Comparing `renats-0.2.2a2/renats/protocol/messages/__pycache__/sub.cpython-310.pyc` & `renats-0.2.2a3/renats/protocol/messages/__pycache__/sub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/pub.py` & `renats-0.2.2a3/renats/protocol/messages/pub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/service.py` & `renats-0.2.2a3/renats/protocol/messages/service.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/messages/sub.py` & `renats-0.2.2a3/renats/protocol/messages/sub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/protocol.py` & `renats-0.2.2a3/renats/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/renats/protocol/utils.py` & `renats-0.2.2a3/renats/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a2/PKG-INFO` & `renats-0.2.2a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renats
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: 
 Author: Respirens
 Author-email: thesergiyprotsanin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

