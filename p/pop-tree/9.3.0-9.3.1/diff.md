# Comparing `tmp/pop-tree-9.3.0.tar.gz` & `tmp/pop-tree-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-tree-9.3.0.tar", last modified: Wed Jun 15 17:11:28 2022, max compression
+gzip compressed data, was "pop-tree-9.3.1.tar", last modified: Thu Nov  3 21:17:40 2022, max compression
```

## Comparing `pop-tree-9.3.0.tar` & `pop-tree-9.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.762269 pop-tree-9.3.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2022-06-15 17:11:13.000000 pop-tree-9.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4607 2022-06-15 17:11:28.761353 pop-tree-9.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3973 2022-06-15 17:11:13.000000 pop-tree-9.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.760436 pop-tree-9.3.0/pop_doc/
--rw-r--r--   0 root         (0) root         (0)      281 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      161 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_doc/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.760436 pop-tree-9.3.0/pop_tree/
--rw-r--r--   0 root         (0) root         (0)     1014 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.761353 pop-tree-9.3.0/pop_tree/graph/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.761353 pop-tree-9.3.0/pop_tree/graph/contracts/
--rw-r--r--   0 root         (0) root         (0)      359 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      337 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/contracts/networkx.py
--rw-r--r--   0 root         (0) root         (0)     1090 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/init.py
--rw-r--r--   0 root         (0) root         (0)     4836 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/networkx.py
--rw-r--r--   0 root         (0) root         (0)      651 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/text_details.py
--rw-r--r--   0 root         (0) root         (0)     1000 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/text_json.py
--rw-r--r--   0 root         (0) root         (0)      943 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/graph/text_simple.py
--rw-r--r--   0 root         (0) root         (0)      157 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.761353 pop-tree-9.3.0/pop_tree/tree/
--rw-r--r--   0 root         (0) root         (0)     2206 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/tree/init.py
--rw-r--r--   0 root         (0) root         (0)     7633 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/tree/mod.py
--rw-r--r--   0 root         (0) root         (0)     1273 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/tree/ref.py
--rw-r--r--   0 root         (0) root         (0)     2364 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pop_tree/tree/sub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-15 17:11:28.760436 pop-tree-9.3.0/pop_tree.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4607 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      602 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-06-15 17:11:28.000000 pop-tree-9.3.0/pop_tree.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      255 2022-06-15 17:11:13.000000 pop-tree-9.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-15 17:11:28.762269 pop-tree-9.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2442 2022-06-15 17:11:13.000000 pop-tree-9.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.414927 pop-tree-9.3.1/
+-rw-r--r--   0 root         (0) root         (0)    11342 2022-11-03 21:17:19.000000 pop-tree-9.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5587 2022-11-03 21:17:40.414927 pop-tree-9.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4447 2022-11-03 21:17:19.000000 pop-tree-9.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.413094 pop-tree-9.3.1/pop_doc/
+-rw-r--r--   0 root         (0) root         (0)      281 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      161 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_doc/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.413094 pop-tree-9.3.1/pop_tree/
+-rw-r--r--   0 root         (0) root         (0)     1014 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.414010 pop-tree-9.3.1/pop_tree/graph/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.414010 pop-tree-9.3.1/pop_tree/graph/contracts/
+-rw-r--r--   0 root         (0) root         (0)      359 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      337 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/contracts/networkx.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/init.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/networkx.py
+-rw-r--r--   0 root         (0) root         (0)      651 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/text_details.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/text_json.py
+-rw-r--r--   0 root         (0) root         (0)      943 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/graph/text_simple.py
+-rw-r--r--   0 root         (0) root         (0)      157 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.414927 pop-tree-9.3.1/pop_tree/tree/
+-rw-r--r--   0 root         (0) root         (0)     2206 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/tree/init.py
+-rw-r--r--   0 root         (0) root         (0)     7633 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/tree/mod.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/tree/ref.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pop_tree/tree/sub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 21:17:40.414010 pop-tree-9.3.1/pop_tree.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5587 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      612 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-11-03 21:17:40.000000 pop-tree-9.3.1/pop_tree.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2022-11-03 21:17:19.000000 pop-tree-9.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-03 21:17:40.414927 pop-tree-9.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2998 2022-11-03 21:17:19.000000 pop-tree-9.3.1/setup.py
```

### Comparing `pop-tree-9.3.0/LICENSE` & `pop-tree-9.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 Tyler Johnson
+   Copyright 2021 VMware, Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pop-tree-9.3.0/PKG-INFO` & `pop-tree-9.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,55 @@
-Metadata-Version: 2.1
-Name: pop-tree
-Version: 9.3.0
-Summary: Visualize POP hub/sub structures
-Home-page: UNKNOWN
-Author: Tyler Johnson
-Author-email: tjohnson@saltstack.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: full
-Provides-Extra: networkx
-License-File: LICENSE
-
 ========
 pop-tree
 ========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
+.. image:: https://img.shields.io/badge/docs%20on-vmware.gitlab.io-blue
+   :alt: Documentation is published with Sphinx on GitLab Pages via vmware.gitlab.io
+   :target: https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html
+
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 **POP structure visualization tool**
 
 About
 =====
 
-asdf
+Visualize POP hub/sub structures with ``pop-tree``, and view embedded rst content
+with ``pop-doc``.
+
+* `pop-tree source code <https://gitlab.com/vmware/pop/pop-tree>`__
+* `pop-tree documentation <https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html>`__
 
 What is POP?
 ------------
 
 This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
 implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
 together concepts and wisdom from the history of computing in new ways to solve
 modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
