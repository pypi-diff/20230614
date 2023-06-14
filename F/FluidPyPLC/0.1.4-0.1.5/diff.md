# Comparing `tmp/FluidPyPLC-0.1.4.tar.gz` & `tmp/FluidPyPLC-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.4.tar", last modified: Wed Jun 14 10:24:20 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.5.tar", last modified: Wed Jun 14 20:00:19 2023, max compression
```

## Comparing `FluidPyPLC-0.1.4.tar` & `FluidPyPLC-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.910019 FluidPyPLC-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.889029 FluidPyPLC-0.1.4/FluidPyPLC/
--rw-rw-rw-   0        0        0     7024 2023-06-14 09:58:00.000000 FluidPyPLC-0.1.4/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.4/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.4/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3462 2023-06-14 09:49:45.000000 FluidPyPLC-0.1.4/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     1612 2023-06-14 10:18:50.000000 FluidPyPLC-0.1.4/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.4/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14266 2023-06-14 09:50:43.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.4/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.4/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.909020 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1413 2023-06-14 10:24:20.910019 FluidPyPLC-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 10:24:20.911031 FluidPyPLC-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-06-14 10:24:17.000000 FluidPyPLC-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.117952 FluidPyPLC-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.075486 FluidPyPLC-0.1.5/FluidPyPLC/
+-rw-rw-rw-   0        0        0     7102 2023-06-14 19:19:20.000000 FluidPyPLC-0.1.5/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.5/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.5/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3541 2023-06-14 19:56:37.000000 FluidPyPLC-0.1.5/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2277 2023-06-14 19:57:55.000000 FluidPyPLC-0.1.5/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.5/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14347 2023-06-14 19:29:38.000000 FluidPyPLC-0.1.5/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.5/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.5/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:00:19.115971 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 20:00:18.000000 FluidPyPLC-0.1.5/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1413 2023-06-14 20:00:19.116956 FluidPyPLC-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:00:19.117952 FluidPyPLC-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-06-14 19:57:27.000000 FluidPyPLC-0.1.5/setup.py
```

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.5/FluidPyPLC/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from FluidPyPLC.get_sequence import *
 from FluidPyPLC.data import Data
 from FluidPyPLC.plc import Plc
 from FluidPyPLC.diagrams import diagrams
+from FluidPyPLC.f import path
 
+import os
 import PySimpleGUI as sg
 
 sg.theme('DarkTanBlue')
 sg.set_options(font=('Helvetica', 14))
 
 def collapse(layout, key, visible):
     return sg.pin(sg.Column(layout, key=key, visible=visible))
@@ -108,15 +110,15 @@
                     if check is False:
                         sg.PopupQuickMessage("The sequence isn't completed.", background_color='Red')
                         continue
                     else:
                         self.data = elaborate_data(self.sequence)
                         diagrams(self.sequence)
                         Plc(self.sequence)
-                        dir1 = './plc/plc.st'
+                        dir1 = os.path.join(path, 'plc/plc.st')
                         with open(dir1, 'r') as p:
                             Text = p.readlines()
                             Text = ''.join(line for line in Text)
                         window['table'].update(self.data, visible = False)
                         window['plc_code'].update(Text)
                                 
             if event == 'Clear':
@@ -134,15 +136,15 @@
                     sequence = sequence[:-3]
                     window['text'].update(sequence)
                 except:
                     print("There is no sequence to delete")
 
             if event == "Display Phases' Diagram" and check:
                 toggle_bool2 = not toggle_bool2
-                im = './Plots/phases_diagram.png'
+                im = os.path.join(path, 'Plots/phases_diagram.png')
                 window['-IMAGE-'].update(im, visible = toggle_bool2)
                 window['image_column'].update(visible = toggle_bool2 or toggle_bool3)
 
             if event == 'show_plc':
                 toggle_bool1 = not toggle_bool1
                 window['plc'].update(visible=toggle_bool1)
                 window['plc_code'].update(Text)
```

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/data.py` & `FluidPyPLC-0.1.5/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.5/FluidPyPLC/diagrams.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import os
 import matplotlib.pyplot as plt
 from FluidPyPLC.data import Data
+from FluidPyPLC.f import path
 
 # get the x and y axis for the Phase's diagrams
 def xy_axis(number_of_pistons, pistons_labels, sequence):
     number_of_pistons , piston_labels = number_of_pistons, pistons_labels
     x_axis = list(range(0, len(sequence) + 1))
     y_axis = [[0 for strokes in range(len(sequence) + 1)] for label in range(number_of_pistons)]
 
