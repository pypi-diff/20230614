# Comparing `tmp/p3bamboo-1.0.7.tar.gz` & `tmp/p3bamboo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3bamboo-1.0.7.tar", last modified: Sat Oct 15 07:49:11 2022, max compression
+gzip compressed data, was "p3bamboo-1.0.9.tar", last modified: Wed Jun 14 11:40:03 2023, max compression
```

## Comparing `p3bamboo-1.0.7.tar` & `p3bamboo-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-15 07:49:11.461774 p3bamboo-1.0.7/
--rw-rw-rw-   0        0        0     1549 2020-10-16 18:55:29.000000 p3bamboo-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1446 2022-10-15 07:49:11.460776 p3bamboo-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2020-10-16 19:17:09.000000 p3bamboo-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-10-15 07:49:11.456774 p3bamboo-1.0.7/p3bamboo/
--rw-rw-rw-   0        0        0      874 2020-10-16 19:32:38.000000 p3bamboo-1.0.7/p3bamboo/BamFactory.py
--rw-rw-rw-   0        0        0    13001 2022-10-15 07:48:06.000000 p3bamboo-1.0.7/p3bamboo/BamFile.py
--rw-rw-rw-   0        0        0     1093 2020-11-07 00:02:05.000000 p3bamboo-1.0.7/p3bamboo/BamGlobals.py
--rw-rw-rw-   0        0        0     1634 2020-11-07 00:02:47.000000 p3bamboo-1.0.7/p3bamboo/BamObject.py
--rw-rw-rw-   0        0        0        0 2020-09-28 08:53:27.000000 p3bamboo-1.0.7/p3bamboo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-15 07:49:11.459773 p3bamboo-1.0.7/p3bamboo.egg-info/
--rw-rw-rw-   0        0        0     1446 2022-10-15 07:49:11.000000 p3bamboo-1.0.7/p3bamboo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2022-10-15 07:49:11.000000 p3bamboo-1.0.7/p3bamboo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-15 07:49:11.000000 p3bamboo-1.0.7/p3bamboo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-10-15 07:49:11.000000 p3bamboo-1.0.7/p3bamboo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-15 07:49:11.461774 p3bamboo-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      607 2022-10-15 07:48:12.000000 p3bamboo-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:40:03.631608 p3bamboo-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-14 11:40:03.631608 p3bamboo-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:40:03.631608 p3bamboo-1.0.9/p3bamboo/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/BamFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/BamFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/BamGlobals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/BamObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/StructDatagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/p3bamboo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:40:03.631608 p3bamboo-1.0.9/p3bamboo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-14 11:40:03.000000 p3bamboo-1.0.9/p3bamboo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 11:40:03.000000 p3bamboo-1.0.9/p3bamboo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:40:03.000000 p3bamboo-1.0.9/p3bamboo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 11:40:03.000000 p3bamboo-1.0.9/p3bamboo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:40:03.631608 p3bamboo-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-14 11:39:54.000000 p3bamboo-1.0.9/setup.py
```

### Comparing `p3bamboo-1.0.7/LICENSE` & `p3bamboo-1.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, Derzsi Dániel
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors
-   may be used to endorse or promote products derived from this software
-   without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+BSD 3-Clause License
+
+Copyright (c) 2020, Derzsi Dániel
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software
+   without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `p3bamboo-1.0.7/PKG-INFO` & `p3bamboo-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: p3bamboo
-Version: 1.0.7
-Summary: Panda3D BAM file parser library
-Home-page: https://github.com/darktohka/p3bamboo
-Author: darktohka
-Author-email: daniel@tohka.us
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-p3bamboo
-========
-
-[![PyPI version](https://img.shields.io/pypi/v/p3bamboo.svg)](https://pypi.python.org/pypi/p3bamboo/)
-
-p3bamboo is a Python library that gives you full access to a Panda3D BAM file's inner structure.
-
-# Getting Started
-
-Simply install p3bamboo using `pip`:
-
-```bash
-python -m pip install p3bamboo
-```
-
-Loading a BAM file is very simple:
-
-```python
-from p3bamboo.BamFile import BamFile
-
-bam = BamFile()
-
-with open('myModel.bam', 'rb') as f:
-    bam.load(f)
-```
-
-Writing out a BAM file is also easy:
-
-```python
-with open('newModel.bam', 'wb') as f:
-    bam.write(f)
-```
-
-To automatically deserialize BAM objects, you must register your own custom BAM object types. For example, to register an object type named `Texture`:
-
-```python
-from p3bamboo.BamFactory import BamFactory
-from myproject.Texture import Texture
-
-BamFactory.register_type('Texture', Texture)
-```
-
-If you register your object types properly and load a BAM file afterwards, you'll be able to access your objects using `bam.object_map`.
+Metadata-Version: 2.1
+Name: p3bamboo
+Version: 1.0.9
+Summary: Panda3D BAM file parser library
+Home-page: https://github.com/darktohka/p3bamboo
+Author: darktohka
+Author-email: daniel@tohka.us
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+p3bamboo
+========
+
+[![PyPI version](https://img.shields.io/pypi/v/p3bamboo.svg)](https://pypi.python.org/pypi/p3bamboo/)
+
+p3bamboo is a Python library that gives you full access to a Panda3D BAM file's inner structure.
+
+# Getting Started
+
+Simply install p3bamboo using `pip`:
+
+```bash
+python -m pip install p3bamboo
+```
+
+Loading a BAM file is very simple:
+
+```python
+from p3bamboo.BamFile import BamFile
+
+bam = BamFile()
+
+with open('myModel.bam', 'rb') as f:
+    bam.load(f)
+```
+
+Writing out a BAM file is also easy:
+
+```python
+with open('newModel.bam', 'wb') as f:
+    bam.write(f)
+```
+
+To automatically deserialize BAM objects, you must register your own custom BAM object types. For example, to register an object type named `Texture`:
+
+```python
+from p3bamboo.BamFactory import BamFactory
+from myproject.Texture import Texture
+
+BamFactory.register_type('Texture', Texture)
+```
+
+If you register your object types properly and load a BAM file afterwards, you'll be able to access your objects using `bam.object_map`.
```

