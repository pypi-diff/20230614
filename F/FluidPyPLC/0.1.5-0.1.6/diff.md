# Comparing `tmp/FluidPyPLC-0.1.5.tar.gz` & `tmp/FluidPyPLC-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.5.tar", last modified: Wed Jun 14 20:00:19 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.6.tar", last modified: Wed Jun 14 20:17:53 2023, max compression
```

## Comparing `FluidPyPLC-0.1.5.tar` & `FluidPyPLC-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.117952 FluidPyPLC-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.075486 FluidPyPLC-0.1.5/FluidPyPLC/
--rw-rw-rw-   0        0        0     7102 2023-06-14 19:19:20.000000 FluidPyPLC-0.1.5/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.5/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.5/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3541 2023-06-14 19:56:37.000000 FluidPyPLC-0.1.5/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2277 2023-06-14 19:57:55.000000 FluidPyPLC-0.1.5/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.5/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14347 2023-06-14 19:29:38.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.5/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.5/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.115971 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1413 2023-06-14 20:00:19.116956 FluidPyPLC-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 20:00:19.117952 FluidPyPLC-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-06-14 19:57:27.000000 FluidPyPLC-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:17:53.413354 FluidPyPLC-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:17:53.386099 FluidPyPLC-0.1.6/FluidPyPLC/
+-rw-rw-rw-   0        0        0     7179 2023-06-14 20:14:25.000000 FluidPyPLC-0.1.6/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 20:16:54.000000 FluidPyPLC-0.1.6/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.6/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3618 2023-06-14 20:14:51.000000 FluidPyPLC-0.1.6/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2484 2023-06-14 20:11:55.000000 FluidPyPLC-0.1.6/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.6/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.6/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.6/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14403 2023-06-14 20:13:58.000000 FluidPyPLC-0.1.6/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.6/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.6/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:17:53.411371 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 20:17:53.000000 FluidPyPLC-0.1.6/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1413 2023-06-14 20:17:53.413354 FluidPyPLC-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4905 2023-06-14 20:04:09.000000 FluidPyPLC-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:17:53.413354 FluidPyPLC-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-06-14 20:15:59.000000 FluidPyPLC-0.1.6/setup.py
```

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.6/FluidPyPLC/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from FluidPyPLC.get_sequence import *
 from FluidPyPLC.data import Data
 from FluidPyPLC.plc import Plc
 from FluidPyPLC.diagrams import diagrams
-from FluidPyPLC.f import path
 
+import json
 import os
 import PySimpleGUI as sg
 
 sg.theme('DarkTanBlue')
 sg.set_options(font=('Helvetica', 14))
 
+with open("config.json") as f:
+    config = json.load(f)
+    path = config["folder_path"]
+
 def collapse(layout, key, visible):
     return sg.pin(sg.Column(layout, key=key, visible=visible))
 
 def elaborate_data(s):
     d = Data(s)
     groups = d.groups
     relay_memory_labels = Plc(s).relay_memory_labels
```

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/data.py` & `FluidPyPLC-0.1.6/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.6/FluidPyPLC/diagrams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import json
 import os
 import matplotlib.pyplot as plt
 from FluidPyPLC.data import Data
-from FluidPyPLC.f import path
+
+with open("config.json") as f:
+    config = json.load(f)
+    path = config["folder_path"]
 
 # get the x and y axis for the Phase's diagrams
 def xy_axis(number_of_pistons, pistons_labels, sequence):
     number_of_pistons , piston_labels = number_of_pistons, pistons_labels
     x_axis = list(range(0, len(sequence) + 1))
     y_axis = [[0 for strokes in range(len(sequence) + 1)] for label in range(number_of_pistons)]
```

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/f.py` & `FluidPyPLC-0.1.6/FluidPyPLC/f.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 import argparse
 import json
 import subprocess
 import textwrap
 import os
 
-global path
-
 def create_folders(folder_path):
     plots_folder = os.path.join(folder_path, 'Plots')
     plc_folder = os.path.join(folder_path, 'plc')
 
     # Create the Plots and plc folders
     os.makedirs(plots_folder, exist_ok=True)
     os.makedirs(plc_folder, exist_ok=True)
@@ -44,22 +42,27 @@
         f.py -t # to use the terminal version
         f.py --plc # to display the plc ST code
         ''')
     )
     parser.add_argument('-g', '--gui', action='store_true', help='gui mode')
     parser.add_argument('-t', '--terminal', action='store_true', help='terminal mode')
     parser.add_argument('--plc', action='store_true', help='show plc code')
+    parser.add_argument('-f', '--folder', type=str, help='Config.json folder path to create the Plot and plc folders')
     args = parser.parse_args()
     try:
         with open("config.json") as f:
             config = json.load(f)
         path = config["folder_path"]
         print(f"Loaded path from config.json: '{path}'.")
     except Exception:
         None
+    if args.folder:
+        folder_path = args.folder
+        create_folders(folder_path)
+        exit(0)
     if args.gui:
         # gui mode
         gui = Gui()
         gui.gui_mode()
         exit(0)
     elif args.terminal:
         # terminal mode
@@ -73,9 +76,7 @@
         except Exception as e:
             print("There is a problem opening the file:")
             print(e)
     else:
         # default argument
         terminal()
         exit(0)
-
-main()
```

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.6/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.6/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.6/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.6/FluidPyPLC/plc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import math
 import os
+import json
 from FluidPyPLC.data import Data
 from FluidPyPLC.set_switches import rotate
-from FluidPyPLC.f import path
+
+with open("config.json") as f:
+    config = json.load(f)
+    path = config["folder_path"]
 
 class Plc():
     def __init__(self, s):
         self.run(s)
     def run(self, s):
