# Comparing `tmp/deepTools-3.5.1.tar.gz` & `tmp/deepTools-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepTools-3.5.1.tar", last modified: Wed Mar 17 14:49:30 2021, max compression
+gzip compressed data, was "dist/deepTools-3.5.2.tar", last modified: Wed Jun 14 15:06:46 2023, max compression
```

## Comparing `deepTools-3.5.1.tar` & `deepTools-3.5.2.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 14:49:30.000000 deepTools-3.5.1/
--rwxr-xr-x   0 runner    (1001) docker     (121)    38559 2021-03-17 14:48:34.000000 deepTools-3.5.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-03-17 14:48:34.000000 deepTools-3.5.1/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      158 2021-03-17 14:48:34.000000 deepTools-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2021-03-17 14:49:30.000000 deepTools-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2021-03-17 14:48:34.000000 deepTools-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-03-17 14:48:34.000000 deepTools-3.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 14:49:30.000000 deepTools-3.5.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      233 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/alignmentSieve
--rwxr-xr-x   0 runner    (1001) docker     (121)      229 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/bamCompare
--rwxr-xr-x   0 runner    (1001) docker     (121)      230 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/bamCoverage
--rwxr-xr-x   0 runner    (1001) docker     (121)      236 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/bamPEFragmentSize
--rwxr-xr-x   0 runner    (1001) docker     (121)      232 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/bigwigCompare
--rwxr-xr-x   0 runner    (1001) docker     (121)      232 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/computeGCBias
--rwxr-xr-x   0 runner    (1001) docker     (121)      326 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/computeMatrix
--rwxr-xr-x   0 runner    (1001) docker     (121)      242 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/computeMatrixOperations
--rwxr-xr-x   0 runner    (1001) docker     (121)      232 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/correctGCBias
--rwxr-xr-x   0 runner    (1001) docker     (121)      239 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/deeptools
--rwxr-xr-x   0 runner    (1001) docker     (121)      241 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/estimateReadFiltering
--rwxr-xr-x   0 runner    (1001) docker     (121)     4655 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/estimateScaleFactor
--rwxr-xr-x   0 runner    (1001) docker     (121)      326 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/multiBamSummary
--rwxr-xr-x   0 runner    (1001) docker     (121)      329 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/multiBigwigSummary
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotCorrelation
--rwxr-xr-x   0 runner    (1001) docker     (121)      232 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotCoverage
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotEnrichment
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotFingerprint
--rwxr-xr-x   0 runner    (1001) docker     (121)      230 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotHeatmap
--rwxr-xr-x   0 runner    (1001) docker     (121)      226 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotPCA
--rwxr-xr-x   0 runner    (1001) docker     (121)      230 2021-03-17 14:48:34.000000 deepTools-3.5.1/bin/plotProfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 14:49:30.000000 deepTools-3.5.1/deepTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2021-03-17 14:49:30.000000 deepTools-3.5.1/deepTools.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 14:49:30.000000 deepTools-3.5.1/deeptools/
--rw-r--r--   0 runner    (1001) docker     (121)     7008 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/SES_scaleFactor.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      179 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    17702 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/alignmentSieve.py
--rw-r--r--   0 runner    (1001) docker     (121)    14239 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/bamCompare.py
--rw-r--r--   0 runner    (1001) docker     (121)    18596 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/bamCoverage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/bamHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21011 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/bamPEFragmentSize.py
--rw-r--r--   0 runner    (1001) docker     (121)     8069 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/bigwigCompare.py
--rw-r--r--   0 runner    (1001) docker     (121)    44831 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/cm.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    30962 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/computeGCBias.py
--rw-r--r--   0 runner    (1001) docker     (121)    23264 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/computeMatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    31989 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/computeMatrixOperations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    26145 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/correctGCBias.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28053 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3796 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/correlation_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (121)    42163 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/countReadsPerBin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10950 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/deepBlue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/deeptools_list_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    16550 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/estimateReadFiltering.py
--rw-r--r--   0 runner    (1001) docker     (121)     7018 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/getFragmentAndReadSize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/getRatio.py
--rw-r--r--   0 runner    (1001) docker     (121)    12772 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/getScaleFactor.py
--rw-r--r--   0 runner    (1001) docker     (121)    11968 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/getScorePerBigWigBin.py
--rw-r--r--   0 runner    (1001) docker     (121)    58994 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/heatmapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7169 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/heatmapper_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     9786 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/mapReduce.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11655 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/multiBamSummary.py
--rw-r--r--   0 runner    (1001) docker     (121)    12675 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/multiBigwigSummary.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    45301 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/parserCommon.py
--rw-r--r--   0 runner    (1001) docker     (121)    10834 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotCorrelation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16183 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotCoverage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    25089 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotEnrichment.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19752 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotFingerprint.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37639 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     9322 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotPCA.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    39162 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/plotProfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     9902 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/sumCoveragePerBin.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14161 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    13224 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/writeBedGraph.py
--rw-r--r--   0 runner    (1001) docker     (121)     8954 2021-03-17 14:48:34.000000 deepTools-3.5.1/deeptools/writeBedGraph_bam_and_bw.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      141 2021-03-17 14:48:34.000000 deepTools-3.5.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 14:49:30.000000 deepTools-3.5.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     7412 2021-03-17 14:48:34.000000 deepTools-3.5.1/scripts/convertChromsBigWig.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      210 2021-03-17 14:48:34.000000 deepTools-3.5.1/scripts/mappabilityBigWig_to_unmappableBed.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      822 2021-03-17 14:48:34.000000 deepTools-3.5.1/scripts/split_bed_into_multiple_files.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-17 14:49:30.000000 deepTools-3.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2913 2021-03-17 14:48:34.000000 deepTools-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:46.000000 deepTools-3.5.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39240 2023-06-14 15:03:34.000000 deepTools-3.5.2/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-14 15:03:34.000000 deepTools-3.5.2/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-06-14 15:03:34.000000 deepTools-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-14 15:06:46.000000 deepTools-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-14 15:03:34.000000 deepTools-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-14 15:03:34.000000 deepTools-3.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:46.000000 deepTools-3.5.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/alignmentSieve
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/bamCompare
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/bamCoverage
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/bamPEFragmentSize
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/bigwigAverage
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/bigwigCompare
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/computeGCBias
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/computeMatrix
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/computeMatrixOperations
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/correctGCBias
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/deeptools
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/estimateReadFiltering
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4654 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/estimateScaleFactor
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/multiBamSummary
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/multiBigwigSummary
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotCorrelation
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotCoverage
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotEnrichment
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotFingerprint
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotHeatmap
+-rwxr-xr-x   0 runner    (1001) docker     (123)      226 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotPCA
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-06-14 15:03:34.000000 deepTools-3.5.2/bin/plotProfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:46.000000 deepTools-3.5.2/deepTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-14 15:06:46.000000 deepTools-3.5.2/deepTools.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:46.000000 deepTools-3.5.2/deeptools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/SES_scaleFactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/alignmentSieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14239 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bamCompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bamCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bamHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21011 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bamPEFragmentSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bigwigAverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/bigwigCompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44831 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/cm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30961 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/computeGCBias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23263 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/computeMatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31989 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/computeMatrixOperations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26144 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/correctGCBias.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28048 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/correlation_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42159 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/countReadsPerBin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/deepBlue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/deeptools_list_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16550 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/estimateReadFiltering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/getFragmentAndReadSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/getRatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/getScaleFactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/getScorePerBigWigBin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59000 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/heatmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/heatmapper_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/mapReduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/multiBamSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/multiBigwigSummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45301 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/parserCommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotCorrelation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16183 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotCoverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25089 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotEnrichment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19752 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotFingerprint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37639 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotPCA.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39160 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/plotProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/sumCoveragePerBin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14161 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/writeBedGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-14 15:03:34.000000 deepTools-3.5.2/deeptools/writeBedGraph_bam_and_bw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-14 15:03:35.000000 deepTools-3.5.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:06:46.000000 deepTools-3.5.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-06-14 15:03:35.000000 deepTools-3.5.2/scripts/convertChromsBigWig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-06-14 15:03:35.000000 deepTools-3.5.2/scripts/mappabilityBigWig_to_unmappableBed.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-06-14 15:03:35.000000 deepTools-3.5.2/scripts/split_bed_into_multiple_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:06:46.000000 deepTools-3.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2934 2023-06-14 15:03:35.000000 deepTools-3.5.2/setup.py
```

### Comparing `deepTools-3.5.1/CHANGES.txt` & `deepTools-3.5.2/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+3.5.2
+* new subcommand: Bigwig average #1169
+* dendogram of plotCorrelation now matches each cell correctly
+* Fix label options
+* add pool
+* several other bugs fixed: #1159, #1185, #1172, #1181, #1183
+* Fix galaxy tests, separate planemo and update pypi push only on tag releases
+* upload artifact
+* allow 1 or 2 lines diff for bowtie2 program
+* change github action to get artifacts
+* fix plotPCA
+* try to fix old samtools installed
+* add forgotten channels
+* default chunklength increased for alignmentSieve
+* chunklength in alignmentSieve is a CLI argument now
+* suppress lack of index warnings from pysam
+* fixedStep in bedGraph output to avoid merging bins with equal values
+
 3.5.1
 * cmp usage is updated to fit the recent mpl updates.
 * The requirements.txt is updated.
 * "NA" occurences in plotFingerprint.py have been replaced by numpy.NAN (PR #1002)
 * computeMatrixOperations.xml is fixed (brought up in #1003)
 * plotly error is fixed. (issue #1013)
 * relase version is updated in planemo.sh
```

### Comparing `deepTools-3.5.1/LICENSE.txt` & `deepTools-3.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/PKG-INFO` & `deepTools-3.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: deepTools
-Version: 3.5.1
+Version: 3.5.2
 Summary: Useful tools for exploring deep sequencing data 
 Home-page: http://pypi.python.org/pypi/deepTools/
 Author: Fidel Ramirez,  Devon P Ryan, Björn Grüning, Friederike Dündar, Sarah Diehl, Vivek Bhardwaj, Fabian Kilpert, Andreas S Richter, Steffen Heyne, Thomas Manke
 Author-email: dpryan79@gmail.com
 License: LICENSE.txt
-Description: ======================================================================
-        deepTools
-        ======================================================================
-        
-        User-friendly tools for exploring deep-sequencing data
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        deepTools addresses the challenge of handling the large amounts of data
-        that are now routinely generated from DNA sequencing centers. deepTools
-        contains useful modules to process the mapped reads data for multiple
-        quality checks, creating **normalized coverage files** in standard
-        bedGraph and bigWig file formats, that allow comparison between
-        different files (for example, treatment and control). Finally, using
-        such normalized and standardized files, deepTools can create many
-        publication-ready **visualizations** to identify enrichments and for
-        functional annotations of the genome.
-        
-        For support or questions please make a post on `Biostars <http://biostars.org>`__. For feature requests, please open an issue on `github <http://github.com/deeptools/deeptools>`__.
-        
-        For further documentation, please see our `read the docs page <http://deeptools.readthedocs.org/>`__.
-        
-        Citation:
-        ^^^^^^^^^
-        
-        Ramírez F, Ryan DP, Grüning B, Bhardwaj V, Kilpert F, Richter AS, Heyne
-        S, Dündar F, Manke T. `deepTools2: a next generation web server for
-        deep-sequencing data
-        analysis. <https://nar.oxfordjournals.org/content/early/2016/04/12/nar.gkw257.abstract>`__
-        Nucleic Acids Research. 2016 Apr 13:gkw257.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE.txt
+
+======================================================================
+deepTools
+======================================================================
+
+User-friendly tools for exploring deep-sequencing data
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+deepTools addresses the challenge of handling the large amounts of data
+that are now routinely generated from DNA sequencing centers. deepTools
+contains useful modules to process the mapped reads data for multiple
+quality checks, creating **normalized coverage files** in standard
+bedGraph and bigWig file formats, that allow comparison between
+different files (for example, treatment and control). Finally, using
+such normalized and standardized files, deepTools can create many
+publication-ready **visualizations** to identify enrichments and for
+functional annotations of the genome.
+
+For support or questions please make a post on `Biostars <http://biostars.org>`__. For feature requests, please open an issue on `github <http://github.com/deeptools/deeptools>`__.
+
+For further documentation, please see our `read the docs page <http://deeptools.readthedocs.org/>`__.
+
+Citation:
+^^^^^^^^^
+
+Ramírez F, Ryan DP, Grüning B, Bhardwaj V, Kilpert F, Richter AS, Heyne
+S, Dündar F, Manke T. `deepTools2: a next generation web server for
+deep-sequencing data
+analysis. <https://nar.oxfordjournals.org/content/early/2016/04/12/nar.gkw257.abstract>`__
+Nucleic Acids Research. 2016 Apr 13:gkw257.
```

### Comparing `deepTools-3.5.1/README.rst` & `deepTools-3.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/bin/estimateScaleFactor` & `deepTools-3.5.2/bin/estimateScaleFactor`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                          version='%(prog)s {}'.format(__version__))
 
     args=parser.parse_args(args)
     if args.ignoreForNormalization:
          args.ignoreForNormalization=[x.strip() for x in args.ignoreForNormalization.split(',')]
     else:
          args.ignoreForNormalization = []
-    return(args)
+    return args
 
 def main(args):
     """
     The algorithm samples the genome a number of times as specified
     by the --numberOfSamples parameter to estimate scaling factors of
     betweeen to samples
```

### Comparing `deepTools-3.5.1/deepTools.egg-info/SOURCES.txt` & `deepTools-3.5.2/deepTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.rst
 requirements.txt
 setup.py
 bin/alignmentSieve
 bin/bamCompare
 bin/bamCoverage
 bin/bamPEFragmentSize
+bin/bigwigAverage
 bin/bigwigCompare
 bin/computeGCBias
 bin/computeMatrix
 bin/computeMatrixOperations
 bin/correctGCBias
 bin/deeptools
 bin/estimateReadFiltering
@@ -30,14 +31,15 @@
 deeptools/__init__.py
 deeptools/_version.py
 deeptools/alignmentSieve.py
 deeptools/bamCompare.py
 deeptools/bamCoverage.py
 deeptools/bamHandler.py
 deeptools/bamPEFragmentSize.py
+deeptools/bigwigAverage.py
 deeptools/bigwigCompare.py
 deeptools/cm.py
 deeptools/computeGCBias.py
 deeptools/computeMatrix.py
 deeptools/computeMatrixOperations.py
 deeptools/correctGCBias.py
 deeptools/correlation.py
```

### Comparing `deepTools-3.5.1/deeptools/SES_scaleFactor.py` & `deepTools-3.5.2/deeptools/SES_scaleFactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     # both p and q are normalized by this value
     diff = np.abs(p / p[-1] - q / q[-1])
     # get the lowest rank for wich the difference is the maximum
     maxIndex = np.flatnonzero(diff == diff.max())[0]
     # Take a lower rank to move to a region with probably
     # less peaks and more background.
     maxIndex = int(maxIndex * 0.8)
-    while(maxIndex < len(p)):
+    while maxIndex < len(p):
         # in rare cases the maxIndex maps to a zero value.
         # In such cases, the next index is used until
         # a non zero value appears.
         cumSum = np.array([float(p[maxIndex]), float(q[maxIndex])])
         if cumSum.min() > 0:
             break
         maxIndex += 1
```

### Comparing `deepTools-3.5.1/deeptools/alignmentSieve.py` & `deepTools-3.5.2/deeptools/alignmentSieve.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
                          type=int,
                          help='Shift the left and right end of a read (for BAM files) or a fragment (for BED files). A positive value shift an end to the right (on the + strand) and a negative value shifts a fragment to the left. Either 2 or 4 integers can be provided. For example, "2 -3" will shift the left-most fragment end two bases to the right and the right-most end 3 bases to the left. If 4 integers are provided, then the first and last two refer to fragments whose read 1 is on the left or right, respectively. Consequently, it is possible to take strand into consideration for strand-specific protocols. A fragment whose length falls below 1 due to shifting will not be written to the output. See the online documentation for graphical examples. Note that non-properly-paired reads will be filtered.')
 
     general.add_argument('--ATACshift',
                          action='store_true',
                          help='Shift the produced BAM file or BEDPE regions as commonly done for ATAC-seq. This is equivalent to --shift 4 -5 5 -4.')
 
+    general.add_argument('--genomeChunkLength',
+                         type=int,
+                         default=int(1e6),
+                         help='Size of the genome (in bps) to be processed per thread. (Default: %(default)s)')
+
     output = parser.add_argument_group('Output arguments')
     output.add_argument('--BED',
                         action='store_true',
                         help='Instead of producing BAM files, write output in BEDPE format (as defined by MACS2). Note that only reads/fragments passing filtering criterion are written in BEDPE format.')
 
     filtering = parser.add_argument_group('Optional arguments')
 
@@ -200,16 +205,15 @@
 
     return b2
 
 
 def filterWorker(arglist):
     chrom, start, end, args, chromDict = arglist
     fh = openBam(args.bam)
-
-    mode = 'wbu'
+    mode = 'wb'
     oname = getTempFileName(suffix='.bam')
     if args.filteredOutReads:
         onameFiltered = getTempFileName(suffix='.bam')
     else:
         onameFiltered = None
     ofh = pysam.AlignmentFile(oname, mode=mode, template=fh)
     if onameFiltered:
@@ -345,16 +349,19 @@
     Stores results in BEDPE format, which is:
     chromosome	frag_leftend	frag_rightend
 
     The fragment ends can be shifted
     """
     ofile = open(oname, "w")
     for tmpFile in tmpFiles:
+        # Setting verbosity to avoid lack of index error/warning
+        pysam.set_verbosity(0)
         fh = pysam.AlignmentFile(tmpFile)
-
+        # Reset verbosity
+        pysam.set_verbosity(3)
         for b in fh.fetch(until_eof=True):
             tLen = getTLen(b, notAbs=True)
             if tLen > 0:
                 start = b.pos
                 end = start + tLen
                 if end > chromDict[b.reference_name]:
                     end = chromDict[b.reference_name]
@@ -383,14 +390,15 @@
 
     # Filter, writing the results to a bunch of temporary files
     res = mapReduce([args, chromDict],
                     filterWorker,
                     chrom_sizes,
                     blackListFileName=args.blackListFileName,
                     numberOfProcessors=args.numberOfProcessors,
+                    genomeChunkLength=args.genomeChunkLength,
                     verbose=args.verbose)
 
     res = sorted(res)  # The temp files are now in order for concatenation
     nFiltered = sum([x[3] for x in res])
     totalSeen = sum([x[2] for x in res])  # The * contig isn't queried
 
     tmpFiles = [x[4] for x in res]
```

### Comparing `deepTools-3.5.1/deeptools/bamCompare.py` & `deepTools-3.5.2/deeptools/bamCompare.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/bamCoverage.py` & `deepTools-3.5.2/deeptools/bamCoverage.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/bamHandler.py` & `deepTools-3.5.2/deeptools/bamHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         bam = pysam.Samfile(bamFile, 'rb', format_options=format_options)
     except IOError:
         sys.exit("The file '{}' does not exist".format(bamFile))
     except:
         sys.exit("The file '{}' does not have BAM or CRAM format ".format(bamFile))
 
     try:
-        assert(bam.check_index() is not False)
+        assert bam.check_index() is not False
     except:
         sys.exit("'{}' does not appear to have an index. You MUST index the file first!".format(bamFile))
 
     if bam.is_cram and returnStats:
         mapped, unmapped, stats = getMappingStats(bam, nThreads)
     elif bam.is_bam:
         mapped = bam.mapped
```

### Comparing `deepTools-3.5.1/deeptools/bamPEFragmentSize.py` & `deepTools-3.5.2/deeptools/bamPEFragmentSize.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/bigwigCompare.py` & `deepTools-3.5.2/deeptools/bigwigCompare.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,18 @@
                         'The decision to skip non-covered regions '
                         'depends on the interpretation of the data. Non-covered regions '
                         'in a bigWig file may represent repetitive regions that should '
                         'be skipped. Alternatively, the interpretation of non-covered regions as '
                         'zeros may be wrong and this option should be used ',
                         action='store_true')
 
+    parser.add_argument('--fixedStep',
+                        help='Write out all bins (of size --binSize) '
+                        'instead of merging neighbouring bins with equal values.',
+                        action='store_true')
     return parser
 
 
 def getType(fname):
     """
     Tries to determine if a file is a wiggle file from deepBlue or a bigWig file.
     Returns 'wiggle' if the file name ends with .wig, otherwise 'bigwig'
@@ -164,15 +168,16 @@
         blackListFileName=args.blackListFileName,
         verbose=args.verbose,
         numberOfProcessors=args.numberOfProcessors,
         skipZeroOverZero=args.skipZeroOverZero,
         format=args.outFileFormat,
         smoothLength=False,
         missingDataAsZero=not args.skipNonCoveredRegions,
-        extendPairedEnds=False)
+        extendPairedEnds=False,
+        fixedStep=args.fixedStep)
 
     # Clean up temporary bigWig files, if applicable
     if not args.deepBlueKeepTemp:
         for k, v in deepBlueFiles:
             if v == 0:
                 os.remove(args.bigwig1)
             else:
