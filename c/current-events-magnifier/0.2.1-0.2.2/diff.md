# Comparing `tmp/current_events_magnifier-0.2.1.tar.gz` & `tmp/current_events_magnifier-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "current_events_magnifier-0.2.1.tar", last modified: Wed Jun 14 11:02:01 2023, max compression
+gzip compressed data, was "dist/current_events_magnifier-0.2.2.tar", last modified: Wed Jun 14 11:08:04 2023, max compression
```

## Comparing `current_events_magnifier-0.2.1.tar` & `current_events_magnifier-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6043 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5396 2023-06-14 11:01:23.000000 current_events_magnifier-0.2.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/current_events_magnifier/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       95 2023-06-14 10:43:38.000000 current_events_magnifier-0.2.1/current_events_magnifier/__init__.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5807 2023-06-14 11:01:09.000000 current_events_magnifier-0.2.1/current_events_magnifier/magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.1/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.2.1/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.1/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.1/current_events_magnifier/read_tombo_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.1/current_events_magnifier/utils.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6043 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      547 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1039 2023-06-14 11:01:44.000000 current_events_magnifier-0.2.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:08:04.740169 current_events_magnifier-0.2.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6006 2023-06-14 11:08:04.740169 current_events_magnifier-0.2.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5396 2023-06-14 11:01:23.000000 current_events_magnifier-0.2.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:08:04.740169 current_events_magnifier-0.2.2/current_events_magnifier/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       95 2023-06-14 10:43:38.000000 current_events_magnifier-0.2.2/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.2/current_events_magnifier/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5833 2023-06-14 11:06:46.000000 current_events_magnifier-0.2.2/current_events_magnifier/magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.2/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.2.2/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.2/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.2/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:08:04.740169 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6006 2023-06-14 11:08:04.000000 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      551 2023-06-14 11:08:04.000000 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 11:08:04.000000 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 11:08:04.000000 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 11:08:04.000000 current_events_magnifier-0.2.2/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 11:08:04.740169 current_events_magnifier-0.2.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1039 2023-06-14 11:07:43.000000 current_events_magnifier-0.2.2/setup.py
```

### Comparing `current_events_magnifier-0.2.1/LICENSE` & `current_events_magnifier-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/PKG-INFO` & `current_events_magnifier-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,9 +124,7 @@
 
 ```
 
 
 
 
 
-
-
```

### Comparing `current_events_magnifier-0.2.1/README.md` & `current_events_magnifier-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/magnifier.py` & `current_events_magnifier-0.2.2/current_events_magnifier/magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+#!/usr/bin/env python
 import argparse
 import os
-from current_events_magnifier.utils import read_fasta_to_dic,reverse_fasta
+from current_events_magnifier.cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
 from current_events_magnifier.plot import signal_plot
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
```

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/normalization.py` & `current_events_magnifier-0.2.2/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/plot.py` & `current_events_magnifier-0.2.2/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.2.2/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.2.2/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier/utils.py` & `current_events_magnifier-0.2.2/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.2.2/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,9 +124,7 @@
 
 ```
 
 
 
 
 
-
-
```

### Comparing `current_events_magnifier-0.2.1/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.2.2/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
 current_events_magnifier/__init__.py
+current_events_magnifier/cem_utils.py
 current_events_magnifier/magnifier.py
 current_events_magnifier/normalization.py
 current_events_magnifier/plot.py
 current_events_magnifier/read_f5c_resquiggle.py
 current_events_magnifier/read_tombo_resquiggle.py
-current_events_magnifier/utils.py
 current_events_magnifier.egg-info/PKG-INFO
 current_events_magnifier.egg-info/SOURCES.txt
 current_events_magnifier.egg-info/dependency_links.txt
 current_events_magnifier.egg-info/requires.txt
 current_events_magnifier.egg-info/top_level.txt
```

### Comparing `current_events_magnifier-0.2.1/setup.py` & `current_events_magnifier-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.2.1",
+    version="0.2.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