-* `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
-* `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
+* `pop-awesome <https://gitlab.com/vmware/pop/pop-awesome>`__
+* `pop-create <https://gitlab.com/vmware/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.7+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
 
@@ -194,16 +181,14 @@
 Use these arguments together to create impressive visuals for your project.
 
 .. image:: hub.png
 
 Roadmap
 =======
 
-Reference the `open issues <https://gitlab.com/saltstack/pop/pop-tree/issues>`__ for a list of
+Reference the `open issues <https://gitlab.com/vmware/pop/pop-tree/issues>`__ for a list of
 proposed features (and known issues).
 
 Acknowledgements
 ================
 
 * `Img Shields <https://shields.io>`__ for making repository badges easy.
-
-
```

### Comparing `pop-tree-9.3.0/pop_tree/conf.py` & `pop-tree-9.3.1/pop_tree/conf.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/graph/init.py` & `pop-tree-9.3.1/pop_tree/graph/init.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/graph/networkx.py` & `pop-tree-9.3.1/pop_tree/graph/networkx.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/graph/text_details.py` & `pop-tree-9.3.1/pop_tree/graph/text_details.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/graph/text_json.py` & `pop-tree-9.3.1/pop_tree/graph/text_json.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/graph/text_simple.py` & `pop-tree-9.3.1/pop_tree/graph/text_simple.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/tree/init.py` & `pop-tree-9.3.1/pop_tree/tree/init.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/tree/mod.py` & `pop-tree-9.3.1/pop_tree/tree/mod.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/tree/ref.py` & `pop-tree-9.3.1/pop_tree/tree/ref.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree/tree/sub.py` & `pop-tree-9.3.1/pop_tree/tree/sub.py`

 * *Files identical despite different names*

### Comparing `pop-tree-9.3.0/pop_tree.egg-info/PKG-INFO` & `pop-tree-9.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,84 @@
 Metadata-Version: 2.1
 Name: pop-tree
-Version: 9.3.0
+Version: 9.3.1
 Summary: Visualize POP hub/sub structures
-Home-page: UNKNOWN
-Author: Tyler Johnson
-Author-email: tjohnson@saltstack.com
-License: UNKNOWN
+Home-page: https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html
+Author: VMware, Inc.
+Author-email: idemproject@vmware.com
+License: Apache Software License 2.0
+Project-URL: Code, https://gitlab.com/vmware/pop/pop-tree
+Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-tree/issues
 Platform: UNKNOWN
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: networkx
 License-File: LICENSE
 
 ========
 pop-tree
 ========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
+.. image:: https://img.shields.io/badge/docs%20on-vmware.gitlab.io-blue
+   :alt: Documentation is published with Sphinx on GitLab Pages via vmware.gitlab.io
+   :target: https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html
+
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
 **POP structure visualization tool**
 
 About
 =====
 
-asdf
+Visualize POP hub/sub structures with ``pop-tree``, and view embedded rst content
+with ``pop-doc``.
+
+* `pop-tree source code <https://gitlab.com/vmware/pop/pop-tree>`__
+* `pop-tree documentation <https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html>`__
 
 What is POP?
 ------------
 
 This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
 implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
 together concepts and wisdom from the history of computing in new ways to solve
 modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
-* `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
-* `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
+* `pop-awesome <https://gitlab.com/vmware/pop/pop-awesome>`__
+* `pop-create <https://gitlab.com/vmware/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.7+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
 
@@ -194,15 +210,15 @@
 Use these arguments together to create impressive visuals for your project.
 
 .. image:: hub.png
 
 Roadmap
 =======
 
-Reference the `open issues <https://gitlab.com/saltstack/pop/pop-tree/issues>`__ for a list of
+Reference the `open issues <https://gitlab.com/vmware/pop/pop-tree/issues>`__ for a list of
 proposed features (and known issues).
 
 Acknowledgements
 ================
 
 * `Img Shields <https://shields.io>`__ for making repository badges easy.
```

### Comparing `pop-tree-9.3.0/pop_tree.egg-info/SOURCES.txt` & `pop-tree-9.3.1/pop_tree.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.rst
 pyproject.toml
+setup.cfg
 setup.py
 pop_doc/conf.py
 pop_doc/scripts.py
 pop_tree/conf.py
 pop_tree/scripts.py
 pop_tree.egg-info/PKG-INFO
 pop_tree.egg-info/SOURCES.txt
```

### Comparing `pop-tree-9.3.0/setup.py` & `pop-tree-9.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 
 from setuptools import Command
 from setuptools import setup
 
 DESC = "Visualize POP hub/sub structures"
 
-VERSION = "9.3.0"
+VERSION = "9.3.1"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
@@ -55,31 +55,42 @@
             modname = pdir.replace(os.sep, ".")
             modules.append(modname)
     return modules
 
 
 setup(
     name="pop-tree",
-    author="Tyler Johnson",
-    author_email="tjohnson@saltstack.com",
-    url="",
+    author="VMware, Inc.",
+    author_email="idemproject@vmware.com",
+    url="https://vmware.gitlab.io/pop/pop-tree/en/latest/index.html",
+    project_urls={
+        "Code": "https://gitlab.com/vmware/pop/pop-tree",
+        "Issue tracker": "https://gitlab.com/vmware/pop/pop-tree/issues",
+    },
     version=VERSION,
-    extras_require=REQUIREMENTS_EXTRA,
     install_requires=REQUIREMENTS,
+    extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
+    license="Apache Software License 2.0",
     classifiers=[
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     entry_points={
         "console_scripts": [
             "pop-tree = pop_tree.scripts:start",
             "pop-doc = pop_doc.scripts:start",
         ]
```

