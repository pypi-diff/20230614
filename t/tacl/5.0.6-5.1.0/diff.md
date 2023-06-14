# Comparing `tmp/tacl-5.0.6.tar.gz` & `tmp/tacl-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacl-5.0.6.tar", last modified: Tue May  9 21:30:59 2023, max compression
+gzip compressed data, was "tacl-5.1.0.tar", last modified: Wed Jun 14 01:04:40 2023, max compression
```

## Comparing `tacl-5.0.6.tar` & `tacl-5.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/
--rw-r--r--   0 jamie     (1000) jamie     (1000)    12631 2023-05-09 20:58:08.000000 tacl-5.0.6/CHANGES
--rw-r--r--   0 jamie     (1000) jamie     (1000)    32472 2021-07-14 09:03:57.000000 tacl-5.0.6/LICENCE
--rw-r--r--   0 jamie     (1000) jamie     (1000)      162 2022-12-26 23:02:02.000000 tacl-5.0.6/MANIFEST.in
--rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-05-09 21:30:59.338202 tacl-5.0.6/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2021-07-14 09:01:38.000000 tacl-5.0.6/README.rst
--rw-r--r--   0 jamie     (1000) jamie     (1000)      879 2023-05-09 21:22:44.000000 tacl-5.0.6/pyproject.toml
--rw-r--r--   0 jamie     (1000) jamie     (1000)       38 2023-05-09 21:30:59.338202 tacl-5.0.6/setup.cfg
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      705 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    32400 2022-09-23 22:30:27.000000 tacl-5.0.6/tacl/__main__.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl/assets/
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/results_highlight/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1229 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/results_highlight/heatmap.js
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/templates/
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/lifetime.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1186 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/ngram_highlight.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)      954 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/results_highlight.html
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1103 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/templates/sequence.html
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/assets/xslt/
--rw-r--r--   0 jamie     (1000) jamie     (1000)      807 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0062_rest.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)      891 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1284 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     2115 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_commentary.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1800 2023-04-07 08:50:00.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_div.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_extract_verse.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)      748 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/assets/xslt/CBETA_remove_divs.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4838 2023-03-05 23:53:29.000000 tacl-5.0.6/tacl/assets/xslt/prepare_tei_cbeta_github.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3381 2023-03-05 08:38:21.000000 tacl-5.0.6/tacl/assets/xslt/strip_tei.xsl
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4330 2021-10-08 21:27:56.000000 tacl-5.0.6/tacl/catalogue.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.338202 tacl-5.0.6/tacl/cli/
--rw-r--r--   0 jamie     (1000) jamie     (1000)        0 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/cli/__init__.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3449 2021-09-27 01:52:24.000000 tacl-5.0.6/tacl/cli/formatters.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3808 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/cli/utils.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1579 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/colour.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    40247 2022-10-01 23:28:52.000000 tacl-5.0.6/tacl/constants.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     4253 2022-09-23 04:53:43.000000 tacl-5.0.6/tacl/corpus.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    36087 2022-09-19 01:51:28.000000 tacl-5.0.6/tacl/data_store.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1044 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/decorators.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)      610 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/exceptions.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     7990 2023-01-30 22:09:57.000000 tacl-5.0.6/tacl/highlighter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    19580 2021-07-14 09:03:57.000000 tacl-5.0.6/tacl/jitc.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6635 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/lifetime_report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    10364 2022-09-23 03:38:57.000000 tacl-5.0.6/tacl/normaliser.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3064 2022-05-05 07:43:28.000000 tacl-5.0.6/tacl/report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    45042 2022-10-16 22:23:08.000000 tacl-5.0.6/tacl/results.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    13355 2021-09-27 01:52:15.000000 tacl-5.0.6/tacl/sequence.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5494 2021-09-12 03:15:37.000000 tacl-5.0.6/tacl/splitter.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     5400 2021-07-14 09:03:56.000000 tacl-5.0.6/tacl/statistics_report.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     3873 2023-04-07 09:23:18.000000 tacl-5.0.6/tacl/stripper.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)    32720 2023-04-10 20:22:44.000000 tacl-5.0.6/tacl/tei_corpus.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     6013 2022-09-20 05:54:17.000000 tacl-5.0.6/tacl/text.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1140 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/tokenizer.py
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1248 2021-07-14 09:03:55.000000 tacl-5.0.6/tacl/work_joiner.py
-drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-05-09 21:30:59.334202 tacl-5.0.6/tacl.egg-info/
--rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/PKG-INFO
--rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/SOURCES.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/dependency_links.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/entry_points.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/requires.txt
--rw-r--r--   0 jamie     (1000) jamie     (1000)        5 2023-05-09 21:30:59.000000 tacl-5.0.6/tacl.egg-info/top_level.txt
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    13072 2023-06-14 01:01:56.000000 tacl-5.1.0/CHANGES
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32472 2023-05-28 05:42:33.000000 tacl-5.1.0/LICENCE
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      162 2023-05-28 05:30:26.000000 tacl-5.1.0/MANIFEST.in
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-06-14 01:04:40.876822 tacl-5.1.0/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2023-05-28 05:28:34.000000 tacl-5.1.0/README.rst
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      885 2023-06-14 01:02:10.000000 tacl-5.1.0/pyproject.toml
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       38 2023-06-14 01:04:40.876822 tacl-5.1.0/setup.cfg
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      705 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32400 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/__main__.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.872822 tacl-5.1.0/tacl/assets/
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl/assets/results_highlight/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1229 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/results_highlight/heatmap.js
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl/assets/templates/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/templates/lifetime.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1186 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/templates/ngram_highlight.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      954 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/templates/results_highlight.html
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1103 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/templates/sequence.html
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl/assets/xslt/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      807 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_T0062_rest.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      891 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1284 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2115 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_extract_commentary.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1800 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_extract_div.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1801 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_extract_verse.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      748 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/CBETA_remove_divs.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4838 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/prepare_tei_cbeta_github.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3381 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/assets/xslt/strip_tei.xsl
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4330 2023-05-28 05:42:33.000000 tacl-5.1.0/tacl/catalogue.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl/cli/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        0 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/cli/__init__.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3449 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/cli/formatters.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3808 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/cli/utils.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1579 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/colour.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    40247 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/constants.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     4253 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/corpus.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    35658 2023-06-04 03:15:05.000000 tacl-5.1.0/tacl/data_store.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1044 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/decorators.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)      610 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/exceptions.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     7990 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/highlighter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    19580 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/jitc.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6635 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/lifetime_report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    10364 2023-05-28 05:42:33.000000 tacl-5.1.0/tacl/normaliser.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     2912 2023-06-12 09:49:59.000000 tacl-5.1.0/tacl/report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    45064 2023-06-14 00:51:55.000000 tacl-5.1.0/tacl/results.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    13514 2023-06-12 22:23:53.000000 tacl-5.1.0/tacl/sequence.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5494 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/splitter.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     5400 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/statistics_report.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     3932 2023-06-12 09:57:28.000000 tacl-5.1.0/tacl/stripper.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    32146 2023-06-12 09:42:59.000000 tacl-5.1.0/tacl/tei_corpus.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     6013 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/text.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1140 2023-05-28 05:42:35.000000 tacl-5.1.0/tacl/tokenizer.py
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1248 2023-05-28 05:42:36.000000 tacl-5.1.0/tacl/work_joiner.py
+drwxr-xr-x   0 jamie     (1000) jamie     (1000)        0 2023-06-14 01:04:40.876822 tacl-5.1.0/tacl.egg-info/
+-rw-r--r--   0 jamie     (1000) jamie     (1000)    39343 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/PKG-INFO
+-rw-r--r--   0 jamie     (1000) jamie     (1000)     1267 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        1 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       44 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/entry_points.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)       50 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/requires.txt
+-rw-r--r--   0 jamie     (1000) jamie     (1000)        5 2023-06-14 01:04:40.000000 tacl-5.1.0/tacl.egg-info/top_level.txt
```

### Comparing `tacl-5.0.6/CHANGES` & `tacl-5.1.0/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+5.1.0  2023-06-14  Jamie Norrish  <jamie@artefact.org.nz>
+
+  * Modified results reduce to properly handle the same witness under
+    different labels, namely to treat them as entirely distinct.
+
+  * Changed from deprecated pkg_resources code to importlib.resources
+    for handling package files.
+
+  * Changed from deprecated Bio.pairwise2 to Bio.Align.
+
+  * Added logging statement when about to output CSV results from tacl
+    results.
+
+
 5.0.6  2023-05-10  Jamie Norrish  <jamie@artefact.org.nz>
 
   * Reworked build configuration.
 
   * Updated corpus preparation for Taisho, both markup handling and
     further splits.
