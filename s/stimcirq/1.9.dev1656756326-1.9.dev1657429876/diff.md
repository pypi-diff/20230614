# Comparing `tmp/stimcirq-1.9.dev1656756326.tar.gz` & `tmp/stimcirq-1.9.dev1657429876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimcirq-1.9.dev1656756326.tar", last modified: Sat Jul  2 10:29:35 2022, max compression
+gzip compressed data, was "stimcirq-1.9.dev1657429876.tar", last modified: Sun Jul 10 05:33:54 2022, max compression
```

## Comparing `stimcirq-1.9.dev1656756326.tar` & `stimcirq-1.9.dev1657429876.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.189618 stimcirq-1.9.dev1656756326/
--rw-r--r--   0 runner     (501) staff       (20)     5272 2022-07-02 10:29:35.189218 stimcirq-1.9.dev1656756326/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4949 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-02 10:29:35.190027 stimcirq-1.9.dev1656756326/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1242 2022-07-02 10:07:06.000000 stimcirq-1.9.dev1656756326/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.186031 stimcirq-1.9.dev1656756326/stimcirq/
--rw-r--r--   0 runner     (501) staff       (20)     1382 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16346 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_cirq_to_stim.py
--rw-r--r--   0 runner     (501) staff       (20)    12468 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_cirq_to_stim_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4383 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_det_annotation.py
--rw-r--r--   0 runner     (501) staff       (20)     5249 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_det_annotation_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4245 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_measure_and_or_reset_gate.py
--rw-r--r--   0 runner     (501) staff       (20)     1305 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_measure_and_or_reset_gate_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4266 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_obs_annotation.py
--rw-r--r--   0 runner     (501) staff       (20)     6329 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_obs_annotation_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1357 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_shift_coords_annotation.py
--rw-r--r--   0 runner     (501) staff       (20)     2748 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_shift_coords_annotation_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1751 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_stim_sampler.py
--rw-r--r--   0 runner     (501) staff       (20)     3026 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_stim_sampler_test.py
--rw-r--r--   0 runner     (501) staff       (20)    20965 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_stim_to_cirq.py
--rw-r--r--   0 runner     (501) staff       (20)    17019 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_stim_to_cirq_test.py
--rw-r--r--   0 runner     (501) staff       (20)     2838 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_sweep_pauli.py
--rw-r--r--   0 runner     (501) staff       (20)     3770 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_sweep_pauli_test.py
--rw-r--r--   0 runner     (501) staff       (20)     2057 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_two_qubit_asymmetric_depolarize.py
--rw-r--r--   0 runner     (501) staff       (20)     1962 2022-07-02 10:07:05.000000 stimcirq-1.9.dev1656756326/stimcirq/_two_qubit_asymmetric_depolarize_test.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:35.188405 stimcirq-1.9.dev1656756326/stimcirq.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5272 2022-07-02 10:29:35.000000 stimcirq-1.9.dev1656756326/stimcirq.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      803 2022-07-02 10:29:35.000000 stimcirq-1.9.dev1656756326/stimcirq.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-02 10:29:35.000000 stimcirq-1.9.dev1656756326/stimcirq.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       15 2022-07-02 10:29:35.000000 stimcirq-1.9.dev1656756326/stimcirq.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2022-07-02 10:29:35.000000 stimcirq-1.9.dev1656756326/stimcirq.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.342683 stimcirq-1.9.dev1657429876/
+-rw-r--r--   0 runner     (501) staff       (20)     5272 2022-07-10 05:33:54.342290 stimcirq-1.9.dev1657429876/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4949 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-10 05:33:54.342988 stimcirq-1.9.dev1657429876/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1242 2022-07-10 05:11:44.000000 stimcirq-1.9.dev1657429876/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.338806 stimcirq-1.9.dev1657429876/stimcirq/
+-rw-r--r--   0 runner     (501) staff       (20)      821 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16346 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_cirq_to_stim.py
+-rw-r--r--   0 runner     (501) staff       (20)    12468 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_cirq_to_stim_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4383 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_det_annotation.py
+-rw-r--r--   0 runner     (501) staff       (20)     5249 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_det_annotation_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4245 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_measure_and_or_reset_gate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1305 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_measure_and_or_reset_gate_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4266 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_obs_annotation.py
+-rw-r--r--   0 runner     (501) staff       (20)     6329 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_obs_annotation_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1357 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_shift_coords_annotation.py
+-rw-r--r--   0 runner     (501) staff       (20)     2748 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_shift_coords_annotation_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1751 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_stim_sampler.py
+-rw-r--r--   0 runner     (501) staff       (20)     3026 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_stim_sampler_test.py
+-rw-r--r--   0 runner     (501) staff       (20)    20965 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_stim_to_cirq.py
+-rw-r--r--   0 runner     (501) staff       (20)    17019 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_stim_to_cirq_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2838 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_sweep_pauli.py
+-rw-r--r--   0 runner     (501) staff       (20)     3770 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_sweep_pauli_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2057 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_two_qubit_asymmetric_depolarize.py
+-rw-r--r--   0 runner     (501) staff       (20)     1962 2022-07-10 05:11:43.000000 stimcirq-1.9.dev1657429876/stimcirq/_two_qubit_asymmetric_depolarize_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:54.341610 stimcirq-1.9.dev1657429876/stimcirq.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5272 2022-07-10 05:33:54.000000 stimcirq-1.9.dev1657429876/stimcirq.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      803 2022-07-10 05:33:54.000000 stimcirq-1.9.dev1657429876/stimcirq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-10 05:33:54.000000 stimcirq-1.9.dev1657429876/stimcirq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       15 2022-07-10 05:33:54.000000 stimcirq-1.9.dev1657429876/stimcirq.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2022-07-10 05:33:54.000000 stimcirq-1.9.dev1657429876/stimcirq.egg-info/top_level.txt
```

### Comparing `stimcirq-1.9.dev1656756326/PKG-INFO` & `stimcirq-1.9.dev1657429876/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimcirq
-Version: 1.9.dev1656756326
+Version: 1.9.dev1657429876
 Summary: Implements a cirq.Sampler backed by stim.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `stimcirq-1.9.dev1656756326/README.md` & `stimcirq-1.9.dev1657429876/README.md`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/setup.py` & `stimcirq-1.9.dev1657429876/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from setuptools import setup
 
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read()
 
