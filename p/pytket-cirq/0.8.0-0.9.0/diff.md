# Comparing `tmp/pytket-cirq-0.8.0.tar.gz` & `tmp/pytket-cirq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-cirq-0.8.0.tar", last modified: Tue Mar  2 14:33:26 2021, max compression
+gzip compressed data, was "pytket-cirq-0.9.0.tar", last modified: Thu Apr  1 10:56:22 2021, max compression
```

## Comparing `pytket-cirq-0.8.0.tar` & `pytket-cirq-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.655988 pytket-cirq-0.8.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/pytket/extensions/cirq/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/pytket/extensions/cirq/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17231 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/backends/cirq.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/backends/cirq_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11343 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/pytket/extensions/cirq/cirq_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/pytket_cirq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-02 14:33:26.000000 pytket-cirq-0.8.0/pytket_cirq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-02 14:33:26.659988 pytket-cirq-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-03-02 14:31:41.000000 pytket-cirq-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.263347 pytket-cirq-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.263347 pytket-cirq-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/pytket/extensions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/pytket/extensions/cirq/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17440 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/backends/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/backends/cirq_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11343 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/pytket/extensions/cirq/cirq_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/pytket_cirq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-01 10:56:22.000000 pytket-cirq-0.9.0/pytket_cirq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 10:56:22.267347 pytket-cirq-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2021-04-01 10:54:45.000000 pytket-cirq-0.9.0/setup.py
```

### Comparing `pytket-cirq-0.8.0/PKG-INFO` & `pytket-cirq-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytket-cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the Cirq framework
-Home-page: https://github.com/CQCL/pytket
+Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-cirq
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
```

### Comparing `pytket-cirq-0.8.0/README.md` & `pytket-cirq-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-cirq-0.8.0/pytket/extensions/cirq/__init__.py` & `pytket-cirq-0.9.0/pytket/extensions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-cirq-0.8.0/pytket/extensions/cirq/backends/__init__.py` & `pytket-cirq-0.9.0/pytket/extensions/cirq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-cirq-0.8.0/pytket/extensions/cirq/backends/cirq.py` & `pytket-cirq-0.9.0/pytket/extensions/cirq/backends/cirq.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import abstractmethod
 from typing import Sequence, cast, Optional, Iterable, List, Union
 from uuid import uuid4
 from cirq.sim import (
+    CliffordSimulator,
+    CliffordSimulatorStepResult,
     DensityMatrixSimulator,
+    DensityMatrixTrialResult,
     Simulator,
-    CliffordSimulator,
+    SparseSimulatorStep,
     StateVectorTrialResult,
-    DensityMatrixTrialResult,
 )
 
 # import cirq
 from cirq import ops
 from cirq.circuits import Circuit as CirqCircuit
 
 from pytket.circuit import Circuit, OpType, Qubit  # type: ignore
@@ -197,15 +199,14 @@
     ) -> BackendResult:
         """
 
         :param circuit: The circuit to simulate.
         :type circuit: CirqCircuit
         :param q_bits: ordered pytket Qubit
         :type q_bits: Sequence[Qubit]
-        Returns BackendResult
         :return: result of simulation
         :rtype: BackendResult
         """
         ...
 
     def run_circuit(self, circuit: Circuit, **kwargs: KwargTypes) -> BackendResult:
         cirq_circ = tk_to_cirq(circuit)
