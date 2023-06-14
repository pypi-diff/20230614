# Comparing `tmp/FluidPyPLC-0.1.2.tar.gz` & `tmp/FluidPyPLC-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.2.tar", last modified: Tue Jun 13 18:41:46 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.3.tar", last modified: Wed Jun 14 09:54:33 2023, max compression
```

## Comparing `FluidPyPLC-0.1.2.tar` & `FluidPyPLC-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.826069 FluidPyPLC-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.784300 FluidPyPLC-0.1.2/FluidPyPLC/
--rw-rw-rw-   0        0        0     6864 2023-06-13 18:35:22.000000 FluidPyPLC-0.1.2/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.2/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2750 2023-06-13 18:34:40.000000 FluidPyPLC-0.1.2/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3452 2023-06-13 18:34:34.000000 FluidPyPLC-0.1.2/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2303 2023-06-13 18:35:30.000000 FluidPyPLC-0.1.2/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.2/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14244 2023-06-13 18:34:24.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.2/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.2/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.823516 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 18:41:46.824512 FluidPyPLC-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 18:41:46.826069 FluidPyPLC-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-13 18:36:18.000000 FluidPyPLC-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.241620 FluidPyPLC-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.209575 FluidPyPLC-0.1.3/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6904 2023-06-14 09:49:30.000000 FluidPyPLC-0.1.3/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.3/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.3/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3462 2023-06-14 09:49:45.000000 FluidPyPLC-0.1.3/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2493 2023-06-14 09:49:12.000000 FluidPyPLC-0.1.3/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.3/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14266 2023-06-14 09:50:43.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.3/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.3/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.239625 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-14 09:54:33.240618 FluidPyPLC-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:54:33.241620 FluidPyPLC-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-14 09:50:16.000000 FluidPyPLC-0.1.3/setup.py
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.3/FluidPyPLC/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .get_sequence import *
-from .data import Data
-from .plc import Plc
-from .diagrams import diagrams
+from FluidPyPLC.get_sequence import *
+from FluidPyPLC.data import Data
+from FluidPyPLC.plc import Plc
+from FluidPyPLC.diagrams import diagrams
 
 import PySimpleGUI as sg
 
 sg.theme('DarkTanBlue')
 sg.set_options(font=('Helvetica', 14))
 
 def collapse(layout, key, visible):
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/data.py` & `FluidPyPLC-0.1.3/FluidPyPLC/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .set_groups import Groups
-from .set_switches import Switches
+from FluidPyPLC.set_groups import Groups
+from FluidPyPLC.set_switches import Switches
 from copy import deepcopy
 
 # get the number of pistons and their labels
 def pistons(s):
     piston_label = []
     tmp = deepcopy(s)
     tmp = [words.replace("-", "") for words in tmp]
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.3/FluidPyPLC/diagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import matplotlib.pyplot as plt
-from .data import Data
+from FluidPyPLC.data import Data
 
 # get the x and y axis for the Phase's diagrams
 def xy_axis(number_of_pistons, pistons_labels, sequence):
     number_of_pistons , piston_labels = number_of_pistons, pistons_labels
     x_axis = list(range(0, len(sequence) + 1))
     y_axis = [[0 for strokes in range(len(sequence) + 1)] for label in range(number_of_pistons)]
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/f.py` & `FluidPyPLC-0.1.3/FluidPyPLC/f.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 from tkinter import *
 from PIL import Image, ImageTk
 
-from .get_sequence import Sequence
-from .diagrams import diagrams
-from .plc import Plc
-from .GUI import Gui
+from FluidPyPLC.get_sequence import Sequence
+from FluidPyPLC.diagrams import diagrams
+from FluidPyPLC.plc import Plc
+from FluidPyPLC.GUI import Gui
 
 import argparse
 import subprocess
 import textwrap
 
 # class to define the plot rendering and opening window
 class Window(Frame):
@@ -61,21 +61,27 @@
         # gui mode
         gui = Gui()
         gui.gui_mode()
         exit(0)
     elif args.terminal:
         # terminal mode
         terminal()
+        exit(0)
     elif args.plot:
         # show plot
-        show_plot()
+        try:
+            show_plot()
+            exit(0)
+        except:
+            print("There is no folder Plots. Create one.")
     elif args.plc:
         try:
             # open plc ST code with notepad
             subprocess.call(['notepad.exe', './plc/plc.st'])
         except:
             print("There is a problem opening the file.")
     else:
         # default argument
         terminal()
+        exit(0)
 
 main()
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.3/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.3/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.3/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.3/FluidPyPLC/plc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
-from .data import Data
-from .set_switches import rotate
+from FluidPyPLC.data import Data
+from FluidPyPLC.set_switches import rotate
 
 class Plc():
     def __init__(self, s):
         self.run(s)
     def run(self, s):
         d = Data(s)
         solenoids = []
@@ -130,15 +130,15 @@
             for i in range(number_of_memories):
                 f.write(f'\t{relay_memory_label[i]} : BOOL;\n')
             for i in range(n_of_plcs_8bit):
                 f.write('\tAB' + str(i) + " : BYTE;\n")
                 f.write('\tEB' + str(i) + " : BYTE;\n")
             f.write('END_VAR\n\n')
 
-            f.write('//Inputs and Outputs connections\n//AB* are FLUIDSIM PLC IN, EB* are FLUIDSIM PLC OUT\n')
+            f.write('//Inputs and Outputs connections\n`n//AB* are FLUIDSIM PLC IN, EB* are FLUIDSIM PLC OUT\n')
             for i in range(l):
                 if d.sequence[i] not in plc_seen_IO:
                     f.write(f'//{d.sequence[i]} -> {solenoids[i]}\t\t')
                     f.write(f'{d.lswitch[i]} -> {limit_switches[i]}\n')
                     plc_seen_IO.append(d.sequence[i])
 
             #---------------FIRST GROUP-----------------------
