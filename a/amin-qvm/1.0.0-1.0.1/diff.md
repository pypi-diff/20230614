# Comparing `tmp/amin_qvm-1.0.0.tar.gz` & `tmp/amin_qvm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.0.tar", last modified: Wed Jun 14 12:10:02 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.1.tar", last modified: Wed Jun 14 12:52:19 2023, max compression
```

## Comparing `amin_qvm-1.0.0.tar` & `amin_qvm-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:02.848355 amin_qvm-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.0/LICENSE.ttxt
--rw-rw-rw-   0        0        0     4249 2023-06-14 12:10:02.847354 amin_qvm-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:02.804834 amin_qvm-1.0.0/amin_qvm/
--rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.0/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.0/amin_qvm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:10:02.845403 amin_qvm-1.0.0/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     4249 2023-06-14 12:10:02.000000 amin_qvm-1.0.0/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-14 12:10:02.000000 amin_qvm-1.0.0/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:10:02.000000 amin_qvm-1.0.0/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-14 12:10:02.000000 amin_qvm-1.0.0/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 12:10:02.000000 amin_qvm-1.0.0/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 12:10:02.848355 amin_qvm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-06-14 11:22:58.000000 amin_qvm-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:52:19.156213 amin_qvm-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.1/LICENSE.ttxt
+-rw-rw-rw-   0        0        0     6047 2023-06-14 12:52:19.154212 amin_qvm-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 12:52:19.128215 amin_qvm-1.0.1/amin_qvm/
+-rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.1/amin_qvm/QuantumComputer.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.1/amin_qvm/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.1/amin_qvm/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 12:52:19.152219 amin_qvm-1.0.1/amin_qvm.egg-info/
+-rw-rw-rw-   0        0        0     6047 2023-06-14 12:52:18.000000 amin_qvm-1.0.1/amin_qvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-14 12:52:19.000000 amin_qvm-1.0.1/amin_qvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 12:52:18.000000 amin_qvm-1.0.1/amin_qvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-14 12:52:18.000000 amin_qvm-1.0.1/amin_qvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 12:52:18.000000 amin_qvm-1.0.1/amin_qvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 12:52:19.156213 amin_qvm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-06-14 12:47:46.000000 amin_qvm-1.0.1/setup.py
```

### Comparing `amin_qvm-1.0.0/LICENSE.ttxt` & `amin_qvm-1.0.1/LICENSE.ttxt`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.0/PKG-INFO` & `amin_qvm-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin_qvm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/your-username/amin-qvm
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,7 +82,71 @@
    new_state = H2_1 * new_state
    new_state = Gate.CNOT2_01 * new_state
    Probability.pretty_print_probabilities(new_state)
 
 Prepare to have your mind blown once again as it displays probabilities and states.
 
 So, whether you're a quantum prodigy or just a curious mind, this code is perfect for unraveling the mysteries of quantum computing. Give it a whirl and explore the wonders of the quantum realm. Have fun!
+amin_qvm.functions Module
+=========================
+
+This module provides functions for quantum machine learning using Pennylane.
+
+Examples
+--------
+
+Training and Testing a Quantum Model
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   import numpy as np
+   from amin_qvm.functions import train, test
+   
+   # Generate training and testing data
+   X_train = np.random.rand(100, 2)
+   Y_train = np.random.choice([-1, 1], 100)
+   X_test = np.random.rand(20, 2)
+   Y_test = np.random.choice([-1, 1], 20)
+   
+   # Train the quantum model
+   num_qubits = 2
+   num_layers = 4
+   num_steps = 100
+   params = train(X_train, Y_train, num_qubits, num_layers, num_steps)
+   
+   # Test the quantum model
+   accuracy = test(X_test, Y_test, params, num_qubits)
+   print("Accuracy:", accuracy)
+
+Custom Quantum Machine Learning
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   import numpy as np
+   from amin_qvm.functions import custom_quantum_machine_learning
+   
+   # Generate custom training and testing data
+   X_train = np.random.rand(100, 2)
+   Y_train = np.random.choice([-1, 1], 100)
+   X_test = np.random.rand(20, 2)
+   Y_test = np.random.choice([-1, 1], 20)
+   
+   # Perform custom quantum machine learning
+   num_qubits = 2
+   num_layers = 4
+   num_steps = 100
+   accuracy = custom_quantum_machine_learning(X_train, Y_train, X_test, Y_test, num_qubits, num_layers, num_steps)
+   print("Accuracy (custom):", accuracy)
+
+Grover's Search Algorithm
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   from amin_qvm.functions import grover_search
+   
+   # Perform Grover's search
+   secret_bitstring = "1010"
+   guessed_bitstring = grover_search(secret_bitstring)
+   print("Guessed bitstring:", guessed_bitstring)
```

