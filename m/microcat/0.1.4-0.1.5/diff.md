# Comparing `tmp/microcat-0.1.4.tar.gz` & `tmp/microcat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.1.4.tar", last modified: Fri Jun  9 04:34:07 2023, max compression
+gzip compressed data, was "microcat-0.1.5.tar", last modified: Wed Jun 14 02:39:30 2023, max compression
```

## Comparing `microcat-0.1.4.tar` & `microcat-0.1.5.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:34:07.952008 microcat-0.1.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-09 04:34:03.000000 microcat-0.1.4/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.4/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.4/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.4/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    18601 2023-06-09 04:29:52.000000 microcat-0.1.4/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 03:16:48.000000 microcat-0.1.4/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-07 06:44:30.000000 microcat-0.1.4/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-07 06:46:24.000000 microcat-0.1.4/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.4/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.4/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.4/microcat/envs/trimming.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.944008 microcat-0.1.4/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/profiles/lsf/
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/CookieCutter.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/OSLayer.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_config.py
--rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_jobscript.sh
--rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/lsf_submit.py
--rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/profiles/lsf/memory_units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.4/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.4/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.4/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    42225 2023-06-09 04:28:20.000000 microcat-0.1.4/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.4/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/scripts/
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.4/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.4/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.4/microcat/scripts/extract_microbiome_output.R
--rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/scripts/get_ncbi_domains.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.4/microcat/scripts/krak2_output_denosing.R
--rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.4/microcat/scripts/kraken2mpa.py
--rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.4/microcat/scripts/kraken2sc.py
--rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.4/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.4/microcat/scripts/sckmer_unpaired.R
--rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.4/microcat/scripts/spilt_bam_by_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.952008 microcat-0.1.4/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.4/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.4/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.4/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 04:34:07.948008 microcat-0.1.4/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 04:34:07.000000 microcat-0.1.4/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 04:34:07.952008 microcat-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-09 03:45:47.000000 microcat-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-14 02:39:30.557833 microcat-0.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.549833 microcat-0.1.5/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-06-14 02:37:50.000000 microcat-0.1.5/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      911 2023-06-09 03:13:23.000000 microcat-0.1.5/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:42:59.000000 microcat-0.1.5/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     8766 2023-06-09 03:49:23.000000 microcat-0.1.5/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    18610 2023-06-14 02:37:44.000000 microcat-0.1.5/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-14 02:38:16.000000 microcat-0.1.5/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 02:38:08.000000 microcat-0.1.5/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.1.5/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.1.5/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 06:24:12.000000 microcat-0.1.5/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.1.5/microcat/envs/trimming.yaml
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-10 01:56:12.000000 microcat-0.1.5/microcat/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.549833 microcat-0.1.5/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat/profiles/lsf/
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-14 02:37:56.000000 microcat-0.1.5/microcat/profiles/lsf/CookieCutter.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/OSLayer.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     1124 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_cancel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_config.py
+-rwxr-xr-x   0 root         (0) root         (0)       48 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_jobscript.sh
+-rwxr-xr-x   0 root         (0) root         (0)     7511 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)     8281 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/lsf_submit.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/profiles/lsf/memory_units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.1.5/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.1.5/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    40814 2023-06-09 02:28:56.000000 microcat-0.1.5/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.1.5/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    42271 2023-06-14 02:39:14.000000 microcat-0.1.5/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    10460 2023-06-05 09:08:14.000000 microcat-0.1.5/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/scripts/
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.1.5/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.1.5/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3849 2023-06-07 07:14:23.000000 microcat-0.1.5/microcat/scripts/extract_microbiome_output.R
+-rwxr-xr-x   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/scripts/get_ncbi_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-07 07:15:11.000000 microcat-0.1.5/microcat/scripts/krak2_output_denosing.R
+-rwxr-xr-x   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.1.5/microcat/scripts/kraken2mpa.py
+-rwxr-xr-x   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.1.5/microcat/scripts/kraken2sc.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-06-07 07:14:59.000000 microcat-0.1.5/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15665 2023-06-07 07:13:48.000000 microcat-0.1.5/microcat/scripts/sckmer_unpaired.R
+-rwxr-xr-x   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.1.5/microcat/scripts/spilt_bam_by_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.557833 microcat-0.1.5/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.1.5/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-09 04:28:17.000000 microcat-0.1.5/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.1.5/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 02:39:30.553833 microcat-0.1.5/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 02:39:30.000000 microcat-0.1.5/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-09 01:50:10.000000 microcat-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 02:39:30.557833 microcat-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-09 03:43:47.000000 microcat-0.1.5/setup.py
```

### Comparing `microcat-0.1.4/LICENSE` & `microcat-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/PKG-INFO` & `microcat-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.4
+Version: 0.1.5
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.4/microcat/__init__.py` & `microcat-0.1.5/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/config/config.yaml` & `microcat-0.1.5/microcat/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/configer.py` & `microcat-0.1.5/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/corer.py` & `microcat-0.1.5/microcat/corer.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,15 +530,15 @@
     args, unknown = parser.parse_known_args()
         
     if hasattr(args, 'host') and args.host == "starsolo" and args.assay is None:
         parser_init.error("--assay option is required when host is starsolo")
 
     try:
         if args.version:
