# Comparing `tmp/save-thread-result-0.1.1.tar.gz` & `tmp/save-thread-result-0.1.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "save-thread-result-0.1.1.tar", last modified: Tue May 30 00:18:57 2023, max compression
+gzip compressed data, was "save-thread-result-0.1.1.post0.tar", last modified: Wed Jun 14 19:09:57 2023, max compression
```

## Comparing `save-thread-result-0.1.1.tar` & `save-thread-result-0.1.1.post0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.599896 save-thread-result-0.1.1/
--rw-r--r--   0 shail      (503) staff       (20)    19072 2023-05-30 00:18:57.599369 save-thread-result-0.1.1/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)     3981 2023-05-29 23:34:08.000000 save-thread-result-0.1.1/README.md
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.596168 save-thread-result-0.1.1/save_thread_result/
--rw-r--r--   0 shail      (503) staff       (20)    16023 2023-05-30 00:16:54.000000 save-thread-result-0.1.1/save_thread_result/__init__.py
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.598467 save-thread-result-0.1.1/save_thread_result.egg-info/
--rw-r--r--   0 shail      (503) staff       (20)    19072 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)      217 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/SOURCES.txt
--rw-r--r--   0 shail      (503) staff       (20)        1 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/dependency_links.txt
--rw-r--r--   0 shail      (503) staff       (20)       19 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/top_level.txt
--rw-r--r--   0 shail      (503) staff       (20)       38 2023-05-30 00:18:57.600051 save-thread-result-0.1.1/setup.cfg
--rw-r--r--   0 shail      (503) staff       (20)    19099 2023-05-30 00:16:54.000000 save-thread-result-0.1.1/setup.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.065144 save-thread-result-0.1.1.post0/
+-rw-r--r--   0 shail      (503) staff       (20)    19275 2023-06-14 19:09:57.064550 save-thread-result-0.1.1.post0/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)     3981 2023-05-29 23:34:08.000000 save-thread-result-0.1.1.post0/README.md
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.060766 save-thread-result-0.1.1.post0/save_thread_result/
+-rw-r--r--   0 shail      (503) staff       (20)    17141 2023-06-14 19:05:43.000000 save-thread-result-0.1.1.post0/save_thread_result/__init__.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.063642 save-thread-result-0.1.1.post0/save_thread_result.egg-info/
+-rw-r--r--   0 shail      (503) staff       (20)    19275 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)      217 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/SOURCES.txt
+-rw-r--r--   0 shail      (503) staff       (20)        1 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/dependency_links.txt
+-rw-r--r--   0 shail      (503) staff       (20)       19 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/top_level.txt
+-rw-r--r--   0 shail      (503) staff       (20)       38 2023-06-14 19:09:57.065366 save-thread-result-0.1.1.post0/setup.cfg
+-rw-r--r--   0 shail      (503) staff       (20)    19297 2023-06-14 19:05:43.000000 save-thread-result-0.1.1.post0/setup.py
```

### Comparing `save-thread-result-0.1.1/PKG-INFO` & `save-thread-result-0.1.1.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.1
+Version: 0.1.1.post0
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
-License: Apache License 2.0
+License: MIT License
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Project-URL: Pull requests, https://github.com/slow-but-steady/save-thread-result/pulls
 Project-URL: Issues, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: Code, https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Keywords: threading thread multi-threading logging logger archiving tracing tracer debugging debugger automation csv txt markdown md YouTube videos URL scraping Selenium macos windows linux
@@ -48,15 +48,20 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Free For Educational Use
+Classifier: License :: Free For Home Use
+Classifier: License :: Free for non-commercial use
+Classifier: License :: Freely Distributable
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Android
 Classifier: Operating System :: BeOS
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS 9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
```

### Comparing `save-thread-result-0.1.1/README.md` & `save-thread-result-0.1.1.post0/README.md`

 * *Files identical despite different names*

### Comparing `save-thread-result-0.1.1/save_thread_result/__init__.py` & `save-thread-result-0.1.1.post0/save_thread_result/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,43 @@
 '''
 Simple subclass wrapper around `threading.Thread` to get the return value
 from a thread in python. Exact same interface as `threading.Thread`!
 
 '''
+
+# MIT License
+#
+# Copyright (c) 2023 Shail Shouryya
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
 import sys
 import time
 import threading
 from datetime import datetime
 
 
-__version__              = '0.1.1'
+__version__              = '0.1.1.post0'
 
 
 _general_documentation = '''
     The `threading.Thread` subclass `ThreadWithResult` saves the result of a thread
     as its `result` attribute - i.e. call `thread_with_result_instance_1.result`
     after `thread_with_result_instance_1` finishes running to get the return
     value from the function that ran on that thread:
```

### Comparing `save-thread-result-0.1.1/save_thread_result.egg-info/PKG-INFO` & `save-thread-result-0.1.1.post0/save_thread_result.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.1
+Version: 0.1.1.post0
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
-License: Apache License 2.0
+License: MIT License
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Project-URL: Pull requests, https://github.com/slow-but-steady/save-thread-result/pulls
 Project-URL: Issues, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: Code, https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Keywords: threading thread multi-threading logging logger archiving tracing tracer debugging debugger automation csv txt markdown md YouTube videos URL scraping Selenium macos windows linux
@@ -48,15 +48,20 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Free For Educational Use
+Classifier: License :: Free For Home Use
+Classifier: License :: Free for non-commercial use
+Classifier: License :: Freely Distributable
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Android
 Classifier: Operating System :: BeOS
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: MacOS :: MacOS 9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
```

### Comparing `save-thread-result-0.1.1/setup.py` & `save-thread-result-0.1.1.post0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     # For new projects, the recommended versioning scheme is based on Semantic Versioning, but adopts a different approach to handling pre-releases and build metadata.
     # The essence of semantic versioning is a 3-part MAJOR.MINOR.MAINTENANCE numbering scheme, where the project author increments:
     # 1. MAJOR version when they make incompatible API changes,
     # 2. MINOR version when they add functionality in a backwards-compatible manner, and
     # 3. MAINTENANCE version when they make backwards-compatible bug fixes.
     # Adopting this approach as a project author allows users to make use of “compatible release” specifiers, where name ~= X.Y requires at least release X.Y, but also allows any later release with a matching MAJOR version.
     # Python projects adopting semantic versioning should abide by clauses 1-8 of the Semantic Versioning 2.0.0 specification: https://semver.org/.
-    version                       = '0.1.1',
+    version                       = '0.1.1.post0',
     name                          = 'save-thread-result',
     description                   = 'Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟',
     long_description              = long_description,
     long_description_content_type = 'text/markdown',
     url                           = 'https://github.com/slow-but-steady/save-thread-result/tree/main/python',
     author                        = 'slow-but-steady',
     author_email                  = 'slowbutsteady1234@gmail.com',
-    license                       = 'Apache License 2.0',
+    license                       = 'MIT License',
 
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: MacOS X',
         'Environment :: No Input/Output (Daemon)',
         'Environment :: OpenStack',
@@ -77,15 +77,20 @@
         'Intended Audience :: Healthcare Industry',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Legal Industry',
         'Intended Audience :: Manufacturing',
         'Intended Audience :: Science/Research',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Telecommunications Industry',
-        'License :: OSI Approved :: Apache Software License',
+        'License :: Free For Educational Use',
+        'License :: Free For Home Use',
+        'License :: Free for non-commercial use',
+        'License :: Freely Distributable',
+        'License :: Freeware',
+        'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: Android',
         'Operating System :: BeOS',
         'Operating System :: MacOS',
         'Operating System :: MacOS :: MacOS 9',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft',
```

