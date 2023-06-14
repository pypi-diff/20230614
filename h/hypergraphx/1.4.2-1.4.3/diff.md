# Comparing `tmp/hypergraphx-1.4.2.tar.gz` & `tmp/hypergraphx-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergraphx-1.4.2.tar", last modified: Fri Jun  9 17:32:00 2023, max compression
+gzip compressed data, was "hypergraphx-1.4.3.tar", last modified: Wed Jun 14 12:32:49 2023, max compression
```

## Comparing `hypergraphx-1.4.2.tar` & `hypergraphx-1.4.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/core_periphery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/core_periphery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/core_periphery/core_periphery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/_linear_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/hy_sc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hy_sc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6376 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hy_sc/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/hypergraph_mt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hypergraph_mt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hypergraph_mt/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx/communities/hyperlink_comm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hyperlink_comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/communities/hyperlink_comm/hyperlink_communities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/core/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31622 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/core/hypergraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/core/meta_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/core/multiplex_hypergraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/core/temporal_hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/dynamics/contagion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/dynamics/randwalk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/dynamics/synch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/dynamics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/activity_driven.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/hy_mmsbm_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/generation/scale_free.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/linalg/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/measures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/edge_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/eigen_centralities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/s_centralities.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/sub_hypergraph_centrality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/measures/temporal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/temporal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/measures/temporal/temporal_correlations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.914370 hypergraphx-1.4.2/hypergraphx/motifs/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/motifs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/motifs/motifs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/motifs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/hypergraphx/readwrite/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25978 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/readwrite/data_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/readwrite/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/readwrite/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/readwrite/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/hypergraphx/representations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/representations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/representations/projections.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/representations/simplicial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/hypergraphx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/utils/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/utils/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/utils/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/utils/visits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/hypergraphx/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/draw_communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/draw_hypergraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/draw_multilayer_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/draw_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/draw_simplicial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/hypergraphx/viz/plot_motifs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:32:00.910370 hypergraphx-1.4.2/hypergraphx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-06-09 17:32:00.000000 hypergraphx-1.4.2/hypergraphx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-09 17:32:00.000000 hypergraphx-1.4.2/hypergraphx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:32:00.000000 hypergraphx-1.4.2/hypergraphx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 17:32:00.000000 hypergraphx-1.4.2/hypergraphx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 17:32:00.000000 hypergraphx-1.4.2/hypergraphx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 17:32:00.918370 hypergraphx-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 17:31:51.000000 hypergraphx-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/core_periphery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/core_periphery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/core_periphery/core_periphery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/_linear_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/hy_sc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hy_sc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6376 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hy_sc/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/hypergraph_mt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hypergraph_mt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hypergraph_mt/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx/communities/hyperlink_comm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hyperlink_comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/communities/hyperlink_comm/hyperlink_communities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31622 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/core/hypergraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/core/meta_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/core/multiplex_hypergraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/core/temporal_hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/dynamics/contagion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/dynamics/randwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/dynamics/synch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/dynamics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/activity_driven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/hy_mmsbm_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/generation/scale_free.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/linalg/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/edge_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/eigen_centralities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/s_centralities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/sub_hypergraph_centrality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/measures/temporal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/temporal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/measures/temporal/temporal_correlations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.840216 hypergraphx-1.4.3/hypergraphx/motifs/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/motifs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/motifs/motifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/motifs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/hypergraphx/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/readwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25978 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/readwrite/data_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/readwrite/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/readwrite/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/readwrite/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/hypergraphx/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/representations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/representations/projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/representations/simplicial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/hypergraphx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/utils/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/utils/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/utils/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/utils/visits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/hypergraphx/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/draw_communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/draw_hypergraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/draw_multilayer_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/draw_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/draw_simplicial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/hypergraphx/viz/plot_motifs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:32:49.836216 hypergraphx-1.4.3/hypergraphx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-06-14 12:32:49.000000 hypergraphx-1.4.3/hypergraphx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-14 12:32:49.000000 hypergraphx-1.4.3/hypergraphx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:32:49.000000 hypergraphx-1.4.3/hypergraphx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 12:32:49.000000 hypergraphx-1.4.3/hypergraphx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 12:32:49.000000 hypergraphx-1.4.3/hypergraphx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 12:32:49.844216 hypergraphx-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 12:32:39.000000 hypergraphx-1.4.3/setup.py
```

### Comparing `hypergraphx-1.4.2/LICENSE.md` & `hypergraphx-1.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/PKG-INFO` & `hypergraphx-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergraphx
-Version: 1.4.2
+Version: 1.4.3
 Summary: HGX is a multi-purpose, open-source Python library for higher-order network analysis
 Home-page: https://github.com/HGX-Team/hypergraphx
 Author: HGX-Team
 Author-email: lotitoqf@gmail.com
 License: BSD-3-Clause license
 Keywords: hypergraphs,networks
 Classifier: Development Status :: 3 - Alpha