```

### Comparing `deepTools-3.5.1/deeptools/cm.py` & `deepTools-3.5.2/deeptools/cm.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/computeGCBias.py` & `deepTools-3.5.2/deeptools/computeGCBias.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         print("%s processing %d (%.1f per sec) @ %s:%s-%s %s" %
               (multiprocessing.current_process().name,
                index, index / (endTime - countTime),
                chromNameBit, start, end, stepSize))
         print("%s total time %.1f @ %s:%s-%s %s" % (multiprocessing.current_process().name,
                                                     (endTime - startTime), chromNameBit, start, end, stepSize))
 
-    return(subN_gc, subF_gc)
+    return subN_gc, subF_gc
 
 
 def tabulateGCcontent(fragmentLength, chrNameBitToBam, stepSize,
                       chromSizes, numberOfProcessors=None, verbose=False,
                       region=None):
     r"""
     Subdivides the genome or the reads into chunks to be analyzed in parallel
```

### Comparing `deepTools-3.5.1/deeptools/computeMatrix.py` & `deepTools-3.5.2/deeptools/computeMatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     elif args.command == 'reference-point':
         if args.beforeRegionStartLength == 0 and \
                 args.afterRegionStartLength == 0:
             sys.exit("\nUpstrean and downstream regions are both "
                      "set to 0. Nothing to output. Maybe you want to "
                      "use the scale-regions mode?\n")
 
-    return(args)
+    return args
 
 
 def main(args=None):
 
     args = process_args(args)
 
     parameters = {'upstream': args.beforeRegionStartLength,
```

### Comparing `deepTools-3.5.1/deeptools/computeMatrixOperations.py` & `deepTools-3.5.2/deeptools/computeMatrixOperations.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/correctGCBias.py` & `deepTools-3.5.2/deeptools/correctGCBias.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
         gc = None
 
         # check if a mate has already been procesed
         # to apply the same correction
         try:
             copies = matePairs[read.qname]['copies']
             gc = matePairs[read.qname]['gc']
-            del(matePairs[read.qname])
+            del matePairs[read.qname]
         except:
             # this exception happens when a mate is
             # not present. This could
             # happen because of removal of the mate
             # by some filtering
             gc = getReadGCcontent(tbit, read, fragmentLength,
                                   chrNameBit)
```

### Comparing `deepTools-3.5.1/deeptools/correlation.py` & `deepTools-3.5.2/deeptools/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,17 +281,17 @@
         if vmin is None:
             vmin = 0 if corr_matrix .min() >= 0 else -1
 
         # Compute and plot dendrogram.
         fig = plt.figure(figsize=(plotWidth, plotHeight))
         plt.suptitle(plot_title)
 
-        axdendro = fig.add_axes([0.02, 0.12, 0.1, 0.66])
+        axdendro = fig.add_axes([0.015, 0.1, 0.1, 0.7])
         axdendro.set_axis_off()
-        y_var = sch.linkage(corr_matrix, method='complete')
+        y_var = sch.linkage(corr_matrix, method='centroid')
         z_var = sch.dendrogram(y_var, orientation='left',
                                link_color_func=lambda k: 'darkred')
         axdendro.set_xticks([])
         axdendro.set_yticks([])
         cmap = copy.copy(plt.get_cmap(colormap))
 
         # this line simply makes a new cmap, based on the original
@@ -302,15 +302,15 @@
         # plotted on black.
         if plot_numbers:
             cmap = pltcolors.LinearSegmentedColormap.from_list(colormap + "clipped",
                                                                cmap(np.linspace(0, 0.9, 10)))
 
         cmap.set_under((0., 0., 1.))
         # Plot distance matrix.
-        axmatrix = fig.add_axes([0.13, 0.1, 0.6, 0.7])
+        axmatrix = fig.add_axes([0.12, 0.1, 0.6, 0.7])
         index = z_var['leaves']
         corr_matrix = corr_matrix[index, :]
         corr_matrix = corr_matrix[:, index]
         if corr_matrix.shape[0] > 30:
             # when there are too many rows it is better to remove
             # the black lines surrounding the boxes in the heatmap
             edge_color = 'none'
@@ -354,15 +354,15 @@
         axmatrix.tick_params(
             axis='y',
             which='both',
             left=False,
             right=False)
 
         # Plot colorbar
-        axcolor = fig.add_axes([0.13, 0.065, 0.6, 0.02])
+        axcolor = fig.add_axes([0.12, 0.065, 0.6, 0.02])
         cobar = plt.colorbar(img_mat, cax=axcolor, orientation='horizontal')
         cobar.solids.set_edgecolor("face")
         if plot_numbers:
             for row in range(num_rows):
                 for col in range(num_rows):
                     axmatrix.text(row + 0.5, col + 0.5,
                                   "{:.2f}".format(corr_matrix[row, col]),
@@ -500,15 +500,15 @@
 
             ax.get_xaxis().set_tick_params(
                 which='both',
                 top=False,
                 bottom=False,
                 direction='out')
             for tick in ax.xaxis.get_major_ticks():
-                tick.label.set_rotation('45')
+                tick.label.set_rotation(45)
 
             if col != num_samples - 1:
                 ax.set_yticklabels([])
             else:
                 ax.yaxis.tick_right()
                 ax.get_yaxis().set_tick_params(
                     which='both',
@@ -519,15 +519,15 @@
                 ax.xaxis.tick_bottom()
                 ax.get_xaxis().set_tick_params(
                     which='both',
                     top=False,
                     bottom=True,
                     direction='out')
                 for tick in ax.xaxis.get_major_ticks():
-                    tick.label.set_rotation('45')
+                    tick.label.set_rotation(45)
 
             else:
                 ax.set_xticklabels([])
 
             ax.set_xlim(min_xvalue, max_xvalue)
             ax.set_ylim(min_yvalue, max_yvalue)
             ax.hist2d(vector2, vector1, bins=200, cmin=0.1)
```

### Comparing `deepTools-3.5.1/deeptools/correlation_heatmap.py` & `deepTools-3.5.2/deeptools/correlation_heatmap.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/countReadsPerBin.py` & `deepTools-3.5.2/deeptools/countReadsPerBin.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,17 +856,17 @@
         >>> c.get_fragment_from_read(test.getRead("paired-forward"))
         [(5000000, 5000036)]
 
         Tests for read centering.
 
         >>> c = CountReadsPerBin([], 1, 1, 200, extendReads=True, center_read=True)
         >>> c.defaultFragmentLength = 100
-        >>> assert(c.get_fragment_from_read(test.getRead("paired-forward")) == [(5000032, 5000068)])
+        >>> assert c.get_fragment_from_read(test.getRead("paired-forward")) == [(5000032, 5000068)]
         >>> c.defaultFragmentLength = 200
-        >>> assert(c.get_fragment_from_read(test.getRead("single-reverse")) == [(5001618, 5001654)])
+        >>> assert c.get_fragment_from_read(test.getRead("single-reverse")) == [(5001618, 5001654)]
         """
         # if no extension is needed, use pysam get_blocks
         # to identify start and end reference positions.
         # get_blocks return a list of start and end positions
         # based on the CIGAR if skipped regions are found.
         # E.g for a cigar of 40M260N22M
         # get blocks return two elements for the first 40 matches
