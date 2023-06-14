# Comparing `tmp/haplotyping-0.0.6.tar.gz` & `tmp/haplotyping-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haplotyping-0.0.6.tar", last modified: Mon May  1 11:52:34 2023, max compression
+gzip compressed data, was "haplotyping-0.0.7.tar", last modified: Wed Jun 14 08:13:42 2023, max compression
```

## Comparing `haplotyping-0.0.6.tar` & `haplotyping-0.0.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2021-06-16 07:44:07.000000 haplotyping-0.0.6/LICENSE
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-05-01 11:52:34.121224 haplotyping-0.0.6/PKG-INFO
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       14 2021-06-16 07:44:07.000000 haplotyping-0.0.6/README.md
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      101 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       22 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/_version.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/api/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      112 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/api/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    22089 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/api/api.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping/data/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      212 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9180 2023-05-01 11:45:58.000000 haplotyping-0.0.6/haplotyping/data/checkDatabase.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    29485 2023-05-01 11:45:04.000000 haplotyping-0.0.6/haplotyping/data/constructDatabase.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/data/schema/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      401 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_experiments.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      454 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_mappings.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1097 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_markers.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      327 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_metadata.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      517 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_scores.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      993 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_sequences.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1029 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/data_default_varieties.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1050 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_ancestors.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      598 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_breeders.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      341 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_countries.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      529 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_synonyms.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      903 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/data/schema/pedigree_varieties.schema.json
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    42098 2023-05-01 08:56:45.000000 haplotyping-0.0.6/haplotyping/data/validator.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1775 2022-03-10 19:41:20.000000 haplotyping-0.0.6/haplotyping/general.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/graph/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      196 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7206 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/api.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    58189 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/baseGraph.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    38481 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/sections.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    62285 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/graph/sequence.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.117224 haplotyping-0.0.6/haplotyping/index/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      119 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/index/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    13104 2023-04-29 07:03:33.000000 haplotyping-0.0.6/haplotyping/index/database.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    41641 2023-05-01 09:11:12.000000 haplotyping-0.0.6/haplotyping/index/direct.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    34252 2023-05-01 09:13:06.000000 haplotyping-0.0.6/haplotyping/index/splits.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   128031 2023-04-28 18:59:52.000000 haplotyping-0.0.6/haplotyping/index/storage.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/haplotyping/service/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      116 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9887 2023-05-01 08:05:15.000000 haplotyping-0.0.6/haplotyping/service/api.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4244 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/api_collection.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1663 2022-09-25 17:35:23.000000 haplotyping-0.0.6/haplotyping/service/api_country.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12310 2023-04-30 09:20:00.000000 haplotyping-0.0.6/haplotyping/service/api_dataset.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20805 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/api_kmer.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4917 2023-04-30 09:20:57.000000 haplotyping-0.0.6/haplotyping/service/api_marker.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12952 2023-04-30 09:20:34.000000 haplotyping-0.0.6/haplotyping/service/api_split.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1093 2021-06-30 08:50:36.000000 haplotyping-0.0.6/haplotyping/service/api_tools.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20951 2023-04-30 09:17:00.000000 haplotyping-0.0.6/haplotyping/service/api_variety.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7177 2022-11-16 14:08:23.000000 haplotyping-0.0.6/haplotyping/service/kmer_kmc.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2956 2022-11-16 14:08:23.000000 haplotyping-0.0.6/haplotyping/service/marker.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    18632 2023-03-20 17:49:58.000000 haplotyping-0.0.6/haplotyping/service/split.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.113224 haplotyping-0.0.6/haplotyping.egg-info/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/PKG-INFO
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1995 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/SOURCES.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        1 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/dependency_links.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      228 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/requires.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       18 2023-05-01 11:52:34.000000 haplotyping-0.0.6/haplotyping.egg-info/top_level.txt
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       38 2023-05-01 11:52:34.121224 haplotyping-0.0.6/setup.cfg
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1202 2023-05-01 11:15:54.000000 haplotyping-0.0.6/setup.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       33 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/__init__.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/index/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       40 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/index/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11079 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/index/test_database.py
-drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-05-01 11:52:34.121224 haplotyping-0.0.6/tests/service/
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       36 2021-06-29 16:25:06.000000 haplotyping-0.0.6/tests/service/__init__.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    26188 2021-10-09 11:28:48.000000 haplotyping-0.0.6/tests/service/test_api.py
--rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1337 2021-06-16 07:44:07.000000 haplotyping-0.0.6/tests/test_general.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.043390 haplotyping-0.0.7/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        0 2021-06-16 07:44:07.000000 haplotyping-0.0.7/LICENSE
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-06-14 08:13:42.043390 haplotyping-0.0.7/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       14 2021-06-16 07:44:07.000000 haplotyping-0.0.7/README.md
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.035390 haplotyping-0.0.7/haplotyping/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      101 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       22 2023-05-01 11:54:54.000000 haplotyping-0.0.7/haplotyping/_version.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.035390 haplotyping-0.0.7/haplotyping/api/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      112 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/api/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    22089 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/api/api.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.035390 haplotyping-0.0.7/haplotyping/data/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      212 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/data/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9180 2023-05-01 11:45:58.000000 haplotyping-0.0.7/haplotyping/data/checkDatabase.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    29485 2023-05-01 11:45:04.000000 haplotyping-0.0.7/haplotyping/data/constructDatabase.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.039390 haplotyping-0.0.7/haplotyping/data/schema/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      401 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_experiments.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      454 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_mappings.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1097 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_markers.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      327 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_metadata.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      517 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_scores.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      993 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_sequences.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1029 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/data_default_varieties.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1050 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/pedigree_ancestors.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      598 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/pedigree_breeders.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      341 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/pedigree_countries.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      529 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/pedigree_synonyms.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      903 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/data/schema/pedigree_varieties.schema.json
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    42098 2023-05-01 08:56:45.000000 haplotyping-0.0.7/haplotyping/data/validator.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1775 2022-03-10 19:41:20.000000 haplotyping-0.0.7/haplotyping/general.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.039390 haplotyping-0.0.7/haplotyping/graph/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      196 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/graph/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7206 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/graph/api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    58189 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/graph/baseGraph.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    38481 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/graph/sections.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    62285 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/graph/sequence.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.039390 haplotyping-0.0.7/haplotyping/index/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      119 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/index/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    13104 2023-04-29 07:03:33.000000 haplotyping-0.0.7/haplotyping/index/database.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    41641 2023-05-01 09:11:12.000000 haplotyping-0.0.7/haplotyping/index/direct.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    34252 2023-05-01 09:13:06.000000 haplotyping-0.0.7/haplotyping/index/splits.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)   128031 2023-04-28 18:59:52.000000 haplotyping-0.0.7/haplotyping/index/storage.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.043390 haplotyping-0.0.7/haplotyping/service/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      116 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/service/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     9887 2023-05-01 08:05:15.000000 haplotyping-0.0.7/haplotyping/service/api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4244 2023-03-20 17:49:58.000000 haplotyping-0.0.7/haplotyping/service/api_collection.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1663 2022-09-25 17:35:23.000000 haplotyping-0.0.7/haplotyping/service/api_country.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12310 2023-04-30 09:20:00.000000 haplotyping-0.0.7/haplotyping/service/api_dataset.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20805 2023-06-14 07:59:19.000000 haplotyping-0.0.7/haplotyping/service/api_kmer.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     4917 2023-04-30 09:20:57.000000 haplotyping-0.0.7/haplotyping/service/api_marker.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    12952 2023-04-30 09:20:34.000000 haplotyping-0.0.7/haplotyping/service/api_split.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1093 2021-06-30 08:50:36.000000 haplotyping-0.0.7/haplotyping/service/api_tools.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    20951 2023-04-30 09:17:00.000000 haplotyping-0.0.7/haplotyping/service/api_variety.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     7177 2022-11-16 14:08:23.000000 haplotyping-0.0.7/haplotyping/service/kmer_kmc.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     2956 2022-11-16 14:08:23.000000 haplotyping-0.0.7/haplotyping/service/marker.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    13973 2023-06-14 08:11:06.000000 haplotyping-0.0.7/haplotyping/service/split.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.035390 haplotyping-0.0.7/haplotyping.egg-info/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      389 2023-06-14 08:13:41.000000 haplotyping-0.0.7/haplotyping.egg-info/PKG-INFO
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1995 2023-06-14 08:13:42.000000 haplotyping-0.0.7/haplotyping.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)        1 2023-06-14 08:13:41.000000 haplotyping-0.0.7/haplotyping.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)      228 2023-06-14 08:13:41.000000 haplotyping-0.0.7/haplotyping.egg-info/requires.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       18 2023-06-14 08:13:41.000000 haplotyping-0.0.7/haplotyping.egg-info/top_level.txt
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       38 2023-06-14 08:13:42.043390 haplotyping-0.0.7/setup.cfg
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1202 2023-05-01 11:15:54.000000 haplotyping-0.0.7/setup.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.043390 haplotyping-0.0.7/tests/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       33 2021-06-16 07:44:07.000000 haplotyping-0.0.7/tests/__init__.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.043390 haplotyping-0.0.7/tests/index/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       40 2021-06-16 07:44:07.000000 haplotyping-0.0.7/tests/index/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    11079 2021-06-16 07:44:07.000000 haplotyping-0.0.7/tests/index/test_database.py
+drwxrwxr-x   0 matthijs  (1000) matthijs  (1000)        0 2023-06-14 08:13:42.043390 haplotyping-0.0.7/tests/service/
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)       36 2021-06-29 16:25:06.000000 haplotyping-0.0.7/tests/service/__init__.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)    26188 2021-10-09 11:28:48.000000 haplotyping-0.0.7/tests/service/test_api.py
+-rw-rw-r--   0 matthijs  (1000) matthijs  (1000)     1337 2021-06-16 07:44:07.000000 haplotyping-0.0.7/tests/test_general.py
```

### Comparing `haplotyping-0.0.6/haplotyping/api/api.py` & `haplotyping-0.0.7/haplotyping/api/api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/checkDatabase.py` & `haplotyping-0.0.7/haplotyping/data/checkDatabase.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/constructDatabase.py` & `haplotyping-0.0.7/haplotyping/data/constructDatabase.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/data_default_markers.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/data_default_markers.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/data_default_scores.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/data_default_scores.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/data_default_sequences.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/data_default_sequences.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/data_default_varieties.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/data_default_varieties.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/pedigree_ancestors.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/pedigree_ancestors.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/pedigree_breeders.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/pedigree_breeders.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/pedigree_synonyms.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/pedigree_synonyms.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/schema/pedigree_varieties.schema.json` & `haplotyping-0.0.7/haplotyping/data/schema/pedigree_varieties.schema.json`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/data/validator.py` & `haplotyping-0.0.7/haplotyping/data/validator.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/general.py` & `haplotyping-0.0.7/haplotyping/general.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/graph/api.py` & `haplotyping-0.0.7/haplotyping/graph/api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/graph/baseGraph.py` & `haplotyping-0.0.7/haplotyping/graph/baseGraph.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/graph/sections.py` & `haplotyping-0.0.7/haplotyping/graph/sections.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/graph/sequence.py` & `haplotyping-0.0.7/haplotyping/graph/sequence.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/index/database.py` & `haplotyping-0.0.7/haplotyping/index/database.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/index/direct.py` & `haplotyping-0.0.7/haplotyping/index/direct.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/index/splits.py` & `haplotyping-0.0.7/haplotyping/index/splits.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/index/storage.py` & `haplotyping-0.0.7/haplotyping/index/storage.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api.py` & `haplotyping-0.0.7/haplotyping/service/api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_collection.py` & `haplotyping-0.0.7/haplotyping/service/api_collection.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_country.py` & `haplotyping-0.0.7/haplotyping/service/api_country.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_dataset.py` & `haplotyping-0.0.7/haplotyping/service/api_dataset.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_kmer.py` & `haplotyping-0.0.7/haplotyping/service/api_kmer.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_marker.py` & `haplotyping-0.0.7/haplotyping/service/api_marker.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_split.py` & `haplotyping-0.0.7/haplotyping/service/api_split.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_tools.py` & `haplotyping-0.0.7/haplotyping/service/api_tools.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/api_variety.py` & `haplotyping-0.0.7/haplotyping/service/api_variety.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/kmer_kmc.py` & `haplotyping-0.0.7/haplotyping/service/kmer_kmc.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/marker.py` & `haplotyping-0.0.7/haplotyping/service/marker.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/haplotyping/service/split.py` & `haplotyping-0.0.7/haplotyping/service/split.py`

 * *Files 25% similar despite different names*

