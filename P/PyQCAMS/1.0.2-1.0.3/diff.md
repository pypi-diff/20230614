# Comparing `tmp/PyQCAMS-1.0.2.tar.gz` & `tmp/PyQCAMS-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQCAMS-1.0.2.tar", last modified: Tue May 30 00:05:48 2023, max compression
+gzip compressed data, was "PyQCAMS-1.0.3.tar", last modified: Wed Jun 14 17:22:33 2023, max compression
```

## Comparing `PyQCAMS-1.0.2.tar` & `PyQCAMS-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.794749 PyQCAMS-1.0.2/
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1063 2023-03-30 15:34:08.000000 PyQCAMS-1.0.2/LICENSE
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1049 2023-05-30 00:05:48.782381 PyQCAMS-1.0.2/PKG-INFO
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.250156 PyQCAMS-1.0.2/PyQCAMS.egg-info/
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1049 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/PKG-INFO
--rwxrwxrwx   0 roots     (1000) roots     (1000)      291 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/SOURCES.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/dependency_links.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)       96 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/requires.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/top_level.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)      564 2023-05-29 15:22:21.000000 PyQCAMS-1.0.2/README.md
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.686720 PyQCAMS-1.0.2/pyqcams/
--rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.2/pyqcams/__init__.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.2/pyqcams/constants.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     4528 2023-05-10 15:47:15.000000 PyQCAMS-1.0.2/pyqcams/plotters.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1986 2023-05-10 15:44:49.000000 PyQCAMS-1.0.2/pyqcams/psave.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)    33455 2023-05-30 00:04:32.000000 PyQCAMS-1.0.2/pyqcams/pymar.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     4094 2023-05-30 00:04:16.000000 PyQCAMS-1.0.2/pyqcams/util.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-05-30 00:05:48.799754 PyQCAMS-1.0.2/setup.cfg
--rwxrwxrwx   0 roots     (1000) roots     (1000)      839 2023-05-30 00:05:42.000000 PyQCAMS-1.0.2/setup.py
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-06-14 17:22:33.000179 PyQCAMS-1.0.3/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1063 2023-03-30 15:34:08.000000 PyQCAMS-1.0.3/LICENSE
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1211 2023-06-14 17:22:32.994181 PyQCAMS-1.0.3/PKG-INFO
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-06-14 17:22:32.393890 PyQCAMS-1.0.3/PyQCAMS.egg-info/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1211 2023-06-14 17:22:31.000000 PyQCAMS-1.0.3/PyQCAMS.egg-info/PKG-INFO
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      291 2023-06-14 17:22:31.000000 PyQCAMS-1.0.3/PyQCAMS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-06-14 17:22:31.000000 PyQCAMS-1.0.3/PyQCAMS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       96 2023-06-14 17:22:31.000000 PyQCAMS-1.0.3/PyQCAMS.egg-info/requires.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-06-14 17:22:31.000000 PyQCAMS-1.0.3/PyQCAMS.egg-info/top_level.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      702 2023-05-30 15:10:16.000000 PyQCAMS-1.0.3/README.md
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-06-14 17:22:32.913781 PyQCAMS-1.0.3/pyqcams/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.3/pyqcams/__init__.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.3/pyqcams/constants.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     4528 2023-05-10 15:47:15.000000 PyQCAMS-1.0.3/pyqcams/plotters.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1986 2023-05-10 15:44:49.000000 PyQCAMS-1.0.3/pyqcams/psave.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)    33485 2023-06-14 16:39:28.000000 PyQCAMS-1.0.3/pyqcams/pymar.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     3989 2023-05-30 00:11:59.000000 PyQCAMS-1.0.3/pyqcams/util.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-06-14 17:22:33.003178 PyQCAMS-1.0.3/setup.cfg
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      839 2023-06-14 16:56:15.000000 PyQCAMS-1.0.3/setup.py
```

### Comparing `PyQCAMS-1.0.2/LICENSE` & `PyQCAMS-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.2/PKG-INFO` & `PyQCAMS-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQCAMS
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Quasi Classical Atom Molecule Scattering
 Home-page: https://github.com/Rkoost/PyQCAMS
 Author: Rian Koots
 Author-email: rian.koots@stonybrook.edu
 License: UNKNOWN
 Description: # PyQCAMS
         Python Quasi-Classical Atom-Molecule Scattering, a Python package for atom-molecule scattering within the quasi-classical trajectory approach. 
@@ -14,14 +14,17 @@
         pip install PyQCAMS
         ``` 
         
         ## Usage
         <p>The `example` folder contains a full example for simulating the reaction H<sub>2</sub> + Ca. </p> 
         
         
+        ## Data
+        A sample dataset to reproduce the figures in the example notebook can be found at https://figshare.com/s/8b923dab304005ae7a5c.  
+        
         ## Contributing
         
         Pull requests are welcome. For major changes, please open an issue first
         to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
```

### Comparing `PyQCAMS-1.0.2/PyQCAMS.egg-info/PKG-INFO` & `PyQCAMS-1.0.3/PyQCAMS.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQCAMS
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Quasi Classical Atom Molecule Scattering
 Home-page: https://github.com/Rkoost/PyQCAMS
 Author: Rian Koots
 Author-email: rian.koots@stonybrook.edu
 License: UNKNOWN
 Description: # PyQCAMS
         Python Quasi-Classical Atom-Molecule Scattering, a Python package for atom-molecule scattering within the quasi-classical trajectory approach. 