@@ -973,18 +973,18 @@
     Compute size factors in the same way as DESeq2.
     The inverse of that is returned, as it's then compatible with bamCoverage.
 
     m : a numpy ndarray
 
     >>> m = np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 10, 0], [10, 5, 100]])
     >>> sf = estimateSizeFactors(m)
-    >>> assert(np.all(np.abs(sf - [1.305, 0.9932, 0.783]) < 1e-4))
+    >>> assert np.all(np.abs(sf - [1.305, 0.9932, 0.783]) < 1e-4)
     >>> m = np.array([[0, 0], [0, 1], [1, 1], [1, 2]])
     >>> sf = estimateSizeFactors(m)
-    >>> assert(np.all(np.abs(sf - [1.1892, 0.8409]) < 1e-4))
+    >>> assert np.all(np.abs(sf - [1.1892, 0.8409]) < 1e-4)
     """
     loggeomeans = np.sum(np.log(m), axis=1) / m.shape[1]
     # Mask after computing the geometric mean
     m = np.ma.masked_where(m <= 0, m)
     loggeomeans = np.ma.masked_where(np.isinf(loggeomeans), loggeomeans)
     # DESeq2 ratio-based size factor
     sf = np.exp(np.ma.median((np.log(m).T - loggeomeans).T, axis=0))
```

### Comparing `deepTools-3.5.1/deeptools/deepBlue.py` & `deepTools-3.5.2/deeptools/deepBlue.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 class deepBlue(object):
     def __init__(self, sample, url="http://deepblue.mpi-inf.mpg.de/xmlrpc", userKey="anonymous_key"):
         """
         Connect to the requested deepblue server with the given user key and request the specifed sample from it.
 
         >>> sample = "S002R5H1.ERX300721.H3K4me3.bwa.GRCh38.20150528.bedgraph"
         >>> db = deepBlue(sample) # doctest: +SKIP
