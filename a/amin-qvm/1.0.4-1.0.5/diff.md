# Comparing `tmp/amin_qvm-1.0.4.tar.gz` & `tmp/amin_qvm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amin_qvm-1.0.4.tar", last modified: Wed Jun 14 13:25:13 2023, max compression
+gzip compressed data, was "amin_qvm-1.0.5.tar", last modified: Wed Jun 14 13:28:10 2023, max compression
```

## Comparing `amin_qvm-1.0.4.tar` & `amin_qvm-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:25:13.629774 amin_qvm-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.4/LICENSE.ttxt
--rw-rw-rw-   0        0        0     6043 2023-06-14 13:25:13.628568 amin_qvm-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 13:25:13.555606 amin_qvm-1.0.4/amin_qvm/
--rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.4/amin_qvm/QuantumComputer.py
--rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.4/amin_qvm/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.4/amin_qvm/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:25:13.623458 amin_qvm-1.0.4/amin_qvm.egg-info/
--rw-rw-rw-   0        0        0     6043 2023-06-14 13:25:13.000000 amin_qvm-1.0.4/amin_qvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-14 13:25:13.000000 amin_qvm-1.0.4/amin_qvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:25:13.000000 amin_qvm-1.0.4/amin_qvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-14 13:25:13.000000 amin_qvm-1.0.4/amin_qvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 13:25:13.000000 amin_qvm-1.0.4/amin_qvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 13:25:13.630783 amin_qvm-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-14 13:24:43.000000 amin_qvm-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.470252 amin_qvm-1.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-14 10:51:44.000000 amin_qvm-1.0.5/LICENSE.ttxt
+-rw-rw-rw-   0        0        0     6043 2023-06-14 13:28:10.469256 amin_qvm-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.418693 amin_qvm-1.0.5/amin_qvm/
+-rw-rw-rw-   0        0        0    89322 2023-06-14 11:39:44.000000 amin_qvm-1.0.5/amin_qvm/QuantumComputer.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 11:00:38.000000 amin_qvm-1.0.5/amin_qvm/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-14 12:36:27.000000 amin_qvm-1.0.5/amin_qvm/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:28:10.466256 amin_qvm-1.0.5/amin_qvm.egg-info/
+-rw-rw-rw-   0        0        0     6043 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 13:28:10.000000 amin_qvm-1.0.5/amin_qvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 13:28:10.474276 amin_qvm-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-06-14 13:28:06.000000 amin_qvm-1.0.5/setup.py
```

### Comparing `amin_qvm-1.0.4/LICENSE.ttxt` & `amin_qvm-1.0.5/LICENSE.ttxt`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.4/PKG-INFO` & `amin_qvm-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin_qvm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `amin_qvm-1.0.4/amin_qvm/QuantumComputer.py` & `amin_qvm-1.0.5/amin_qvm/QuantumComputer.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.4/amin_qvm/functions.py` & `amin_qvm-1.0.5/amin_qvm/functions.py`

 * *Files identical despite different names*

### Comparing `amin_qvm-1.0.4/amin_qvm.egg-info/PKG-INFO` & `amin_qvm-1.0.5/amin_qvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amin-qvm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Amin-QVM: Quantum Computing Library
 Home-page: https://github.com/amin1029384756/QVM
 Author: Amin Alogaili
 Author-email: aminalogai@gmail.com
 Keywords: quantum computing library simulation amin alogaili QVM aminalogaili
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `amin_qvm-1.0.4/setup.py` & `amin_qvm-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 with open('DESCRIPTION.rst') as file:
 	long_description = file.read()
 
 
 # specify requirements of your package here
 REQUIREMENTS = [
     'numpy',
-    'itertools',
-    'functools',
     'qiskit',
     'pennylane',
     'scikit-learn',
 ]
 setup(
     name='amin_qvm',
-    version='1.0.4',
+    version='1.0.5',
     author='Amin Alogaili',
     author_email='aminalogai@gmail.com',
     description='Amin-QVM: Quantum Computing Library',
     long_description=long_description,
     url='https://github.com/amin1029384756/QVM',
     packages=['amin_qvm'],
     classifiers=[
```

