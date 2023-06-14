# Comparing `tmp/current_events_magnifier-0.2.0.tar.gz` & `tmp/current_events_magnifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.2.0.tar", last modified: Wed Jun 14 10:46:53 2023, max compression
+gzip compressed data, was "current_events_magnifier-0.2.1.tar", last modified: Wed Jun 14 11:02:01 2023, max compression
```

## Comparing `current_events_magnifier-0.2.0.tar` & `current_events_magnifier-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:46:53.536898 current_events_magnifier-0.2.0/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.0/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 10:46:53.536898 current_events_magnifier-0.2.0/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5456 2023-06-14 08:59:36.000000 current_events_magnifier-0.2.0/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:46:53.536898 current_events_magnifier-0.2.0/current_events_magnifier/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       95 2023-06-14 10:43:38.000000 current_events_magnifier-0.2.0/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.0/current_events_magnifier/cm_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5810 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.0/current_events_magnifier/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.0/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.2.0/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.0/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.0/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 10:46:53.536898 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6066 2023-06-14 10:46:53.000000 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      565 2023-06-14 10:46:53.000000 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 10:46:53.000000 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 10:46:53.000000 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 10:46:53.000000 current_events_magnifier-0.2.0/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 10:46:53.536898 current_events_magnifier-0.2.0/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1054 2023-06-14 10:46:52.000000 current_events_magnifier-0.2.0/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.2.1/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6043 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5396 2023-06-14 11:01:23.000000 current_events_magnifier-0.2.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/current_events_magnifier/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       95 2023-06-14 10:43:38.000000 current_events_magnifier-0.2.1/current_events_magnifier/__init__.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5807 2023-06-14 11:01:09.000000 current_events_magnifier-0.2.1/current_events_magnifier/magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.2.1/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7487 2023-06-14 08:32:18.000000 current_events_magnifier-0.2.1/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.1/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13271 2023-06-14 10:46:36.000000 current_events_magnifier-0.2.1/current_events_magnifier/read_tombo_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.2.1/current_events_magnifier/utils.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6043 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      547 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       69 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 11:02:01.000000 current_events_magnifier-0.2.1/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 11:02:01.709844 current_events_magnifier-0.2.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1039 2023-06-14 11:01:44.000000 current_events_magnifier-0.2.1/setup.py
```

### Comparing `current_events_magnifier-0.2.0/LICENSE` & `current_events_magnifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/PKG-INFO` & `current_events_magnifier-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: current_events_magnifier
-Version: 0.2.0
-Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
-Home-page: https://github.com/lrslab/current_events_magnifier
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
@@ -41,15 +27,15 @@
 cd Current_Magnifier/
 pip install -r requirements.txt
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python current_events_magnifier.py tombo -h
+python magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -65,15 +51,15 @@
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
 ```
 ### read_f5c_resquiggle
 ```sh
-python current_events_magnifier.py f5c -h
+python magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -102,29 +88,29 @@
 
 minimap2 -ax map-ont -t 16 --MD <reference-fasta> <reads.fastq> | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
 
 f5c resquiggle -c final.fastq file.blow5 -o file.paf
 
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python current_events_magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
+python magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
 
 ```
 If you used Tombo(v1.5.0),
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames <reads.fastq> --processes 16 
 tombo resquiggle single/ <reference-fasta> --processes 16 --num-most-common-errors 5
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 
-python current_events_magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
+python magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
 
 ```
```

### Comparing `current_events_magnifier-0.2.0/README.md` & `current_events_magnifier-0.2.1/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: current-events-magnifier
+Version: 0.2.1
+Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
+Home-page: https://github.com/lrslab/current_events_magnifier
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
 ![alt text](example/boxplot.png)
@@ -27,15 +43,15 @@
 cd Current_Magnifier/
 pip install -r requirements.txt
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python current_events_magnifier.py tombo -h
+python magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -51,15 +67,15 @@
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
 ```
 ### read_f5c_resquiggle
 ```sh