@@ -79,14 +79,20 @@
 
 ## Quick start
 
 ### Installation
 Install R-base, then
 
 ```
+pip install hypergraphx
+```
+
+or, if you really want the latest updates
+
+```
 pip install hypergraphx@git+https://github.com/HGX-Team/hypergraphx
 ```
 
 !! we are working on removing R-base from the dependancies of the library.
 
 ### First steps
 TODO: add basic tutorial
```

### Comparing `hypergraphx-1.4.2/README.md` & `hypergraphx-1.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 
 ## Quick start
 
 ### Installation
 Install R-base, then
 
 ```
+pip install hypergraphx
+```
+
+or, if you really want the latest updates
+
+```
 pip install hypergraphx@git+https://github.com/HGX-Team/hypergraphx
 ```
 
 !! we are working on removing R-base from the dependancies of the library.
 
 ### First steps
 TODO: add basic tutorial
```

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/core_periphery/core_periphery.py` & `hypergraphx-1.4.3/hypergraphx/communities/core_periphery/core_periphery.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/_linear_ops.py` & `hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/_linear_ops.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/hy_mmsbm/model.py` & `hypergraphx-1.4.3/hypergraphx/communities/hy_mmsbm/model.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/hy_sc/model.py` & `hypergraphx-1.4.3/hypergraphx/communities/hy_sc/model.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/hypergraph_mt/model.py` & `hypergraphx-1.4.3/hypergraphx/communities/hypergraph_mt/model.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/communities/hyperlink_comm/hyperlink_communities.py` & `hypergraphx-1.4.3/hypergraphx/communities/hyperlink_comm/hyperlink_communities.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/core/hypergraph.py` & `hypergraphx-1.4.3/hypergraphx/core/hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/core/meta_handler.py` & `hypergraphx-1.4.3/hypergraphx/core/meta_handler.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/core/multiplex_hypergraph.py` & `hypergraphx-1.4.3/hypergraphx/core/multiplex_hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/core/temporal_hypergraph.py` & `hypergraphx-1.4.3/hypergraphx/core/temporal_hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/dynamics/contagion.py` & `hypergraphx-1.4.3/hypergraphx/dynamics/contagion.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/dynamics/randwalk.py` & `hypergraphx-1.4.3/hypergraphx/dynamics/randwalk.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/dynamics/synch.py` & `hypergraphx-1.4.3/hypergraphx/dynamics/synch.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/dynamics/utils.py` & `hypergraphx-1.4.3/hypergraphx/dynamics/utils.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/filters/filters.py` & `hypergraphx-1.4.3/hypergraphx/filters/filters.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/generation/activity_driven.py` & `hypergraphx-1.4.3/hypergraphx/generation/activity_driven.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/generation/configuration_model.py` & `hypergraphx-1.4.3/hypergraphx/generation/configuration_model.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/generation/hy_mmsbm_sampling.py` & `hypergraphx-1.4.3/hypergraphx/generation/hy_mmsbm_sampling.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/generation/random.py` & `hypergraphx-1.4.3/hypergraphx/generation/random.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/generation/scale_free.py` & `hypergraphx-1.4.3/hypergraphx/generation/scale_free.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/linalg/linalg.py` & `hypergraphx-1.4.3/hypergraphx/linalg/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
     Returns
     -------
     The incidence matrix.
     If return_mapping is True, return the dictionary of node mappings.
     """
     binary_incidence, mapping = binary_incidence_matrix(
-        hypergraph.get_edges(order=order, subhypergraph=True, keep_isolated_nodes=keep_isolated_nodes), shape, return_mapping
+        hypergraph.get_edges(order=order, subhypergraph=True, keep_isolated_nodes=keep_isolated_nodes), return_mapping
     )
     incidence = binary_incidence.multiply(hypergraph.get_weights(order=order)).tocsr()
     return incidence, mapping
 
 
 def incidence_matrices_all_orders(
     hypergraph: Hypergraph, shape: Optional[Tuple[int]] = None, keep_isolated_nodes:bool=False, return_mapping: bool = False,
```

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/degree.py` & `hypergraphx-1.4.3/hypergraphx/measures/degree.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/edge_similarity.py` & `hypergraphx-1.4.3/hypergraphx/measures/edge_similarity.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/eigen_centralities.py` & `hypergraphx-1.4.3/hypergraphx/measures/eigen_centralities.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/s_centralities.py` & `hypergraphx-1.4.3/hypergraphx/measures/s_centralities.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/sub_hypergraph_centrality.py` & `hypergraphx-1.4.3/hypergraphx/measures/sub_hypergraph_centrality.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/measures/temporal/temporal_correlations.py` & `hypergraphx-1.4.3/hypergraphx/measures/temporal/temporal_correlations.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/motifs/motifs.py` & `hypergraphx-1.4.3/hypergraphx/motifs/motifs.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/motifs/utils.py` & `hypergraphx-1.4.3/hypergraphx/motifs/utils.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/readwrite/data_to_json.py` & `hypergraphx-1.4.3/hypergraphx/readwrite/data_to_json.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/readwrite/load.py` & `hypergraphx-1.4.3/hypergraphx/readwrite/load.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/readwrite/loaders.py` & `hypergraphx-1.4.3/hypergraphx/readwrite/loaders.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/readwrite/save.py` & `hypergraphx-1.4.3/hypergraphx/readwrite/save.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/representations/projections.py` & `hypergraphx-1.4.3/hypergraphx/representations/projections.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/representations/simplicial.py` & `hypergraphx-1.4.3/hypergraphx/representations/simplicial.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/utils/cc.py` & `hypergraphx-1.4.3/hypergraphx/utils/cc.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/utils/community.py` & `hypergraphx-1.4.3/hypergraphx/utils/community.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/utils/labeling.py` & `hypergraphx-1.4.3/hypergraphx/utils/labeling.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/utils/visits.py` & `hypergraphx-1.4.3/hypergraphx/utils/visits.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/viz/draw_communities.py` & `hypergraphx-1.4.3/hypergraphx/viz/draw_communities.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/viz/draw_hypergraph.py` & `hypergraphx-1.4.3/hypergraphx/viz/draw_hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/viz/draw_projections.py` & `hypergraphx-1.4.3/hypergraphx/viz/draw_projections.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/viz/draw_simplicial.py` & `hypergraphx-1.4.3/hypergraphx/viz/draw_simplicial.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx/viz/plot_motifs.py` & `hypergraphx-1.4.3/hypergraphx/viz/plot_motifs.py`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/hypergraphx.egg-info/PKG-INFO` & `hypergraphx-1.4.3/hypergraphx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergraphx
-Version: 1.4.2
+Version: 1.4.3
 Summary: HGX is a multi-purpose, open-source Python library for higher-order network analysis
 Home-page: https://github.com/HGX-Team/hypergraphx
 Author: HGX-Team
 Author-email: lotitoqf@gmail.com
 License: BSD-3-Clause license
 Keywords: hypergraphs,networks
 Classifier: Development Status :: 3 - Alpha
@@ -79,14 +79,20 @@
 
 ## Quick start
 
 ### Installation
 Install R-base, then
 
 ```
