# Comparing `tmp/nanomonsv-0.5.1.tar.gz` & `tmp/nanomonsv-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomonsv-0.5.1.tar", last modified: Tue May  9 05:35:22 2023, max compression
+gzip compressed data, was "nanomonsv-0.6.0.tar", last modified: Wed Jun 14 10:11:09 2023, max compression
```

## Comparing `nanomonsv-0.5.1.tar` & `nanomonsv-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.134528 nanomonsv-0.5.1/nanomonsv/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/cluster_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20284 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/count_sread_by_alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/nanomonsv/data/
--rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/filt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/gather_support_read_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/generate_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/insert_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/locate_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/locate_bp_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/long_read_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/merge_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/my_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/post_proc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/pyssw.py
--rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/smith_waterman.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/ssw_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/swalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/vcf_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/nanomonsv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/nanomonsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 05:35:22.000000 nanomonsv-0.5.1/nanomonsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:35:22.138529 nanomonsv-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 05:35:06.000000 nanomonsv-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/cluster_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20284 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/count_sread_by_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/gather_support_read_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/generate_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/insert_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/locate_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/locate_bp_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/long_read_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/merge_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/my_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/post_proc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/pyssw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/smith_waterman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/ssw_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/swalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/vcf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/nanomonsv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/nanomonsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 10:11:09.000000 nanomonsv-0.6.0/nanomonsv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:11:09.711058 nanomonsv-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-14 10:10:58.000000 nanomonsv-0.6.0/setup.py
```

### Comparing `nanomonsv-0.5.1/LICENSE` & `nanomonsv-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/PKG-INFO` & `nanomonsv-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `nanomonsv-0.5.1/README.md` & `nanomonsv-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/arg_parser.py` & `nanomonsv-0.6.0/nanomonsv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/cluster.py` & `nanomonsv-0.6.0/nanomonsv/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                     control_panel_flag = True
 
         if control_flag == True or control_panel_flag == True: is_filter = True 
 
         return(is_filter)
 
     
-    def filter_indel_cluster(self, cl):
+    def filter_indel_cluster(self, cl, matched_control_margin = 0):
 
         is_filter = False
         # add breakpoint info
         if self.bp_tb is not None:
             tabix_error_flag1 = False
             try:
                 records = self.bp_tb.fetch(cl.chr1, max(0, cl.start1), cl.end2)
@@ -250,44 +250,57 @@
         median_mapQ1 = statistics.median([int(x.split(',')[5]) for x in cl.info1])
         if median_mapQ1 < self.median_mapQ_thres: is_filter = True
 
         # supporting read number of non secondary alignments
         non_secondary_readnum = len([x.split(',')[10] for x in cl.info1 if x.split(',')[10] == "False"])
         if non_secondary_readnum < self.read_num_thres: is_filter = True
 
+        median_size = statistics.median([int(x) for x in cl.size if x not in ['-', '+']])
+
+        # for indels whose size is below 300, there should be sufficient non-soft-clipping support reads
+        if median_size < 300 and len([int(x) for x in cl.size if x not in ['-', '+']]) < self.read_num_thres: 
+            is_filter = True
+        
         if is_filter == True: return(True)
 
 
-        median_size = statistics.median([int(x) for x in cl.size if x not in ['-', '+']]) 
+
 
         control_flag = False
         control_panel_flag = False
         if self.control_tb is not None:
 
+            control_read_num = 0
             tabix_error_flag2 = False
             try:
-                records = self.control_tb.fetch(cl.chr1, max(0, cl.start1 - 50), cl.end2 + 50)
+                records = self.control_tb.fetch(cl.chr1, max(0, cl.start1 - matched_control_margin), cl.end2 + matched_control_margin)
             except Exception as e: 
                 logger.debug(f'{e}')
                 tabix_error_flag2 = True
 
             if not tabix_error_flag2:
                 for record_line in records:
                     rec = record_line.split('\t')
 
                     """
                     if cl.chr1 == rec[0] and cl.start1 - self.control_check_margin <= int(rec[2]) and \
                         cl.end2 + self.control_check_margin >= int(rec[1]) and \
                         int(rec[4]) >= median_size * 0.5:
                     """
+                    
+                    """
                     if cl.chr1 == rec[0] and cl.start1 <= int(rec[1]) <= cl.end1 and \
                         cl.start2 <= int(rec[2]) <= cl.end2 and \
                         median_size * 0.75 <= int(rec[4]) <= median_size * 1.25:
+                    """
+                    if int(rec[4]) >= median_size * 0.5:
+                        control_read_num = control_read_num + 1
 
-                        control_flag = True
+            if control_read_num > self.max_control_read_num or float(control_read_num) / len(cl.readids) >= 0.2:
+                control_flag = True
 
 
         if self.control_panel_tb is not None:
     
             tabix_error_flag2 = False
             try:
                 records = self.control_panel_tb.fetch(cl.chr1, max(0, cl.start1 - 50), cl.end2 + 50)
@@ -341,15 +354,16 @@
         
                     print(f'{cl.chr1}\t{cl.start1}\t{cl.end1}\t{cl.chr2}\t{cl.start2}\t{cl.end2}\t' +
                         f'{print_line_readids}\t0\t{cl.dir1}\t{cl.dir2}\t{print_line_info1}\t{print_line_info2}',
                         file = self.hout)
 
                 elif self.svtype in ["insertion", "deletion"]:
 
-                    if self.filter_indel_cluster(cl): continue
+                    matched_control_margin_choice = 100 if self.svtype == "insertion" else 10
+                    if self.filter_indel_cluster(cl, matched_control_margin = matched_control_margin_choice): continue
                     print_line_readids = ';'.join(cl.readids)
                     print_line_size = ';'.join([str(x) for x in cl.size])
                     print_line_info1 = ';'.join(cl.info1)
 
                     print(f'{cl.chr1}\t{cl.start1}\t{cl.end1}\t{cl.chr2}\t{cl.start2}\t{cl.end2}\t' +
                         f'{print_line_readids}\t0\t{cl.dir1}\t{cl.dir2}\t{print_line_size}\t{print_line_info1}',
                         file = self.hout)
```

