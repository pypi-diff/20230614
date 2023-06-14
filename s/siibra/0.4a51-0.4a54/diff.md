# Comparing `tmp/siibra-0.4a51.tar.gz` & `tmp/siibra-0.4a54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a51.tar", last modified: Tue May 30 15:17:41 2023, max compression
+gzip compressed data, was "siibra-0.4a54.tar", last modified: Wed Jun 14 07:14:03 2023, max compression
```

## Comparing `siibra-0.4a51.tar` & `siibra-0.4a54.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.917296 siibra-0.4a51/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 15:16:11.000000 siibra-0.4a51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 15:16:11.000000 siibra-0.4a51/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-30 15:17:41.913296 siibra-0.4a51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-30 15:16:11.000000 siibra-0.4a51/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:17:41.917296 siibra-0.4a51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-30 15:16:11.000000 siibra-0.4a51/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.901295 siibra-0.4a51/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/streamline_lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/connectivity/tracer_connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.909296 siibra-0.4a51/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26563 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-05-30 15:16:11.000000 siibra-0.4a51/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.905295 siibra-0.4a51/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 15:17:41.000000 siibra-0.4a51/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:17:41.913296 siibra-0.4a51/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 15:16:11.000000 siibra-0.4a51/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.514327 siibra-0.4a54/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 07:12:46.000000 siibra-0.4a54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 07:12:46.000000 siibra-0.4a54/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-14 07:14:03.514327 siibra-0.4a54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-14 07:12:46.000000 siibra-0.4a54/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:14:03.514327 siibra-0.4a54/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-14 07:12:46.000000 siibra-0.4a54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.502327 siibra-0.4a54/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/connectivity/tracer_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.510327 siibra-0.4a54/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.510327 siibra-0.4a54/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.510327 siibra-0.4a54/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.510327 siibra-0.4a54/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.510327 siibra-0.4a54/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.514327 siibra-0.4a54/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.514327 siibra-0.4a54/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42302 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-14 07:12:46.000000 siibra-0.4a54/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.506327 siibra-0.4a54/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-14 07:14:03.000000 siibra-0.4a54/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-14 07:14:03.000000 siibra-0.4a54/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:14:03.000000 siibra-0.4a54/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 07:14:03.000000 siibra-0.4a54/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 07:14:03.000000 siibra-0.4a54/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:14:03.514327 siibra-0.4a54/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-14 07:12:46.000000 siibra-0.4a54/test/test_siibra.py
```

### Comparing `siibra-0.4a51/LICENSE` & `siibra-0.4a54/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/PKG-INFO` & `siibra-0.4a54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a51
+Version: 0.4a54
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a51/README.rst` & `siibra-0.4a54/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/setup.py` & `siibra-0.4a54/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/__init__.py` & `siibra-0.4a54/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/commons.py` & `siibra-0.4a54/siibra/commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,23 +41,25 @@
 SIIBRA_USE_CONFIGURATION = os.getenv("SIIBRA_USE_CONFIGURATION")
 
 SIIBRA_USE_LOCAL_SNAPSPOT = os.getenv("SIIBRA_USE_LOCAL_SNAPSPOT")
 
 with open(os.path.join(ROOT_DIR, "VERSION"), "r") as fp:
     __version__ = fp.read().strip()
 
+
 @dataclass
 class CompareMapsResult:
     intersection_over_union: float
     intersection_over_first: float
     intersection_over_second: float
     correlation: float
     weighted_mean_of_first: float
     weighted_mean_of_second: float
 
