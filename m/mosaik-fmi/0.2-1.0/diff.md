# Comparing `tmp/mosaik_fmi-0.2.tar.gz` & `tmp/mosaik_fmi-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mosaik_fmi-0.2.tar", last modified: Wed Feb 23 17:16:11 2022, max compression
+gzip compressed data, was "mosaik_fmi-1.0.tar", last modified: Wed Jun 14 08:55:25 2023, max compression
```

## Comparing `mosaik_fmi-0.2.tar` & `mosaik_fmi-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)    24436 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3343 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2012 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi/
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/mosaik_fmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10511 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/mosaik_fmi/mosaik_fmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/mosaik_fmi/parse_xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3343 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/mosaik_fmi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-02-23 17:16:11.000000 mosaik_fmi-0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1402 2022-02-23 17:15:59.000000 mosaik_fmi-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:55:25.228680 mosaik_fmi-1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-06-14 08:55:25.228680 mosaik_fmi-1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:55:25.227680 mosaik_fmi-1.0/mosaik_fmi/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/mosaik_fmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10572 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/mosaik_fmi/mosaik_fmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/mosaik_fmi/parse_xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:55:25.227680 mosaik_fmi-1.0/mosaik_fmi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-06-14 08:55:25.000000 mosaik_fmi-1.0/mosaik_fmi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-14 08:55:25.000000 mosaik_fmi-1.0/mosaik_fmi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 08:55:25.000000 mosaik_fmi-1.0/mosaik_fmi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-14 08:55:25.000000 mosaik_fmi-1.0/mosaik_fmi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-14 08:55:25.000000 mosaik_fmi-1.0/mosaik_fmi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 08:55:25.228680 mosaik_fmi-1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-06-14 08:55:15.000000 mosaik_fmi-1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mosaik_fmi-0.2/PKG-INFO` & `mosaik_fmi-1.0/mosaik_fmi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
-Name: mosaik_fmi
-Version: 0.2
+Name: mosaik-fmi
+Version: 1.0
 Summary: Adapter for FMUs (ME or CS) in mosaik
 Home-page: https://mosaik.offis.de
 Author: Cornelius Steinbrink
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 ==========
 mosaik-fmi
@@ -35,18 +34,15 @@
 
 * mosaik-fmi is based on the FMI++ library, which can be found at https://fmipp.sourceforge.io/
 * The FMI++ python interface is used, which can be found at https://github.com/AIT-IES/py-fmipp. See this page also for details about installation and requirements of the python interface.
 
 Test
 ====
 
-The tests for Co-Simulation and ModelExchange in test_fmuAdapter.py don't work together yet and have to be called separately
-(by commenting out the respective other one in @pytest.mark.parametrize("fmi_type,fmu_dir").
-
-The FMU for the test is based on https://github.com/qtronic/fmusdk.
+The FMUs for the test is based on https://github.com/modelica/Reference-FMUs.
 
 How to Use
 ==========
 Specify simulator configurations within your scenario script::
 
     sim_config = {
         'FMI': {
@@ -54,15 +50,15 @@
         },
         ...
     }
 
 Initialize the FMU Simulator::
 
     fmu_sim = world.start('FMI',
-                        integrator='dp',
+                        integrator='integratorCK',
                         work_dir='path/to/the/fmu/directory',
                         fmu_name='FMU_name',
                         fmi_version='2',
                         fmi_type='cs',
                         logging_on=False,
                         instance_name='FMU_name',
                         step_size=60*60)
@@ -75,34 +71,49 @@
                                  ...
                                  )
 
 Connect FMU output to another simulator's input::
 
     world.connect(fmu_entity[0], other_simulator,'fmu_output_1', 'simulator_input_1')
 
+Selecting integrator
+
+Refer to https://fmipp.readthedocs.io/projects/py-fmipp/en/latest/getting-started/model-exchange.html#classes-fmumodelexchangev1-and-fmumodelexchangev2 for choosing different integration algorithms
+
+
 Getting help
 ============
 
 If you need help, please visit the `mosaik-users mailing list`__ .
 
 __ https://mosaik.offis.de/mailinglist
 
 
 Changelog
 =========
 