-        >>> assert(db.chroms("chr1") == 248956422) # doctest: +SKIP
+        >>> assert db.chroms("chr1") == 248956422 # doctest: +SKIP
         """
         self.sample = sample
         self.url = url
         self.userKey = userKey
         self.server = xmlrpclib.Server(url, allow_none=True)
         self.info = None
         self.experimentID = None
```

### Comparing `deepTools-3.5.1/deeptools/deeptools_list_tools.py` & `deepTools-3.5.2/deeptools/deeptools_list_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 [ Tools for BAM and bigWig file processing ]
     multiBamSummary         compute read coverages over bam files. Output used for plotCorrelation or plotPCA
     multiBigwigSummary      extract scores from bigwig files. Output used for plotCorrelation or plotPCA
     correctGCBias           corrects GC bias from bam file. Don't use it with ChIP data
     bamCoverage             computes read coverage per bins or regions
     bamCompare              computes log2 ratio and other operations of read coverage of two samples per bins or regions
     bigwigCompare           computes log2 ratio and other operations from bigwig scores of two samples per bins or regions
+    bigwigAverage           computes average from bigwig scores of multiple samples per bins or regions
     computeMatrix           prepares the data from bigwig scores for plotting with plotHeatmap or plotProfile
     alignmentSieve          filters BAM alignments according to specified parameters, optionally producing a BEDPE file
 
 
 [ Tools for QC ]
     plotCorrelation         plots heatmaps or scatterplots of data correlation
     plotPCA                 plots PCA
```

### Comparing `deepTools-3.5.1/deeptools/estimateReadFiltering.py` & `deepTools-3.5.2/deeptools/estimateReadFiltering.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/getFragmentAndReadSize.py` & `deepTools-3.5.2/deeptools/getFragmentAndReadSize.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/getRatio.py` & `deepTools-3.5.2/deeptools/getRatio.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/getScaleFactor.py` & `deepTools-3.5.2/deeptools/getScaleFactor.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/getScorePerBigWigBin.py` & `deepTools-3.5.2/deeptools/getScorePerBigWigBin.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     """
     Get chromosome sizes from bigWig file with pyBigWig
 
     Test dataset with two samples covering 200 bp.
     >>> test = Tester()
 
     Chromosome name(s) and size(s).
