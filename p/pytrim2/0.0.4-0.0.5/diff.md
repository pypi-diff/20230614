# Comparing `tmp/pytrim2-0.0.4.tar.gz` & `tmp/pytrim2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrim2-0.0.4.tar", last modified: Wed Sep 14 01:05:55 2022, max compression
+gzip compressed data, was "pytrim2-0.0.5.tar", last modified: Wed Jun 14 01:49:22 2023, max compression
```

## Comparing `pytrim2-0.0.4.tar` & `pytrim2-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-09-14 01:05:55.640809 pytrim2-0.0.4/
--rw-rw-r--   0 jovyan    (1000) users      (100)    11337 2022-09-05 16:31:43.000000 pytrim2-0.0.4/LICENSE
--rw-rw-r--   0 jovyan    (1000) users      (100)      111 2022-09-05 16:31:43.000000 pytrim2-0.0.4/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     1180 2022-09-14 01:05:55.640809 pytrim2-0.0.4/PKG-INFO
--rw-rw-r--   0 jovyan    (1000) users      (100)      393 2022-09-13 22:33:34.000000 pytrim2-0.0.4/README.md
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-09-14 01:05:55.630809 pytrim2-0.0.4/pytrim2/
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2022-09-14 01:05:36.000000 pytrim2-0.0.4/pytrim2/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1273 2022-09-14 01:05:36.000000 pytrim2-0.0.4/pytrim2/_modidx.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4649 2022-09-14 01:05:36.000000 pytrim2-0.0.4/pytrim2/demultiplex.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-09-14 01:05:55.640809 pytrim2-0.0.4/pytrim2.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1180 2022-09-14 01:05:54.000000 pytrim2-0.0.4/pytrim2.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      331 2022-09-14 01:05:55.000000 pytrim2-0.0.4/pytrim2.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-09-14 01:05:55.000000 pytrim2-0.0.4/pytrim2.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       36 2022-09-14 01:05:55.000000 pytrim2-0.0.4/pytrim2.egg-info/entry_points.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-09-13 22:05:57.000000 pytrim2-0.0.4/pytrim2.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       23 2022-09-14 01:05:55.000000 pytrim2-0.0.4/pytrim2.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        8 2022-09-14 01:05:55.000000 pytrim2-0.0.4/pytrim2.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      916 2022-09-14 01:05:26.000000 pytrim2-0.0.4/settings.ini
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2022-09-14 01:05:55.640809 pytrim2-0.0.4/setup.cfg
--rw-rw-r--   0 jovyan    (1000) users      (100)     2541 2022-09-05 16:31:43.000000 pytrim2-0.0.4/setup.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 01:49:22.181845 pytrim2-0.0.5/
+-rw-r--r--   0 jovyan    (1000) users      (100)    11337 2023-06-13 23:48:31.000000 pytrim2-0.0.5/LICENSE
+-rw-r--r--   0 jovyan    (1000) users      (100)      111 2023-06-13 23:48:31.000000 pytrim2-0.0.5/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     1180 2023-06-14 01:49:22.181845 pytrim2-0.0.5/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      393 2023-06-13 23:48:31.000000 pytrim2-0.0.5/README.md
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 01:49:22.181845 pytrim2-0.0.5/pytrim2/
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 01:49:06.000000 pytrim2-0.0.5/pytrim2/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1361 2023-06-14 01:49:06.000000 pytrim2-0.0.5/pytrim2/_modidx.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4664 2023-06-14 01:49:06.000000 pytrim2-0.0.5/pytrim2/demultiplex.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 01:49:22.181845 pytrim2-0.0.5/pytrim2.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1180 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      331 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       36 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 01:41:27.000000 pytrim2-0.0.5/pytrim2.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)       23 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        8 2023-06-14 01:49:22.000000 pytrim2-0.0.5/pytrim2.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      916 2023-06-14 01:48:54.000000 pytrim2-0.0.5/settings.ini
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 01:49:22.181845 pytrim2-0.0.5/setup.cfg
+-rw-r--r--   0 jovyan    (1000) users      (100)     2541 2023-06-13 23:48:31.000000 pytrim2-0.0.5/setup.py
```

### Comparing `pytrim2-0.0.4/LICENSE` & `pytrim2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrim2-0.0.4/PKG-INFO` & `pytrim2-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrim2
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python program to trim and demultiplex nanopore reads
 Home-page: https://github.com/hcstubbe/pytrim2
 Author: hcstubbe
 Author-email: hstubbe@med.lmu.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrim2-0.0.4/pytrim2/_modidx.py` & `pytrim2-0.0.5/pytrim2/_modidx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'master',
                 'doc_baseurl': '/pytrim2',
                 'doc_host': 'https://hcstubbe.github.io',
                 'git_url': 'https://github.com/hcstubbe/pytrim2',
                 'lib_path': 'pytrim2'},