```

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.3/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.3/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.3/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.2
+Version: 0.1.3
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.1.2/LICENSE` & `FluidPyPLC-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.2/PKG-INFO` & `FluidPyPLC-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.2
+Version: 0.1.3
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.1.2/README.md` & `FluidPyPLC-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,32 +35,28 @@
 ```bash
 winget install python3 python3-pip
 ```
 For Linux users you can install it via apt:
 ```bash
 sudo apt-get install python3 python3-pip
 ```
-Then you need to install the modules using pip install:
+## ⬇️ Installation <a name="installation"></a>
+Use pip to install FluidPyPLC:
 ```bash
-python3 -m pip install -r requirements.txt
+pip install FluidPyPLC
 ```
-Now you are ready to install FluidPyPLC
 
-## ⬇️ Installation <a name="installation"></a>
-```bash
-git clone https://github.com/MrLostInTheInternet/PLC_FluidPy.git
+P.S. I still have to manage the files that will be saved by FluidPyPLC and where to store them. For now, you have to create a dedicated folder to make it work. <br>
+I will manage to do that ASAP.
 
-```
 
 ## 🎈 Usage <a name="usage"></a>
-
+You can invoke the command from anywhere on your terminal:
 ```bash
-cd FluidPyPLC/src
-
-python3 f.py
+FluidPyPLC
 ```
 
 To view all the usage's methods use the tags ```--help``` or ```-h```.
  
 ## ⚙️ CODESYS configuration <a name="codesys_configuration"></a>
 [+] To test your PLC's sequence code you can use the plc.py and one of the CONFIGURATION pdfs in the fluidsim folder.
```

#### html2text {}

```diff
@@ -14,33 +14,34 @@
 and converts the solution in Structured Text for PLCs. The GUI mode will show
 you the data structure of the sequence, the plc ST code and the plot. You can
 then copy and paste the ST code in any program you want that reads it, e.g.
 CODESYS. (I tried with CODESYS and works) ## âï¸ Configuration  To use this
 tool you need to install Python and Pip on your computer. For Windows users you
 can find it [here](https://python.org/downloads) or by using: ```bash winget
 install python3 python3-pip ``` For Linux users you can install it via apt:
-```bash sudo apt-get install python3 python3-pip ``` Then you need to install
-the modules using pip install: ```bash python3 -m pip install -
-r requirements.txt ``` Now you are ready to install FluidPyPLC ## â¬ï¸
-Installation  ```bash git clone https://github.com/MrLostInTheInternet/
-PLC_FluidPy.git ``` ## ð Usage  ```bash cd FluidPyPLC/src python3 f.py ```
-To view all the usage's methods use the tags ```--help``` or ```-h```. ##
-âï¸ CODESYS configuration  [+] To test your PLC's sequence code you can use
-the plc.py and one of the CONFIGURATION pdfs in the fluidsim folder. [+] If you
-want to test the code with the CODESYS Visualization, use the plc.bak2.py as
-plc.py, and the tutorial below. In CODESYS you have to create a project. In the
-project you will have your PLC device, your main application with your main PRG
-file. To test the ST code you must add a Modbus Serial Device to handle the
-inputs and outputs of your plc. The Modbus will act as an intermediate between
-your code and a virtual plc device, like you are setting up the inputs and
-outputs on a plc in real life. To do that, open your CODESYS project, go to
-```bash Tools -> CODESYS installer ``` then search for "Modbus" and install the
-modules required. After that you have to ```bash right-click your PLC device -
-> Add device ``` and then select ```bash Modbus -> Modbus serial port -> Modbus
-COM ``` Now that the Modbus COM is added:
+```bash sudo apt-get install python3 python3-pip ``` ## â¬ï¸ Installation
+Use pip to install FluidPyPLC: ```bash pip install FluidPyPLC ``` P.S. I still
+have to manage the files that will be saved by FluidPyPLC and where to store
+them. For now, you have to create a dedicated folder to make it work.
+I will manage to do that ASAP. ## ð Usage  You can invoke the command from
+anywhere on your terminal: ```bash FluidPyPLC ``` To view all the usage's
+methods use the tags ```--help``` or ```-h```. ## âï¸ CODESYS configuration
+[+] To test your PLC's sequence code you can use the plc.py and one of the
+CONFIGURATION pdfs in the fluidsim folder. [+] If you want to test the code
+with the CODESYS Visualization, use the plc.bak2.py as plc.py, and the tutorial
+below. In CODESYS you have to create a project. In the project you will have
+your PLC device, your main application with your main PRG file. To test the ST
+code you must add a Modbus Serial Device to handle the inputs and outputs of
+your plc. The Modbus will act as an intermediate between your code and a
+virtual plc device, like you are setting up the inputs and outputs on a plc in
+real life. To do that, open your CODESYS project, go to ```bash Tools -
+> CODESYS installer ``` then search for "Modbus" and install the modules
+required. After that you have to ```bash right-click your PLC device -> Add
+device ``` and then select ```bash Modbus -> Modbus serial port -> Modbus COM
+``` Now that the Modbus COM is added:
 ```bash right-click Modbus_COM -> Add device -> Select Modbus -> Modbus serial
 device -> Modbus Serial Device ``` If you want to rename it you can (e.g.
 Modbus I/O handler, etc..).
 Now right-click it -> Map I/O and finally you can map your inputs and outputs
 based on the ST code generated by FluidPyPLC.
 Now you only have to design your Machine in the visualization file and assign
 the switches to the limit switches (To test the code, you have to manually
```

### Comparing `FluidPyPLC-0.1.2/setup.py` & `FluidPyPLC-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