+
 T = TypeVar("T")
 
 
 class InstanceTable(Generic[T], Iterable):
     """
     Lookup table for instances of a given class by name/id.
     Provide attribute-access and iteration to a set of named elements,
@@ -239,14 +241,15 @@
                             attribute: val.__getattribute__(attribute).name
                             for attribute in ['parcellation', 'space', 'maptype']
                         }
                     )
             self._dataframe_cached = pd.DataFrame(index=list(self._elements.keys()), data=attrs)
         return self._dataframe_cached
 
+
 class LoggingContext:
     def __init__(self, level):
         self.level = level
 
     def __enter__(self):
         self.old_level = logger.level
         logger.setLevel(self.level)
@@ -260,21 +263,21 @@
 
 
 set_log_level(SIIBRA_LOG_LEVEL)
 QUIET = LoggingContext("ERROR")
 VERBOSE = LoggingContext("DEBUG")
 
 
-def siibra_tqdm(iterable: Iterable[T]=None, *args, **kwargs):
+def siibra_tqdm(iterable: Iterable[T] = None, *args, **kwargs):
     return tqdm(
         iterable,
         *args,
         disable=kwargs.pop("disable", False) or (logger.level > 20),
         **kwargs
-        )
+    )
 
 
 def create_key(name: str):
     """
     Creates an uppercase identifier string that includes only alphanumeric
     characters and underscore from a natural language name.
     """
```

### Comparing `siibra-0.4a51/siibra/configuration/__init__.py` & `siibra-0.4a54/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/configuration/configuration.py` & `siibra-0.4a54/siibra/configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,14 @@
     CONFIGURATIONS = [
         GitlabConnector(server, project, "siibra-{}".format(__version__), skip_branchtest=True)
         for server, project in CONFIG_REPOS
     ]
 
     CONFIGURATION_EXTENSIONS = []
 
-
-
     _cleanup_funcs = []
 
     @staticmethod
     def get_folders(connector: RepositoryConnector):
         return {
             path.dirname(f)
             for f in connector.search_files(suffix='.json', recursive=True)
```

### Comparing `siibra-0.4a51/siibra/configuration/factory.py` & `siibra-0.4a54/siibra/configuration/factory.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/core/__init__.py` & `siibra-0.4a54/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/core/atlas.py` & `siibra-0.4a54/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/core/concept.py` & `siibra-0.4a54/siibra/core/concept.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,24 +84,24 @@
         self._species_cached = None if species is None \
             else Species.decode(species)  # overwritable property implementation below
         self.shortname = shortname
         self.modality = modality
         self._description = description
         self._publications = publications
         self.datasets = datasets
-    
+
     @property
     def description(self):
         if self._description:
             return self._description
         for ds in self.datasets:
             if ds.description:
                 return ds.description
         return ''
-    
+
     @property
     def publications(self) -> List[TypePublication]:
         return [
             *self._publications,
             *[{
                 'citation': 'DOI',
                 'url': url.get("url")
```

### Comparing `siibra-0.4a51/siibra/core/parcellation.py` & `siibra-0.4a54/siibra/core/parcellation.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Hierarchal brain regions and metadata."""
 from . import region
 
-from ..commons import logger, MapType, MapIndex, Species
+from ..commons import logger, MapType, Species
 from ..volumes import parcellationmap
 
 from typing import Union, List, Dict
 import re
 
 
 # NOTE : such code could be used to automatically resolve
@@ -280,15 +280,15 @@
             - a Region object
         find_topmost: bool, default: True
             If True, will automatically return the parent of a decoded region
             the decoded region is its only child.
         allow_tuple: bool, default: False
             If multiple candidates without a common parent are found,
             return a tuple of matches instead of raising an exception.
-            
+
         Returns
         -------
         Region
             A region object defined in the parcellation
 
         Raises
         ------
```

### Comparing `siibra-0.4a51/siibra/core/region.py` & `siibra-0.4a54/siibra/core/region.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,25 +39,26 @@
 from dataclasses import dataclass, field
 
 
 REGEX_TYPE = type(re.compile("test"))
 
 THRESHOLD_STATISTICAL_MAPS = None
 
+
 @dataclass
 class SpatialPropCmpt:
     centroid: point.Point
     volume: int
 
 
 @dataclass
 class SpatialProp:
-    cog:SpatialPropCmpt=None
-    components:List[SpatialPropCmpt]=field(default_factory=list)
-    space:_space.Space=None
+    cog: SpatialPropCmpt = None
+    components: List[SpatialPropCmpt] = field(default_factory=list)
+    space: _space.Space = None
 
 
 class Region(anytree.NodeMixin, concept.AtlasConcept):
     """
     Representation of a region with name and more optional attributes
     """
```

### Comparing `siibra-0.4a51/siibra/core/space.py` & `siibra-0.4a54/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/__init__.py` & `siibra-0.4a54/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/anchor.py` & `siibra-0.4a54/siibra/features/anchor.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 self.species = {sp}
         self._location_cached = location
         self._assignments = {}
         self._last_matched_concept = None
         self._regions_cached = None
         self._regionspec = None
         if isinstance(region, Region):
-            self._regions_cached = { region: AssignmentQualification.EXACT }
+            self._regions_cached = {region: AssignmentQualification.EXACT}
         elif isinstance(region, str):
             self._regionspec = region
         else:
             if region is not None:
                 raise ValueError(f"Invalid region specification: {region}")
         self._aliases_cached = None
 
@@ -177,15 +177,15 @@
         # decoding region strings is quite compute intensive, so we cache this at the class level
         if self._regions_cached is not None:
             return self._regions_cached
 
         if self._regionspec is None:
             self._regions_cached = {}
             return self._regions_cached