+1.0 – 2023-06-14
+----------------
+
+- New: add test cases to test FMI v1 and v2
+- Fix: model identifier parsing fixed for FMI v1
+- Update: use fmipp.export.fmippex instead of fmipp
+
 0.2 – 2022-02-23
 ----------------
 
 - Fix: FMI model identifier instead of model name needed to create FMU using fmipp
 
 0.1 – 2020-08-14
 ----------------
 
 - Initial release
 
 
+
+
 Authors
 =======
 
-The adapter was initially developed by Cornelius Steinbrink and updated and extended by Thomas Raub and Jan Sören Schwarz.
+The adapter was initially developed by Cornelius Steinbrink and updated and extended by Thomas Raub,
+ Jan Sören Schwarz, Sharaf Alsharif and Annika Ofenloch.
```

### Comparing `mosaik_fmi-0.2/README.rst` & `mosaik_fmi-1.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 * mosaik-fmi is based on the FMI++ library, which can be found at https://fmipp.sourceforge.io/
 * The FMI++ python interface is used, which can be found at https://github.com/AIT-IES/py-fmipp. See this page also for details about installation and requirements of the python interface.
 
 Test
 ====
 
-The tests for Co-Simulation and ModelExchange in test_fmuAdapter.py don't work together yet and have to be called separately
-(by commenting out the respective other one in @pytest.mark.parametrize("fmi_type,fmu_dir").
-
-The FMU for the test is based on https://github.com/qtronic/fmusdk.
+The FMUs for the test is based on https://github.com/modelica/Reference-FMUs.
 
 How to Use
 ==========
 Specify simulator configurations within your scenario script::
 
     sim_config = {
         'FMI': {
@@ -28,15 +25,15 @@
         },
         ...
     }
 
 Initialize the FMU Simulator::
 
     fmu_sim = world.start('FMI',
-                        integrator='dp',
+                        integrator='integratorCK',
                         work_dir='path/to/the/fmu/directory',
                         fmu_name='FMU_name',
                         fmi_version='2',
                         fmi_type='cs',
                         logging_on=False,
                         instance_name='FMU_name',
                         step_size=60*60)
@@ -49,13 +46,18 @@
                                  ...
                                  )
 
 Connect FMU output to another simulator's input::
 
     world.connect(fmu_entity[0], other_simulator,'fmu_output_1', 'simulator_input_1')
 
+Selecting integrator
+
+Refer to https://fmipp.readthedocs.io/projects/py-fmipp/en/latest/getting-started/model-exchange.html#classes-fmumodelexchangev1-and-fmumodelexchangev2 for choosing different integration algorithms
+
+
 Getting help
 ============
 
 If you need help, please visit the `mosaik-users mailing list`__ .
 
 __ https://mosaik.offis.de/mailinglist
```

### Comparing `mosaik_fmi-0.2/mosaik_fmi/mosaik_fmi.py` & `mosaik_fmi-1.0/mosaik_fmi/mosaik_fmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 import os
 import mosaik_api
 import fmipp
 import mosaik_fmi.parse_xml