```

### Comparing `tacl-5.0.6/LICENCE` & `tacl-5.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/PKG-INFO` & `tacl-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacl
-Version: 5.0.6
+Version: 5.1.0
 Summary: Text analyser for corpus linguistics
 Author-email: Jamie Norrish <jamie@artefact.org.nz>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tacl-5.0.6/README.rst` & `tacl-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/pyproject.toml` & `tacl-5.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tacl"
-version = "5.0.6"
+version = "5.1.0"
 authors = [
   { name = "Jamie Norrish", email = "jamie@artefact.org.nz" },
 ]
 description = "Text analyser for corpus linguistics"
 readme = "README.rst"
 license = { file = "LICENCE" }
 requires-python = ">=3.8"
@@ -16,15 +16,15 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Topic :: Text Processing :: Linguistic",
 ]
 dependencies = [
-    "biopython",
+    "biopython>=1.80",
     "colorlog",
     "Jinja2>3.1.0",
     "lxml",
     "pandas",
 ]
 
 [project.urls]
```

### Comparing `tacl-5.0.6/tacl/__init__.py` & `tacl-5.1.0/tacl/__init__.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/__main__.py` & `tacl-5.1.0/tacl/__main__.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/results_highlight/heatmap.js` & `tacl-5.1.0/tacl/assets/results_highlight/heatmap.js`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/templates/lifetime.html` & `tacl-5.1.0/tacl/assets/templates/lifetime.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/templates/ngram_highlight.html` & `tacl-5.1.0/tacl/assets/templates/ngram_highlight.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/templates/results_highlight.html` & `tacl-5.1.0/tacl/assets/templates/results_highlight.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/templates/sequence.html` & `tacl-5.1.0/tacl/assets/templates/sequence.html`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_T0062_rest.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_T0062_rest.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_T0220_reparent_divs.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_T0418_fix_verse.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_commentary.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_extract_commentary.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_div.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_extract_div.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_extract_verse.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_extract_verse.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/CBETA_remove_divs.xsl` & `tacl-5.1.0/tacl/assets/xslt/CBETA_remove_divs.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/prepare_tei_cbeta_github.xsl` & `tacl-5.1.0/tacl/assets/xslt/prepare_tei_cbeta_github.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/assets/xslt/strip_tei.xsl` & `tacl-5.1.0/tacl/assets/xslt/strip_tei.xsl`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/catalogue.py` & `tacl-5.1.0/tacl/catalogue.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/cli/formatters.py` & `tacl-5.1.0/tacl/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/cli/utils.py` & `tacl-5.1.0/tacl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/colour.py` & `tacl-5.1.0/tacl/colour.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/constants.py` & `tacl-5.1.0/tacl/constants.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/corpus.py` & `tacl-5.1.0/tacl/corpus.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/data_store.py` & `tacl-5.1.0/tacl/data_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,29 +258,28 @@
         :type join: `function`
         :rtype: pandas.Series
 
         """
         ngram_tokens = tokenize(row[constants.NGRAM_FIELDNAME])
         sub_ngram1 = join(ngram_tokens[:-1])
         sub_ngram2 = join(ngram_tokens[1:])
-        count = constants.COUNT_FIELDNAME
         discard = False
         # For performance reasons, avoid searching through matches
         # unless necessary.
         status1 = matches.get(sub_ngram1)
         if status1 == 0:
             discard = True
         else:
             status2 = matches.get(sub_ngram2)
             if status2 == 0:
                 discard = True
             elif (status1 is None) ^ (status2 is None):
                 discard = True
         if discard:
-            row[count] = 0
+            row[constants.COUNT_FIELDNAME] = 0
         return row
 
     def counts(self, catalogue, output_fh):
         """Returns `output_fh` populated with CSV results giving
         n-gram counts of the witnesses of the works in `catalogue`.
 
         :param catalogue: catalogue matching filenames to labels
@@ -699,27 +698,21 @@
         self._logger.info('Removing filler results')
         # For performance, perform the attribute accesses once.
         tokenize = tokenizer.tokenize
         join = tokenizer.joiner.join
         results = []
         previous_witness = (None, None)
         previous_data = {}
-        # Calculate the index of ngram and count columns in a Pandas
-        # named tuple row, as used below. The +1 is due to the tuple
-        # having the row index as the first element.
-        ngram_index = constants.QUERY_FIELDNAMES.index(
-            constants.NGRAM_FIELDNAME) + 1
-        count_index = constants.QUERY_FIELDNAMES.index(
-            constants.COUNT_FIELDNAME) + 1
         # Operate over individual witnesses and sizes, so that there
         # is no possible results pollution between them.
         grouped = pd.read_csv(matches_path, encoding='utf-8',
                               na_filter=False).groupby(
             [constants.WORK_FIELDNAME, constants.SIGLUM_FIELDNAME,
              constants.SIZE_FIELDNAME])
+        cols = [constants.NGRAM_FIELDNAME, constants.COUNT_FIELDNAME]
         for (work, siglum, size), group in grouped:
             if (work, siglum) != previous_witness:
                 previous_matches = group
                 previous_witness = (work, siglum)
             else:
                 self._logger.debug(
                     'Reducing down {} {}-grams for {} {}'.format(
@@ -732,17 +725,15 @@
                         args=(previous_data, tokenize, join))
                     reduced_count = len(previous_matches[previous_matches[
                                         constants.COUNT_FIELDNAME] != 0].index)
                 self._logger.debug('Reduced down to {} grams'.format(
                     reduced_count))
             # Put the previous matches into a form that is more
             # performant for the lookups made in _check_diff_result.
-            previous_data = {}
-            for row in previous_matches.itertuples():
-                previous_data[row[ngram_index]] = row[count_index]
+            previous_data = dict(previous_matches[cols].values)
             if not previous_matches.empty:
                 results.append(previous_matches[previous_matches[
                     constants.COUNT_FIELDNAME] != 0])
         reduced_results = pd.concat(results, ignore_index=True).reindex(
             columns=constants.QUERY_FIELDNAMES)
         reduced_results.to_csv(output_fh, encoding='utf-8', float_format='%d',
                                index=False)
```