-            
+
         if self._regionspec not in self.__class__._MATCH_MEMO:
             self._regions_cached = {}
             # decode the region specification into a set of region objects
             regions = {
                 r: AssignmentQualification.EXACT
                 for species in self.species
                 for r in Parcellation.find_regions(self._regionspec, species)
@@ -194,15 +194,15 @@
             for alt_species, aliases in self.region_aliases.items():
                 for regionspec, qualificationspec in aliases.items():
                     for r in Parcellation.find_regions(regionspec, alt_species):
                         if r not in self._regions_cached:
                             regions[r] = AssignmentQualification[qualificationspec.upper()]
             self.__class__._MATCH_MEMO[self._regionspec] = regions
         self._regions_cached = self.__class__._MATCH_MEMO[self._regionspec]
-        
+
         return self._regions_cached
 
     def __str__(self):
         region = "" if self._regionspec is None else str(self._regionspec)
         location = "" if self.location is None else str(self.location)
         separator = " " if min(len(region), len(location)) > 0 else ""
         return region + separator + location
```

### Comparing `siibra-0.4a51/siibra/features/connectivity/__init__.py` & `siibra-0.4a54/siibra/features/connectivity/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 from .functional_connectivity import FunctionalConnectivity
 from .streamline_counts import StreamlineCounts
 from .streamline_lengths import StreamlineLengths
 from .tracer_connectivity import TracerConnectivity
 
+
 def __dir__():
     return [
         "FunctionalConnectivity",
         "StreamlineCounts",
         "StreamlineLengths",
         "TracerConnectivity"
     ]
```

### Comparing `siibra-0.4a51/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a54/siibra/features/connectivity/functional_connectivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import regional_connectivity
 from hashlib import md5
 
+
 class FunctionalConnectivity(
     regional_connectivity.RegionalConnectivity,
     configuration_folder="features/connectivity/regional/functional",
     category="connectivity"
 ):
     """Functional connectivity matrix grouped by a parcellation."""
 
     def __init__(self, paradigm: str, **kwargs):
         regional_connectivity.RegionalConnectivity.__init__(self, **kwargs)
         self.paradigm = paradigm
 
         # paradign is used to distinguish functional connectivity features from each other.
-        assert self.paradigm, f"Functional connectivity must have paradigm defined!"
+        assert self.paradigm, "Functional connectivity must have paradigm defined!"
 
     @property
     def id(self):
         return super().id + "--" + md5(self.paradigm.encode("utf-8")).hexdigest()
```

### Comparing `siibra-0.4a51/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a54/siibra/features/connectivity/regional_connectivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from ...locations import pointset
 from ...retrieval.repositories import RepositoryConnector
 
 from typing import Callable, Dict, Union, List
 import pandas as pd
 import numpy as np
 
+
 class RegionalConnectivity(Feature):
     """
     Parcellation-averaged connectivity, providing one or more matrices of a
     given modality for a given parcellation.
     """
 
     def __init__(
@@ -156,15 +157,15 @@
             Can take all the arguments `nilearn.plotting.plot_matrix` can take. See the doc at
             https://nilearn.github.io/stable/modules/generated/nilearn.plotting.plot_matrix.html
         """
         if regions is None:
             regions = self.regions
         indices = [self.regions.index(r) for r in regions]
         matrix = self.get_matrix(subject=subject).iloc[indices, indices].to_numpy()  # nilearn.plotting.plot_matrix works better with a numpy array
-        
+
         if logscale:
             matrix = np.log10(matrix)
 
         # default kwargs
         subject_title = subject or ""
         kwargs["title"] = kwargs.get(
             "title",
```

### Comparing `siibra-0.4a51/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a54/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a54/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/connectivity/tracer_connectivity.py` & `siibra-0.4a54/siibra/features/connectivity/tracer_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/dataset/__init__.py` & `siibra-0.4a54/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/dataset/ebrains.py` & `siibra-0.4a54/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/feature.py` & `siibra-0.4a54/siibra/features/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,27 +184,27 @@
         if len(id_set) == 1:
             prefix = list(id_set)[0] + '--'
         return prefix + md5(self.name.encode("utf-8")).hexdigest()
 
     @staticmethod
     def serialize_query_context(feat: 'Feature', concept: concept.AtlasConcept) -> str:
         """
-        Serialize feature from livequery and query context. 
+        Serialize feature from livequery and query context.
 
         It is currently impossible to retrieve a livequery with a generic UUID.
         As such, the query context (e.g. region, space or parcellation) needs to
         be encoded in the id.
 
         Whilst it is possible to (de)serialize *any* queries, the method is setup to only serialize
         livequery features.
 
         The serialized livequery id follows the following pattern:
 
         <livequeryid_version>::<feature_cls_name>::<query_context>::<unserialized_id>
-        
+
         Where:
 
         - livequeryid_version: version of the serialization. (e.g. lq0)
         - feature_cls_name: class name to query. (e.g. BigBrainIntensityProfile)
         - query_context: string to retrieve atlas concept in the query context. Can be one of the following:
             - s:<space_id>
             - p:<parcellation_id>
@@ -229,15 +229,15 @@
             raise EncodeLiveQueryIdException("no concept is encoded")
 
         return f"lq0::{feat.__class__.__name__}::{'::'.join(encoded_c)}::{feat.id}"
 
     @classmethod
     def deserialize_query_context(Cls, feature_id: str) -> Tuple[Type['Feature'], concept.AtlasConcept, str]:
         """
-        Deserialize id into query context. 
+        Deserialize id into query context.
 
         See docstring of serialize_query_context for context.
         """
         lq_version, *rest = feature_id.split("::")
         if lq_version != "lq0":
             raise ParseLiveQueryIdException("livequery id must start with lq0::")
```

### Comparing `siibra-0.4a51/siibra/features/image/__init__.py` & `siibra-0.4a54/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/image/image.py` & `siibra-0.4a54/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/image/sections.py` & `siibra-0.4a54/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/image/volume_of_interest.py` & `siibra-0.4a54/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/__init__.py` & `siibra-0.4a54/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a54/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a54/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a54/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/gene_expression.py` & `siibra-0.4a54/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a54/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a54/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a54/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a54/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a54/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/features/tabular/tabular.py` & `siibra-0.4a54/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/livequeries/__init__.py` & `siibra-0.4a54/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/livequeries/allen.py` & `siibra-0.4a54/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/livequeries/bigbrain.py` & `siibra-0.4a54/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/livequeries/ebrains.py` & `siibra-0.4a54/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/livequeries/query.py` & `siibra-0.4a54/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/locations/__init__.py` & `siibra-0.4a54/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/locations/boundingbox.py` & `siibra-0.4a54/siibra/locations/boundingbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
 
     def shift(self, offset):
         return self.__class__(
             point1=self.minpoint + offset,
             point2=self.maxpoint + offset,
             space=self.space,
             sigma_mm=[self.minpoint.sigma, self.maxpoint.sigma]
-        )  
+        )
 
     def zoom(self, ratio: float):
         """
         Create a new bounding box by zooming this one around its center.
         """
         c = self.center
         self.maxpoint - c
```

### Comparing `siibra-0.4a51/siibra/locations/location.py` & `siibra-0.4a54/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/locations/point.py` & `siibra-0.4a54/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/locations/pointset.py` & `siibra-0.4a54/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/retrieval/__init__.py` & `siibra-0.4a54/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/retrieval/cache.py` & `siibra-0.4a54/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/retrieval/datasets.py` & `siibra-0.4a54/siibra/retrieval/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,24 +41,25 @@
 
 EbrainsDatasetEmbargoStatus = TypedDict('EbrainsDatasetEmbargoStatus', {
     "@id": str,
     'name': str,
     'identifier': List[str]
 })
 
+
 class EbrainsBaseDataset(ABC):
-    
+
     @abstractproperty
     def id(self) -> str:
         raise NotImplementedError
-    
+
     @abstractproperty
     def name(self) -> str:
         raise NotImplementedError
-    
+
     @abstractproperty
     def urls(self) -> List[EbrainsDatasetUrl]:
         raise NotImplementedError
 
     @abstractproperty
     def description(self) -> str:
         raise NotImplementedError
@@ -70,21 +71,21 @@
     @abstractproperty
     def ebrains_page(self) -> str:
         raise NotImplementedError
 
     @abstractproperty
     def custodians(self) -> List[EbrainsDatasetPerson]:
         raise NotImplementedError
-    
+
     def __hash__(self):
         return hash(self.id)
-    
+
     def __eq__(self, o: object) -> bool:
         return hasattr(o, "id") and self.id == o.id
-    
+
     def match(self, spec: Union[str, 'EbrainsBaseDataset']) -> bool:
         """
         Checks if the given specification describes this dataset.
 
         Parameters
         ----------
         spec (str, EbrainsBaseDataset)
@@ -95,14 +96,15 @@
         """
         if spec is self:
             return True
         if isinstance(spec, str):
             return self.id == spec
         raise RuntimeError(f"Cannot match {spec.__class__}, must be either str or EbrainsBaseDataset")
 
+
 class EbrainsDataset(EbrainsBaseDataset):
 
     def __init__(self, id, name=None, embargo_status: List[EbrainsDatasetEmbargoStatus] = None, *, cached_data=None):
         super().__init__()
 
         self._id = id
         self._name = name
@@ -164,19 +166,20 @@
     def ebrains_page(self):
         return f"https://search.kg.ebrains.eu/instances/{self.id}"
 
     @property
     def custodians(self) -> EbrainsDatasetPerson:
         return self.detail.get("custodians")
 
+
 class EbrainsV3DatasetVersion(EbrainsBaseDataset):
 
     @staticmethod
     def parse_person(d: dict) -> EbrainsDatasetPerson:
-        assert "https://openminds.ebrains.eu/core/Person" in d.get("type"), f"Cannot convert a non person to a person dict!"
+        assert "https://openminds.ebrains.eu/core/Person" in d.get("type"), "Cannot convert a non person to a person dict!"
         _id = d.get('id')
         name = f"{d.get('givenName')} {d.get('familyName')}"
         return {
             '@id': _id,
             'schema.org/shortName': name,
             'identifier': _id,
             "shortName": name,
@@ -184,73 +187,74 @@
         }
 
     def __init__(self, id, *, cached_data=None) -> None:
         super().__init__()
 
         self._id = id
         self._cached_data = cached_data
-    
+
     @property
     def detail(self):
         if not self._cached_data:
             match = re.search(r"([a-f0-9-]+)$", self._id)
             instance_id = match.group(1)
             self._cached_data = MultiSourcedRequest(
                 requests=[
                     GitlabProxy(
                         GitlabProxyEnum.DATASETVERSION_V3,
                         instance_id=instance_id,
                     ),
                 ]
             ).data
         return self._cached_data
-    
+
     @property
-    def id(self) -> str :
+    def id(self) -> str:
         return self._id
 
     @property
-    def name(self) -> str :
+    def name(self) -> str:
         fullname = self.detail.get("fullName")
         version_id = self.detail.get("versionIdentifier")
         return f"{fullname} ({version_id})"
-        
+
     @property
-    def urls(self) -> List[EbrainsDatasetUrl] :
+    def urls(self) -> List[EbrainsDatasetUrl]:
         return [{
             "url": doi.get("identifier", None)
-        } for doi in self.detail.get("doi", []) ]
-    
+        } for doi in self.detail.get("doi", [])]
+
     @property