+import fmipp.export.fmippex as fmippex
 
 meta = {
     'models': {},
     'extra_methods': ['fmi_set', 'fmi_get']
 }
 
 '''
@@ -58,15 +59,15 @@
         self.integrator = None
         self.stop_before_event = False
         self.event_search_precision = None
 
     def init(self, sid, work_dir, fmu_name, fmi_type, instance_name='fmu_model', step_size=1, logging_on=False,
              step_factor=1.0, fmi_version=None, var_table=None, translation_table=None,
              time_diff_resolution=1e-9, interactive=False, visible=False, stop_time_defined=False, stop_time=10000,
-             integrator='ck', stop_before_event=False, event_search_precision=1e-10):
+             integrator='integratorCK', stop_before_event=False, event_search_precision=1e-10):
 
         self.sid = sid
 
         self.fmu_name = fmu_name
         self.instance_name = instance_name
         self.step_size = step_size
         self.step_factor = step_factor  # Factor to translate mosaik integer time into FMI float time
@@ -140,39 +141,39 @@
                 attrs_open = [self.stop_before_event, self.event_search_precision, self.integrator]
                 attrs_inst = []
                 attrs_init = []
 
             fmu = f_open_fmu(self.uri_to_extracted_fmu, self.model_identifier, self.logging_on, *attrs_open)
             self._entities[eid] = fmu
             inst_stat = self._entities[eid].instantiate(self.instance_name, *attrs_inst)
-            assert inst_stat == fmipp.fmi2OK
+            assert inst_stat == fmippex.fmi2OK
             self.set_values(eid, model_params, 'parameter')
             init_stat = self._entities[eid].initialize(*attrs_init)
-            assert init_stat == fmipp.fmi2OK
+            assert init_stat == fmippex.fmi2OK
 
             entities.append({'eid': eid, 'type': model, 'rel': []})
 
         return entities
 
     def step(self, t, inputs=None):
         if self.fmi_type=="CoSimulation":
             # If no input data is provided, all entities are stepped:
             if inputs is None or inputs == {}:
                 for fmu in self._entities.values():
                     step_stat = fmu.doStep(t * self.step_factor, self.step_size * self.step_factor, True)
-                    assert step_stat == fmipp.fmi2OK
+                    assert step_stat == fmippex.fmi2OK
 
             else:
                 for eid, attrs in inputs.items():
                     for attr, vals in attrs.items():
                         for val in vals.values():
                             self.set_values(eid, {attr: val}, 'input')
 
                     step_stat = self._entities[eid].doStep(t * self.step_factor, self.step_size * self.step_factor, True)
-                    assert step_stat == fmipp.fmiOK
+                    assert step_stat == fmippex.fmi2OK
 
             return t + self.step_size
 
         elif self.fmi_type=="ModelExchange":
             stepped_time = None
 
             # If no input data is provided, all entities are stepped:
@@ -233,15 +234,15 @@
     def set_values(self, eid, val_dict, var_type):
         '''Help function to set values to a given variable of an FMU. This is done via a "var_table" and a
         "translation_table" to avoid problems due to missmatching naming conventions in mosaik and FMI.'''
         for alt_name, val in val_dict.items():
             name = self.translation_table[var_type][alt_name]
             set_func = getattr(self._entities[eid], 'set' + self.var_table[var_type][name] + 'Value')
             set_stat = set_func(name, val)
-            assert set_stat == fmipp.fmiOK
+            assert set_stat == fmippex.fmi2OK
 
     def get_value(self, eid, alt_attr):
         '''Help function to get values from given variables of an FMU.'''
         attr = self.translation_table['output'][alt_attr]
         get_func = getattr(self._entities[eid], 'get' + self.var_table['output'][attr] + 'Value')
         val = get_func(attr)
         return val
```

### Comparing `mosaik_fmi-0.2/mosaik_fmi/parse_xml.py` & `mosaik_fmi-1.0/mosaik_fmi/parse_xml.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import xml.etree.ElementTree as ETree
 
+
 def get_var_table(filename):
     '''This function reads the XML description file of an FMU, extracts the variable
     information and stores it in dict structures for the mosaik adapter to read.'''
     var_table = {}
     translation_table = {}
 
     base = ETree.parse(filename).getroot()
@@ -17,15 +18,15 @@
             translation_table.setdefault(causality, {})
             # Mosaik requires python-conform variable naming (no periods)
             if '.' in name:
                 alt_name = name.replace('.', '_')
             else:
                 alt_name = name
             translation_table[causality][alt_name] = name
-            
+
             # In practice, input variables may sometimes be used as
             # parameters and vice versa (typically due to unclear FMU design)
             if causality == 'input':
                 var_table.setdefault('parameter', {})
                 translation_table.setdefault('parameter', {})
                 translation_table['parameter'][alt_name] = name
             if causality == 'parameter':
@@ -53,12 +54,17 @@
     version = base.get('fmiVersion')
     version = version.split('.')[0]
     return version
 
 
 def get_model_identifier(filename, fmi_type):
     base = ETree.parse(filename).getroot()
-    for child in base:
-        if child.tag in fmi_type:
-            model_identifier = child.get('modelIdentifier')
-
+    fmu_version = get_fmi_version(filename)
+    if fmu_version == '1':
+        model_identifier = base.get('modelIdentifier')
+    elif fmu_version == '2':
+        for child in base:
+            if child.tag in fmi_type:
+                model_identifier = child.get('modelIdentifier')
+    else:
+        raise ValueError('FMI %s is not supported' % fmu_version)
     return model_identifier
```

### Comparing `mosaik_fmi-0.2/mosaik_fmi.egg-info/PKG-INFO` & `mosaik_fmi-1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
-Name: mosaik-fmi
-Version: 0.2
+Name: mosaik_fmi
+Version: 1.0
 Summary: Adapter for FMUs (ME or CS) in mosaik
 Home-page: https://mosaik.offis.de
 Author: Cornelius Steinbrink
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 ==========
 mosaik-fmi
@@ -35,18 +34,15 @@
 
 * mosaik-fmi is based on the FMI++ library, which can be found at https://fmipp.sourceforge.io/
 * The FMI++ python interface is used, which can be found at https://github.com/AIT-IES/py-fmipp. See this page also for details about installation and requirements of the python interface.
 
 Test
 ====
 
-The tests for Co-Simulation and ModelExchange in test_fmuAdapter.py don't work together yet and have to be called separately
-(by commenting out the respective other one in @pytest.mark.parametrize("fmi_type,fmu_dir").
-
-The FMU for the test is based on https://github.com/qtronic/fmusdk.
+The FMUs for the test is based on https://github.com/modelica/Reference-FMUs.
 
 How to Use
 ==========
 Specify simulator configurations within your scenario script::
 
     sim_config = {
         'FMI': {
@@ -54,15 +50,15 @@
         },
         ...
     }
 
 Initialize the FMU Simulator::
 
     fmu_sim = world.start('FMI',
-                        integrator='dp',
+                        integrator='integratorCK',
                         work_dir='path/to/the/fmu/directory',
                         fmu_name='FMU_name',
                         fmi_version='2',
                         fmi_type='cs',
                         logging_on=False,
                         instance_name='FMU_name',
                         step_size=60*60)
@@ -75,34 +71,49 @@
                                  ...
                                  )
 
 Connect FMU output to another simulator's input::
 
     world.connect(fmu_entity[0], other_simulator,'fmu_output_1', 'simulator_input_1')
 
+Selecting integrator
+
+Refer to https://fmipp.readthedocs.io/projects/py-fmipp/en/latest/getting-started/model-exchange.html#classes-fmumodelexchangev1-and-fmumodelexchangev2 for choosing different integration algorithms
+
+
 Getting help
 ============
 
 If you need help, please visit the `mosaik-users mailing list`__ .
 
 __ https://mosaik.offis.de/mailinglist
 
 
 Changelog
 =========
 
+1.0 – 2023-06-14
+----------------
+
+- New: add test cases to test FMI v1 and v2
+- Fix: model identifier parsing fixed for FMI v1
+- Update: use fmipp.export.fmippex instead of fmipp
+
 0.2 – 2022-02-23
 ----------------
 
 - Fix: FMI model identifier instead of model name needed to create FMU using fmipp
 
 0.1 – 2020-08-14
 ----------------
 
 - Initial release
 
 
+
+
 Authors
 =======
 
-The adapter was initially developed by Cornelius Steinbrink and updated and extended by Thomas Raub and Jan Sören Schwarz.
+The adapter was initially developed by Cornelius Steinbrink and updated and extended by Thomas Raub,
+ Jan Sören Schwarz, Sharaf Alsharif and Annika Ofenloch.
```

### Comparing `mosaik_fmi-0.2/setup.py` & `mosaik_fmi-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='mosaik_fmi',
-      version='0.2',
+      version='1.0',
       description='Adapter for FMUs (ME or CS) in mosaik',
       long_description='\n\n'.join(
         open(f, 'rb').read().decode('utf-8')
         for f in ['README.rst', 'CHANGELOG', 'AUTHORS.txt']),
       author='Cornelius Steinbrink',
       author_email='mosaik@offis.de',
       url='https://mosaik.offis.de',
@@ -18,19 +18,18 @@
       packages=find_packages(exclude=['tests*']),
       include_package_data=True,
       classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Console',
             'Intended Audience :: Science/Research',
             'Natural Language :: English',
-            'License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)',
+            'License :: OSI Approved :: MIT License',
             'Natural Language :: English',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.6',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
             'Topic :: Scientific/Engineering',
             'Topic :: Software Development :: Libraries :: Python Modules',
       ],
 )
```