### Comparing `tacl-5.0.6/tacl/decorators.py` & `tacl-5.1.0/tacl/decorators.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/exceptions.py` & `tacl-5.1.0/tacl/exceptions.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/highlighter.py` & `tacl-5.1.0/tacl/highlighter.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/jitc.py` & `tacl-5.1.0/tacl/jitc.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/lifetime_report.py` & `tacl-5.1.0/tacl/lifetime_report.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/normaliser.py` & `tacl-5.1.0/tacl/normaliser.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/report.py` & `tacl-5.1.0/tacl/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import importlib.resources
 import os.path
 import shutil
 
 from jinja2 import Environment, PackageLoader
 
-from pkg_resources import resource_filename, resource_listdir
-
 
 class Report:
 
     """Base class for HTML reports.
 
     Subclasses should implement the `generate` method, used to
     generate and output the report into the supplied directory. The
@@ -29,19 +28,17 @@
     def _copy_static_assets(self, output_dir):
         """Copy assets for the report to `output_dir`.
 
         :param output_dir: directory to output assets to
         :type output_dir: `str`
 
         """
-        base_directory = 'assets/{}'.format(self._report_name)
-        for asset in resource_listdir(self._package_name, base_directory):
-            filename = resource_filename(
-                self._package_name, '{}/{}'.format(base_directory, asset))
-            shutil.copy2(filename, output_dir)
+        base_directory = 'tacl.assets.{}'.format(self._report_name)
+        for asset in importlib.resources.files(base_directory).iterdir():
+            shutil.copy2(asset, output_dir)
 
     def generate(self, output_dir):
         """Generate the report, writing it to `output_dir`."""
         raise NotImplementedError
 
     def _get_template(self):
         """Returns a template for this report.