-version = '1.9.dev1656756326'
+version = '1.9.dev1657429876'
 
 setup(
     name='stimcirq',
     version=version,
     author='Craig Gidney',
     author_email='craig.gidney@gmail.com',
     url='https://github.com/quantumlib/stim',
```

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/__init__.py` & `stimcirq-1.9.dev1657429876/stimcirq/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,20 +15,7 @@
     "DetAnnotation": DetAnnotation,
     "MeasureAndOrResetGate": MeasureAndOrResetGate,
     "ShiftCoordsAnnotation": ShiftCoordsAnnotation,
     "SweepPauli": SweepPauli,
     "TwoQubitAsymmetricDepolarizingChannel": TwoQubitAsymmetricDepolarizingChannel,
 }
 JSON_RESOLVER = JSON_RESOLVERS_DICT.get
-
-# Workaround for doctest not searching imported objects.
-__test__ = {
-    "cirq_circuit_to_stim_circuit": cirq_circuit_to_stim_circuit,
-    "CumulativeObservableAnnotation": CumulativeObservableAnnotation,
-    "DetAnnotation": DetAnnotation,
-    "MeasureAndOrResetGate": MeasureAndOrResetGate,
-    "ShiftCoordsAnnotation": ShiftCoordsAnnotation,
-    "stim_circuit_to_cirq_circuit": stim_circuit_to_cirq_circuit,
-    "StimSampler": StimSampler,
-    "SweepPauli": SweepPauli,
-    "TwoQubitAsymmetricDepolarizingChannel": TwoQubitAsymmetricDepolarizingChannel,
-}
```

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_cirq_to_stim.py` & `stimcirq-1.9.dev1657429876/stimcirq/_cirq_to_stim.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_cirq_to_stim_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_cirq_to_stim_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_det_annotation.py` & `stimcirq-1.9.dev1657429876/stimcirq/_det_annotation.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_det_annotation_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_det_annotation_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_measure_and_or_reset_gate.py` & `stimcirq-1.9.dev1657429876/stimcirq/_measure_and_or_reset_gate.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_measure_and_or_reset_gate_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_measure_and_or_reset_gate_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_obs_annotation.py` & `stimcirq-1.9.dev1657429876/stimcirq/_obs_annotation.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_obs_annotation_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_obs_annotation_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_shift_coords_annotation.py` & `stimcirq-1.9.dev1657429876/stimcirq/_shift_coords_annotation.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_shift_coords_annotation_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_shift_coords_annotation_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_stim_sampler.py` & `stimcirq-1.9.dev1657429876/stimcirq/_stim_sampler.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_stim_sampler_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_stim_sampler_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_stim_to_cirq.py` & `stimcirq-1.9.dev1657429876/stimcirq/_stim_to_cirq.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_stim_to_cirq_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_stim_to_cirq_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_sweep_pauli.py` & `stimcirq-1.9.dev1657429876/stimcirq/_sweep_pauli.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_sweep_pauli_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_sweep_pauli_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_two_qubit_asymmetric_depolarize.py` & `stimcirq-1.9.dev1657429876/stimcirq/_two_qubit_asymmetric_depolarize.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq/_two_qubit_asymmetric_depolarize_test.py` & `stimcirq-1.9.dev1657429876/stimcirq/_two_qubit_asymmetric_depolarize_test.py`

 * *Files identical despite different names*

### Comparing `stimcirq-1.9.dev1656756326/stimcirq.egg-info/PKG-INFO` & `stimcirq-1.9.dev1657429876/stimcirq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimcirq
-Version: 1.9.dev1656756326
+Version: 1.9.dev1657429876
 Summary: Implements a cirq.Sampler backed by stim.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
```

### Comparing `stimcirq-1.9.dev1656756326/stimcirq.egg-info/SOURCES.txt` & `stimcirq-1.9.dev1657429876/stimcirq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