-  'syms': { 'pytrim2.demultiplex': { 'pytrim2.demultiplex.align_barcodes': ('demultiplex.html#align_barcodes', 'pytrim2/demultiplex.py'),
+  'syms': { 'pytrim2.demultiplex': { 'pytrim2.demultiplex.align_barcodes_mp': ( 'demultiplex.html#align_barcodes_mp',
+                                                                                'pytrim2/demultiplex.py'),
                                      'pytrim2.demultiplex.decide_barcode_id': ( 'demultiplex.html#decide_barcode_id',
                                                                                 'pytrim2/demultiplex.py'),
                                      'pytrim2.demultiplex.demultiplex': ('demultiplex.html#demultiplex', 'pytrim2/demultiplex.py'),
                                      'pytrim2.demultiplex.findAlingments': ('demultiplex.html#findalingments', 'pytrim2/demultiplex.py'),
                                      'pytrim2.demultiplex.sort_records_to_file': ( 'demultiplex.html#sort_records_to_file',
                                                                                    'pytrim2/demultiplex.py'),
-                                     'pytrim2.demultiplex.trim_record': ('demultiplex.html#trim_record', 'pytrim2/demultiplex.py')}}}
+                                     'pytrim2.demultiplex.trim_record': ('demultiplex.html#trim_record', 'pytrim2/demultiplex.py')}}}
```

### Comparing `pytrim2-0.0.4/pytrim2/demultiplex.py` & `pytrim2-0.0.5/pytrim2/demultiplex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../00_demultiplex.ipynb.
 
 # %% auto 0
-__all__ = ['findAlingments', 'align_barcodes', 'decide_barcode_id', 'trim_record', 'sort_records_to_file', 'demultiplex']
+__all__ = ['findAlingments', 'align_barcodes_mp', 'decide_barcode_id', 'trim_record', 'sort_records_to_file', 'demultiplex']
 
 # %% ../00_demultiplex.ipynb 3
 from Bio import SeqIO
 from Bio import Align
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
+import multiprocessing as mp
+from multiprocessing.pool import ThreadPool
 import numpy as np
 
 # %% ../00_demultiplex.ipynb 4
 def findAlingments(seq_record, primer_dict, inward_end, max_alignments):
     "Find alignments for each primer in a sequence record"
   
     primer_keys = list(primer_dict.keys())
@@ -24,15 +26,14 @@
 
     n_sequences = len(primer_keys)
 
     array_cols = max_alignments + 3
     al_array = np.zeros( (n_sequences, array_cols) )
 
     for i in list(range(0, n_sequences, 1)):
-        print(primer_keys[i])
         al = []
         seq = primer_dict[primer_keys[i]].seq        
         alignments = aligner.align(seq_record[0:inward_end], seq)
         len_alignments = len(alignments)
         if(len_alignments <= max_alignments):
             score = alignments.score
             al = [j.aligned for j in alignments]
@@ -43,26 +44,23 @@
             al_array[i, -3] = max(al) # maximum posistion of each alignment
             al_array[i, -2] = len_alignments # number of alingments
             al_array[i, -1] = np.around(alignments.score/len(seq)*100, 0) # normalized local alingnment score
             
     return(al_array)
 
 # %% ../00_demultiplex.ipynb 6
-def align_barcodes(primer_dict, record_dict, inward_end, max_alignments):
-    "Aligne all barcodes in a list of seq records"
+def align_barcodes_mp(primer_dict, record_dict, inward_end, max_alignments):
+    "Aligne all barcodes in a list of seq records using multiprocessing"
 
     record_keys = list(record_dict.keys())
-    n_sequences = len(record_keys)
-    
-    alingments = list( range(0, n_sequences) )
-    for i in list(range(0, n_sequences, 1)):
-        print(record_keys[i])
-        seq_i = record_dict[record_keys[i]].seq
+    n_sequences = len(record_keys)   
+
+    with ThreadPool() as pool:
+        alingments = pool.starmap(findAlingments, [(record_dict[record_keys[i]].seq, primer_dict, inward_end, max_alignments) for i in list(range(0, n_sequences, 1))])
     
-        alingments[i] = findAlingments(seq_i, primer_dict, inward_end, max_alignments)
     return(alingments)
 
 # %% ../00_demultiplex.ipynb 9
 def decide_barcode_id(alginment_arrays):
     "Decide which barcode is best hit; remove if tie"
     
     id_array = np.zeros((np.shape(alginment_arrays)[0],3), dtype=np.int64)
@@ -112,11 +110,11 @@
     print("Create barcode dictionary")
     primer_dict = SeqIO.index(primer_file, primer_file_type)
     
     print("Create sequence dictionary")
     record_dict = SeqIO.index(input_file, input_file_type)
     
     print("Align barcodes")
-    alginment_arrays = align_barcodes(primer_dict, record_dict, max_distance, max_alignments)
+    alginment_arrays = align_barcodes_mp(primer_dict, record_dict, max_distance, max_alignments)
     
     print("Sort records to file")
     sort_records_to_file(record_dict, primer_dict, output_folder, alginment_arrays, input_file_type)
```

### Comparing `pytrim2-0.0.4/pytrim2.egg-info/PKG-INFO` & `pytrim2-0.0.5/pytrim2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrim2
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python program to trim and demultiplex nanopore reads
 Home-page: https://github.com/hcstubbe/pytrim2
 Author: hcstubbe
 Author-email: hstubbe@med.lmu.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrim2-0.0.4/settings.ini` & `pytrim2-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pytrim2
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pytrim2
 nbs_path = .
```

### Comparing `pytrim2-0.0.4/setup.py` & `pytrim2-0.0.5/setup.py`

 * *Files identical despite different names*