```

### Comparing `tacl-5.0.6/tacl/results.py` & `tacl-5.1.0/tacl/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module containing the Results class."""
 
 import csv
 import logging
 import os
-import re
 import tempfile
 
 import pandas as pd
 
 from . import constants
 from .decorators import requires_columns
 from .exceptions import MalformedResultsError
@@ -276,14 +275,15 @@
         """Writes the results data to `fh` in CSV format and returns `fh`.
 
         :param fh: file to write data to
         :type fh: file object
         :rtype: file object
 
         """
+        self._logger.info('Writing results to CSV')
         self._matches.to_csv(fh, encoding='utf-8', float_format='%d',
                              index=False)
         return fh
 
     @requires_columns([constants.NGRAM_FIELDNAME, constants.WORK_FIELDNAME,
                        constants.SIGLUM_FIELDNAME, constants.COUNT_FIELDNAME,
                        constants.LABEL_FIELDNAME])
@@ -874,44 +874,43 @@
     def reduce(self):
         """Removes results rows whose n-grams are contained in larger
         n-grams."""
         self._logger.info('Reducing the n-grams')
         # This does not make use of any pandas functionality; it
         # probably could, and if so ought to.
         data = {}
-        labels = {}
         # Derive a convenient data structure from the rows.
         for row_index, row in self._matches.iterrows():
             work = row[constants.WORK_FIELDNAME]
             siglum = row[constants.SIGLUM_FIELDNAME]
-            labels[work] = row[constants.LABEL_FIELDNAME]
-            witness_data = data.setdefault((work, siglum), {})
+            label = row[constants.LABEL_FIELDNAME]
+            witness_data = data.setdefault((work, siglum, label), {})
             witness_data[row[constants.NGRAM_FIELDNAME]] = {
                 'count': int(row[constants.COUNT_FIELDNAME]),
                 'size': int(row[constants.SIZE_FIELDNAME])}
         for witness_data in data.values():
             ngrams = list(witness_data.keys())
             ngrams.sort(key=lambda ngram: witness_data[ngram]['size'],
                         reverse=True)
             for ngram in ngrams:
                 if witness_data[ngram]['count'] > 0:
                     self._reduce_by_ngram(witness_data, ngram)
         # Recreate rows from the modified data structure.
         rows = []
-        for (work, siglum), witness_data in data.items():
+        for (work, siglum, label), witness_data in data.items():
             for ngram, ngram_data in witness_data.items():
                 count = ngram_data['count']
                 if count > 0:
                     rows.append(
                         {constants.NGRAM_FIELDNAME: ngram,
                          constants.SIZE_FIELDNAME: ngram_data['size'],
                          constants.WORK_FIELDNAME: work,
                          constants.SIGLUM_FIELDNAME: siglum,
                          constants.COUNT_FIELDNAME: count,
-                         constants.LABEL_FIELDNAME: labels[work]})
+                         constants.LABEL_FIELDNAME: label})
         self._matches = pd.DataFrame(
             rows, columns=constants.QUERY_FIELDNAMES)
 
     def _reduce_by_ngram(self, data, ngram):
         """Lowers the counts of all n-grams in `data` that are
         substrings of `ngram` by `ngram`\'s count.
