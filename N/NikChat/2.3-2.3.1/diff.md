# Comparing `tmp/NikChat-2.3.tar.gz` & `tmp/NikChat-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.3.tar", last modified: Sun Jun 11 03:57:34 2023, max compression
+gzip compressed data, was "NikChat-2.3.1.tar", last modified: Wed Jun 14 02:26:38 2023, max compression
```

## Comparing `NikChat-2.3.tar` & `NikChat-2.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:57:34.023815 NikChat-2.3/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-11 03:57:33.998300 NikChat-2.3/NikChat/
--rw-rw-rw-   0        0        0     6650 2023-06-11 03:47:26.000000 NikChat-2.3/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3/NikChat/results.py
--rw-rw-rw-   0        0        0     4356 2023-06-11 03:28:01.000000 NikChat-2.3/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:57:34.020823 NikChat-2.3/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1676 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 03:57:33.000000 NikChat-2.3/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1676 2023-06-11 03:57:34.025848 NikChat-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.3/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3/pyproject.toml
--rw-rw-rw-   0        0        0      631 2023-06-11 03:57:34.029861 NikChat-2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.213622 NikChat-2.3.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.166626 NikChat-2.3.1/NikChat/
+-rw-rw-rw-   0        0        0     6650 2023-06-14 02:23:35.000000 NikChat-2.3.1/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.1/NikChat/results.py
+-rw-rw-rw-   0        0        0     4356 2023-06-11 03:28:01.000000 NikChat-2.3.1/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.208031 NikChat-2.3.1/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1678 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1678 2023-06-14 02:26:38.214618 NikChat-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.3.1/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      633 2023-06-14 02:26:38.218604 NikChat-2.3.1/setup.cfg
```

### Comparing `NikChat-2.3/LICENSE` & `NikChat-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.3/NikChat/__init__.py` & `NikChat-2.3.1/NikChat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,23 +68,23 @@
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
             return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
         
-def train():
+def train(filePath):
     import NikChat.training as traning
-    traning.init2()
+    traning.init2filePath()
 
-def init(filePath):
+def init():
     from os.path import exists
     if exists('words.pkl') == False:
         import NikChat.training as traning
-        traning.init(filePath)
+        traning.init()
         return 'done'
     else:
         return 'done'
 
 def NChat(filePath):
     try:
         import nltk
```

### Comparing `NikChat-2.3/NikChat/results.py` & `NikChat-2.3.1/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3/NikChat/training.py` & `NikChat-2.3.1/NikChat/training.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3/NikChat.egg-info/PKG-INFO` & `NikChat-2.3.1/NikChat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3
+Version: 2.3.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3/PKG-INFO` & `NikChat-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3
+Version: 2.3.1
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikChat-2.3/README.md` & `NikChat-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `NikChat-2.3/setup.cfg` & `NikChat-2.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 330d 0a61 7574 686f  ion = 2.3..autho
-00000030: 7220 3d20 4e69 6b68 696c 2054 616d 7661  r = Nikhil Tamva
-00000040: 6461 2028 4e69 6b68 696c 6f64 656f 6e31  da (Nikhilodeon1
-00000050: 290d 0a61 7574 686f 725f 656d 6169 6c20  )..author_email 
-00000060: 3d20 6e69 6b68 696c 7461 6d76 6164 6140  = nikhiltamvada@
-00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
-00000080: 6970 7469 6f6e 203d 2041 2066 756c 6c2d  iption = A full-
-00000090: 666c 6564 6765 6420 6368 6174 626f 7420  fledged chatbot 
-000000a0: 6465 7369 676e 6564 2074 6f20 6265 2069  designed to be i
-000000b0: 6e63 6f72 7065 7261 7465 6420 696e 746f  ncorperated into
-000000c0: 206f 7468 6572 2070 726f 6a65 6374 732e   other projects.
-000000d0: 2028 5370 6565 6473 206f 6620 302e 3120   (Speeds of 0.1 
-000000e0: 7365 636f 6e64 7329 0d0a 6c6f 6e67 5f64  seconds)..long_d
-000000f0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000100: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-00000110: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000120: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000130: 7874 2f6d 6172 6b64 6f77 6e0d 0a68 6f6d  xt/markdown..hom
-00000140: 655f 7061 6765 203d 2068 7474 7073 3a2f  e_page = https:/
-00000150: 2f67 6974 6875 622e 636f 6d2f 4e69 6b68  /github.com/Nikh
-00000160: 696c 6f64 656f 6e31 2f4e 696b 4368 6174  ilodeon1/NikChat
-00000170: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000180: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000190: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001a0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001c0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000001f0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000200: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
-00000210: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000220: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
-00000230: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000240: 7461 203d 2054 7275 650d 0a0d 0a5b 6567  ta = True....[eg
-00000250: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000260: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000270: 3d20 300d 0a0d 0a                        = 0....
+00000020: 696f 6e20 3d20 322e 332e 310d 0a61 7574  ion = 2.3.1..aut
+00000030: 686f 7220 3d20 4e69 6b68 696c 2054 616d  hor = Nikhil Tam
+00000040: 7661 6461 2028 4e69 6b68 696c 6f64 656f  vada (Nikhilodeo
+00000050: 6e31 290d 0a61 7574 686f 725f 656d 6169  n1)..author_emai
+00000060: 6c20 3d20 6e69 6b68 696c 7461 6d76 6164  l = nikhiltamvad
+00000070: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
+00000080: 6372 6970 7469 6f6e 203d 2041 2066 756c  cription = A ful
+00000090: 6c2d 666c 6564 6765 6420 6368 6174 626f  l-fledged chatbo
+000000a0: 7420 6465 7369 676e 6564 2074 6f20 6265  t designed to be
+000000b0: 2069 6e63 6f72 7065 7261 7465 6420 696e   incorperated in
+000000c0: 746f 206f 7468 6572 2070 726f 6a65 6374  to other project
+000000d0: 732e 2028 5370 6565 6473 206f 6620 302e  s. (Speeds of 0.
+000000e0: 3120 7365 636f 6e64 7329 0d0a 6c6f 6e67  1 seconds)..long
+000000f0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000100: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000120: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000130: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a68  text/markdown..h
+00000140: 6f6d 655f 7061 6765 203d 2068 7474 7073  ome_page = https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e69  ://github.com/Ni
+00000160: 6b68 696c 6f64 656f 6e31 2f4e 696b 4368  khilodeon1/NikCh
+00000170: 6174 0d0a 636c 6173 7369 6669 6572 7320  at..classifiers 
+00000180: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
+00000190: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001a0: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
+000001b0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001c0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+000001d0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+000001e0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001f0: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
+00000200: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+00000210: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000220: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
+00000230: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000240: 6461 7461 203d 2054 7275 650d 0a0d 0a5b  data = True....[
+00000250: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000260: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000270: 6520 3d20 300d 0a0d 0a                   e = 0....
```