```diff
@@ -148,21 +148,17 @@
                         "distinct": int(row[4][1][0]),
                         "number": int(row[4][1][1])
                     },"right": {
                         "distinct": int(row[4][2][0]),
                         "number": int(row[4][2][1])
                     }
                 },
-                "connected": {
-                    "number": int(row[5][1]),
-                    "connected": int(row[5][2])
-                },
-                "paired": int(row[6][1]),
-                "cycle": int(row[7][0]),
-                "reverse": int(row[8][0]),
+                "cycle": int(row[6][0]),
+                "reverse": int(row[7][0]),
+                "paired": int(row[8][1]),                
             }
             baseTable = h5file.get("/split/base")
             if response["split"] in ["left","both"]:
                 baseRow=baseTable[row[3][0]]
                 if expandBase:
                     response["rightSplitBase"]["left"] = Split._base_result(baseRow,h5file,False)
                 else:
@@ -216,38 +212,14 @@
                     response["direct"]["left"].append(item)
                 elif fromDirection=="r":
                     response["direct"]["right"].append(item)
         else:
             response = None
         return response
     
-    def _kmer_connected_result(ckmerId, ckmerRow, connectionsIndexRows: list, connectionsPairedRows: list, h5file: h5py.File):
-        response = {"ckmer": ckmerRow[0].decode("ascii"), "connections":[], "paired": {}}
-        ckmerTable = h5file.get("/split/ckmer")
-        if len(connectionsIndexRows)>0:
-            connectionsDataTable = h5file.get("/connections/data")
-            for connectionsIndexRow in connectionsIndexRows:
-                assert connectionsIndexRow[0]==ckmerId
-                direct = connectionsIndexRow[3]
-                number = connectionsIndexRow[4]
-                connections = connectionsDataTable[connectionsIndexRow[1]:connectionsIndexRow[1]+connectionsIndexRow[2]]
-                assert connectionsIndexRow[0] in connections
-                connectionsCkmers = []
-                for ckmerLink in connections:
-                    if not ckmerLink==ckmerId:
-                        connectionsCkmers.append(ckmerTable[ckmerLink][0].decode("ascii"))
-                response["connections"].append({"connections": connectionsCkmers, 
-                                                "direct": int(connectionsIndexRow[3]),
-                                                "number": int(connectionsIndexRow[4])})
-        for connectionsPairedRow in connectionsPairedRows:
-            assert connectionsPairedRow[0]==ckmerId
-            linkedCkmer = ckmerTable[connectionsPairedRow[1]][0].decode("ascii")
-            response["paired"][linkedCkmer] = int(connectionsPairedRow[2])                
-        return response
-    
     #---
     
     def _info(h5file: h5py.File):
         response = {}
         configTable = h5file.get("/config")
         for k in configTable.attrs.keys():
             value = configTable.attrs[k]
@@ -313,69 +285,14 @@
             if ckmerRow:
                 (directRows,directId,directCache) = Split._findId(id,directTable)
                 response.append(Split._kmer_direct_result(ckmerRow,directRows,h5file))
                 start = id+1
             else:
                 start = id 
         return list(filter(None, response))
-    
-    def _kmer_connected(h5file: h5py.File, kmer: str):
-        ckmer = haplotyping.General.canonical(kmer)
-        ckmerTable = h5file.get("/split/ckmer")
-        (ckmerRow,id,cache) = Split._findItem(ckmer,ckmerTable)
-        if ckmerRow:
-            if ckmerRow[5][1]>0:   
-                connectionsIndexTable = h5file.get("/connections/index")                
-                connectionsIndexRows = connectionsIndexTable[ckmerRow[5][0]:ckmerRow[5][0]+ckmerRow[5][1]]               
-            else:
-                connectionsIndexRows = []
-            if ckmerRow[6][1]>0:   
-                connectionsPairedTable = h5file.get("/connections/paired")                
-                connectionsPairedRows = connectionsPairedTable[ckmerRow[6][0]:ckmerRow[6][0]+ckmerRow[6][1]]
-            else:
-                connectionsPairedRows = []
-            return Split._kmer_connected_result(id, ckmerRow, connectionsIndexRows, connectionsPairedRows, h5file)
-        else:
-            return None
-    
-    def _kmers_connected(h5file: h5py.File, kmers: list):
-        #get canonical k-mers
-        ckmerList = set()
-        for kmer in kmers:
-            ckmerList.add(haplotyping.General.canonical(kmer))
-        ckmerList = list(ckmerList)
-        ckmerList.sort()
-        #get ids
-        ckmerTable = h5file.get("/split/ckmer")
-        number = ckmerTable.shape[0]
-        start = 0
-        cache = {}
-        #construct response
-        response = []
-        for i in range(len(ckmerList)):
-            ckmer = ckmerList[i]
-            (ckmerRow,id,cache) = Split._findItem(ckmer,ckmerTable,start,number,cache)
-            if ckmerRow:
-                start = id+1
-                if ckmerRow[5][1]>0:   
-                    connectionsIndexTable = h5file.get("/connections/index")                
-                    connectionsIndexRows = connectionsIndexTable[ckmerRow[5][0]:ckmerRow[5][0]+ckmerRow[5][1]]               
-                else:
-                    connectionsIndexRows = []
-                if ckmerRow[6][1]>0:   
-                    connectionsPairedTable = h5file.get("/connections/paired")                
-                    connectionsPairedRows = connectionsPairedTable[ckmerRow[6][0]:ckmerRow[6][0]+ckmerRow[6][1]]
-                else:
-                    connectionsPairedRows = []
-                response.append(Split._kmer_connected_result(id, ckmerRow, connectionsIndexRows, 
-                                                             connectionsPairedRows, h5file))
-            else:
-                start = id 
-        return response
-            
    
     #---
     
     def info(location_split: str):
         with h5py.File(location_split, mode="r") as h5file:            
             return Split._info(h5file)
     
@@ -399,23 +316,15 @@
     def kmer_direct(location_split: str, kmer: str):
         with h5py.File(location_split, mode="r") as h5file:            
             return Split._kmer_direct(h5file,kmer)
     
     def kmer_list_direct(location_split: str, kmers: list):
         with h5py.File(location_split, mode="r") as h5file:            
             return Split._kmers_direct(h5file,kmers)
-    
-    def kmer_connected(location_split: str, kmer: str):
-        with h5py.File(location_split, mode="r") as h5file:            
-            return Split._kmer_connected(h5file,kmer)
-    
-    def kmer_list_connected(location_split: str, kmers: list):
-        with h5py.File(location_split, mode="r") as h5file:            
-            return Split._kmers_connected(h5file,kmers)
-    
+        
     #---
     
     def base_info(location_split: str, base: str):
         with h5py.File(location_split, mode="r") as h5file:            
             baseTable = h5file.get("/split/base")
             (baseRow,id,cache) = Split._findItem(base,baseTable)
             return Split._base_result(baseRow,h5file)
```

### Comparing `haplotyping-0.0.6/haplotyping.egg-info/SOURCES.txt` & `haplotyping-0.0.7/haplotyping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/setup.py` & `haplotyping-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/tests/index/test_database.py` & `haplotyping-0.0.7/tests/index/test_database.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/tests/service/test_api.py` & `haplotyping-0.0.7/tests/service/test_api.py`

 * *Files identical despite different names*

### Comparing `haplotyping-0.0.6/tests/test_general.py` & `haplotyping-0.0.7/tests/test_general.py`

 * *Files identical despite different names*