-            print("microcat version %s" % __version__)
+            print("microcat version %s" % microcat.__version__)
             sys.exit(0)
         args.func(args, unknown)
     except AttributeError as e:
         print(e)
         parser.print_help()
 
 if __name__ == "__main__":
```

### Comparing `microcat-0.1.4/microcat/profiles/lsf/CookieCutter.py` & `microcat-0.1.5/microcat/profiles/lsf/CookieCutter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
     @staticmethod
     def get_log_dir() -> str:
         return "logs/cluster"
 
     @staticmethod
     def get_default_queue() -> str:
-        return "short"
+        return "smp"
 
     @staticmethod
     def get_default_project() -> str:
         return ""
 
     @staticmethod
     def get_lsf_unit_for_limits() -> str:
-        return "GB"
+        return "MB"
 
     @staticmethod
     def get_unknwn_behaviour() -> str:
         return "wait"
 
     @staticmethod
     def get_zombi_behaviour() -> str:
```

### Comparing `microcat-0.1.4/microcat/profiles/lsf/OSLayer.py` & `microcat-0.1.5/microcat/profiles/lsf/OSLayer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/profiles/lsf/lsf_cancel.py` & `microcat-0.1.5/microcat/profiles/lsf/lsf_cancel.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/profiles/lsf/lsf_config.py` & `microcat-0.1.5/microcat/profiles/lsf/lsf_config.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/profiles/lsf/lsf_status.py` & `microcat-0.1.5/microcat/profiles/lsf/lsf_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/profiles/lsf/lsf_submit.py` & `microcat-0.1.5/microcat/profiles/lsf/lsf_submit.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/profiles/lsf/memory_units.py` & `microcat-0.1.5/microcat/profiles/lsf/memory_units.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/rules/ERCC.smk` & `microcat-0.1.5/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/rules/classfier.smk` & `microcat-0.1.5/microcat/rules/classfier.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/rules/database.smk` & `microcat-0.1.5/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/rules/host.smk` & `microcat-0.1.5/microcat/rules/host.smk`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
                     --soloUMIstart 17 \
                     --soloUMIlen 12 \
                     --genomeDir {params.reference} \
                     --readFilesIn {params.cdna_reads} {params.barcode_reads} \
                     --runThreadN {params.threads} \
                     --clipAdapterType CellRanger4 \
                     --outFilterScoreMin 30 \
+                    --readFilesCommand zcat \
                     --soloCBmatchWLtype 1MM_multi_Nbase_pseudocounts \
                     --soloUMIfiltering MultiGeneUMI_CR \
                     --outSAMtype BAM SortedByCoordinate\
                     --outSAMattrRGline ID:{wildcards.sample} PL:illumina SM:{wildcards.sample} LB:tenX_v3 \
                     --outSAMattributes NH HI AS nM CB UB CR CY UR UY GX GN \
                     --soloUMIdedup 1MM_CR \
                     --outSAMunmapped Within \
```

### Comparing `microcat-0.1.4/microcat/sample.py` & `microcat-0.1.5/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/INVADEseq.py` & `microcat-0.1.5/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/extract_kraken_reads.py` & `microcat-0.1.5/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/extract_microbiome_output.R` & `microcat-0.1.5/microcat/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/get_ncbi_domains.py` & `microcat-0.1.5/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/krak2_output_denosing.R` & `microcat-0.1.5/microcat/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/kraken2mpa.py` & `microcat-0.1.5/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/kraken2sc.py` & `microcat-0.1.5/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/sample_denosing.R` & `microcat-0.1.5/microcat/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/sckmer_unpaired.R` & `microcat-0.1.5/microcat/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.1.5/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.1.5/microcat/snakefiles/scRNA_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.1.4/microcat.egg-info/PKG-INFO` & `microcat-0.1.5/microcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.1.4
+Version: 0.1.5
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.1.4/microcat.egg-info/SOURCES.txt` & `microcat-0.1.5/microcat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 requirements.txt
 setup.py
 microcat/__about__.py
 microcat/__init__.py
 microcat/configer.py
 microcat/corer.py
+microcat/prepare.py
 microcat/sample.py
 microcat.egg-info/PKG-INFO
 microcat.egg-info/SOURCES.txt
 microcat.egg-info/dependency_links.txt
 microcat.egg-info/entry_points.txt
 microcat.egg-info/requires.txt
 microcat.egg-info/top_level.txt
@@ -29,14 +30,15 @@
 microcat/profiles/lsf/lsf_cancel.py
 microcat/profiles/lsf/lsf_config.py
 microcat/profiles/lsf/lsf_jobscript.sh
 microcat/profiles/lsf/lsf_status.py
 microcat/profiles/lsf/lsf_submit.py
 microcat/profiles/lsf/memory_units.py
 microcat/rules/ERCC.smk
+microcat/rules/build.smk
 microcat/rules/classfier.smk
 microcat/rules/database.smk
 microcat/rules/host.smk
 microcat/scripts/INVADEseq.py
 microcat/scripts/extract_kraken_reads.py
 microcat/scripts/extract_microbiome_output.R
 microcat/scripts/get_ncbi_domains.py
```

### Comparing `microcat-0.1.4/setup.py` & `microcat-0.1.5/setup.py`

 * *Files identical despite different names*