-    >>> assert(getChromSizes([test.bwFile1, test.bwFile2]) == ([('3R', 200)], set([])))
+    >>> assert getChromSizes([test.bwFile1, test.bwFile2]) == ([('3R', 200)], set([]))
     """
     def print_chr_names_and_size(chr_set):
         sys.stderr.write("chromosome\tlength\n")
         for name, size in chr_set:
             sys.stderr.write("{0:>15}\t{1:>10}\n".format(name, size))
 
     bigwigFilesList = bigwigFilesList[:]
```

### Comparing `deepTools-3.5.1/deeptools/heatmapper.py` & `deepTools-3.5.2/deeptools/heatmapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -773,15 +773,15 @@
                 self.parameters = json.loads(line[1:].strip())
                 max_group_bound = self.parameters['group_boundaries'][1]
                 continue
 
             # split the line into bed interval and matrix values
             region = line.split('\t')
             chrom, start, end, name, score, strand = region[0:6]
-            matrix_row = np.ma.masked_invalid(np.fromiter(region[6:], np.float))
+            matrix_row = np.ma.masked_invalid(np.fromiter(region[6:], np.float64))
             matrix_rows.append(matrix_row)
             starts = start.split(",")
             ends = end.split(",")
             regs = [(int(x), int(y)) for x, y in zip(starts, ends)]
             # get the group index
             if len(regions) >= max_group_bound:
                 current_group_index += 1
@@ -848,15 +848,15 @@
         params_str = json.dumps(h, separators=(',', ':'))
         fh.write(toBytes("@" + params_str + "\n"))
         score_list = np.ma.masked_invalid(np.mean(self.matrix.matrix, axis=1))
         for idx, region in enumerate(self.matrix.regions):
             # join np_array values
             # keeping nans while converting them to strings
             if not np.ma.is_masked(score_list[idx]):
-                np.float(score_list[idx])
+                np.float64(score_list[idx])
             matrix_values = "\t".join(
                 np.char.mod('%f', self.matrix.matrix[idx, :]))
             starts = ["{0}".format(x[0]) for x in region[1]]
             ends = ["{0}".format(x[1]) for x in region[1]]
             starts = ",".join(starts)
             ends = ",".join(ends)
             # BEDish format (we don't currently store the score)
@@ -1341,15 +1341,15 @@
     def removeempty(self):
         """
         removes matrix rows containing only zeros or nans
         """
         to_keep = []
         score_list = np.ma.masked_invalid(np.mean(self.matrix, axis=1))
         for idx, region in enumerate(self.regions):
-            if np.ma.is_masked(score_list[idx]) or np.float(score_list[idx]) == 0:
+            if np.ma.is_masked(score_list[idx]) or np.float64(score_list[idx]) == 0:
                 continue
             else:
                 to_keep.append(idx)
         self.regions = [self.regions[x] for x in to_keep]
         self.matrix = self.matrix[to_keep, :]
         # adjust sample boundaries
         to_keep = np.array(to_keep)
```

### Comparing `deepTools-3.5.1/deeptools/heatmapper_utilities.py` & `deepTools-3.5.2/deeptools/heatmapper_utilities.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/mapReduce.py` & `deepTools-3.5.2/deeptools/mapReduce.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/misc.py` & `deepTools-3.5.2/deeptools/misc.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/multiBamSummary.py` & `deepTools-3.5.2/deeptools/multiBamSummary.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/multiBigwigSummary.py` & `deepTools-3.5.2/deeptools/multiBigwigSummary.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/parserCommon.py` & `deepTools-3.5.2/deeptools/parserCommon.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotCorrelation.py` & `deepTools-3.5.2/deeptools/plotCorrelation.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotCoverage.py` & `deepTools-3.5.2/deeptools/plotCoverage.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotEnrichment.py` & `deepTools-3.5.2/deeptools/plotEnrichment.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotFingerprint.py` & `deepTools-3.5.2/deeptools/plotFingerprint.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotHeatmap.py` & `deepTools-3.5.2/deeptools/plotHeatmap.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotPCA.py` & `deepTools-3.5.2/deeptools/plotPCA.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/plotProfile.py` & `deepTools-3.5.2/deeptools/plotProfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
 
 def process_args(args=None):
     args = parse_arguments().parse_args(args)
 
     # Ensure that yMin/yMax are there and a list
     try:
-        assert(args.yMin is not None)
+        assert args.yMin is not None
     except:
         args.yMin = [None]
     try:
-        assert(args.yMax is not None)
+        assert args.yMax is not None
     except:
         args.yMax = [None]
 
     # Sometimes Galaxy sends --yMax '' and --yMin ''
     if args.yMin == ['']:
         args.yMin = [None]
     if args.yMax == ['']:
```

### Comparing `deepTools-3.5.1/deeptools/sumCoveragePerBin.py` & `deepTools-3.5.2/deeptools/sumCoveragePerBin.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             try:
                 # BAM input
                 if chrom not in bamHandle.references:
                     raise NameError("chromosome {} not found in bam file".format(chrom))
             except:
                 # bigWig input, as used by plotFingerprint
                 if bamHandle.chroms(chrom):
-                    _ = np.array(bamHandle.stats(chrom, regStart, regEnd, type="mean", nBins=nRegBins), dtype=np.float)
+                    _ = np.array(bamHandle.stats(chrom, regStart, regEnd, type="mean", nBins=nRegBins), dtype=np.float64)
                     _[np.isnan(_)] = 0.0
                     _ = _ * tileSize
                     coverages += _
                     continue
                 else:
                     raise NameError("chromosome {} not found in bigWig file with chroms {}".format(chrom, bamHandle.chroms()))
```

### Comparing `deepTools-3.5.1/deeptools/utilities.py` & `deepTools-3.5.2/deeptools/utilities.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/deeptools/writeBedGraph.py` & `deepTools-3.5.2/deeptools/writeBedGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
 def bedGraphToBigWig(chromSizes, bedGraphFiles, bigWigPath):
     """
     Takes a sorted list of bedgraph files and write them to a single bigWig file using pyBigWig.
     The order of bedGraphFiles must match that of chromSizes!
     """
     bw = pyBigWig.open(bigWigPath, "w")
-    assert(bw is not None)
+    assert bw is not None
     bw.addHeader(chromSizes, maxZooms=10)
     lastChrom = None
     starts = []
     ends = []
     vals = []
     for bg in bedGraphFiles:
         if bg is not None:
```

### Comparing `deepTools-3.5.1/deeptools/writeBedGraph_bam_and_bw.py` & `deepTools-3.5.2/deeptools/writeBedGraph_bam_and_bw.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def writeBedGraph_wrapper(args):
     return writeBedGraph_worker(*args)
 
 
 def writeBedGraph_worker(
         chrom, start, end, tileSize, defaultFragmentLength,
         bamOrBwFileList, func, funcArgs, extendPairedEnds=True, smoothLength=0,
-        skipZeroOverZero=False, missingDataAsZero=False, fixed_step=False):
+        skipZeroOverZero=False, missingDataAsZero=False, fixedStep=False):
     r"""
     Writes a bedgraph having as base a number of bam files.
 
     The given func is called to compute the desired bedgraph value
     using the funcArgs
 
     tileSize