```

### Comparing `tacl-5.0.6/tacl/sequence.py` & `tacl-5.1.0/tacl/sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing the Sequence and SequenceReport classes."""
 
 import logging
 import os
 import re
 
-from Bio import pairwise2
+from Bio import Align
 import pandas as pd
 
 from . import constants
 from .report import Report
 from .text import Text
 
 
@@ -127,26 +127,29 @@
         """
         old_length = 0
         self._logger.debug('Match found; generating new sequence')
         while True:
             s1, span1 = self._get_text_sequence(t1, t1_span, context_length)
             s2, span2 = self._get_text_sequence(t2, t2_span, context_length)
             length = len(s1)
-            alignment = pairwise2.align.globalms(
-                s1, s2, constants.IDENTICAL_CHARACTER_SCORE,
-                constants.DIFFERENT_CHARACTER_SCORE,
-                constants.OPEN_GAP_PENALTY, constants.EXTEND_GAP_PENALTY)[0]
-            context_length = length
-            score = alignment[2] / length
+            aligner = Align.PairwiseAligner(
+                mode="global", match_score=constants.IDENTICAL_CHARACTER_SCORE,
+                mismatch_score=constants.DIFFERENT_CHARACTER_SCORE,
+                open_gap_score=constants.OPEN_GAP_PENALTY,
+                extend_gap_score=constants.EXTEND_GAP_PENALTY)
+            alignments = aligner.align(s1, s2)
+            score = alignments.score / length
+            alignment = alignments[0]
             if not alignment:
                 return None
             elif score < constants.SCORE_THRESHOLD or length == old_length:
                 break
             else:
                 self._logger.debug('Score: {}'.format(score))