-    def description(self) -> str :
+    def description(self) -> str:
         return self.detail.get("description", "")
 
     @property
-    def contributors(self) -> List[EbrainsDatasetPerson] :
+    def contributors(self) -> List[EbrainsDatasetPerson]:
         return [EbrainsV3DatasetVersion.parse_person(d) for d in self.detail.get("author", [])]
 
     @property
-    def ebrains_page(self) -> str :
+    def ebrains_page(self) -> str:
         if len(self.urls) > 0:
             return self.urls[0].get("url")
         return None
-    
+
     @property
     def custodians(self) -> EbrainsDatasetPerson:
         return [EbrainsV3DatasetVersion.parse_person(d) for d in self.detail.get("custodian", [])]
 
+
 class EbrainsV3Dataset(EbrainsBaseDataset):
     # TODO finish implementing me
     # some fields are currently missing, e.g. desc, contributors etc.
     def __init__(self, id, *, cached_data=None) -> None:
         super().__init__()
 
         self._id = id
         self._cached_data = cached_data
-    
+
     @property
     def detail(self):
         if not self._cached_data:
             match = re.search(r"([a-f0-9-]+)$", self._id)
             instance_id = match.group(1)
             self._cached_data = MultiSourcedRequest(
                 requests=[
```

### Comparing `siibra-0.4a51/siibra/retrieval/repositories.py` & `siibra-0.4a54/siibra/retrieval/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,20 +328,20 @@
         Loads a file from the zip archive, but mimics the behaviour
         of cached http requests used in other connectors.
         """
         def __init__(self, zipfile, filename, decode_func):
             self.zipfile = zipfile
             self.filename = filename
             self.func = decode_func
-            self.cachefile = CACHE.build_filename(zipfile+filename)
+            self.cachefile = CACHE.build_filename(zipfile + filename)
 
         @property
         def cached(self):
             return os.path.isfile(self.cachefile)
-        
+
         @property
         def data(self):
             container = ZipFile(self.zipfile)
             return self.func(container.open(self.filename).read())
 
     def get_loader(self, filename, folder="", decode_func=None):
         """Get a lazy loader for a file, for loading data
```

### Comparing `siibra-0.4a51/siibra/retrieval/requests.py` & `siibra-0.4a54/siibra/retrieval/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
         )
 
 
 class HttpRequest:
     def __init__(
         self,
         url: str,
-        func: Callable=None,
-        msg_if_not_cached: str=None,
+        func: Callable = None,
+        msg_if_not_cached: str = None,
         refresh=False,
         post=False,
         **kwargs,
     ):
         """
         Initialize a cached http data loader.
         It takes a URL and optional data conversion function.
@@ -140,19 +140,19 @@
     def _retrieve(self, block_size=1024, min_bytesize_with_no_progress_info=2e8):
         # Populates the file cache with the data from http if required.
         # noop if 1/ data is already cached and 2/ refresh flag not set
         # The caller should load the cachefile after _retrieve successfuly executes
 
         if self.cached and not self.refresh:
             return
-        
+
         # not yet in cache, perform http request.
         if self.msg_if_not_cached is not None:
             logger.debug(self.msg_if_not_cached)
-            
+
         headers = self.kwargs.get('headers', {})
         other_kwargs = {key: self.kwargs[key] for key in self.kwargs if key != "headers"}
 
         http_method = requests.post if self.post else requests.get
         r = http_method(self.url, headers={
             **USER_AGENT_HEADER,
             **headers,
@@ -166,28 +166,27 @@
             progress_bar = siibra_tqdm(
                 total=size_bytes, unit='iB', unit_scale=True,
                 position=0, leave=True,
                 desc=f"Downloading {os.path.split(self.url)[-1]} ({size_bytes / 1024**2:.1f} MiB)"
             )
         temp_cachefile = f"{self.cachefile}_temp"
         lock = Lock(f"{temp_cachefile}.lock")
-        
+
         with lock:
             with open(temp_cachefile, "wb") as f:
                 for data in r.iter_content(block_size):
                     if size_bytes > min_bytesize_with_no_progress_info:
                         progress_bar.update(len(data))
                     f.write(data)
             if size_bytes > min_bytesize_with_no_progress_info:
                 progress_bar.close()
             if self.refresh and os.path.isfile(self.cachefile):
                 os.remove(self.cachefile)
             self.refresh = False
             os.rename(temp_cachefile, self.cachefile)
-            
 
     def get(self):
         self._retrieve()
         with open(self.cachefile, "rb") as f:
             data = f.read()
         try:
             return data if self.func is None else self.func(data)
@@ -275,19 +274,19 @@
             logger.warning("expected device_authorization_endpoint in .well-known/openid-configuration, but was not present")
 
     @classmethod
     def fetch_token(cls, **kwargs):
         """
         Fetch an EBRAINS token using commandline-supplied username/password
         using the data proxy endpoint.
-        
+
         :ref:`Details on how to access EBRAINS are here.<accessEBRAINS>`
         """
         cls.device_flow(**kwargs)
-        
+
     @classmethod
     def device_flow(cls, **kwargs):
         if all([
             not sys.__stdout__.isatty(),  # if is tty, do not raise
             not any(k in ['JPY_INTERRUPT_EVENT', "JPY_PARENT_PID"] for k in os.environ),  # if is notebook environment, do not raise
             not os.getenv("SIIBRA_ENABLE_DEVICE_FLOW"),  # if explicitly enabled by env var, do not raise
         ]):
@@ -299,26 +298,26 @@
         cls.init_oidc()
 
         def get_scopes() -> str:
             scopes = kwargs.get("scopes")
             if not scopes:
                 return None
             if not isinstance(scopes, list):
-                logger.warning(f"scopes needs to be a list, is but is not... skipping")
+                logger.warning("scopes needs to be a list, is but is not... skipping")
                 return None
             if not all(isinstance(scope, str) for scope in scopes):
-                logger.warning(f"scopes needs to be all str, but is not")
+                logger.warning("scopes needs to be all str, but is not")
                 return None
             if len(scopes) == 0:
-                logger.warning(f'provided empty list as scopes... skipping')
+                logger.warning('provided empty list as scopes... skipping')
                 return None
             return "+".join(scopes)
-        
+
         scopes = get_scopes()
-        
+
         data = {
             'client_id': cls._IAM_DEVICE_FLOW_CLIENTID
         }
 
         if scopes:
             data['scopes'] = scopes
         resp = requests.post(
```

### Comparing `siibra-0.4a51/siibra/vocabularies/__init__.py` & `siibra-0.4a54/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/vocabularies/gene_names.json` & `siibra-0.4a54/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a54/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/vocabularies/region_aliases.json` & `siibra-0.4a54/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/volumes/__init__.py` & `siibra-0.4a54/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/volumes/gifti.py` & `siibra-0.4a54/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/volumes/neuroglancer.py` & `siibra-0.4a54/siibra/volumes/neuroglancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
         vertices, triangles = affine_transform_mesh(vertices_vox, triangles_vox, transform_nm)
         vertices /= 1e6
         return {'verts': vertices, 'faces': triangles}
 
     def fetch(self, label: int, fragment: str):
         """
         Fetches a particular mesh. Each mesh is a dictionary with keys:
-        
+
         Parameters
         ----------
         label: int
             Label of the volume
         fragment: str, default: None
             A fragment name can be specified to choose from multiple fragments.
```

### Comparing `siibra-0.4a51/siibra/volumes/nifti.py` & `siibra-0.4a54/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/siibra/volumes/parcellationmap.py` & `siibra-0.4a54/siibra/volumes/parcellationmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,28 @@
 
 
 class ConflictingArgumentException(ValueError): pass
 
 
 class NonUniqueIndexError(RuntimeError): pass
 
+
 @dataclass
 class Assignment:
     input_structure: int
     centroid: Union[Tuple[np.ndarray], point.Point] 
     volume: int
     fragment: str
     map_value: np.ndarray
 
 
 @dataclass
 class AssignImageResult(CompareMapsResult, Assignment): pass
 
+
 class Map(concept.AtlasConcept, configuration_folder="maps"):
 
     def __init__(
         self,
         identifier: str,
         name: str,
         space_spec: dict,
@@ -259,15 +261,15 @@
 
         Returns
         -------
         Region
             A region object defined in the parcellation map.
         """
         if isinstance(label, MapIndex) and index is None:
-            raise TypeError(f"Specify MapIndex with index keyword.")
+            raise TypeError("Specify MapIndex with 'index' keyword.")
         if index is None:
             index = MapIndex(volume, label)
         matches = [
             regionname
             for regionname, indexlist in self._indices.items()
             if index in indexlist
         ]
@@ -468,18 +470,21 @@
 
     @property
     def affine(self):
         if self._affine_cached is None:
             # we compute the affine from a volumetric volume provider
             for fmt in _volume.Volume.SUPPORTED_FORMATS:
                 if fmt not in _volume.Volume.MESH_FORMATS:
+                    if fmt not in self.formats:
+                        continue
                     try:
                         self._affine_cached = self.fetch(index=MapIndex(volume=0), format=fmt).affine
                         break
-                    except RuntimeError:
+                    except Exception:
+                        logger.debug("Caught exceptions:\n", exc_info=1)
                         continue
             else:
                 raise RuntimeError(f"No volumetric provider in {self} to derive the affine matrix.")
         if not isinstance(self._affine_cached, np.ndarray):
             logger.error("invalid affine:", self._affine_cached)
         return self._affine_cached
 
@@ -757,32 +762,32 @@
             return [
                 (pointindex, volume, fragment, value)
                 for fragment in fragments
                 for volume, volimg in enumerate(self.fetch_iter(fragment=fragment))
                 for pointindex, value
                 in enumerate(np.asanyarray(volimg.dataobj)[x, y, z])
             ]
-        
+
     def _assign(
         self,
         item: Union[point.Point, pointset.PointSet, Nifti1Image],
         minsize_voxel=1,
         lower_threshold=0.0
-    ) -> List[Union[Assignment,AssignImageResult]]:
+    ) -> List[Union[Assignment, AssignImageResult]]:
         """
         For internal use only. Returns a dataclass, which provides better static type checking.
         """
-        
+
         if isinstance(item, point.Point):
             return self._assign_points(pointset.PointSet([item], item.space, sigma_mm=item.sigma), lower_threshold)
         if isinstance(item, pointset.PointSet):
             return self._assign_points(item, lower_threshold)
         if isinstance(item, Nifti1Image):
             return self._assign_image(item, minsize_voxel, lower_threshold)
-        
+
         raise RuntimeError(
             f"Items of type {item.__class__.__name__} cannot be used for region assignment."
         )
 
     def assign(
         self,
         item: Union[point.Point, pointset.PointSet, Nifti1Image],
@@ -914,25 +919,25 @@
                         "map weighted mean": None,
                         "map containedness": None,
                         "input weighted mean": None,
                         "input containedness": None,
                     }
                 }
             else:
-                raise RuntimeError(f"assignments must be of type Assignment or AssignImageResult!")
-            
+                raise RuntimeError("assignments must be of type Assignment or AssignImageResult!")
+
             dataframe_list.append(item_to_append)
         df = pd.DataFrame(dataframe_list)
         return (
             df
             .convert_dtypes()  # convert will guess numeric column types
             .reindex(columns=columns)
         )
 
-    def _assign_points(self, points:pointset.PointSet, lower_threshold: float) -> List[Assignment]:
+    def _assign_points(self, points: pointset.PointSet, lower_threshold: float) -> List[Assignment]:
         """
         assign a PointSet to this parcellation map.
 
         Parameters:
         -----------
         lower_threshold: float, default: 0
             Lower threshold on values in the statistical map. Values smaller than
@@ -1006,16 +1011,16 @@
                 xyz_vox = (np.dot(phys2vox, pt.homogeneous) + 0.5).astype("int")
                 shift = np.identity(4)
                 shift[:3, -1] = xyz_vox[:3] - r
                 # build niftiimage with the Gaussian blob,
                 # then recurse into this method with the image input
                 W = Nifti1Image(dataobj=kernel, affine=np.dot(self.affine, shift))
                 for entry in self._assign(W, lower_threshold=lower_threshold):
-                    entry.input_structure=pointindex
-                    entry.centroid=tuple(pt)
+                    entry.input_structure = pointindex
+                    entry.centroid = tuple(pt)
                     assignments.append(entry)
         return assignments
 
     def _assign_image(self, queryimg: Nifti1Image, minsize_voxel: int, lower_threshold: float) -> List[AssignImageResult]:
         """
         Assign an image volume to this parcellation map.
```

### Comparing `siibra-0.4a51/siibra/volumes/sparsemap.py` & `siibra-0.4a54/siibra/volumes/sparsemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             modality=modality,
             publications=publications,
             datasets=datasets,
             volumes=volumes,
         )
         self._sparse_index_cached = None
         self._sparseindex_zip_url = cache_url if is_cached else ""
-    
+
     @property
     def _cache_prefix(self):
         return f"{self.parcellation.id}_{self.space.id}_{self.maptype}_{self.name}_index"
 
     @property
     def sparse_index(self):
         if self._sparse_index_cached is None:
```

### Comparing `siibra-0.4a51/siibra/volumes/volume.py` & `siibra-0.4a54/siibra/volumes/volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 from ..locations import boundingbox as _boundingbox
 from ..core import space
 
 import nibabel as nib
 from abc import ABC, abstractmethod
 from typing import List, Dict, Union, Set, TYPE_CHECKING
 import json
+from time import sleep
 
 if TYPE_CHECKING:
     from ..retrieval.datasets import EbrainsDataset
     TypeDataset = EbrainsDataset
 
+
 class ColorVolumeNotSupported(NotImplementedError):
     pass
 
 
 class Volume:
     """
     A volume is a specific mesh or 3D array,
@@ -48,14 +50,22 @@
         "neuroglancer/precompmesh/surface",
         "gii-mesh",
         "gii-label"
     ]
 
     SUPPORTED_FORMATS = IMAGE_FORMATS + MESH_FORMATS
 
+    _FORMAT_LOOKUP = {
+        "image": IMAGE_FORMATS,
+        "mesh": MESH_FORMATS,
+        "surface": MESH_FORMATS,
+        "nifti": ["nii", "zip/nii"],
+        "nii": ["nii", "zip/nii"]
+    }
+
     def __init__(
         self,
         space_spec: dict,
         providers: List['VolumeProvider'],
         name: str = "",
         variant: str = None,
         datasets: List['TypeDataset'] = [],
@@ -155,53 +165,66 @@
         **kwargs
     ):
         """
         Fetch a volumetric or surface representation from one of the providers.
 
         Parameters
         ----------
-        format: str
-            Requested format. Per default, several formats are tried,
-            starting with volumetric formats. It can be explicitly specified as:
+        format: str, default=None
+            Requested format. If `None`, the first supported format matching in
+            `self.formats` is tried, starting with volumetric formats.
+            It can be explicitly specified as:
                 - 'surface' or 'mesh' to fetch a surface format
                 - 'volumetric' or 'voxel' to fetch a volumetric format
                 - supported format types, see SUPPORTED_FORMATS. This includes
                 'nii', 'zip/nii', 'neuroglancer/precomputed', 'gii-mesh',
                 'neuroglancer/precompmesh', 'gii-label'
 
         Returns
         -------
         An image or mesh
         """
 
         if format is None:
             requested_formats = self.SUPPORTED_FORMATS
-        elif format == 'mesh':
-            requested_formats = self.MESH_FORMATS
-        elif format == 'image':
-            requested_formats = self.IMAGE_FORMATS
+        elif format in self._FORMAT_LOOKUP:  # allow use of aliases
+            requested_formats = self._FORMAT_LOOKUP[format]
         elif format in self.SUPPORTED_FORMATS:
             requested_formats = [format]
         else:
             raise ValueError(f"Invalid format requested: {format}")
 
+        # select the first source unless the user specifically requests a format
         for fmt in requested_formats:
             if fmt in self.formats:
-                try:
-                    if fmt == "gii-label":
-                        tpl = self.space.get_template(variant=kwargs.get('variant'))
-                        mesh = tpl.fetch(**kwargs)
-                        labels = self._providers[fmt].fetch(**kwargs)
-                        return dict(**mesh, **labels)
-                    else:
-                        return self._providers[fmt].fetch(**kwargs)
-                except requests.SiibraHttpRequestError as e:
-                    logger.error(f"Cannot access {self._providers[fmt]}")
-                    print(str(e))
-                    continue
+                selected_format = fmt
+                logger.debug(f"Requested format was '{format}', selected format is '{selected_format}'")
+                break
+        else:
+            raise ValueError(f"Invalid format requested: {format}")
+
+        # try the selected format only
+        for try_count in range(6):
+            try:
+                if selected_format == "gii-label":
+                    tpl = self.space.get_template(variant=kwargs.get('variant'))
+                    mesh = tpl.fetch(**kwargs)
+                    labels = self._providers[selected_format].fetch(**kwargs)
+                    return dict(**mesh, **labels)
+                else:
+                    return self._providers[selected_format].fetch(**kwargs)
+            except requests.SiibraHttpRequestError as e:
+                if e.status_code == 429:  # too many requests
+                    sleep(0.1)
+                logger.error(f"Cannot access {self._providers[selected_format]}", exc_info=(try_count == 5))
+        if format is None and len(self.formats) > 1:
+            logger.info(
+                f"No format was specified and auto-selected format '{selected_format}' "
+                "was unsuccesful. You can specify another format from "
+                f"{set(self.formats) - set(selected_format)} to try.")
         return None
 
 
 class Subvolume(Volume):
     """
     Wrapper class for exposing a z level of a 4D volume to be used like a 3D volume.
     """
```

### Comparing `siibra-0.4a51/siibra.egg-info/PKG-INFO` & `siibra-0.4a54/siibra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a51
+Version: 0.4a54
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a51/siibra.egg-info/SOURCES.txt` & `siibra-0.4a54/siibra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siibra-0.4a51/test/test_siibra.py` & `siibra-0.4a54/test/test_siibra.py`

 * *Files identical despite different names*