@@ -99,20 +99,20 @@
 
         if skipZeroOverZero and np.sum(tileCoverage) == 0:
             previousValue = None
             continue
 
         value = func(tileCoverage, funcArgs)
 
-        if fixed_step:
+        if fixedStep:
             writeStart = start + tileIndex * tileSize
             writeEnd = min(writeStart + tileSize, end)
             try:
-                _file.write(toBytes("%s\t%d\t%d\t%.2f\n" % (chrom, writeStart,
-                                                            writeEnd, value)))
+                _file.write(toBytes("{0}\t{1}\t{2}\t{3:g}\n".format(chrom, writeStart,
+                                                                    writeEnd, value)))
             except TypeError:
                 _file.write(toBytes("{}\t{}\t{}\t{}\n".format(chrom, writeStart,
                                                               writeEnd, value)))
         else:
             if previousValue is None:
                 writeStart = start + tileIndex * tileSize
                 writeEnd = min(writeStart + tileSize, end)
@@ -126,15 +126,15 @@
                     _file.write(
                         toBytes("{0}\t{1}\t{2}\t{3:g}\n".format(chrom, writeStart,
                                                                 writeEnd, previousValue)))
                 previousValue = value
                 writeStart = writeEnd
                 writeEnd = min(writeStart + tileSize, end)
 