+            context_length = length
             old_length = length
         covered_spans[0].append(span1)
         covered_spans[1].append(span2)
         return Sequence(alignment, self._reverse_substitutes, t1_span[0])
 
     def _generate_sequences(self, primary_label, secondary_label, ngrams):
         """Generates aligned sequences between each witness labelled
```

### Comparing `tacl-5.0.6/tacl/splitter.py` & `tacl-5.1.0/tacl/splitter.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/statistics_report.py` & `tacl-5.1.0/tacl/statistics_report.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/stripper.py` & `tacl-5.1.0/tacl/stripper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing the Stripper class."""
 
+import importlib.resources
 import logging
 import os
 
 from lxml import etree
-from pkg_resources import resource_filename
 
 from . import constants
 
 
 class Stripper:
 
     """Class used for preprocessing a corpus of texts by stripping out all
@@ -20,17 +20,18 @@
 
     """
 
     def __init__(self, input_dir, output_dir):
         self._logger = logging.getLogger(__name__)
         self._input_dir = os.path.abspath(input_dir)
         self._output_dir = os.path.abspath(output_dir)
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/strip_tei.xsl')
-        self.transform = etree.XSLT(etree.parse(xslt_filename))
+        xslt_ref = importlib.resources.files('tacl') / \
+            'assets/xslt/strip_tei.xsl'
+        with importlib.resources.as_file(xslt_ref) as xslt_path:
+            self.transform = etree.XSLT(etree.parse(xslt_path))
 
     def get_witnesses(self, source_tree):
         """Returns a list of all witnesses of variant readings in
         `source_tree` along with their XML ids.
 
         :param source_tree: XML tree of source document
         :type source_tree: `etree._ElementTree`
@@ -70,15 +71,15 @@
             try:
                 os.makedirs(self._output_dir)
             except OSError as err:
                 self._logger.error(
                     'Could not create output directory: {}'.format(err))
                 raise
         for dirpath, dirnames, filenames in os.walk(self._input_dir):
-            for filename in filenames:
+            for filename in sorted(filenames):
                 if os.path.splitext(filename)[1] == '.xml':
                     work, witnesses = self.strip_file(
                         os.path.join(dirpath, filename))
                     self._output_file(work, witnesses)
 
     def strip_file(self, filename):
         file_path = os.path.join(self._input_dir, filename)
```

### Comparing `tacl-5.0.6/tacl/tei_corpus.py` & `tacl-5.1.0/tacl/tei_corpus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module containing the TEICorpus class."""
 
+import importlib.resources
 import logging
 import os
 import re
 
 from lxml import etree