-python current_events_magnifier.py f5c -h
+python magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -88,29 +104,31 @@
 
 minimap2 -ax map-ont -t 16 --MD <reference-fasta> <reads.fastq> | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
 
 f5c resquiggle -c final.fastq file.blow5 -o file.paf
 
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python current_events_magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
+python magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
 
 ```
 If you used Tombo(v1.5.0),
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames <reads.fastq> --processes 16 
 tombo resquiggle single/ <reference-fasta> --processes 16 --num-most-common-errors 5
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 
-python current_events_magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
+python magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
 
 ```
 
 
 
 
 
+
+
```

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/cm_utils.py` & `current_events_magnifier-0.2.1/current_events_magnifier/utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/current_events_magnifier.py` & `current_events_magnifier-0.2.1/current_events_magnifier/magnifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-#!/usr/bin/env python3
 import argparse
 import os
-from current_events_magnifier.cm_utils import read_fasta_to_dic,reverse_fasta
+from current_events_magnifier.utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
 from current_events_magnifier.plot import signal_plot
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
@@ -74,15 +73,15 @@
             df['type'] = df['type'].astype(category)
         except:
             args.control = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
-    else:
+    elif args.function == 'f5c':
         from read_f5c_resquiggle import read_blow5
         df_wt, aligned_num_wt = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand, subsample_num)
         df_wt['type'] = 'Sample'
         try:
             df_ivt, aligned_num_ivt = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
             df_ivt['type'] = 'Control'
```

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/normalization.py` & `current_events_magnifier-0.2.1/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/plot.py` & `current_events_magnifier-0.2.1/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.2.1/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.2.1/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: current-events-magnifier
-Version: 0.2.0
+Name: current_events_magnifier
+Version: 0.2.1
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,15 +43,15 @@
 cd Current_Magnifier/
 pip install -r requirements.txt
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python current_events_magnifier.py tombo -h
+python magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -65,15 +67,15 @@
   -t CPU, --cpu CPU     num of process (default:8)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
 ```
 ### read_f5c_resquiggle
 ```sh
-python current_events_magnifier.py f5c -h
+python magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -102,29 +104,31 @@
 
 minimap2 -ax map-ont -t 16 --MD <reference-fasta> <reads.fastq> | samtools view -hbS -F 260 - | samtools sort -@ 6 -o file.bam
 samtools index file.bam
 
 f5c resquiggle -c final.fastq file.blow5 -o file.paf
 
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-python current_events_magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
+python magnifier.py f5c -i wt/file -c control/file -o f5c_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --ref reference.fa
 
 ```
 If you used Tombo(v1.5.0),
 ```sh
 # if fast5 is not single format need to transfer to single format by ont-fast-api
 # single is fast5s-base-directory
 
 tombo preprocess annotate_raw_with_fastqs --fast5-basedir  single/ --fastq-filenames <reads.fastq> --processes 16 
 tombo resquiggle single/ <reference-fasta> --processes 16 --num-most-common-errors 5
 # Notes:
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 
-python current_events_magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
+python magnifier.py tombo -i wt/single -c control/single -o tombo_result --chrom NC_000xxx --strand + --pos 3929 --len 5 --cpu 4 --ref reference.fa
 
 ```
 
 
 
 
 
+
+
```

### Comparing `current_events_magnifier-0.2.0/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.2.1/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
 current_events_magnifier/__init__.py
-current_events_magnifier/cm_utils.py
-current_events_magnifier/current_events_magnifier.py
+current_events_magnifier/magnifier.py
 current_events_magnifier/normalization.py
 current_events_magnifier/plot.py
 current_events_magnifier/read_f5c_resquiggle.py
 current_events_magnifier/read_tombo_resquiggle.py
+current_events_magnifier/utils.py
 current_events_magnifier.egg-info/PKG-INFO
 current_events_magnifier.egg-info/SOURCES.txt
 current_events_magnifier.egg-info/dependency_links.txt
 current_events_magnifier.egg-info/requires.txt
 current_events_magnifier.egg-info/top_level.txt
```

### Comparing `current_events_magnifier-0.2.0/setup.py` & `current_events_magnifier-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.2.0",
+    version="0.2.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
@@ -23,9 +23,9 @@
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.21.6',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
     ],
-    scripts=['current_events_magnifier/current_events_magnifier.py']
+    scripts=['current_events_magnifier/magnifier.py']
 )
```