-    if not fixed_step:
+    if not fixedStep:
         # write remaining value if not a nan
         if previousValue and writeStart != end and \
                 not np.isnan(previousValue):
             _file.write(toBytes("{0}\t{1}\t{2}\t{3:g}\n".format(chrom, writeStart,
                                                                 end, previousValue)))
 
     tempFileName = _file.name
@@ -142,15 +142,15 @@
     return chrom, start, end, tempFileName
 
 
 def writeBedGraph(
         bamOrBwFileList, outputFileName, fragmentLength,
         func, funcArgs, tileSize=25, region=None, blackListFileName=None, numberOfProcessors=1,
         format="bedgraph", extendPairedEnds=True, missingDataAsZero=False,
-        skipZeroOverZero=False, smoothLength=0, fixed_step=False, verbose=False):
+        skipZeroOverZero=False, smoothLength=0, fixedStep=False, verbose=False):
     r"""
     Given a list of bamfiles, a function and a function arguments,
     this method writes a bedgraph file (or bigwig) file
     for a partition of the genome into tiles of given size
     and a value for each tile that corresponds to the given function
     and that is related to the coverage underlying the tile.
 
@@ -192,24 +192,27 @@
                         chromNamesAndSize[chromName] = min(
                             chromNamesAndSize[chromName], size)
                 else:
                     chromNamesAndSize[chromName] = size
             fh.close()
 
         # get the list of common chromosome names and sizes
-        chromNamesAndSize = [(k, v) for k, v in chromNamesAndSize.items()
-                             if k in cCommon]
+        if len(bamOrBwFileList) == 1:
+            chromNamesAndSize = [(k, v) for k, v in chromNamesAndSize.items()]
+        else:
+            chromNamesAndSize = [(k, v) for k, v in chromNamesAndSize.items()
+                                 if k in cCommon]
 
     if region:
         # in case a region is used, append the tilesize
         region += ":{}".format(tileSize)
 
     res = mapReduce.mapReduce((tileSize, fragmentLength, bamOrBwFileList,
                                func, funcArgs, extendPairedEnds, smoothLength,
-                               skipZeroOverZero, missingDataAsZero, fixed_step),
+                               skipZeroOverZero, missingDataAsZero, fixedStep),
                               writeBedGraph_wrapper,
                               chromNamesAndSize,
                               genomeChunkLength=genomeChunkLength,
                               region=region,
                               blackListFileName=blackListFileName,
                               numberOfProcessors=numberOfProcessors,
                               verbose=verbose)
```

### Comparing `deepTools-3.5.1/scripts/convertChromsBigWig.py` & `deepTools-3.5.2/scripts/convertChromsBigWig.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/scripts/split_bed_into_multiple_files.py` & `deepTools-3.5.2/scripts/split_bed_into_multiple_files.py`

 * *Files identical despite different names*

### Comparing `deepTools-3.5.1/setup.py` & `deepTools-3.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     packages=find_packages(),
     scripts=['bin/bamCompare', 'bin/bamCoverage', 'bin/multiBamSummary',
              'bin/plotHeatmap', 'bin/plotFingerprint', 'bin/estimateScaleFactor',
              'bin/bamPEFragmentSize', 'bin/computeMatrix', 'bin/plotProfile',
              'bin/computeGCBias', 'bin/correctGCBias', 'bin/multiBigwigSummary',
              'bin/bigwigCompare', 'bin/plotCoverage', 'bin/plotPCA', 'bin/plotCorrelation',
              'bin/plotEnrichment', 'bin/deeptools', 'bin/computeMatrixOperations',
-             'bin/estimateReadFiltering', 'bin/alignmentSieve'],
+             'bin/estimateReadFiltering', 'bin/alignmentSieve', 'bin/bigwigAverage'],
     include_package_data=True,
     url='http://pypi.python.org/pypi/deepTools/',
     license='LICENSE.txt',
     description='Useful tools for exploring deep sequencing data ',
     long_description=openREADME(),
     classifiers=[
         'Intended Audience :: Science/Research',
```