@@ -14,14 +14,17 @@
         pip install PyQCAMS
         ``` 
         
         ## Usage
         <p>The `example` folder contains a full example for simulating the reaction H<sub>2</sub> + Ca. </p> 
         
         
+        ## Data
+        A sample dataset to reproduce the figures in the example notebook can be found at https://figshare.com/s/8b923dab304005ae7a5c.  
+        
         ## Contributing
         
         Pull requests are welcome. For major changes, please open an issue first
         to discuss what you would like to change.
         
         Please make sure to update tests as appropriate.
```

### Comparing `PyQCAMS-1.0.2/pyqcams/plotters.py` & `PyQCAMS-1.0.3/pyqcams/plotters.py`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.2/pyqcams/psave.py` & `PyQCAMS-1.0.3/pyqcams/psave.py`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.2/pyqcams/pymar.py` & `PyQCAMS-1.0.3/pyqcams/pymar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.integrate import solve_ivp, quad
 from scipy.optimize import root_scalar, fsolve
+import sys
 import warnings
 from pyqcams import util, constants
 import json
 
 
 class Energy(object):
     '''DVR with sine function basis for non-periodic functions over
@@ -92,17 +93,17 @@
             fig = input('Would you like to see a plot of your potential? '
                         'Type "y" for yes, or "n" for no: \n')
             if fig == 'y':
                 # Show re guess compared with elev
                 plt.plot(x,V(x))
                 plt.plot(re,V(re), marker = 'o')
                 plt.hlines(self.evj[self.v], 0, 5)
-                plt.ylim(self.evj[self.v]*3, V(re)*3) # zoom in
+                # plt.ylim(self.evj[self.v]*3, V(re)*3) # zoom in
                 plt.show()
-            quit()
+            sys.exit()
         # Integrate to solve for tau, n_vib
         tau = quad(lambda x: 1/np.sqrt(vbrot(x)),rm,rp)[0]
         vib = quad(lambda x: np.sqrt(vbrot(x)),rm,rp)[0]
         tau *= np.sqrt(2*self.mu)
         n_vib = np.round(-0.5 + vib*np.sqrt(2*self.mu)/np.pi)
         self.n_vib = n_vib
         self.tau = tau
@@ -811,33 +812,33 @@
             mol2_V, mol2_dV, _ = vF.buckingham(**mol2)
     else:
         mol2 = {}
         r_bc, mol2_V, mol2_dV, mol2['re'] = util.numToV(f'{potential_BC}')
         # Ensure calculation is within bounds of potential data 
         if data['r0'] < min(r_bc):
             print(f'Initial distance must be greater than minimum r value provided ({min(r_bc)}).')
-            quit()
+            sys.exit()
         if data['int_params']['r_stop'] > max(r_bc):
             print(f'Stop condition too large! Ensure "r_stop" <= maximum r value of potential ({max(r_bc)}).')
-            quit()
+            sys.exit()
     if potential_CA in vList:
         mol3 = data['potential_params']["CA"][f"{potential_CA}"]
         if potential_CA == 'morse':
             mol3_V, mol3_dV = vF.morse(**mol3)
         elif potential_CA == 'lj':
             mol3_V, mol3_dV = vF.lj(**mol3)
         elif potential_CA == 'buck':
             mol3_V, mol3_dV, _ = vF.buckingham(**mol3)
     else:
         mol3 = {}
         r_ca, mol3_V, mol3_dV, mol3['re'] = util.numToV(f'{potential_CA}')
         # Ensure calculation is within bounds of potential data 
         if data['r0'] < min(r_ca):
             print(f'Initial distance must be greater than minimum r value provided ({min(r_bc)}).')
-            quit()
+            sys.exit()
         if data['int_params']['r_stop'] > max(r_ca):
             print(f'Stop condition too large! Ensure "r_stop" < maximum r value of potential ({max(r_ca)}).')
 
     # Calculate relevant attributes
     inputs = {'m1' : m1, 'm2': m2, 'm3': m3, 
          'd0' : data['r0'], 'e0' : data['Ec (K)']*constants.cEK2H,
          'b': data['b'],'mol': AB, 'v1' : mol1_V, 'v2' : mol2_V, 'v3':mol3_V,
```

### Comparing `PyQCAMS-1.0.2/pyqcams/util.py` & `PyQCAMS-1.0.3/pyqcams/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,17 +97,14 @@
     num_V, function
         interpolated potential
     num_dV, function
         interpolated potential derivative
     num_re, float
         equilibrium point (min of potential)
     '''
-    # types = ['.csv','.txt','.dat']
-    # split = os.path.splitext(f'{file}')
-    # filetype = split[1]
     try:
         df = pd.read_csv(f'{file}',header = None, sep = None, engine='python')
         num_x = np.array([float(i) for i in df[0][:].values.tolist()])
         num_y = np.array([float(i) for i in df[1][:].values.tolist()])
     except Exception as e:
             print(e)
             quit()
```

### Comparing `PyQCAMS-1.0.2/setup.py` & `PyQCAMS-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setup(
     name = 'PyQCAMS',
-    version = '1.0.2',
+    version = '1.0.3',
     description = 'Python Quasi Classical Atom Molecule Scattering',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Rian Koots',
     author_email = 'rian.koots@stonybrook.edu',
     url = 'https://github.com/Rkoost/PyQCAMS',
     packages = find_packages(),
```