### Comparing `nanomonsv-0.5.1/nanomonsv/cluster_sbnd.py` & `nanomonsv-0.6.0/nanomonsv/cluster_sbnd.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,22 @@
         
         is_filter = False
         if len(cl.readids) < self.read_num_thres: is_filter = True
 
         median_mapQ = statistics.median([int(x.split(',')[5]) for x in cl.info])
         if median_mapQ < self.median_mapQ_thres: is_filter = True
 
+        bp_size_vec = []
+        for x in cl.info:
+            xx = x.split(',')
+            if xx[0] == xx[1]: bp_size_vec.append(int(xx[0]))
+            if xx[1] == xx[2]: bp_size_vec.append(int(xx[3]) - int(xx[2]))
+
+        if statistics.median(bp_size_vec) < 1000: is_filter = True
+
         if is_filter == True: return(True)
 
         control_flag = False
         if self.control_tb is not None:
     
             support_read_num = 0
             tabix_error_flag = False
```

### Comparing `nanomonsv-0.5.1/nanomonsv/count_sread_by_alignment.py` & `nanomonsv-0.6.0/nanomonsv/count_sread_by_alignment.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz` & `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi` & `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz` & `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi` & `nanomonsv-0.6.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/filt.py` & `nanomonsv-0.6.0/nanomonsv/filt.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/gather_support_read_seq.py` & `nanomonsv-0.6.0/nanomonsv/gather_support_read_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/generate_consensus.py` & `nanomonsv-0.6.0/nanomonsv/generate_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/identify.py` & `nanomonsv-0.6.0/nanomonsv/identify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/insert_classify.py` & `nanomonsv-0.6.0/nanomonsv/insert_classify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/locate_bp.py` & `nanomonsv-0.6.0/nanomonsv/locate_bp.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/locate_bp_sbnd.py` & `nanomonsv-0.6.0/nanomonsv/locate_bp_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/long_read_validate.py` & `nanomonsv-0.6.0/nanomonsv/long_read_validate.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/merge_control.py` & `nanomonsv-0.6.0/nanomonsv/merge_control.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/my_seq.py` & `nanomonsv-0.6.0/nanomonsv/my_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/parse.py` & `nanomonsv-0.6.0/nanomonsv/parse.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/post_proc.py` & `nanomonsv-0.6.0/nanomonsv/post_proc.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/pyssw.py` & `nanomonsv-0.6.0/nanomonsv/pyssw.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/run.py` & `nanomonsv-0.6.0/nanomonsv/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,17 @@
             fw_support_read_seq_sbnds[last_tpos].write(row)
 
     for i in range(parallel_num):
         fw_support_read_seqs[i].close()
         fw_support_read_seq_sbnds[i].close()
 
     if parallel_num == 1:
