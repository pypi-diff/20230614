# Comparing `tmp/FluidPyPLC-0.1.3.tar.gz` & `tmp/FluidPyPLC-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.3.tar", last modified: Wed Jun 14 09:54:33 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.4.tar", last modified: Wed Jun 14 10:24:20 2023, max compression
```

## Comparing `FluidPyPLC-0.1.3.tar` & `FluidPyPLC-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.241620 FluidPyPLC-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.209575 FluidPyPLC-0.1.3/FluidPyPLC/
--rw-rw-rw-   0        0        0     6904 2023-06-14 09:49:30.000000 FluidPyPLC-0.1.3/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.3/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.3/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3462 2023-06-14 09:49:45.000000 FluidPyPLC-0.1.3/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2493 2023-06-14 09:49:12.000000 FluidPyPLC-0.1.3/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.3/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14266 2023-06-14 09:50:43.000000 FluidPyPLC-0.1.3/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.3/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.3/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:54:33.239625 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 09:54:33.000000 FluidPyPLC-0.1.3/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-14 09:54:33.240618 FluidPyPLC-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 09:54:33.241620 FluidPyPLC-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-14 09:50:16.000000 FluidPyPLC-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.910019 FluidPyPLC-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.889029 FluidPyPLC-0.1.4/FluidPyPLC/
+-rw-rw-rw-   0        0        0     7024 2023-06-14 09:58:00.000000 FluidPyPLC-0.1.4/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.4/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.4/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3462 2023-06-14 09:49:45.000000 FluidPyPLC-0.1.4/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     1612 2023-06-14 10:18:50.000000 FluidPyPLC-0.1.4/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.4/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14266 2023-06-14 09:50:43.000000 FluidPyPLC-0.1.4/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.4/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.4/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-14 10:24:20.909020 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-14 10:24:20.000000 FluidPyPLC-0.1.4/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1413 2023-06-14 10:24:20.910019 FluidPyPLC-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4697 2023-06-14 09:54:14.000000 FluidPyPLC-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 10:24:20.911031 FluidPyPLC-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-06-14 10:24:17.000000 FluidPyPLC-0.1.4/setup.py
```

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.4/FluidPyPLC/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,20 @@
                 window['text'].update('')
                 toggle_bool2 = False
                 window['-IMAGE-'].update(visible = False)
                 window['plc_code'].update('')
                 window['table'].update('')
             
             if event == 'Delete':
-                self.sequence.pop()
-                sequence = sequence[:-3]
-                window['text'].update(sequence)
+                try:
+                    self.sequence.pop()
+                    sequence = sequence[:-3]
+                    window['text'].update(sequence)
+                except:
+                    print("There is no sequence to delete")
 
             if event == "Display Phases' Diagram" and check:
                 toggle_bool2 = not toggle_bool2
                 im = './Plots/phases_diagram.png'
                 window['-IMAGE-'].update(im, visible = toggle_bool2)
                 window['image_column'].update(visible = toggle_bool2 or toggle_bool3)
```

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/data.py` & `FluidPyPLC-0.1.4/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.4/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.4/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.4/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.4/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.4/FluidPyPLC/plc.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.4/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.4/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/LICENSE` & `FluidPyPLC-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/README.md` & `FluidPyPLC-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.3/setup.py` & `FluidPyPLC-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
-LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
+
+with open("FluidPyPLC/README.md", "r") as f:
+    long_description = f.read()
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
     author="MrLostInTheInternet (Eugen Iofciu Vasile)",
     author_email="<eugen.iofciuvasile@hotmail.com>",
     license="GPLv3",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
+    url="https://github.com/MrLostInTheInternet/FluidPyPLC",
     packages=find_packages(),
     install_requires=['PySimpleGUI', 'matplotlib', 'tk', 'pillow'],
     entry_points={
         'console_scripts': [
             'FluidPyPLC = FluidPyPLC.f:main',
         ]},
     keywords=['python', 'plc', 'fluidsim', 'structured text', 'plc python', 'codesys', 'circuits', 'pneumatics', 'oleodynamics', 'plc programming'],
```

