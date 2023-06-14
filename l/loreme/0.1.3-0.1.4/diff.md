# Comparing `tmp/loreme-0.1.3.tar.gz` & `tmp/loreme-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.3.tar", last modified: Tue Jun 13 17:06:24 2023, max compression
+gzip compressed data, was "loreme-0.1.4.tar", last modified: Wed Jun 14 05:06:06 2023, max compression
```

## Comparing `loreme-0.1.3.tar` & `loreme-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.342747 loreme-0.1.3/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.3/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5166 2023-06-13 17:06:24.342137 loreme-0.1.3/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4651 2023-06-13 17:03:35.000000 loreme-0.1.3/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.306628 loreme-0.1.3/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5166 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-10 09:03:08.000000 loreme-0.1.3/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-13 17:06:24.342878 loreme-0.1.3/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.297881 loreme-0.1.3/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.340872 loreme-0.1.3/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-10 18:11:11.000000 loreme-0.1.3/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-10 18:19:42.000000 loreme-0.1.3/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-13 05:56:48.000000 loreme-0.1.3/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5921 2023-06-10 17:32:09.000000 loreme-0.1.3/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3602 2023-06-10 17:30:49.000000 loreme-0.1.3/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37354 2023-06-13 05:58:08.000000 loreme-0.1.3/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-10 17:48:02.000000 loreme-0.1.3/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-10 18:20:20.000000 loreme-0.1.3/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-10 09:03:11.000000 loreme-0.1.3/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.869357 loreme-0.1.4/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.4/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-14 05:06:06.869016 loreme-0.1.4/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.4/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.821605 loreme-0.1.4/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-14 04:51:11.000000 loreme-0.1.4/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-14 05:06:06.869778 loreme-0.1.4/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.811983 loreme-0.1.4/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.868207 loreme-0.1.4/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5921 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3602 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37347 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/version.py
```

### Comparing `loreme-0.1.3/LICENSE` & `loreme-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/PKG-INFO` & `loreme-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +45,15 @@
 
 The recommended way to install `loreme` is with a dedicated `conda` environment:
 
 First create an environment including all dependencies:
 ```sh
 conda create -n loreme -c conda-forge -c bioconda samtools pbmm2 \
   urllib3 pybedtools gff2bed seaborn pyfaidx psutil gputil tabulate \
-  cython h5py iso8601 more-itertools polars tqdm
+  cython h5py iso8601 more-itertools tqdm
 conda activate loreme
 ```
 
 Then install with `pip`:
 ```sh
 pip install loreme
 ```