-from pkg_resources import resource_filename
 
 from . import constants
 from .exceptions import TACLError
 
 
 LEAVE_UNNAMED_DIVS = 'leave'
 MERGE_UNNAMED_DIVS_TO_PRECEDING = 'merge_to_preceding'
@@ -65,17 +65,15 @@
 
     xslt = ''
 
     def __init__(self, input_dir, output_dir):
         self._logger = logging.getLogger(__name__)
         self._input_dir = os.path.abspath(input_dir)
         self._output_dir = os.path.abspath(output_dir)
-        xslt_filename = resource_filename(__name__, 'assets/xslt/{}'.format(
-            self.xslt))
-        self.transform = etree.XSLT(etree.parse(xslt_filename))
+        self.transform = self._get_xslt('assets/xslt/{}'.format(self.xslt))
 
     def _assemble_parts(self, work, paths):
         parts = list(paths.keys())
         parts.sort()
         # If the whitespace between tags in the supplied document is
         # not removed, pretty-printing will fail to handle the added
         # documents nicely.
@@ -112,14 +110,19 @@
                             dirpath, filename)
         self._logger.debug('Finished assembling parts.')
         return works
 
     def _extract_work(self, filename):
         raise NotImplementedError
 
+    def _get_xslt(self, path):
+        ref = importlib.resources.files('tacl') / path
+        with importlib.resources.as_file(ref) as xslt_path:
+            return etree.XSLT(etree.parse(xslt_path))
+
     def get_witnesses(self, source_tree):
         """Returns a sorted list of all witnesses of readings in
         `source_tree`, and the elements that bear @wit attributes.
 
         :param source_tree: XML tree of source document
         :type source_tree: `etree._ElementTree`
         :rtype: `tuple` of `list`s
@@ -271,20 +274,17 @@
 
     work_pattern = re.compile(
         r'^(?P<prefix>[A-Z]{1,2})\d+n(?P<number>[A-Z]?\d+)(?P<part>[A-Za-z]?)$')
     xslt = 'prepare_tei_cbeta_github.xsl'
 
     def __init__(self, *args):
         super().__init__(*args)
-        div_xslt = resource_filename(
-            __name__, 'assets/xslt/CBETA_extract_div.xsl')
-        self._transform_div = etree.XSLT(etree.parse(div_xslt))
-        remove_divs_xslt = resource_filename(
-            __name__, 'assets/xslt/CBETA_remove_divs.xsl')
-        self._remove_divs = etree.XSLT(etree.parse(remove_divs_xslt))
+        self._transform_div = self._get_xslt(
+            'assets/xslt/CBETA_extract_div.xsl')
+        self._remove_divs = self._get_xslt('assets/xslt/CBETA_remove_divs.xsl')
 
     def _extract_divs(self, work, tree, div_types, exclude=None):
         """Writes out to files the individual parts of a work corresponding to
         various types of cb:div.
 
         After a div type has been extracted, it must be removed from
         the tree so that future extractions/manipulations do not
@@ -528,17 +528,15 @@
     def _postprocess_T0186(self, work, tree):
         """Post-process the XML document T0186.xml.
 
         Divide into two files, one containing all of the tei:l
         material, and one the rest.
 
         """
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_extract_verse.xsl')
-        extract_verse = etree.XSLT(etree.parse(xslt_filename))
+        extract_verse = self._get_xslt('assets/xslt/CBETA_extract_verse.xsl')
         verse_tree = extract_verse(tree)
         verse_filename = '{}-verses.xml'.format(work)
         self._output_tree(verse_filename, verse_tree)
         prose_tree = extract_verse(tree, inverse='1')
         prose_filename = '{}-ex-verses.xml'.format(work)
         self._output_tree(prose_filename, prose_tree)
 