@@ -241,15 +242,14 @@
     ) -> List[BackendResult]:
         """
 
         :param circuit: The circuit to simulate.
         :type circuit: CirqCircuit
         :param q_bits: ordered pytket Qubit
         :type q_bits: Sequence[Qubit]
-        Returns BackendResult
         :return: sequence of moments from simulator
         :rtype: List[BackendResult]
         """
         ...
 
     def run_circuit_moments(
         self, circuit: Circuit, **kwargs: KwargTypes
@@ -346,15 +346,18 @@
         moments = self._simulator.simulate_moment_steps(
             circuit,
             qubit_order=ops.QubitOrder.as_qubit_order(ops.QubitOrder.DEFAULT).order_for(
                 circuit.all_qubits()
             ),
         )
         all_backres = [
-            BackendResult(state=run.state_vector(copy=True), q_bits=q_bits)
+            BackendResult(
+                state=cast(SparseSimulatorStep, run).state_vector(copy=True),
+                q_bits=q_bits,
+            )
             for run in moments
         ]
         return all_backres
 
 
 class CirqDensityMatrixSimBackend(_CirqSimBackend):
     """Backend for Cirq density matrix simulator density_matrix return."""
@@ -373,15 +376,18 @@
         return BackendResult(density_matrix=run.final_density_matrix, q_bits=q_bits)
 
     def package_results(
         self, circuit: CirqCircuit, q_bits: Sequence[Qubit]
     ) -> List[BackendResult]:
         moments = self._simulator.simulate_moment_steps(circuit)
         all_backres = [
-            BackendResult(density_matrix=run.density_matrix(copy=True), q_bits=q_bits)
+            BackendResult(
+                density_matrix=run.density_matrix(copy=True),  # type: ignore
+                q_bits=q_bits,
+            )
             for run in moments
         ]
 
         return all_backres
 
 
 class CirqCliffordSimBackend(_CirqSimBackend):
@@ -406,27 +412,30 @@
             self._simulator.simulate(
                 circuit,
                 qubit_order=ops.QubitOrder.as_qubit_order(
                     ops.QubitOrder.DEFAULT
                 ).order_for(circuit.all_qubits()),
             ),
         )
-        return BackendResult(state=run.final_state.state_vector(), q_bits=q_bits)
+        return BackendResult(state=run.final_state_vector, q_bits=q_bits)
 
     def package_results(
         self, circuit: CirqCircuit, q_bits: Sequence[Qubit]
     ) -> List[BackendResult]:
         moments = self._simulator.simulate_moment_steps(
             circuit,
             qubit_order=ops.QubitOrder.as_qubit_order(ops.QubitOrder.DEFAULT).order_for(
                 circuit.all_qubits()
             ),
         )
         all_backres = [
-            BackendResult(state=run.state.state_vector(), q_bits=q_bits)
+            BackendResult(
+                state=cast(CliffordSimulatorStepResult, run).state.state_vector(),
+                q_bits=q_bits,
+            )
             for run in moments
         ]
         return all_backres
 
 
 def _tk1_to_phasedxrz(a: float, b: float, c: float) -> Circuit:
     circ = Circuit(1)
```

### Comparing `pytket-cirq-0.8.0/pytket/extensions/cirq/backends/cirq_utils.py` & `pytket-cirq-0.9.0/pytket/extensions/cirq/backends/cirq_utils.py`

 * *Files identical despite different names*

### Comparing `pytket-cirq-0.8.0/pytket/extensions/cirq/cirq_convert.py` & `pytket-cirq-0.9.0/pytket/extensions/cirq/cirq_convert.py`

 * *Files identical despite different names*

### Comparing `pytket-cirq-0.8.0/pytket_cirq.egg-info/PKG-INFO` & `pytket-cirq-0.9.0/pytket_cirq.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pytket-cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the Cirq framework
-Home-page: https://github.com/CQCL/pytket
+Home-page: https://github.com/CQCL/pytket-extensions
 Author: Will Simmons
 Author-email: will.simmons@cambridgequantum.com
 License: Apache 2
 Description: # pytket-cirq
         
         [Pytket](https://cqcl.github.io/pytket) is a Python module for interfacing
         with CQC tket, a set of quantum programming tools.
```

### Comparing `pytket-cirq-0.8.0/setup.py` & `pytket-cirq-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
 setup(
     name=metadata["__extension_name__"],
     version=metadata["__extension_version__"],
     author="Will Simmons",
     author_email="will.simmons@cambridgequantum.com",
     python_requires=">=3.7",
-    url="https://github.com/CQCL/pytket",
+    url="https://github.com/CQCL/pytket-extensions",
     description="Extension for pytket, providing translation to and from the Cirq "
     "framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.8.0", "cirq ~= 0.9"],
+    install_requires=["pytket ~= 0.9.0", "cirq ~= 0.10"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