+pip install hypergraphx
+```
+
+or, if you really want the latest updates
+
+```
 pip install hypergraphx@git+https://github.com/HGX-Team/hypergraphx
 ```
 
 !! we are working on removing R-base from the dependancies of the library.
 
 ### First steps
 TODO: add basic tutorial
```

### Comparing `hypergraphx-1.4.2/hypergraphx.egg-info/SOURCES.txt` & `hypergraphx-1.4.3/hypergraphx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergraphx-1.4.2/setup.py` & `hypergraphx-1.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import io
 import os
 from setuptools import find_packages, setup
 
+
 def read(*paths, **kwargs):
     content = ""
     with io.open(
-        os.path.join(os.path.dirname(__file__), *paths),
-        encoding=kwargs.get("encoding", "utf8"),
+            os.path.join(os.path.dirname(__file__), *paths),
+            encoding=kwargs.get("encoding", "utf8"),
     ) as open_file:
         content = open_file.read().strip()
     return content
 
+
 setup(
-  name = 'hypergraphx',         
-  version = '1.4.2',      
-  license='BSD-3-Clause license',        
-  description = 'HGX is a multi-purpose, open-source Python library for higher-order network analysis',
-  long_description=read("README.md"),
-  long_description_content_type="text/markdown",
-  author = 'HGX-Team',              
-  author_email = 'lotitoqf@gmail.com',      
-  url = 'https://github.com/HGX-Team/hypergraphx',   
-  keywords = ['hypergraphs', 'networks'], 
-  packages=find_packages(exclude=["tests", ".github"]),
-  install_requires=['numpy',
-                   'scipy',
-                   'networkx',
-                   'rpy2',
-                   'pandas',
-                   'scikit-learn',
-                   'pytest',
-                   'matplotlib',
-                   'seaborn'],
-  classifiers=[
-    'Development Status :: 3 - Alpha',      
-    'Intended Audience :: Developers',      
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: BSD License',   
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
-  ],
+    name='hypergraphx',
+    version='1.4.3',
+    license='BSD-3-Clause license',
+    description='HGX is a multi-purpose, open-source Python library for higher-order network analysis',
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
+    author='HGX-Team',
+    author_email='lotitoqf@gmail.com',
+    url='https://github.com/HGX-Team/hypergraphx',
+    keywords=['hypergraphs', 'networks'],
+    packages=find_packages(exclude=["tests", ".github"]),
+    install_requires=['numpy',
+                      'scipy',
+                      'networkx',
+                      'rpy2',
+                      'pandas',
+                      'scikit-learn',
+                      'pytest',
+                      'matplotlib',
+                      'seaborn'],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: BSD License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+    ],
 )
```