@@ -626,17 +624,16 @@
         fact that one of the parts (T0220b) is meant to be entirely
         within the single hui of T0220a but does not have any
         containing div.
 
         Also divide into one file for each cb:div[@type='dharani'].
 
         """
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_T0220_reparent_divs.xsl')
-        move_non_hui_divs = etree.XSLT(etree.parse(xslt_filename))
+        move_non_hui_divs = self._get_xslt(
+            'assets/xslt/CBETA_T0220_reparent_divs.xsl')
         tree = move_non_hui_divs(tree)
         divs = tree.xpath('//cb:div[@type="hui"]',
                           namespaces=constants.NAMESPACES)
         for position, div in enumerate(divs):
             div_tree = self._transform_div(tree, position=str(position),
                                            div_type='"hui"')
             div_filename = '{}-{}.xml'.format(work, position + 1)
@@ -646,17 +643,16 @@
     def _postprocess_T0225(self, work, tree):
         """Post-process the XML document T0225.xml.
 
         Divide into two files, one containing all of the
         tei:note[@place='inline'] material, and one the rest.
 
         """
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_extract_commentary.xsl')
-        extract_commentary = etree.XSLT(etree.parse(xslt_filename))
+        extract_commentary = self._get_xslt(
+            'assets/xslt/CBETA_extract_commentary.xsl')
         commentary_tree = extract_commentary(tree)
         commentary_filename = '{}-commentary.xml'.format(work)
         self._output_tree(commentary_filename, commentary_tree)
         ex_commentary_tree = extract_commentary(tree, inverse='1')
         ex_commentary_filename = '{}-ex-commentary.xml'.format(work)
         self._output_tree(ex_commentary_filename, ex_commentary_tree)
 
@@ -678,17 +674,15 @@
     def _postprocess_T0328(self, work, tree):
         """Post-process the XML document T0328.xml.
 
         Divide into two files, one containing all of the tei:l
         material, and one the rest.
 
         """
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_extract_verse.xsl')
-        extract_verse = etree.XSLT(etree.parse(xslt_filename))
+        extract_verse = self._get_xslt('assets/xslt/CBETA_extract_verse.xsl')
         verse_tree = extract_verse(tree)
         verse_filename = '{}-verses.xml'.format(work)
         self._output_tree(verse_filename, verse_tree)
         prose_tree = extract_verse(tree, inverse='1')
         prose_filename = '{}-ex-verses.xml'.format(work)
         self._output_tree(prose_filename, prose_tree)
 
@@ -708,21 +702,17 @@
         Divide into two files, one containing all of the tei:l
         material, and one the rest.
 
         """
         # There are verse elements within tei:app/tei:rdg that occur
         # within a prose context and have no markup specifying that
         # they are verse, so add that in.
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_T0418_fix_verse.xsl')
-        fix_verse = etree.XSLT(etree.parse(xslt_filename))
+        fix_verse = self._get_xslt('assets/xslt/CBETA_T0418_fix_verse.xsl')
         tree = fix_verse(tree)
-        xslt_filename = resource_filename(
-            __name__, 'assets/xslt/CBETA_extract_verse.xsl')
-        extract_verse = etree.XSLT(etree.parse(xslt_filename))
+        extract_verse = self._get_xslt('assets/xslt/CBETA_extract_verse.xsl')
         verse_tree = extract_verse(tree)
         verse_filename = '{}-revised-verses.xml'.format(work)
         self._output_tree(verse_filename, verse_tree)
         prose_tree = extract_verse(tree, inverse='1')
         prose_filename = '{}-ex-verses.xml'.format(work)
         self._output_tree(prose_filename, prose_tree)
```

### Comparing `tacl-5.0.6/tacl/text.py` & `tacl-5.1.0/tacl/text.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/tokenizer.py` & `tacl-5.1.0/tacl/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl/work_joiner.py` & `tacl-5.1.0/tacl/work_joiner.py`

 * *Files identical despite different names*

### Comparing `tacl-5.0.6/tacl.egg-info/PKG-INFO` & `tacl-5.1.0/tacl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacl
-Version: 5.0.6
+Version: 5.1.0
 Summary: Text analyser for corpus linguistics
 Author-email: Jamie Norrish <jamie@artefact.org.nz>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tacl-5.0.6/tacl.egg-info/SOURCES.txt` & `tacl-5.1.0/tacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