### Comparing `p3bamboo-1.0.7/p3bamboo/BamFactory.py` & `p3bamboo-1.0.9/p3bamboo/BamFactory.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""
-  P3BAMBOO
-  Panda3D BAM file library
-
-  Author: Disyer
-  Date: 2020/10/16
-"""
-class BamFactory(object):
-    types = {}
-
-    @staticmethod
-    def register_type(handle_name, handle_type):
-        if handle_name in BamFactory.types:
-            raise Exception('Type {0} has already been registered.'.format(handle_name))
-
-        BamFactory.types[handle_name] = handle_type
-
-    @staticmethod
-    def unregister_type(handle_name):
-        if handle_name not in BamFactory.types:
-            raise Exception('Type {0} has not been registered yet.'.format(handle_name))
-
-        del BamFactory.types[handle_name]
-
-    @staticmethod
-    def create(bam_file, version, *handle_names):
-        for handle_name in handle_names:
-            if handle_name in BamFactory.types:
-                return BamFactory.types[handle_name](bam_file, version)
+"""
+  P3BAMBOO
+  Panda3D BAM file library
+
+  Author: Disyer
+  Date: 2020/10/16
+"""
+class BamFactory(object):
+    types = {}
+
+    @staticmethod
+    def register_type(handle_name, handle_type):
+        if handle_name in BamFactory.types:
+            raise Exception('Type {0} has already been registered.'.format(handle_name))
+
+        BamFactory.types[handle_name] = handle_type
+
+    @staticmethod
+    def unregister_type(handle_name):
+        if handle_name not in BamFactory.types:
+            raise Exception('Type {0} has not been registered yet.'.format(handle_name))
+
+        del BamFactory.types[handle_name]
+
+    @staticmethod
+    def create(bam_file, version, *handle_names):
+        for handle_name in handle_names:
+            if handle_name in BamFactory.types:
+                return BamFactory.types[handle_name](bam_file, version)
```

### Comparing `p3bamboo-1.0.7/p3bamboo.egg-info/PKG-INFO` & `p3bamboo-1.0.9/p3bamboo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: p3bamboo
-Version: 1.0.7
-Summary: Panda3D BAM file parser library
-Home-page: https://github.com/darktohka/p3bamboo
-Author: darktohka
-Author-email: daniel@tohka.us
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-p3bamboo
-========
-
-[![PyPI version](https://img.shields.io/pypi/v/p3bamboo.svg)](https://pypi.python.org/pypi/p3bamboo/)
-
-p3bamboo is a Python library that gives you full access to a Panda3D BAM file's inner structure.
-
-# Getting Started
-
-Simply install p3bamboo using `pip`:
-
-```bash
-python -m pip install p3bamboo
-```
-
-Loading a BAM file is very simple:
-
-```python
-from p3bamboo.BamFile import BamFile
-
-bam = BamFile()
-
-with open('myModel.bam', 'rb') as f:
-    bam.load(f)
-```
-
-Writing out a BAM file is also easy:
-
-```python
-with open('newModel.bam', 'wb') as f:
-    bam.write(f)
-```
-
-To automatically deserialize BAM objects, you must register your own custom BAM object types. For example, to register an object type named `Texture`:
-
-```python
-from p3bamboo.BamFactory import BamFactory
-from myproject.Texture import Texture
-
-BamFactory.register_type('Texture', Texture)
-```
-
-If you register your object types properly and load a BAM file afterwards, you'll be able to access your objects using `bam.object_map`.
+Metadata-Version: 2.1
+Name: p3bamboo
+Version: 1.0.9
+Summary: Panda3D BAM file parser library
+Home-page: https://github.com/darktohka/p3bamboo
+Author: darktohka
+Author-email: daniel@tohka.us
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+p3bamboo
+========
+
+[![PyPI version](https://img.shields.io/pypi/v/p3bamboo.svg)](https://pypi.python.org/pypi/p3bamboo/)
+
+p3bamboo is a Python library that gives you full access to a Panda3D BAM file's inner structure.
+
+# Getting Started
+
+Simply install p3bamboo using `pip`:
+
+```bash
+python -m pip install p3bamboo
+```
+
+Loading a BAM file is very simple:
+
+```python
+from p3bamboo.BamFile import BamFile
+
+bam = BamFile()
+
+with open('myModel.bam', 'rb') as f:
+    bam.load(f)
+```
+
+Writing out a BAM file is also easy:
+
+```python
+with open('newModel.bam', 'wb') as f:
+    bam.write(f)
+```
+
+To automatically deserialize BAM objects, you must register your own custom BAM object types. For example, to register an object type named `Texture`:
+
+```python
+from p3bamboo.BamFactory import BamFactory
+from myproject.Texture import Texture
+
+BamFactory.register_type('Texture', Texture)
+```
+
+If you register your object types properly and load a BAM file afterwards, you'll be able to access your objects using `bam.object_map`.
```

### Comparing `p3bamboo-1.0.7/setup.py` & `p3bamboo-1.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import setuptools
-
-with open('README.md', 'r') as f:
-    long_description = f.read()
-
-setuptools.setup(
-    name='p3bamboo',
-    version='1.0.7',
-    author='darktohka',
-    author_email='daniel@tohka.us',
-    description='Panda3D BAM file parser library',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/darktohka/p3bamboo',
-    packages=setuptools.find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-)
+import setuptools
+
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
+setuptools.setup(
+    name='p3bamboo',
+    version='1.0.9',
+    author='darktohka',
+    author_email='daniel@tohka.us',
+    description='Panda3D BAM file parser library',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/darktohka/p3bamboo',
+    packages=setuptools.find_packages(),
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.6',
+)
```