@@ -73,12 +75,13 @@
                     rowLabels = ['limit switches'],
                     colLabels = columns,
                     loc = 'bottom',
                     bbox =[0.0, -0.25, 1, 0.12])
         diagram.axis('off')
         diagram.axis('off')
         plt.subplots_adjust(left=0.190, bottom=0.210, right=0.900, top=0.970, wspace=None, hspace=1.000)
-        plt.savefig('./Plots/phases_diagram.png')
+        dir = os.path.join(path, 'Plots/phases_diagram.png')
+        plt.savefig(dir)
 
     except:
         if number_of_pistons == 1:
             print("There is only one piston, no need for the graphic plot")
```

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/f.py` & `FluidPyPLC-0.1.5/FluidPyPLC/f.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,52 +5,75 @@
 
 from FluidPyPLC.get_sequence import Sequence
 from FluidPyPLC.diagrams import diagrams
 from FluidPyPLC.plc import Plc
 from FluidPyPLC.GUI import Gui
 
 import argparse
+import json
 import subprocess
 import textwrap
+import os
+
+global path
+
+def create_folders(folder_path):
+    plots_folder = os.path.join(folder_path, 'Plots')
+    plc_folder = os.path.join(folder_path, 'plc')
+
+    # Create the Plots and plc folders
+    os.makedirs(plots_folder, exist_ok=True)
+    os.makedirs(plc_folder, exist_ok=True)
+
+    print(f"Created 'Plots' and 'plc' folders inside '{folder_path}'.")
 
 # function to start the terminal version
 def terminal():
     sequence = Sequence()
     s = sequence.s
     diagrams(s)
     Plc(s)
 
 # args management
 def main():
+    global path
     parser = argparse.ArgumentParser(
         description='FluidPyPLC',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog=textwrap.dedent('''Example:
         f.py --gui # to use the user interface mode
         f.py -t # to use the terminal version
         f.py --plc # to display the plc ST code
         ''')
     )
     parser.add_argument('-g', '--gui', action='store_true', help='gui mode')
     parser.add_argument('-t', '--terminal', action='store_true', help='terminal mode')
     parser.add_argument('--plc', action='store_true', help='show plc code')
     args = parser.parse_args()
+    try:
+        with open("config.json") as f:
+            config = json.load(f)
+        path = config["folder_path"]
+        print(f"Loaded path from config.json: '{path}'.")
+    except Exception:
+        None
     if args.gui:
         # gui mode
         gui = Gui()
         gui.gui_mode()
         exit(0)
     elif args.terminal:
         # terminal mode
         terminal()
         exit(0)
     elif args.plc:
         try:
             # open plc ST code with notepad
-            subprocess.call(['notepad.exe', './plc/plc.st'])
+            dir = os.path.join(path, 'plc/plc.st')
+            subprocess.call(['notepad.exe', dir])
         except Exception as e:
             print("There is a problem opening the file:")
             print(e)
     else:
         # default argument
         terminal()
         exit(0)
```

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.5/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.5/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.5/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.5/FluidPyPLC/plc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import math
+import os
 from FluidPyPLC.data import Data
 from FluidPyPLC.set_switches import rotate
+from FluidPyPLC.f import path
 
 class Plc():
     def __init__(self, s):
         self.run(s)
     def run(self, s):
+        print(path)
         d = Data(s)
         solenoids = []
         g = len(d.groups)
         l = len(d.sequence)
         # change labels to e.g. Apositive, Bnegative, etc ..
         plc_groups = [[] for _ in range(g)]
         solenoids = [stroke.replace('+', 'positive') for stroke in d.sequence]
@@ -118,15 +121,15 @@
                 plc_seen_IO.append(limit_switches[i])
                 plc_index_8bit += 1
         plc_seen_IO_description = []
         plc_seen_IO = []
         n_of_plcs_8bit = 1 + math.floor(len(set(d.sequence)) / 7)
         d.lswitch = rotate(d.lswitch, 1)
         # open the plc.txt file and write the code, in ST language, on it
-        dir = "./plc/plc.st"
+        dir = os.path.join(path, 'plc/plc.st')
         with open(dir,'w') as f:
             #relays variables ----------------------------------------------------
             f.write('PROGRAM PLC_PRG\n')
             f.write('VAR\n')
             for i in range(number_of_memories):
                 f.write(f'\t{relay_memory_label[i]} : BOOL;\n')
             for i in range(n_of_plcs_8bit):
```

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.5/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.5/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.5/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.4
+Version: 0.1.5
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.4/LICENSE` & `FluidPyPLC-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/PKG-INFO` & `FluidPyPLC-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.4
+Version: 0.1.5
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.4/README.md` & `FluidPyPLC-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.4/setup.py` & `FluidPyPLC-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 
 with open("FluidPyPLC/README.md", "r") as f:
     long_description = f.read()
 
 # Setting up
 setup(
```