-        call_slow_request(args, 0)
+        ret_code, err_message = call_slow_request(args, 0)
+        if ret_code != 0:
+            raise Exception(err_message)
     else:
         import concurrent.futures
 
         if args.processes > 1:
             with concurrent.futures.ProcessPoolExecutor(max_workers=parallel_num) as executor:
                 features = [executor.submit(call_slow_request, args, i) for i in range(parallel_num)]
                 for feature in features:
@@ -348,19 +350,30 @@
                 features = [executor.submit(call_slow_request, args, i) for i in range(parallel_num)]
                 for feature in features:
                     (ret_code, err_message) = feature.result()
                     if ret_code != 0:
                         raise Exception(err_message)
 
     logger.info("Merge parallel execution")
+
+    """
     def merge_txt(prefix):
         with open(prefix + ".txt", 'w') as hout:
             for i in range(parallel_num):
                 for l in open(prefix + ".%d.txt" % (i)):
                     hout.write(l)
+    """
+
+    def merge_txt(prefix):
+        with open(prefix + ".txt", 'w') as hout:
+            for i in range(parallel_num):
+                with open(prefix + ".%d.txt" % (i), 'r') as hin:
+                    for l in hin:
+                        hout.write(l)
+
     merge_txt(args.tumor_prefix + ".refined_bp.sbnd")
     merge_txt(args.tumor_prefix + ".realignment.tumor.sread_count")
     merge_txt(args.tumor_prefix + ".realignment.tumor.sread_info")
     merge_txt(args.tumor_prefix + ".realignment.tumor.sread_count.sbnd")
     merge_txt(args.tumor_prefix + ".realignment.tumor.sread_info.sbnd")
     if args.control_bam is not None:
         merge_txt(args.tumor_prefix + ".realignment.control.sread_count")
```

### Comparing `nanomonsv-0.5.1/nanomonsv/smith_waterman.py` & `nanomonsv-0.6.0/nanomonsv/smith_waterman.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #! /usr/bin/env python3
 
 import numpy as np
 
 def sw_jump(contig, region1_seq, region2_seq, match_score = 1, mismatch_penalty = 2, gap_cost = 2, jump_cost = 2):
 
-    H1 = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int)
-    H1_path = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int)
-    H2 = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int)
-    H2_path = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int)
-    H2_origin_i = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int)
-    H2_origin_j = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int)
+    H1 = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int32)
+    H1_path = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int32)
+    H2 = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
+    H2_path = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
+    H2_origin_i = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
+    H2_origin_j = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
     # jump_ind = np.zeros((len(contig) + 1), np.int)
 
     
     for i in range(1, H1.shape[0]):
         for j in range(1, H1.shape[1]):
             match = H1[i - 1, j - 1] + (match_score if contig[i - 1] == region1_seq[j - 1] else - mismatch_penalty)
             delete = H1[i - 1, j] - gap_cost
```

### Comparing `nanomonsv-0.5.1/nanomonsv/ssw_lib.py` & `nanomonsv-0.6.0/nanomonsv/ssw_lib.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/swalign.py` & `nanomonsv-0.6.0/nanomonsv/swalign.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/utils.py` & `nanomonsv-0.6.0/nanomonsv/utils.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv/vcf_convert.py` & `nanomonsv-0.6.0/nanomonsv/vcf_convert.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/nanomonsv.egg-info/PKG-INFO` & `nanomonsv-0.6.0/nanomonsv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanomonsv
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `nanomonsv-0.5.1/nanomonsv.egg-info/SOURCES.txt` & `nanomonsv-0.6.0/nanomonsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.5.1/setup.py` & `nanomonsv-0.6.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,20 +25,22 @@
     long_description_content_type='text/markdown',
     url = 'https://github.com/friend1ws/nanomonsv',
     author = 'Yuichi Shiraishi',
     author_email = 'friend1ws@gamil.com',
     license = 'GPLv3',
 
     classifiers = [
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: Unix',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Bio-Informatics'
     ],
 
     packages = find_packages(exclude = ['tests', 'LINE_db']),
     package_data={'nanomonsv': ['data/*']},
 
     # install_requires = ["numpy", "parasail", "pysam"],
```