### Comparing `amin_qvm-1.0.0/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.1/amin_qvm/QuantumComputer.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.0/amin_qvm.egg-info/PKG-INFO` & `amin_qvm-1.0.1/amin_qvm.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin-qvm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/your-username/amin-qvm
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,7 +82,71 @@
    new_state = H2_1 * new_state
    new_state = Gate.CNOT2_01 * new_state
    Probability.pretty_print_probabilities(new_state)
 
 Prepare to have your mind blown once again as it displays probabilities and states.
 
 So, whether you're a quantum prodigy or just a curious mind, this code is perfect for unraveling the mysteries of quantum computing. Give it a whirl and explore the wonders of the quantum realm. Have fun!
+amin_qvm.functions Module
+=========================
+
+This module provides functions for quantum machine learning using Pennylane.
+
+Examples
+--------
+
+Training and Testing a Quantum Model
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   import numpy as np
+   from amin_qvm.functions import train, test
+   
+   # Generate training and testing data
+   X_train = np.random.rand(100, 2)
+   Y_train = np.random.choice([-1, 1], 100)
+   X_test = np.random.rand(20, 2)
+   Y_test = np.random.choice([-1, 1], 20)
+   
+   # Train the quantum model
+   num_qubits = 2
+   num_layers = 4
+   num_steps = 100
+   params = train(X_train, Y_train, num_qubits, num_layers, num_steps)
+   
+   # Test the quantum model
+   accuracy = test(X_test, Y_test, params, num_qubits)
+   print("Accuracy:", accuracy)
+
+Custom Quantum Machine Learning
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   import numpy as np
+   from amin_qvm.functions import custom_quantum_machine_learning
+   
+   # Generate custom training and testing data
+   X_train = np.random.rand(100, 2)
+   Y_train = np.random.choice([-1, 1], 100)
+   X_test = np.random.rand(20, 2)
+   Y_test = np.random.choice([-1, 1], 20)
+   
+   # Perform custom quantum machine learning
+   num_qubits = 2
+   num_layers = 4
+   num_steps = 100
+   accuracy = custom_quantum_machine_learning(X_train, Y_train, X_test, Y_test, num_qubits, num_layers, num_steps)
+   print("Accuracy (custom):", accuracy)
+
+Grover's Search Algorithm
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+   from amin_qvm.functions import grover_search
+   
+   # Perform Grover's search
+   secret_bitstring = "1010"
+   guessed_bitstring = grover_search(secret_bitstring)
+   print("Guessed bitstring:", guessed_bitstring)
```

### Comparing `amin_qvm-1.0.0/setup.py` & `amin_qvm-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import twine
 from setuptools import setup, find_packages
 
 # reading long description from file
-with open('DESCRIPTION.txt') as file:
+with open('DESCRIPTION.rst') as file:
 	long_description = file.read()
 
 
 # specify requirements of your package here
 REQUIREMENTS = [
     'numpy',
     'unittest',
     're',
     'random',
     'itertools',
     'functools',
     'math',
-    'time'
+    'time',
+    'qiskit',
+    'pennylane',
+    'scikit-learn'
 ]
-
 setup(
     name='amin_qvm',
-    version='1.0.0',
+    version='1.0.1',
     author='Amin Alogaili',
     author_email='aminalogai@gmail.com',
     description='Amin-QVM: Quantum Computing Library',
     long_description=long_description,
     url='https://github.com/your-username/amin-qvm',
     packages=['amin_qvm'],
     classifiers=[
```

