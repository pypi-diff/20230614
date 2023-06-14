# Comparing `tmp/amin_qvm-1.0.2.tar.gz` & `tmp/amin_qvm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.2.tar", last modified: Wed Jun 14 13:02:52 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.3.tar", last modified: Wed Jun 14 13:20:28 2023, max compression
```

## Comparing `amin_qvm-1.0.2.tar` & `amin_qvm-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:52.190743 amin_qvm-1.0.2/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.2/LICENSE.ttxt
--rw-rw-rw-   0        0        0     6047 2023-06-14 13:02:52.188717 amin_qvm-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:52.119039 amin_qvm-1.0.2/amin_qvm/
--rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.2/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.2/amin_qvm/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.2/amin_qvm/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:02:52.185168 amin_qvm-1.0.2/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     6047 2023-06-14 13:02:51.000000 amin_qvm-1.0.2/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-14 13:02:51.000000 amin_qvm-1.0.2/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:02:51.000000 amin_qvm-1.0.2/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-06-14 13:02:51.000000 amin_qvm-1.0.2/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 13:02:51.000000 amin_qvm-1.0.2/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 13:02:52.191252 amin_qvm-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-06-14 13:02:36.000000 amin_qvm-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:20:28.149362 amin_qvm-1.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.3/LICENSE.ttxt
+-rw-rw-rw-   0        0        0     6043 2023-06-14 13:20:28.146317 amin_qvm-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 13:20:28.022304 amin_qvm-1.0.3/amin_qvm/
+-rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.3/amin_qvm/QuantumComputer.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.3/amin_qvm/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.3/amin_qvm/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:20:28.135717 amin_qvm-1.0.3/amin_qvm.egg-info/
+-rw-rw-rw-   0        0        0     6043 2023-06-14 13:20:27.000000 amin_qvm-1.0.3/amin_qvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-14 13:20:27.000000 amin_qvm-1.0.3/amin_qvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:20:27.000000 amin_qvm-1.0.3/amin_qvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-14 13:20:27.000000 amin_qvm-1.0.3/amin_qvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 13:20:27.000000 amin_qvm-1.0.3/amin_qvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:20:28.151407 amin_qvm-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-06-14 13:20:22.000000 amin_qvm-1.0.3/setup.py
```

### Comparing `amin_qvm-1.0.2/LICENSE.ttxt` & `amin_qvm-1.0.3/LICENSE.ttxt`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.2/PKG-INFO` & `amin_qvm-1.0.3/amin_qvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: amin_qvm
-Version: 1.0.2
+Name: amin-qvm
+Version: 1.0.3
 Summary: Amin-QVM: Quantum Computing Library
-Home-page: https://github.com/your-username/amin-qvm
+Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.4
 License-File: LICENSE.ttxt
 
 This awesome code allows you to run some mind-boggling quantum stuff that you get from the Quantum Composer. It's all about playing with qubits, gates, and measurements, just like the pros do. You can do cool things like checking out the available qubits, applying gates, and even measuring the results.
 
 You won't believe it, but this code supports 100% of the examples from the IBM tutorial. Yep, every single one. And it's not just limited to that. There are tons of additional tests and examples that you can explore. The whole implementation is pretty compact too, with only 675 lines of code for the 5-qubit quantum computer simulator. Plus, there are twice as many lines dedicated to test programs and examples.
 
 To give you a taste of what you can do, check out this example. You can create a quantum computer object, write some mind-bending code in the Quantum Composer style, and execute it. In this case, we're creating a super cool GHZ state:
```

### Comparing `amin_qvm-1.0.2/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.3/amin_qvm/QuantumComputer.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.2/amin_qvm/functions.py` & `amin_qvm-1.0.3/amin_qvm/functions.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.2/amin_qvm.egg-info/PKG-INFO` & `amin_qvm-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: amin-qvm
-Version: 1.0.2
+Name: amin_qvm
+Version: 1.0.3
 Summary: Amin-QVM: Quantum Computing Library
-Home-page: https://github.com/your-username/amin-qvm
+Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.4
 License-File: LICENSE.ttxt
 
 This awesome code allows you to run some mind-boggling quantum stuff that you get from the Quantum Composer. It's all about playing with qubits, gates, and measurements, just like the pros do. You can do cool things like checking out the available qubits, applying gates, and even measuring the results.
 
 You won't believe it, but this code supports 100% of the examples from the IBM tutorial. Yep, every single one. And it's not just limited to that. There are tons of additional tests and examples that you can explore. The whole implementation is pretty compact too, with only 675 lines of code for the 5-qubit quantum computer simulator. Plus, there are twice as many lines dedicated to test programs and examples.
 
 To give you a taste of what you can do, check out this example. You can create a quantum computer object, write some mind-bending code in the Quantum Composer style, and execute it. In this case, we're creating a super cool GHZ state:
```

### Comparing `amin_qvm-1.0.2/setup.py` & `amin_qvm-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,32 +13,33 @@
     'random',
     'itertools',
     'functools',
     'math',
     'time',
     'qiskit',
     'pennylane',
-    'scikit-learn'
+    'scikit-learn',
+    'unittest'
 ]
 setup(
     name='amin_qvm',
-    version='1.0.2',
+    version='1.0.3',
     author='Amin Alogaili',
     author_email='aminalogai@gmail.com',
     description='Amin-QVM: Quantum Computing Library',
     long_description=long_description,
-    url='https://github.com/your-username/amin-qvm',
+    url='https://github.com/amin1029384756/QVM',
     packages=['amin_qvm'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     keywords='quantum computing library simulation amin alogaili QVM aminalogaili',
     install_requires=REQUIREMENTS,
-    python_requires='>=3.6',
+    python_requires='>=3.4',
 )
```