-        print(path)
         d = Data(s)
         solenoids = []
         g = len(d.groups)
         l = len(d.sequence)
         # change labels to e.g. Apositive, Bnegative, etc ..
         plc_groups = [[] for _ in range(g)]
         solenoids = [stroke.replace('+', 'positive') for stroke in d.sequence]
```

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.6/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.6/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.6/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.5
+Version: 0.1.6
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.5/LICENSE` & `FluidPyPLC-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.5/PKG-INFO` & `FluidPyPLC-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.5
+Version: 0.1.6
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.5/README.md` & `FluidPyPLC-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -106,189 +106,202 @@
 00000690: 6e73 7461 6c6c 6174 696f 6e20 3c61 206e  nstallation <a n
 000006a0: 616d 653d 2269 6e73 7461 6c6c 6174 696f  ame="installatio
 000006b0: 6e22 3e3c 2f61 3e0d 0a55 7365 2070 6970  n"></a>..Use pip
 000006c0: 2074 6f20 696e 7374 616c 6c20 466c 7569   to install Flui
 000006d0: 6450 7950 4c43 3a0d 0a60 6060 6261 7368  dPyPLC:..```bash
 000006e0: 0d0a 7069 7020 696e 7374 616c 6c20 466c  ..pip install Fl
 000006f0: 7569 6450 7950 4c43 0d0a 6060 600d 0a0d  uidPyPLC..```...
-00000700: 0a50 2e53 2e20 4920 7374 696c 6c20 6861  .P.S. I still ha
-00000710: 7665 2074 6f20 6d61 6e61 6765 2074 6865  ve to manage the
-00000720: 2066 696c 6573 2074 6861 7420 7769 6c6c   files that will
-00000730: 2062 6520 7361 7665 6420 6279 2046 6c75   be saved by Flu
-00000740: 6964 5079 504c 4320 616e 6420 7768 6572  idPyPLC and wher
-00000750: 6520 746f 2073 746f 7265 2074 6865 6d2e  e to store them.
-00000760: 2046 6f72 206e 6f77 2c20 796f 7520 6861   For now, you ha
-00000770: 7665 2074 6f20 6372 6561 7465 2061 2064  ve to create a d
-00000780: 6564 6963 6174 6564 2066 6f6c 6465 7220  edicated folder 
-00000790: 746f 206d 616b 6520 6974 2077 6f72 6b2e  to make it work.
-000007a0: 203c 6272 3e0d 0a49 2077 696c 6c20 6d61   <br>..I will ma
-000007b0: 6e61 6765 2074 6f20 646f 2074 6861 7420  nage to do that 
-000007c0: 4153 4150 2e0d 0a0d 0a0d 0a23 2320 f09f  ASAP.......## ..
-000007d0: 8e88 2055 7361 6765 203c 6120 6e61 6d65  .. Usage <a name
-000007e0: 3d22 7573 6167 6522 3e3c 2f61 3e0d 0a59  ="usage"></a>..Y
-000007f0: 6f75 2063 616e 2069 6e76 6f6b 6520 7468  ou can invoke th
-00000800: 6520 636f 6d6d 616e 6420 6672 6f6d 2061  e command from a
-00000810: 6e79 7768 6572 6520 6f6e 2079 6f75 7220  nywhere on your 
-00000820: 7465 726d 696e 616c 3a0d 0a60 6060 6261  terminal:..```ba
-00000830: 7368 0d0a 466c 7569 6450 7950 4c43 0d0a  sh..FluidPyPLC..
-00000840: 6060 600d 0a0d 0a54 6f20 7669 6577 2061  ```....To view a
-00000850: 6c6c 2074 6865 2075 7361 6765 2773 206d  ll the usage's m
-00000860: 6574 686f 6473 2075 7365 2074 6865 2074  ethods use the t
-00000870: 6167 7320 6060 602d 2d68 656c 7060 6060  ags ```--help```
-00000880: 206f 7220 6060 602d 6860 6060 2e0d 0a20   or ```-h```... 
-00000890: 0d0a 2323 20e2 9a99 efb8 8f20 434f 4445  ..## ...... CODE
-000008a0: 5359 5320 636f 6e66 6967 7572 6174 696f  SYS configuratio
-000008b0: 6e20 3c61 206e 616d 653d 2263 6f64 6573  n <a name="codes
-000008c0: 7973 5f63 6f6e 6669 6775 7261 7469 6f6e  ys_configuration
-000008d0: 223e 3c2f 613e 0d0a 5b2b 5d20 546f 2074  "></a>..[+] To t
-000008e0: 6573 7420 796f 7572 2050 4c43 2773 2073  est your PLC's s
-000008f0: 6571 7565 6e63 6520 636f 6465 2079 6f75  equence code you
-00000900: 2063 616e 2075 7365 2074 6865 2070 6c63   can use the plc
-00000910: 2e70 7920 616e 6420 6f6e 6520 6f66 2074  .py and one of t
-00000920: 6865 2043 4f4e 4649 4755 5241 5449 4f4e  he CONFIGURATION
-00000930: 2070 6466 7320 696e 2074 6865 2066 6c75   pdfs in the flu
-00000940: 6964 7369 6d20 666f 6c64 6572 2e0d 0a0d  idsim folder....
-00000950: 0a0d 0a5b 2b5d 2049 6620 796f 7520 7761  ...[+] If you wa
-00000960: 6e74 2074 6f20 7465 7374 2074 6865 2063  nt to test the c
-00000970: 6f64 6520 7769 7468 2074 6865 2043 4f44  ode with the COD
-00000980: 4553 5953 2056 6973 7561 6c69 7a61 7469  ESYS Visualizati
-00000990: 6f6e 2c20 7573 6520 7468 6520 706c 632e  on, use the plc.
-000009a0: 6261 6b32 2e70 7920 6173 2070 6c63 2e70  bak2.py as plc.p
-000009b0: 792c 2061 6e64 2074 6865 2074 7574 6f72  y, and the tutor
-000009c0: 6961 6c20 6265 6c6f 772e 200d 0a0d 0a49  ial below. ....I
-000009d0: 6e20 434f 4445 5359 5320 796f 7520 6861  n CODESYS you ha
-000009e0: 7665 2074 6f20 6372 6561 7465 2061 2070  ve to create a p
-000009f0: 726f 6a65 6374 2e20 496e 2074 6865 2070  roject. In the p
-00000a00: 726f 6a65 6374 2079 6f75 2077 696c 6c20  roject you will 
-00000a10: 6861 7665 2079 6f75 7220 504c 4320 6465  have your PLC de
-00000a20: 7669 6365 2c20 796f 7572 206d 6169 6e20  vice, your main 
-00000a30: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-00000a40: 2079 6f75 7220 6d61 696e 2050 5247 2066   your main PRG f
-00000a50: 696c 652e 2054 6f20 7465 7374 2074 6865  ile. To test the
-00000a60: 2053 5420 636f 6465 2079 6f75 206d 7573   ST code you mus
-00000a70: 7420 6164 6420 6120 4d6f 6462 7573 2053  t add a Modbus S
-00000a80: 6572 6961 6c20 4465 7669 6365 2074 6f20  erial Device to 
-00000a90: 6861 6e64 6c65 2074 6865 2069 6e70 7574  handle the input
-00000aa0: 7320 616e 6420 6f75 7470 7574 7320 6f66  s and outputs of
-00000ab0: 2079 6f75 7220 706c 632e 2054 6865 204d   your plc. The M
-00000ac0: 6f64 6275 7320 7769 6c6c 2061 6374 2061  odbus will act a
-00000ad0: 7320 616e 2069 6e74 6572 6d65 6469 6174  s an intermediat
-00000ae0: 6520 6265 7477 6565 6e20 796f 7572 2063  e between your c
-00000af0: 6f64 6520 616e 6420 6120 7669 7274 7561  ode and a virtua
-00000b00: 6c20 706c 6320 6465 7669 6365 2c20 6c69  l plc device, li
-00000b10: 6b65 2079 6f75 2061 7265 2073 6574 7469  ke you are setti
-00000b20: 6e67 2075 7020 7468 6520 696e 7075 7473  ng up the inputs
-00000b30: 2061 6e64 206f 7574 7075 7473 206f 6e20   and outputs on 
-00000b40: 6120 706c 6320 696e 2072 6561 6c20 6c69  a plc in real li
-00000b50: 6665 2e0d 0a0d 0a54 6f20 646f 2074 6861  fe.....To do tha
-00000b60: 742c 206f 7065 6e20 796f 7572 2043 4f44  t, open your COD
-00000b70: 4553 5953 2070 726f 6a65 6374 2c20 676f  ESYS project, go
-00000b80: 2074 6f0d 0a60 6060 6261 7368 0d0a 546f   to..```bash..To
-00000b90: 6f6c 7320 2d3e 2043 4f44 4553 5953 2069  ols -> CODESYS i
-00000ba0: 6e73 7461 6c6c 6572 0d0a 6060 600d 0a74  nstaller..```..t
-00000bb0: 6865 6e20 7365 6172 6368 2066 6f72 2022  hen search for "
-00000bc0: 4d6f 6462 7573 2220 616e 6420 696e 7374  Modbus" and inst
-00000bd0: 616c 6c20 7468 6520 6d6f 6475 6c65 7320  all the modules 
-00000be0: 7265 7175 6972 6564 2e20 4166 7465 7220  required. After 
-00000bf0: 7468 6174 2079 6f75 2068 6176 6520 746f  that you have to
-00000c00: 0d0a 6060 6062 6173 680d 0a72 6967 6874  ..```bash..right
-00000c10: 2d63 6c69 636b 2079 6f75 7220 504c 4320  -click your PLC 
-00000c20: 6465 7669 6365 202d 3e20 4164 6420 6465  device -> Add de
-00000c30: 7669 6365 200d 0a60 6060 0d0a 616e 6420  vice ..```..and 
-00000c40: 7468 656e 2073 656c 6563 740d 0a60 6060  then select..```
-00000c50: 6261 7368 0d0a 4d6f 6462 7573 202d 3e20  bash..Modbus -> 
-00000c60: 4d6f 6462 7573 2073 6572 6961 6c20 706f  Modbus serial po
-00000c70: 7274 202d 3e20 4d6f 6462 7573 2043 4f4d  rt -> Modbus COM
-00000c80: 0d0a 6060 600d 0a4e 6f77 2074 6861 7420  ..```..Now that 
-00000c90: 7468 6520 4d6f 6462 7573 2043 4f4d 2069  the Modbus COM i
-00000ca0: 7320 6164 6465 643a 203c 6272 3e0d 0a60  s added: <br>..`
-00000cb0: 6060 6261 7368 0d0a 7269 6768 742d 636c  ``bash..right-cl
-00000cc0: 6963 6b20 4d6f 6462 7573 5f43 4f4d 202d  ick Modbus_COM -
-00000cd0: 3e20 4164 6420 6465 7669 6365 202d 3e20  > Add device -> 
-00000ce0: 5365 6c65 6374 204d 6f64 6275 7320 2d3e  Select Modbus ->
-00000cf0: 204d 6f64 6275 7320 7365 7269 616c 2064   Modbus serial d
-00000d00: 6576 6963 6520 2d3e 204d 6f64 6275 7320  evice -> Modbus 
-00000d10: 5365 7269 616c 2044 6576 6963 650d 0a60  Serial Device..`
-00000d20: 6060 0d0a 4966 2079 6f75 2077 616e 7420  ``..If you want 
-00000d30: 746f 2072 656e 616d 6520 6974 2079 6f75  to rename it you
-00000d40: 2063 616e 2028 652e 672e 204d 6f64 6275   can (e.g. Modbu
-00000d50: 7320 492f 4f20 6861 6e64 6c65 722c 2065  s I/O handler, e
-00000d60: 7463 2e2e 292e 203c 6272 3e0d 0a4e 6f77  tc..). <br>..Now
-00000d70: 203c 623e 7269 6768 742d 636c 6963 6b20   <b>right-click 
-00000d80: 6974 202d 3e20 4d61 7020 492f 4f3c 2f62  it -> Map I/O</b
-00000d90: 3e20 616e 6420 6669 6e61 6c6c 7920 796f  > and finally yo
-00000da0: 7520 6361 6e20 6d61 7020 796f 7572 2069  u can map your i
-00000db0: 6e70 7574 7320 616e 6420 6f75 7470 7574  nputs and output
-00000dc0: 7320 6261 7365 6420 6f6e 2074 6865 2053  s based on the S
-00000dd0: 5420 636f 6465 2067 656e 6572 6174 6564  T code generated
-00000de0: 2062 7920 466c 7569 6450 7950 4c43 2e20   by FluidPyPLC. 
-00000df0: 3c62 723e 0d0a 4e6f 7720 796f 7520 6f6e  <br>..Now you on
-00000e00: 6c79 2068 6176 6520 746f 2064 6573 6967  ly have to desig
-00000e10: 6e20 796f 7572 204d 6163 6869 6e65 2069  n your Machine i
-00000e20: 6e20 7468 6520 7669 7375 616c 697a 6174  n the visualizat
-00000e30: 696f 6e20 6669 6c65 2061 6e64 2061 7373  ion file and ass
-00000e40: 6967 6e20 7468 6520 7377 6974 6368 6573  ign the switches
-00000e50: 2074 6f20 7468 6520 6c69 6d69 7420 7377   to the limit sw
-00000e60: 6974 6368 6573 2028 546f 2074 6573 7420  itches (To test 
-00000e70: 7468 6520 636f 6465 2c20 796f 7520 6861  the code, you ha
-00000e80: 7665 2074 6f20 6d61 6e75 616c 6c79 2063  ve to manually c
-00000e90: 6861 6e67 6520 7468 6520 6c69 6d69 7420  hange the limit 
-00000ea0: 7377 6974 6368 6573 2061 7320 796f 7520  switches as you 
-00000eb0: 646f 6e27 7420 6861 7665 2070 6879 7369  don't have physi
-00000ec0: 6361 6c20 506e 6575 6d61 7469 6320 5069  cal Pneumatic Pi
-00000ed0: 7374 6f6e 7320 7769 7468 2070 6879 7369  stons with physi
-00000ee0: 6361 6c20 6c69 6d69 7420 7377 6974 6368  cal limit switch
-00000ef0: 6573 292e 2045 6e6a 6f79 2079 6f75 7220  es). Enjoy your 
-00000f00: 504c 4327 7320 7369 6d75 6c61 7469 6f6e  PLC's simulation
-00000f10: 2e0d 0a0d 0a23 20f0 9f93 8420 4c69 6365  .....# .... Lice
-00000f20: 6e73 6520 3c61 206e 616d 6520 3d20 226c  nse <a name = "l
-00000f30: 6963 656e 7365 223e 3c2f 613e 0d0a 4750  icense"></a>..GP
-00000f40: 4c76 330d 0a0d 0a23 20e2 9c8d efb8 8f20  Lv3....# ...... 
-00000f50: 4175 7468 6f72 7320 3c61 206e 616d 6520  Authors <a name 
-00000f60: 3d20 2261 7574 686f 7273 223e 3c2f 613e  = "authors"></a>
-00000f70: 0d0a 2d20 5b4d 724c 6f73 7449 6e54 6865  ..- [MrLostInThe
-00000f80: 496e 7465 726e 6574 5d28 6874 7470 733a  Internet](https:
-00000f90: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 724c  //github.com/MrL
-00000fa0: 6f73 7449 6e54 6865 496e 7465 726e 6574  ostInTheInternet
-00000fb0: 290d 0a0d 0a3c 7020 616c 6967 6e3d 2263  )....<p align="c
-00000fc0: 656e 7465 7222 3e0d 0a3c 6272 3e0d 0a3c  enter">..<br>..<
-00000fd0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000fe0: 6769 7468 7562 2e63 6f6d 2f4d 724c 6f73  github.com/MrLos
-00000ff0: 7449 6e54 6865 496e 7465 726e 6574 2220  tInTheInternet" 
-00001000: 7461 7267 6574 3d27 5f62 6c61 6e6b 273e  target='_blank'>
-00001010: 0d0a 3c69 6d67 2068 6569 6768 743d 2733  ..<img height='3
-00001020: 3227 2073 7479 6c65 3d27 626f 7264 6572  2' style='border
-00001030: 3a30 7078 3b68 6569 6768 743a 3332 7078  :0px;height:32px
-00001040: 3b62 6f72 6465 722d 7261 6469 7573 3a2e  ;border-radius:.
-00001050: 3572 656d 2720 7372 633d 2768 7474 7073  5rem' src='https
-00001060: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001070: 6f2f 6261 6467 652f 4769 7448 7562 2d31  o/badge/GitHub-1
-00001080: 3030 3030 303f 7374 796c 6526 2378 3344  00000?style&#x3D
-00001090: 3b66 6f72 2d74 6865 2d62 6164 6765 2661  ;for-the-badge&a
-000010a0: 6d70 3b6c 6f67 6f26 2378 3344 3b67 6974  mp;logo&#x3D;git
-000010b0: 6875 6226 616d 703b 6c6f 676f 436f 6c6f  hub&amp;logoColo
-000010c0: 7226 2378 3344 3b77 6869 7465 2720 626f  r&#x3D;white' bo
-000010d0: 7264 6572 3d27 3027 0d0a 3c2f 613e 0d0a  rder='0'..</a>..
-000010e0: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-000010f0: 3a2f 2f79 6f75 7475 2e62 652f 614d 4373  ://youtu.be/aMCs
-00001100: 716d 5831 704f 4922 2074 6172 6765 743d  qmX1pOI" target=
-00001110: 275f 626c 616e 6b27 3e0d 0a3c 696d 6720  '_blank'>..<img 
-00001120: 6865 6967 6874 3d27 3332 2720 7374 796c  height='32' styl
-00001130: 653d 2762 6f72 6465 723a 3070 783b 6865  e='border:0px;he
-00001140: 6967 6874 3a33 3270 783b 626f 7264 6572  ight:32px;border
-00001150: 2d72 6164 6975 733a 2e35 7265 6d27 2073  -radius:.5rem' s
-00001160: 7263 3d27 6874 7470 733a 2f2f 696d 672e  rc='https://img.
-00001170: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00001180: 2f59 6f75 5475 6265 2d46 4630 3030 303f  /YouTube-FF0000?
-00001190: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-000011a0: 6467 6526 6c6f 676f 3d79 6f75 7475 6265  dge&logo=youtube
-000011b0: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-000011c0: 270d 0a62 6f72 6465 723d 2730 270d 0a3c  '..border='0'..<
-000011d0: 2f61 3e0d 0a20 2020 200d 0a3c 7020 616c  /a>..    ..<p al
-000011e0: 6967 6e3d 2263 656e 7465 7222 3e0d 0a74  ign="center">..t
-000011f0: 6861 6e6b 7320 746f 203c 6120 6872 6566  hanks to <a href
-00001200: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001210: 2e63 6f6d 2f77 7269 7465 6d65 2d70 726f  .com/writeme-pro
-00001220: 6a65 6374 2f77 7269 7465 6d65 223e 7772  ject/writeme">wr
-00001230: 6974 656d 653c 2f61 3e20 666f 7220 7468  iteme</a> for th
-00001240: 6520 5245 4144 4d45 2074 656d 706c 6174  e README templat
-00001250: 650d 0a3c 2f70 3e0d 0a                   e..</p>..
+00000700: 0a42 6566 6f72 6520 796f 7520 7573 6520  .Before you use 
+00000710: 6974 2c20 796f 7520 6861 7665 2074 6f20  it, you have to 
+00000720: 636f 6e66 6967 2074 6865 2063 6f6e 6669  config the confi
+00000730: 672e 6a73 6f6e 2066 696c 652e 2043 6861  g.json file. Cha
+00000740: 6e67 6520 7468 6520 2266 6f6c 6465 725f  nge the "folder_
+00000750: 7061 7468 2220 696e 2074 6865 2063 6f6e  path" in the con
+00000760: 6669 672e 6a73 6f6e 2066 696c 653a 0d0a  fig.json file:..
+00000770: 0d0a 6060 6062 6173 680d 0a63 6f6e 6669  ..```bash..confi
+00000780: 672e 6a73 6f6e 203a 0d0a 7b0d 0a20 2022  g.json :..{..  "
+00000790: 666f 6c64 6572 5f70 6174 6822 3a20 2266  folder_path": "f
+000007a0: 756c 6c2f 7061 7468 2f74 6f2f 7468 652f  ull/path/to/the/
+000007b0: 666f 6c64 6572 2f74 6861 742f 796f 752f  folder/that/you/
+000007c0: 7761 6e74 220d 0a7d 0d0a 6060 600d 0a0d  want"..}..```...
+000007d0: 0a50 2e53 2e20 4920 7374 696c 6c20 6861  .P.S. I still ha
+000007e0: 7665 2074 6f20 6d61 6e61 6765 2074 6865  ve to manage the
+000007f0: 2066 696c 6573 2074 6861 7420 7769 6c6c   files that will
+00000800: 2062 6520 7361 7665 6420 6279 2046 6c75   be saved by Flu
+00000810: 6964 5079 504c 4320 616e 6420 7768 6572  idPyPLC and wher
+00000820: 6520 746f 2073 746f 7265 2074 6865 6d2e  e to store them.
+00000830: 2046 6f72 206e 6f77 2c20 796f 7520 6861   For now, you ha
+00000840: 7665 2074 6f20 6372 6561 7465 2061 2064  ve to create a d
+00000850: 6564 6963 6174 6564 2066 6f6c 6465 7220  edicated folder 
+00000860: 746f 206d 616b 6520 6974 2077 6f72 6b2e  to make it work.
+00000870: 203c 6272 3e0d 0a49 2077 696c 6c20 6d61   <br>..I will ma
+00000880: 6e61 6765 2074 6f20 646f 2074 6861 7420  nage to do that 
+00000890: 4153 4150 2e0d 0a0d 0a0d 0a23 2320 f09f  ASAP.......## ..
+000008a0: 8e88 2055 7361 6765 203c 6120 6e61 6d65  .. Usage <a name
+000008b0: 3d22 7573 6167 6522 3e3c 2f61 3e0d 0a59  ="usage"></a>..Y
+000008c0: 6f75 2063 616e 2069 6e76 6f6b 6520 7468  ou can invoke th
+000008d0: 6520 636f 6d6d 616e 6420 6672 6f6d 2061  e command from a
+000008e0: 6e79 7768 6572 6520 6f6e 2079 6f75 7220  nywhere on your 
+000008f0: 7465 726d 696e 616c 3a0d 0a60 6060 6261  terminal:..```ba
+00000900: 7368 0d0a 466c 7569 6450 7950 4c43 0d0a  sh..FluidPyPLC..
+00000910: 6060 600d 0a0d 0a54 6f20 7669 6577 2061  ```....To view a
+00000920: 6c6c 2074 6865 2075 7361 6765 2773 206d  ll the usage's m
+00000930: 6574 686f 6473 2075 7365 2074 6865 2074  ethods use the t
+00000940: 6167 7320 6060 602d 2d68 656c 7060 6060  ags ```--help```
+00000950: 206f 7220 6060 602d 6860 6060 2e0d 0a20   or ```-h```... 
+00000960: 0d0a 2323 20e2 9a99 efb8 8f20 434f 4445  ..## ...... CODE
+00000970: 5359 5320 636f 6e66 6967 7572 6174 696f  SYS configuratio
+00000980: 6e20 3c61 206e 616d 653d 2263 6f64 6573  n <a name="codes
+00000990: 7973 5f63 6f6e 6669 6775 7261 7469 6f6e  ys_configuration
+000009a0: 223e 3c2f 613e 0d0a 5b2b 5d20 546f 2074  "></a>..[+] To t
+000009b0: 6573 7420 796f 7572 2050 4c43 2773 2073  est your PLC's s
+000009c0: 6571 7565 6e63 6520 636f 6465 2079 6f75  equence code you
+000009d0: 2063 616e 2075 7365 2074 6865 2070 6c63   can use the plc
+000009e0: 2e70 7920 616e 6420 6f6e 6520 6f66 2074  .py and one of t
+000009f0: 6865 2043 4f4e 4649 4755 5241 5449 4f4e  he CONFIGURATION
+00000a00: 2070 6466 7320 696e 2074 6865 2066 6c75   pdfs in the flu
+00000a10: 6964 7369 6d20 666f 6c64 6572 2e0d 0a0d  idsim folder....
+00000a20: 0a0d 0a5b 2b5d 2049 6620 796f 7520 7761  ...[+] If you wa
+00000a30: 6e74 2074 6f20 7465 7374 2074 6865 2063  nt to test the c
+00000a40: 6f64 6520 7769 7468 2074 6865 2043 4f44  ode with the COD
+00000a50: 4553 5953 2056 6973 7561 6c69 7a61 7469  ESYS Visualizati
+00000a60: 6f6e 2c20 7573 6520 7468 6520 706c 632e  on, use the plc.
+00000a70: 6261 6b32 2e70 7920 6173 2070 6c63 2e70  bak2.py as plc.p
+00000a80: 792c 2061 6e64 2074 6865 2074 7574 6f72  y, and the tutor
+00000a90: 6961 6c20 6265 6c6f 772e 200d 0a0d 0a49  ial below. ....I
+00000aa0: 6e20 434f 4445 5359 5320 796f 7520 6861  n CODESYS you ha
+00000ab0: 7665 2074 6f20 6372 6561 7465 2061 2070  ve to create a p
+00000ac0: 726f 6a65 6374 2e20 496e 2074 6865 2070  roject. In the p
+00000ad0: 726f 6a65 6374 2079 6f75 2077 696c 6c20  roject you will 
+00000ae0: 6861 7665 2079 6f75 7220 504c 4320 6465  have your PLC de
+00000af0: 7669 6365 2c20 796f 7572 206d 6169 6e20  vice, your main 
+00000b00: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
+00000b10: 2079 6f75 7220 6d61 696e 2050 5247 2066   your main PRG f
+00000b20: 696c 652e 2054 6f20 7465 7374 2074 6865  ile. To test the
+00000b30: 2053 5420 636f 6465 2079 6f75 206d 7573   ST code you mus
+00000b40: 7420 6164 6420 6120 4d6f 6462 7573 2053  t add a Modbus S
+00000b50: 6572 6961 6c20 4465 7669 6365 2074 6f20  erial Device to 
+00000b60: 6861 6e64 6c65 2074 6865 2069 6e70 7574  handle the input
+00000b70: 7320 616e 6420 6f75 7470 7574 7320 6f66  s and outputs of
+00000b80: 2079 6f75 7220 706c 632e 2054 6865 204d   your plc. The M
+00000b90: 6f64 6275 7320 7769 6c6c 2061 6374 2061  odbus will act a
+00000ba0: 7320 616e 2069 6e74 6572 6d65 6469 6174  s an intermediat
+00000bb0: 6520 6265 7477 6565 6e20 796f 7572 2063  e between your c
+00000bc0: 6f64 6520 616e 6420 6120 7669 7274 7561  ode and a virtua
+00000bd0: 6c20 706c 6320 6465 7669 6365 2c20 6c69  l plc device, li
+00000be0: 6b65 2079 6f75 2061 7265 2073 6574 7469  ke you are setti
+00000bf0: 6e67 2075 7020 7468 6520 696e 7075 7473  ng up the inputs
+00000c00: 2061 6e64 206f 7574 7075 7473 206f 6e20   and outputs on 
+00000c10: 6120 706c 6320 696e 2072 6561 6c20 6c69  a plc in real li
+00000c20: 6665 2e0d 0a0d 0a54 6f20 646f 2074 6861  fe.....To do tha
+00000c30: 742c 206f 7065 6e20 796f 7572 2043 4f44  t, open your COD
+00000c40: 4553 5953 2070 726f 6a65 6374 2c20 676f  ESYS project, go
+00000c50: 2074 6f0d 0a60 6060 6261 7368 0d0a 546f   to..```bash..To
+00000c60: 6f6c 7320 2d3e 2043 4f44 4553 5953 2069  ols -> CODESYS i
+00000c70: 6e73 7461 6c6c 6572 0d0a 6060 600d 0a74  nstaller..```..t
+00000c80: 6865 6e20 7365 6172 6368 2066 6f72 2022  hen search for "
+00000c90: 4d6f 6462 7573 2220 616e 6420 696e 7374  Modbus" and inst
+00000ca0: 616c 6c20 7468 6520 6d6f 6475 6c65 7320  all the modules 
+00000cb0: 7265 7175 6972 6564 2e20 4166 7465 7220  required. After 
+00000cc0: 7468 6174 2079 6f75 2068 6176 6520 746f  that you have to
+00000cd0: 0d0a 6060 6062 6173 680d 0a72 6967 6874  ..```bash..right
+00000ce0: 2d63 6c69 636b 2079 6f75 7220 504c 4320  -click your PLC 
+00000cf0: 6465 7669 6365 202d 3e20 4164 6420 6465  device -> Add de
+00000d00: 7669 6365 200d 0a60 6060 0d0a 616e 6420  vice ..```..and 
+00000d10: 7468 656e 2073 656c 6563 740d 0a60 6060  then select..```
+00000d20: 6261 7368 0d0a 4d6f 6462 7573 202d 3e20  bash..Modbus -> 
+00000d30: 4d6f 6462 7573 2073 6572 6961 6c20 706f  Modbus serial po
+00000d40: 7274 202d 3e20 4d6f 6462 7573 2043 4f4d  rt -> Modbus COM
+00000d50: 0d0a 6060 600d 0a4e 6f77 2074 6861 7420  ..```..Now that 
+00000d60: 7468 6520 4d6f 6462 7573 2043 4f4d 2069  the Modbus COM i
+00000d70: 7320 6164 6465 643a 203c 6272 3e0d 0a60  s added: <br>..`
+00000d80: 6060 6261 7368 0d0a 7269 6768 742d 636c  ``bash..right-cl
+00000d90: 6963 6b20 4d6f 6462 7573 5f43 4f4d 202d  ick Modbus_COM -
+00000da0: 3e20 4164 6420 6465 7669 6365 202d 3e20  > Add device -> 
+00000db0: 5365 6c65 6374 204d 6f64 6275 7320 2d3e  Select Modbus ->
+00000dc0: 204d 6f64 6275 7320 7365 7269 616c 2064   Modbus serial d
+00000dd0: 6576 6963 6520 2d3e 204d 6f64 6275 7320  evice -> Modbus 
+00000de0: 5365 7269 616c 2044 6576 6963 650d 0a60  Serial Device..`
+00000df0: 6060 0d0a 4966 2079 6f75 2077 616e 7420  ``..If you want 
+00000e00: 746f 2072 656e 616d 6520 6974 2079 6f75  to rename it you
+00000e10: 2063 616e 2028 652e 672e 204d 6f64 6275   can (e.g. Modbu
+00000e20: 7320 492f 4f20 6861 6e64 6c65 722c 2065  s I/O handler, e
+00000e30: 7463 2e2e 292e 203c 6272 3e0d 0a4e 6f77  tc..). <br>..Now
+00000e40: 203c 623e 7269 6768 742d 636c 6963 6b20   <b>right-click 
+00000e50: 6974 202d 3e20 4d61 7020 492f 4f3c 2f62  it -> Map I/O</b
+00000e60: 3e20 616e 6420 6669 6e61 6c6c 7920 796f  > and finally yo
+00000e70: 7520 6361 6e20 6d61 7020 796f 7572 2069  u can map your i
+00000e80: 6e70 7574 7320 616e 6420 6f75 7470 7574  nputs and output
+00000e90: 7320 6261 7365 6420 6f6e 2074 6865 2053  s based on the S
+00000ea0: 5420 636f 6465 2067 656e 6572 6174 6564  T code generated
+00000eb0: 2062 7920 466c 7569 6450 7950 4c43 2e20   by FluidPyPLC. 
+00000ec0: 3c62 723e 0d0a 4e6f 7720 796f 7520 6f6e  <br>..Now you on
+00000ed0: 6c79 2068 6176 6520 746f 2064 6573 6967  ly have to desig
+00000ee0: 6e20 796f 7572 204d 6163 6869 6e65 2069  n your Machine i
+00000ef0: 6e20 7468 6520 7669 7375 616c 697a 6174  n the visualizat
+00000f00: 696f 6e20 6669 6c65 2061 6e64 2061 7373  ion file and ass
+00000f10: 6967 6e20 7468 6520 7377 6974 6368 6573  ign the switches
+00000f20: 2074 6f20 7468 6520 6c69 6d69 7420 7377   to the limit sw
+00000f30: 6974 6368 6573 2028 546f 2074 6573 7420  itches (To test 
+00000f40: 7468 6520 636f 6465 2c20 796f 7520 6861  the code, you ha
+00000f50: 7665 2074 6f20 6d61 6e75 616c 6c79 2063  ve to manually c
+00000f60: 6861 6e67 6520 7468 6520 6c69 6d69 7420  hange the limit 
+00000f70: 7377 6974 6368 6573 2061 7320 796f 7520  switches as you 
+00000f80: 646f 6e27 7420 6861 7665 2070 6879 7369  don't have physi
+00000f90: 6361 6c20 506e 6575 6d61 7469 6320 5069  cal Pneumatic Pi
+00000fa0: 7374 6f6e 7320 7769 7468 2070 6879 7369  stons with physi
+00000fb0: 6361 6c20 6c69 6d69 7420 7377 6974 6368  cal limit switch
+00000fc0: 6573 292e 2045 6e6a 6f79 2079 6f75 7220  es). Enjoy your 
+00000fd0: 504c 4327 7320 7369 6d75 6c61 7469 6f6e  PLC's simulation
+00000fe0: 2e0d 0a0d 0a23 20f0 9f93 8420 4c69 6365  .....# .... Lice
+00000ff0: 6e73 6520 3c61 206e 616d 6520 3d20 226c  nse <a name = "l
+00001000: 6963 656e 7365 223e 3c2f 613e 0d0a 4750  icense"></a>..GP
+00001010: 4c76 330d 0a0d 0a23 20e2 9c8d efb8 8f20  Lv3....# ...... 
+00001020: 4175 7468 6f72 7320 3c61 206e 616d 6520  Authors <a name 
+00001030: 3d20 2261 7574 686f 7273 223e 3c2f 613e  = "authors"></a>
+00001040: 0d0a 2d20 5b4d 724c 6f73 7449 6e54 6865  ..- [MrLostInThe
+00001050: 496e 7465 726e 6574 5d28 6874 7470 733a  Internet](https:
+00001060: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 724c  //github.com/MrL
+00001070: 6f73 7449 6e54 6865 496e 7465 726e 6574  ostInTheInternet
+00001080: 290d 0a0d 0a3c 7020 616c 6967 6e3d 2263  )....<p align="c
+00001090: 656e 7465 7222 3e0d 0a3c 6272 3e0d 0a3c  enter">..<br>..<
+000010a0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000010b0: 6769 7468 7562 2e63 6f6d 2f4d 724c 6f73  github.com/MrLos
+000010c0: 7449 6e54 6865 496e 7465 726e 6574 2220  tInTheInternet" 
+000010d0: 7461 7267 6574 3d27 5f62 6c61 6e6b 273e  target='_blank'>
+000010e0: 0d0a 3c69 6d67 2068 6569 6768 743d 2733  ..<img height='3
+000010f0: 3227 2073 7479 6c65 3d27 626f 7264 6572  2' style='border
+00001100: 3a30 7078 3b68 6569 6768 743a 3332 7078  :0px;height:32px
+00001110: 3b62 6f72 6465 722d 7261 6469 7573 3a2e  ;border-radius:.
+00001120: 3572 656d 2720 7372 633d 2768 7474 7073  5rem' src='https
+00001130: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001140: 6f2f 6261 6467 652f 4769 7448 7562 2d31  o/badge/GitHub-1
+00001150: 3030 3030 303f 7374 796c 6526 2378 3344  00000?style&#x3D
+00001160: 3b66 6f72 2d74 6865 2d62 6164 6765 2661  ;for-the-badge&a
+00001170: 6d70 3b6c 6f67 6f26 2378 3344 3b67 6974  mp;logo&#x3D;git
+00001180: 6875 6226 616d 703b 6c6f 676f 436f 6c6f  hub&amp;logoColo
+00001190: 7226 2378 3344 3b77 6869 7465 2720 626f  r&#x3D;white' bo
+000011a0: 7264 6572 3d27 3027 0d0a 3c2f 613e 0d0a  rder='0'..</a>..
+000011b0: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+000011c0: 3a2f 2f79 6f75 7475 2e62 652f 614d 4373  ://youtu.be/aMCs
+000011d0: 716d 5831 704f 4922 2074 6172 6765 743d  qmX1pOI" target=
+000011e0: 275f 626c 616e 6b27 3e0d 0a3c 696d 6720  '_blank'>..<img 
+000011f0: 6865 6967 6874 3d27 3332 2720 7374 796c  height='32' styl
+00001200: 653d 2762 6f72 6465 723a 3070 783b 6865  e='border:0px;he
+00001210: 6967 6874 3a33 3270 783b 626f 7264 6572  ight:32px;border
+00001220: 2d72 6164 6975 733a 2e35 7265 6d27 2073  -radius:.5rem' s
+00001230: 7263 3d27 6874 7470 733a 2f2f 696d 672e  rc='https://img.
+00001240: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00001250: 2f59 6f75 5475 6265 2d46 4630 3030 303f  /YouTube-FF0000?
+00001260: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00001270: 6467 6526 6c6f 676f 3d79 6f75 7475 6265  dge&logo=youtube
+00001280: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00001290: 270d 0a62 6f72 6465 723d 2730 270d 0a3c  '..border='0'..<
+000012a0: 2f61 3e0d 0a20 2020 200d 0a3c 7020 616c  /a>..    ..<p al
+000012b0: 6967 6e3d 2263 656e 7465 7222 3e0d 0a74  ign="center">..t
+000012c0: 6861 6e6b 7320 746f 203c 6120 6872 6566  hanks to <a href
+000012d0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000012e0: 2e63 6f6d 2f77 7269 7465 6d65 2d70 726f  .com/writeme-pro
+000012f0: 6a65 6374 2f77 7269 7465 6d65 223e 7772  ject/writeme">wr
+00001300: 6974 656d 653c 2f61 3e20 666f 7220 7468  iteme</a> for th
+00001310: 6520 5245 4144 4d45 2074 656d 706c 6174  e README templat
+00001320: 650d 0a3c 2f70 3e0d 0a                   e..</p>..
```

### Comparing `FluidPyPLC-0.1.5/setup.py` & `FluidPyPLC-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 
 with open("FluidPyPLC/README.md", "r") as f:
     long_description = f.read()
 
 # Setting up
 setup(
```