@@ -99,26 +99,26 @@
 > For members of [Michael Lab](https://michael.salk.edu/) at Salk running on seabiscuit, use `loreme download-dorado linux-x64`.
 
 ### Modified basecalling
 
 You can carry out modified basecalling (i.e. DNA methylation) with default parameters by running:
 
 ```
-loreme dorado-basecall <input.pod5> <output.sam>
+loreme dorado-basecall <pod5s/> <output.sam>
 ```
 
-For other parameter options, see `loreme dorado --help`
+The input argument `pod5s/` should be a directory containing one or more POD5 files. For other parameter options, see `loreme dorado-basecall --help`
 
 > #### Note
 > Basecalling ONT data is disk-read intensive, so for best performance the input POD5 data should be on a fast SSD (For example, `/scratch/<username>` for members of [Michael Lab](https://michael.salk.edu/) at Salk).
 
 To run dorado with only regular basecalling, use the `--no-mod` option:
 
 ```
-loreme dorado-basecall --no-mod <input.pod5> <output.sam>
+loreme dorado-basecall --no-mod <pod5s/> <output.sam>
 ```
 
 If you wish to convert the SAM file to a FASTQ file, use:
 ```
 samtools view -bo output.bam output.sam
 samtools fastq -T '*' output.bam > output.fq
 ```
```

### Comparing `loreme-0.1.3/README.md` & `loreme-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 The recommended way to install `loreme` is with a dedicated `conda` environment:
 
 First create an environment including all dependencies:
 ```sh
 conda create -n loreme -c conda-forge -c bioconda samtools pbmm2 \
   urllib3 pybedtools gff2bed seaborn pyfaidx psutil gputil tabulate \
-  cython h5py iso8601 more-itertools polars tqdm
+  cython h5py iso8601 more-itertools tqdm
 conda activate loreme
 ```
 
 Then install with `pip`:
 ```sh
 pip install loreme
 ```
@@ -85,26 +85,26 @@
 > For members of [Michael Lab](https://michael.salk.edu/) at Salk running on seabiscuit, use `loreme download-dorado linux-x64`.
 
 ### Modified basecalling
 
 You can carry out modified basecalling (i.e. DNA methylation) with default parameters by running:
 
 ```
-loreme dorado-basecall <input.pod5> <output.sam>
+loreme dorado-basecall <pod5s/> <output.sam>
 ```
 
-For other parameter options, see `loreme dorado --help`
+The input argument `pod5s/` should be a directory containing one or more POD5 files. For other parameter options, see `loreme dorado-basecall --help`
 
 > #### Note
 > Basecalling ONT data is disk-read intensive, so for best performance the input POD5 data should be on a fast SSD (For example, `/scratch/<username>` for members of [Michael Lab](https://michael.salk.edu/) at Salk).
 
 To run dorado with only regular basecalling, use the `--no-mod` option:
 
 ```
-loreme dorado-basecall --no-mod <input.pod5> <output.sam>
+loreme dorado-basecall --no-mod <pod5s/> <output.sam>
 ```
 
 If you wish to convert the SAM file to a FASTQ file, use:
 ```
 samtools view -bo output.bam output.sam
 samtools fastq -T '*' output.bam > output.fq
 ```
```

### Comparing `loreme-0.1.3/loreme.egg-info/PKG-INFO` & `loreme-0.1.4/loreme.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -45,15 +45,15 @@
 
 The recommended way to install `loreme` is with a dedicated `conda` environment:
 
 First create an environment including all dependencies:
 ```sh
 conda create -n loreme -c conda-forge -c bioconda samtools pbmm2 \
   urllib3 pybedtools gff2bed seaborn pyfaidx psutil gputil tabulate \
-  cython h5py iso8601 more-itertools polars tqdm
+  cython h5py iso8601 more-itertools tqdm
 conda activate loreme
 ```
 
 Then install with `pip`:
 ```sh
 pip install loreme
 ```
@@ -99,26 +99,26 @@
 > For members of [Michael Lab](https://michael.salk.edu/) at Salk running on seabiscuit, use `loreme download-dorado linux-x64`.
 
 ### Modified basecalling
 
 You can carry out modified basecalling (i.e. DNA methylation) with default parameters by running:
 
 ```
-loreme dorado-basecall <input.pod5> <output.sam>
+loreme dorado-basecall <pod5s/> <output.sam>
 ```
 
-For other parameter options, see `loreme dorado --help`
+The input argument `pod5s/` should be a directory containing one or more POD5 files. For other parameter options, see `loreme dorado-basecall --help`
 
 > #### Note
 > Basecalling ONT data is disk-read intensive, so for best performance the input POD5 data should be on a fast SSD (For example, `/scratch/<username>` for members of [Michael Lab](https://michael.salk.edu/) at Salk).
 
 To run dorado with only regular basecalling, use the `--no-mod` option:
 
 ```
-loreme dorado-basecall --no-mod <input.pod5> <output.sam>
+loreme dorado-basecall --no-mod <pod5s/> <output.sam>
 ```
 
 If you wish to convert the SAM file to a FASTQ file, use:
 ```
 samtools view -bo output.bam output.sam
 samtools fastq -T '*' output.bam > output.fq
 ```
```

### Comparing `loreme-0.1.3/loreme.egg-info/SOURCES.txt` & `loreme-0.1.4/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/pyproject.toml` & `loreme-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.3" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.4" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.3/src/loreme/__init__.py` & `loreme-0.1.4/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/check_gpu_availability.py` & `loreme-0.1.4/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/dorado.py` & `loreme-0.1.4/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/download.py` & `loreme-0.1.4/src/loreme/download.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/env.py` & `loreme-0.1.4/src/loreme/env.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/export_bedgraph.py` & `loreme-0.1.4/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/gene_body_methylation.py` & `loreme-0.1.4/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/intersect.py` & `loreme-0.1.4/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/loreme.py` & `loreme-0.1.4/src/loreme/loreme.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
                                help='input FAST5 files, or direcories containing FAST5')
     parser_dorado_convert.add_argument('output', metavar='<output.pod5>',
                                help='path to output POD5 file')
     parser_dorado_convert.add_argument("-t", "--threads", metavar="<int>",
         type=int, default=1, help="Number of threads. (default: %(default)d)")
 
     parser_dorado_basecall = subparsers.add_parser('dorado-basecall',
-        help='run full dorado pipeline')
+        help='run dorado basecaller')
     parser_dorado_basecall.set_defaults(func=run_dorado_basecall)
     parser_dorado_basecall.add_argument('reads', metavar='<reads>', nargs='+',
                                help='input FAST5 files, or single directory containing FAST5 or POD5 files')
     parser_dorado_basecall.add_argument('output', metavar='<output.sam>',
                                help='path to output SAM file')
     parser_dorado_basecall.add_argument('--convert', action='store_true',
                                help='convert FAST5 to POD5 before basecalling')
@@ -464,15 +464,15 @@
     # parser_dorado_basecall.add_argument('--reference', metavar='<index>',
     #                            help='map to a reference index (fastq/fasta/mmi)')
     parser_dorado_basecall.add_argument("-t", "--threads", metavar="<int>",
         type=int, default=1,
         help="Number of cpu threads. (default: %(default)d)")
 
     parser_dorado_align = subparsers.add_parser('dorado-align',
-        help='align dorado basecalls')
+        help='run dorado aligner')
     parser_dorado_align.set_defaults(func=_dorado_align)
     parser_dorado_align.add_argument('index', metavar='<index>',
                                      help='reference index for alignment')
     parser_dorado_align.add_argument('reads', metavar='<reads>',
                                      help='reads for alignment')
     parser_dorado_align.add_argument('output', metavar='<output.bam>',
                                      help='path to output BAM file')
```

### Comparing `loreme-0.1.3/src/loreme/mean.py` & `loreme-0.1.4/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/merge.py` & `loreme-0.1.4/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/methylation_hist.py` & `loreme-0.1.4/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/parse_gff.py` & `loreme-0.1.4/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/pbcpg.py` & `loreme-0.1.4/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/plot.py` & `loreme-0.1.4/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/plot_bedtools.py` & `loreme-0.1.4/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/plot_genes.py` & `loreme-0.1.4/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/plot_repeats.py` & `loreme-0.1.4/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.3/src/loreme/promoter_methylation.py` & `loreme-0.1.4/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

