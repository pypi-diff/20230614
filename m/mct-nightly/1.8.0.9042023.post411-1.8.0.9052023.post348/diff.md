# Comparing `tmp/mct-nightly-1.8.0.9042023.post411.tar.gz` & `tmp/mct-nightly-1.8.0.9052023.post348.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.8.0.9042023.post411.tar", last modified: Sun Apr  9 00:04:12 2023, max compression
+gzip compressed data, was "mct-nightly-1.8.0.9052023.post348.tar", last modified: Tue May  9 00:03:48 2023, max compression
```

## Comparing `mct-nightly-1.8.0.9042023.post411.tar` & `mct-nightly-1.8.0.9052023.post348.tar`

### file list

```diff
@@ -1,577 +1,587 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37136 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34634 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26858 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27514 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 00:04:12.875868 mct-nightly-1.8.0.9042023.post411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-09 00:04:11.000000 mct-nightly-1.8.0.9042023.post411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.916520 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.916520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17223 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/setup.py
```

### Comparing `mct-nightly-1.8.0.9042023.post411/LICENSE.md` & `mct-nightly-1.8.0.9052023.post348/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/PKG-INFO` & `mct-nightly-1.8.0.9052023.post348/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9042023.post411
+Version: 1.8.0.9052023.post348
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -42,23 +42,24 @@
         
         
         In addition, MCT supports different quantization schemes for quantizing weights and activations:
         * Power-Of-Two (hardware-friendly quantization [1])
         * Symmetric
         * Uniform
         
-        Core features:
+        Main features:
         * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Errorm but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
         * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
           * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
           * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
         * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
         * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
         * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
         
         
         #### Experimental features 
         
         Some features are experimental and subject to future changes. 
          
         For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/README.md` & `mct-nightly-1.8.0.9052023.post348/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 
 
 In addition, MCT supports different quantization schemes for quantizing weights and activations:
 * Power-Of-Two (hardware-friendly quantization [1])
 * Symmetric
 * Uniform
 
-Core features:
+Main features:
 * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Errorm but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
 * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
   * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
   * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
 * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
 * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
 * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
 
 
 #### Experimental features 
 
 Some features are experimental and subject to future changes. 
  
 For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9042023.post411
+Version: 1.8.0.9052023.post348
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -42,23 +42,24 @@
         
         
         In addition, MCT supports different quantization schemes for quantizing weights and activations:
         * Power-Of-Two (hardware-friendly quantization [1])
         * Symmetric
         * Uniform
         
-        Core features:
+        Main features:
         * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Errorm but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
         * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
           * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
           * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
         * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
         * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
         * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
         
         
         #### Experimental features 
         
         Some features are experimental and subject to future changes. 
          
         For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 setup.py
 mct_nightly.egg-info/PKG-INFO
 mct_nightly.egg-info/SOURCES.txt
 mct_nightly.egg-info/dependency_links.txt
 mct_nightly.egg-info/requires.txt
 mct_nightly.egg-info/top_level.txt
 model_compression_toolkit/__init__.py
+model_compression_toolkit/constants.py
+model_compression_toolkit/logger.py
 model_compression_toolkit/core/__init__.py
 model_compression_toolkit/core/analyzer.py
 model_compression_toolkit/core/exporter.py
 model_compression_toolkit/core/runner.py
 model_compression_toolkit/core/common/__init__.py
 model_compression_toolkit/core/common/base_substitutions.py
-model_compression_toolkit/core/common/constants.py
 model_compression_toolkit/core/common/data_loader.py
 model_compression_toolkit/core/common/defaultdict.py
 model_compression_toolkit/core/common/framework_implementation.py
 model_compression_toolkit/core/common/framework_info.py
-model_compression_toolkit/core/common/immutable.py
-model_compression_toolkit/core/common/logger.py
 model_compression_toolkit/core/common/memory_computation.py
 model_compression_toolkit/core/common/model_builder_mode.py
 model_compression_toolkit/core/common/model_collector.py
 model_compression_toolkit/core/common/model_validation.py
 model_compression_toolkit/core/common/node_prior_info.py
 model_compression_toolkit/core/common/similarity_analyzer.py
 model_compression_toolkit/core/common/user_info.py
@@ -125,40 +124,25 @@
 model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
 model_compression_toolkit/core/common/substitutions/residual_collapsing.py
 model_compression_toolkit/core/common/substitutions/scale_equalization.py
 model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/common/substitutions/softmax_shift.py
 model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/common/substitutions/weights_activation_split.py
-model_compression_toolkit/core/common/target_platform/__init__.py
-model_compression_toolkit/core/common/target_platform/current_tp_model.py
-model_compression_toolkit/core/common/target_platform/fusing.py
-model_compression_toolkit/core/common/target_platform/op_quantization_config.py
-model_compression_toolkit/core/common/target_platform/operators.py
-model_compression_toolkit/core/common/target_platform/target_platform_model.py
-model_compression_toolkit/core/common/target_platform/target_platform_model_component.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py
-model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py
 model_compression_toolkit/core/common/visualization/__init__.py
 model_compression_toolkit/core/common/visualization/final_config_visualizer.py
 model_compression_toolkit/core/common/visualization/nn_visualizer.py
 model_compression_toolkit/core/common/visualization/tensorboard_writer.py
 model_compression_toolkit/core/keras/__init__.py
 model_compression_toolkit/core/keras/constants.py
 model_compression_toolkit/core/keras/default_framework_info.py
 model_compression_toolkit/core/keras/keras_implementation.py
 model_compression_toolkit/core/keras/keras_model_validation.py
 model_compression_toolkit/core/keras/keras_node_prior_info.py
 model_compression_toolkit/core/keras/kpi_data_facade.py
-model_compression_toolkit/core/keras/quantization_facade.py
 model_compression_toolkit/core/keras/tf_tensor_numpy.py
 model_compression_toolkit/core/keras/back2framework/__init__.py
 model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
 model_compression_toolkit/core/keras/back2framework/float_model_builder.py
 model_compression_toolkit/core/keras/back2framework/instance_builder.py
 model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
 model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
@@ -209,15 +193,14 @@
 model_compression_toolkit/core/keras/visualization/__init__.py
 model_compression_toolkit/core/pytorch/__init__.py
 model_compression_toolkit/core/pytorch/constants.py
 model_compression_toolkit/core/pytorch/default_framework_info.py
 model_compression_toolkit/core/pytorch/kpi_data_facade.py
 model_compression_toolkit/core/pytorch/pytorch_implementation.py
 model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-model_compression_toolkit/core/pytorch/quantization_facade.py
 model_compression_toolkit/core/pytorch/utils.py
 model_compression_toolkit/core/pytorch/back2framework/__init__.py
 model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
 model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
 model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
 model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
 model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
@@ -251,68 +234,14 @@
 model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
 model_compression_toolkit/core/pytorch/reader/__init__.py
 model_compression_toolkit/core/pytorch/reader/graph_builders.py
 model_compression_toolkit/core/pytorch/reader/node_holders.py
 model_compression_toolkit/core/pytorch/reader/reader.py
 model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
 model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
-model_compression_toolkit/core/tpc_models/__init__.py
-model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py
-model_compression_toolkit/core/tpc_models/default_tpc/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py
-model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py
-model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py
-model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py
-model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py
-model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py
-model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py
-model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py
 model_compression_toolkit/exporter/__init__.py
 model_compression_toolkit/exporter/model_exporter/__init__.py
 model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
 model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
 model_compression_toolkit/exporter/model_exporter/keras/__init__.py
 model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
 model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
@@ -340,56 +269,62 @@
 model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
 model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
 model_compression_toolkit/gptq/__init__.py
 model_compression_toolkit/gptq/runner.py
 model_compression_toolkit/gptq/common/__init__.py
 model_compression_toolkit/gptq/common/gptq_config.py
 model_compression_toolkit/gptq/common/gptq_constants.py
+model_compression_toolkit/gptq/common/gptq_framework_implementation.py
 model_compression_toolkit/gptq/common/gptq_graph.py
 model_compression_toolkit/gptq/common/gptq_training.py
 model_compression_toolkit/gptq/keras/__init__.py
+model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
 model_compression_toolkit/gptq/keras/gptq_loss.py
 model_compression_toolkit/gptq/keras/gptq_training.py
 model_compression_toolkit/gptq/keras/graph_info.py
 model_compression_toolkit/gptq/keras/quantization_facade.py
 model_compression_toolkit/gptq/keras/quantizer/__init__.py
 model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
 model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
 model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
 model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
 model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
 model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
 model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
 model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/gptq/pytorch/__init__.py
 model_compression_toolkit/gptq/pytorch/gptq_loss.py
+model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
 model_compression_toolkit/gptq/pytorch/gptq_training.py
 model_compression_toolkit/gptq/pytorch/graph_info.py
 model_compression_toolkit/gptq/pytorch/quantization_facade.py
 model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
 model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
 model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
 model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
 model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
 model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+model_compression_toolkit/legacy/__init__.py
+model_compression_toolkit/legacy/keras_quantization_facade.py
+model_compression_toolkit/legacy/pytorch_quantization_facade.py
 model_compression_toolkit/ptq/__init__.py
 model_compression_toolkit/ptq/runner.py
 model_compression_toolkit/ptq/keras/__init__.py
 model_compression_toolkit/ptq/keras/quantization_facade.py
 model_compression_toolkit/ptq/pytorch/__init__.py
 model_compression_toolkit/ptq/pytorch/quantization_facade.py
 model_compression_toolkit/qat/__init__.py
 model_compression_toolkit/qat/common/__init__.py
-model_compression_toolkit/qat/common/constants.py
 model_compression_toolkit/qat/common/qat_config.py
 model_compression_toolkit/qat/keras/__init__.py
 model_compression_toolkit/qat/keras/quantization_facade.py
 model_compression_toolkit/qat/keras/quantizer/__init__.py
 model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
 model_compression_toolkit/qat/keras/quantizer/quant_utils.py
 model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
@@ -402,14 +337,15 @@
 model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
 model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
 model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
 model_compression_toolkit/quantizers_infrastructure/__init__.py
+model_compression_toolkit/quantizers_infrastructure/constants.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
@@ -460,8 +396,80 @@
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
 model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+model_compression_toolkit/target_platform_capabilities/__init__.py
+model_compression_toolkit/target_platform_capabilities/constants.py
+model_compression_toolkit/target_platform_capabilities/immutable.py
+model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 # limitations under the License.
 # ==============================================================================
 
 
 from typing import Callable
 
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
-from model_compression_toolkit.core.common import FrameworkInfo, Logger
-from model_compression_toolkit.core.common.constants import NUM_SAMPLES_DISTANCE_TENSORBOARD
+from model_compression_toolkit.core.common import FrameworkInfo
+from model_compression_toolkit.constants import NUM_SAMPLES_DISTANCE_TENSORBOARD
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 
 from model_compression_toolkit.core.common.similarity_analyzer import compute_cs
 from model_compression_toolkit.core.common.visualization.nn_visualizer import NNVisualizer
 
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import TensorboardWriter
+from model_compression_toolkit.logger import Logger
 
 
 def analyzer_model_quantization(representative_data_gen: Callable,
                                 tb_w: TensorboardWriter,
                                 tg: Graph,
                                 fw_impl: FrameworkImplementation,
                                 fw_info: FrameworkInfo):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,12 +13,11 @@
 # limitations under the License.
 # ==============================================================================
 from model_compression_toolkit.core.common.quantization import quantization_params_generation
 from model_compression_toolkit.core.common.base_substitutions import BaseSubstitution
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.logger import Logger
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, DEFAULTCONFIG
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import max_power_of_two
 from model_compression_toolkit.core.common.collectors.statistics_collector import StatsCollector, NoStatsCollector
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 class BaseCollector(object):
     """
     Base class for statistics collection object.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import numpy as np
 
 from model_compression_toolkit.core.common.collectors.base_collector import BaseCollector
-from model_compression_toolkit.core.common.constants import LAST_AXIS
+from model_compression_toolkit.constants import LAST_AXIS
 
 
 class MeanCollector(BaseCollector):
     """
         Class to collect observed per channel mean values of tensors that goes through it (passed to update).
         The mean is calculated using a exponential moving average with bias correction.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
 from model_compression_toolkit.core.common.collectors.base_collector import BaseCollector
-from model_compression_toolkit.core.common.constants import LAST_AXIS
+from model_compression_toolkit.constants import LAST_AXIS
 
 
 class MinMaxPerChannelCollector(BaseCollector):
     """
     Class to collect observed mix/max values of tensors that goes through it (passed to update).
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
 import importlib
 
 # Supported frameworks in MCT:
 TENSORFLOW = 'tensorflow'
 PYTORCH = 'pytorch'
 FOUND_TF = importlib.util.find_spec(TENSORFLOW) is not None and importlib.util.find_spec(
     "tensorflow_model_optimization") is not None
@@ -43,17 +44,14 @@
 REUSE_GROUP = 'reuse_group'
 LAST_AXIS = -1
 
 # Data types:
 DATA_TYPE = 'dtype'
 FLOAT_32 = 'float32'
 
-# Version
-LATEST = 'latest'
-
 # Number of Tensorboard cosine-similarity plots to add:
 NUM_SAMPLES_DISTANCE_TENSORBOARD = 20
 
 # num bits for shift negative non linear node
 SHIFT_NEGATIVE_NON_LINEAR_NUM_BITS = 16
 
 # Default bitwidth for disabled quantization candidate
@@ -115,16 +113,14 @@
 WEIGHTS_QUANT_PARAMS_FN = 'weights_quantization_params_fn'
 WEIGHTS_CHANNELS_AXIS = 'weights_channels_axis'
 
 # Memory graph constants
 DUMMY_NODE = 'dummy_node'
 DUMMY_TENSOR = 'dummy_tensor'
 
-# TP Model constants
-OPS_SET_LIST = 'ops_set_list'
 
 # TF Input node base name
 INPUT_BASE_NAME = 'base_input'
 
 # Jacobian-weights constants
 MIN_JACOBIANS_ITER = 10
-JACOBIANS_COMP_TOLERANCE = 1e-3
+JACOBIANS_COMP_TOLERANCE = 1e-3
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 from abc import ABC, abstractmethod
 from typing import Callable, Any, List, Tuple, Dict
 
 import numpy as np
 
-from model_compression_toolkit import MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.mixed_precision.sensitivity_evaluation import SensitivityEvaluation
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
@@ -284,21 +284,14 @@
         Returns:
             A list of the framework substitutions used after we apply second moment statistics.
         """
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s get_substitutions_after_second_moment_correction '
                              f'method.')  # pragma: no cover
 
-    @abstractmethod
-    def get_gptq_trainer_obj(self):
-        """
-        Returns: GPTQTrainer object
-        """
-        raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_gptq_trainer method.')  # pragma: no cover
 
     @abstractmethod
     def get_sensitivity_evaluator(self,
                                   graph: Graph,
                                   quant_config: MixedPrecisionQuantizationConfigV2,
                                   representative_data_gen: Callable,
                                   fw_info: FrameworkInfo,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from enum import Enum
 from typing import Dict, Any, List
 
 
 
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import QuantizationMethod
 
 
 class ChannelAxis(Enum):
     """
 
     Index of output channels axis:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from typing import Any, List
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.layer_filter_params import LayerFilterParams
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.layer_filter_params import LayerFilterParams
 
 
 def filter_fusing_patterns(fusing_patterns: List[List[Any]], node: BaseNode, idx: int = 0) -> List[List[Any]]:
     """
     Update relevant fusing patterns object if layer number 'idx' inside the fusion matches the node
     Args:
         fusing_patterns: supported fusings
@@ -29,15 +29,15 @@
         idx: index of layer in the fusion
     Returns:
         fusing_patterns after filtering non-relevant fusions
     """
     valid_fusing_patterns = []
     for i,fusing_pattern in enumerate(fusing_patterns):
         if idx < len(fusing_pattern):
-            if (type(fusing_pattern[idx]) == LayerFilterParams and fusing_pattern[idx].match(node)) or fusing_pattern[idx] == node.type:
+            if (type(fusing_pattern[idx]) == LayerFilterParams and node.is_match_filter_params(fusing_pattern[idx])) or fusing_pattern[idx] == node.type:
                 valid_fusing_patterns.append(fusing_pattern)
 
     # Return only valid patterns for this node
     return valid_fusing_patterns
 
 
 def is_valid_fusion(fusing_patterns: List[List[Any]], nodes: List[BaseNode]) -> bool:
@@ -53,15 +53,15 @@
     if fusion_depth <= 1:
         return False
     for fusing_pattern in fusing_patterns:
         if fusion_depth != len(fusing_pattern):
             continue
         counter = 0
         for i,layer in enumerate(fusing_pattern):
-            if (type(layer) == LayerFilterParams and layer.match(nodes[i])) or layer == nodes[i].type:
+            if (type(layer) == LayerFilterParams and nodes[i].is_match_filter_params(layer)) or layer == nodes[i].type:
                 counter += 1
         if counter == fusion_depth:
             return True
     return False
 
 
 def disable_nodes_activation_quantization(nodes: List[BaseNode]):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX, EDGE_SOURCE_INDEX
 from model_compression_toolkit.core.common.graph.edge import Edge, convert_to_edge
 from model_compression_toolkit.core.common.graph.graph_searches import GraphSearches
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 from model_compression_toolkit.core.common.collectors.statistics_collector import scale_statistics, shift_statistics
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 
 OutTensor = namedtuple('OutTensor', 'node node_out_index')
 
 
 class Graph(nx.MultiDiGraph, GraphSearches):
     """
     Base graph representing a model to be optimized.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 # ==============================================================================
 
 import copy
 from typing import Dict, Any, Tuple, List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import WEIGHTS_NBITS_ATTRIBUTE, CORRECTED_BIAS_ATTRIBUTE, \
+from model_compression_toolkit.constants import WEIGHTS_NBITS_ATTRIBUTE, CORRECTED_BIAS_ATTRIBUTE, \
     ACTIVATION_NBITS_ATTRIBUTE
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationConfigOptions, \
+    TargetPlatformCapabilities, LayerFilterParams
 
 
 class BaseNode:
     """
     Class to represent a node in a graph that represents the model.
     """
 
@@ -425,7 +428,60 @@
         Checks whether the node has quantization configuration candidates that enable activation quantization.
 
         Returns: True if the node has at list one quantization configuration candidate with activation quantization enabled.
         """
 
         return len(self.candidates_quantization_cfg) > 0 and \
                any([c.activation_quantization_cfg.enable_activation_quantization for c in self.candidates_quantization_cfg])
+
+    def get_qco(self, tpc: TargetPlatformCapabilities) -> QuantizationConfigOptions:
+        """
+        Get the QuantizationConfigOptions of the node according
+        to the mappings from layers/LayerFilterParams to the OperatorsSet in the TargetPlatformModel.
+
+        Args:
+            tpc: TPC to extract the QuantizationConfigOptions for the node
+
+        Returns:
+            QuantizationConfigOptions of the node.
+        """
+
+        if tpc is None:
+            Logger.error(f'Can not retrieve QC options for None TPC')  # pragma: no cover
+
+        for fl, qco in tpc.filterlayer2qco.items():
+            if self.is_match_filter_params(fl):
+                return qco
+        if self.type in tpc.layer2qco:
+            return tpc.layer2qco.get(self.type)
+        return tpc.tp_model.default_qco
+
+
+    def is_match_filter_params(self, layer_filter_params: LayerFilterParams) -> bool:
+        """
+        Check if the node matches a LayerFilterParams according to its
+        layer, conditions and keyword-arguments.
+
+        Args:
+            layer_filter_params: LayerFilterParams to check if the node matches its properties.
+
+        Returns:
+            Whether the node matches to the LayerFilterParams properties.
+        """
+        # Check the node has the same type as the layer in LayerFilterParams
+        if layer_filter_params.layer != self.type:
+            return False
+
+        # Get attributes from node to filter
+        layer_config = self.framework_attr
+        if hasattr(self, "op_call_kwargs"):
+            layer_config.update(self.op_call_kwargs)
+
+        for attr, value in layer_filter_params.kwargs.items():
+            if layer_config.get(attr) != value:
+                return False
+
+        for c in layer_filter_params.conditions:
+            if not c.match(layer_config):
+                return False
+
+        return True
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Any, List, Tuple
 import networkx as nx
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 class DirectedBipartiteGraph(nx.DiGraph):
     """
     Directed Bipartite graph representation.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from typing import List, Tuple, Dict
 
 from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.constants import DUMMY_TENSOR, DUMMY_NODE
+from model_compression_toolkit.constants import DUMMY_TENSOR, DUMMY_NODE
 from model_compression_toolkit.core.common.graph.memory_graph.cut import Cut
 from model_compression_toolkit.core.common.graph.memory_graph.memory_element import MemoryElements
 from model_compression_toolkit.core.common.graph.memory_graph.memory_graph import ActivationMemoryTensor, MemoryGraph
 
 
 class DummyType:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Dict, Any, Tuple
 
-from model_compression_toolkit import FrameworkInfo
-from model_compression_toolkit.core.common.constants import VIRTUAL_ACTIVATION_WEIGHTS_NODE_PREFIX, \
+from model_compression_toolkit.core import FrameworkInfo
+from model_compression_toolkit.constants import VIRTUAL_ACTIVATION_WEIGHTS_NODE_PREFIX, \
     VIRTUAL_WEIGHTS_SUFFIX, VIRTUAL_ACTIVATION_SUFFIX, FLOAT_BITWIDTH
 
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 import numpy as np
 
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/immutable.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/logger.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common.constants import BITS_TO_BYTES
 
-
-def compute_quantize_tensor_memory_bytes(tensor_size: float, n_bits: int) -> float:
-    """
-    A utility function to compute the actual memory size of a tensor for a given bit-width.
-
-    Args:
-        tensor_size: The number of parameters in the tensor.
-        n_bits: The bit-width in which the tensor values are represented.
-
-    Returns: The size of the tensor in memory in bytes.
-
-    """
-    return tensor_size * n_bits / BITS_TO_BYTES
+# Quantizers constants (for GPTQ, QAT, etc.)
+FQ_MIN = "min"
+FQ_MAX = "max"
+THRESHOLD_TENSOR = "ptq_threshold_tensor"
+WEIGHTS_QUANTIZATION_PARAMS = 'weights_quantization_params'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,33 +14,31 @@
 # ==============================================================================
 
 import copy
 
 from typing import Any, List
 
 from model_compression_toolkit.core.common import Graph, BaseNode
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def set_bit_widths(mixed_precision_enable: bool,
-                   graph_to_set_bit_widths: Graph,
+                   graph: Graph,
                    bit_widths_config: List[int] = None) -> Graph:
     """
     Set bit widths configuration to nodes in a graph. For each node, use the desired index
     in bit_widths_config to finalize the node weights and activation quantization configuration.
 
     Args:
         mixed_precision_enable: Is mixed precision enabled.
-        graph_to_set_bit_widths: A prepared for quantization graph to set its bit widths.
+        graph: A prepared for quantization graph to set its bit widths.
         bit_widths_config: MP configuration (a list of indices: one for each node's candidate
         quantization configuration).
 
     """
-    graph = copy.deepcopy(graph_to_set_bit_widths)
-
     if mixed_precision_enable:
         assert all([len(n.candidates_quantization_cfg) > 0 for n in graph.get_configurable_sorted_nodes()]), \
             "All configurable nodes in graph should have at least one candidate configuration in mixed precision mode"
 
         Logger.info(f'Set bit widths from configuration: {bit_widths_config}')
         # Get a list of nodes' names we need to finalize (that they have at least one weight qc candidate).
         sorted_nodes_names = graph.get_configurable_sorted_nodes_names()
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable, Any
 import numpy as np
 
-from model_compression_toolkit import FrameworkInfo, KPI, CoreConfig
+from model_compression_toolkit.core import FrameworkInfo, KPI, CoreConfig
 from model_compression_toolkit.core.common import Graph
-from model_compression_toolkit.core.common.constants import FLOAT_BITWIDTH
+from model_compression_toolkit.constants import FLOAT_BITWIDTH
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.runner import read_model_to_graph, get_finalized_graph
-from model_compression_toolkit.core.common.logger import Logger
 
 
 def compute_kpi_data(in_model: Any,
                      representative_data_gen: Callable,
                      core_config: CoreConfig,
                      tpc: TargetPlatformCapabilities,
                      fw_info: FrameworkInfo,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # ==============================================================================
 from enum import Enum
 from functools import partial
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import Graph, BaseNode
-from model_compression_toolkit.core.common.constants import BITS_TO_BYTES, FLOAT_BITWIDTH
+from model_compression_toolkit.constants import BITS_TO_BYTES, FLOAT_BITWIDTH
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.virtual_activation_weights_node import VirtualActivationWeightsNode, \
     VirtualSplitWeightsNode, VirtualSplitActivationNode
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def weights_size_kpi(mp_cfg: List[int],
                      graph: Graph,
                      fw_info: FrameworkInfo,
                      fw_impl: FrameworkImplementation) -> np.ndarray:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from enum import Enum
 from typing import List, Callable, Tuple
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.mixed_precision.distance_weighting import get_average_weights
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, DEFAULTCONFIG
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse
 
 
 class MixedPrecisionQuantizationConfigV2:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 # ==============================================================================
 
 import copy
 from enum import Enum
 import numpy as np
 from typing import List, Callable, Dict
 
-from model_compression_toolkit import MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.core.common import Graph, Logger
+from model_compression_toolkit.core import MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core.common import Graph
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI, KPITarget
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_functions_mapping import kpi_functions_mapping
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_search_manager import MixedPrecisionSearchManager
 from model_compression_toolkit.core.common.mixed_precision.search_methods.linear_programming import \
     mp_integer_programming_search
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.solution_refinement_procedure import \
     greedy_solution_refinement_procedure
 from model_compression_toolkit.core.common.substitutions.apply_substitutions import substitute
+from model_compression_toolkit.logger import Logger
 
 
 class BitWidthSearchMethod(Enum):
     # When adding a new search_methods MP configuration method, these enum and factory dictionary
     # should be updated with it's kind and a search_method implementation.
     INTEGER_PROGRAMMING = 0
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 
 from typing import Callable, Tuple
 from typing import Dict, List
 import numpy as np
 
 from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.virtual_activation_weights_node import VirtualActivationWeightsNode, \
     VirtualSplitWeightsNode, VirtualSplitActivationNode
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPITarget, KPI
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_aggregation_methods import MpKpiAggregation
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_methods import MpKpiMetric
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 
 import numpy as np
 from pulp import *
 from tqdm import tqdm
 from typing import Dict, List, Tuple, Callable
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI, KPITarget
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_search_manager import MixedPrecisionSearchManager
 
 # Limit ILP solver runtime in seconds
 SOLVER_TIME_LIMIT = 60
 
 def mp_integer_programming_search(search_manager: MixedPrecisionSearchManager,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 import copy
 
 import numpy as np
 from typing import Callable, Any, List
 
-from model_compression_toolkit import FrameworkInfo, MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import FrameworkInfo, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 
 
 class SensitivityEvaluation:
     """
     Class to wrap and manage the computation on distance metric for Mixed-Precision quantization search.
     It provides a function that evaluates the sensitivity of a bit-width configuration for the MP model.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import List
 
-from model_compression_toolkit import KPI
+from model_compression_toolkit.core import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_search_manager import \
     MixedPrecisionSearchManager
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 import numpy as np
 
 
 def greedy_solution_refinement_procedure(mp_solution: List[int],
                                          search_manager: MixedPrecisionSearchManager,
                                          target_kpi: KPI) -> List[int]:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import numpy as np
 from typing import List
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 
 
 class ModelCollector:
     """
     Build a Keras model from a graph for statistics collection purposes.
     The ModelCollector builds a float model that its outputs are all layers outputs, so after
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import Any
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 
 
 class ModelValidation:
     """
     Class to define validation methods in order to validate the received model to quantize.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from typing import Callable
 
-from model_compression_toolkit.core.common import Graph, Logger
+from model_compression_toolkit.core.common import Graph
+from model_compression_toolkit.logger import Logger
+
+
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.quantization.quantization_params_fn_selection import \
     get_activation_quantization_params_fn, get_weights_quantization_params_fn
 from model_compression_toolkit.core.common.quantization.quantization_fn_selection import \
     get_weights_quantization_fn
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import copy
 from typing import List
 
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.network_editors import EditRule
 
 
@@ -32,13 +31,12 @@
         groups of layers by how they should be quantized, etc.)
         network_editor: List of edit rules to apply to the graph.
 
     Returns:
         The graph after it has been applied the edit rules from the network editor list.
 
     """
-    # graph = copy.deepcopy(graph_to_edit)
     for edit_rule in network_editor:
         filtered_nodes = graph.filter(edit_rule.filter)
         for node in filtered_nodes:
             edit_rule.action.apply(node, graph, fw_info)
     # return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common.constants import ACTIVATION_QUANTIZATION_CFG, WEIGHTS_QUANTIZATION_CFG, QC, \
+from model_compression_toolkit.constants import ACTIVATION_QUANTIZATION_CFG, WEIGHTS_QUANTIZATION_CFG, QC, \
     OP_CFG, ACTIVATION_QUANTIZATION_FN, WEIGHTS_QUANTIZATION_FN, ACTIVATION_QUANT_PARAMS_FN, WEIGHTS_QUANT_PARAMS_FN, \
     WEIGHTS_CHANNELS_AXIS
 from model_compression_toolkit.core.common.quantization.node_quantization_config import BaseNodeQuantizationConfig, \
     NodeWeightsQuantizationConfig, NodeActivationQuantizationConfig
 
 
 ##########################################
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from typing import List
 
 from model_compression_toolkit.core.common import Graph, BaseNode
-from model_compression_toolkit.core.common.constants import FLOAT_BITWIDTH
+from model_compression_toolkit.constants import FLOAT_BITWIDTH
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 
 
-def filter_nodes_candidates(graph_to_filter: Graph):
+def filter_nodes_candidates(graph: Graph):
     """
     Filters the graph's nodes candidates configuration list.
     We apply this after mark activation operation to eliminate nodes that their activation are no longer being quantized
     from the mixed-precision search.
     Updating the lists is preformed inplace on the graph object.
 
     Args:
-        graph_to_filter: Graph for which to add quantization info to each node.
+        graph: Graph for which to add quantization info to each node.
     """
-    graph = copy.deepcopy(graph_to_filter)
     nodes = list(graph.nodes)
     for n in nodes:
         n.candidates_quantization_cfg = filter_node_candidates(node=n)
 
     return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # ==============================================================================
 
 
 from typing import Callable, Any
 
 import numpy as np
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.quantization.quantization_params_fn_selection import \
     get_activation_quantization_params_fn, get_weights_quantization_params_fn
 
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, \
     QuantizationErrorMethod
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig
 
 
 ##########################################
 # Every node holds a quantization configuration
 # for its weights and activations quantization, and a different quantization
 # configuration for its activation quantization configuration.
 ##########################################
@@ -252,15 +252,15 @@
         self.weights_channels_axis = weights_channels_axis
         self.weights_quantization_params = {}
         self.weights_quantization_method = op_cfg.weights_quantization_method
         self.weights_error_method = qc.weights_error_method
         self.weights_n_bits = op_cfg.weights_n_bits
         self.weights_bias_correction = qc.weights_bias_correction
         self.weights_second_moment_correction = qc.weights_second_moment_correction
-        self.weights_per_channel_threshold = qc.weights_per_channel_threshold
+        self.weights_per_channel_threshold = op_cfg.weights_per_channel_threshold
         self.enable_weights_quantization = op_cfg.enable_weights_quantization
         self.min_threshold = qc.min_threshold
         self.l_p_value = qc.l_p_value
 
 
     @property
     def weights_error_method(self) -> QuantizationErrorMethod:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import math
 from enum import Enum
 
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD
 
 
 class QuantizationErrorMethod(Enum):
     """
     Method for quantization threshold selection:
 
     NOCLIPPING - Use min/max values as thresholds.
@@ -90,15 +90,15 @@
             One may create a quantization configuration to quantize a model according to.
             For example, to quantize a model's weights and activation using thresholds, such that
             weights threshold selection is done using MSE, activation threshold selection is done using NOCLIPPING (min/max),
             enabling relu_bound_to_power_of_2, weights_bias_correction, and quantizing the weights per-channel,
             one can instantiate a quantization configuration:
 
             >>> import model_compression_toolkit as mct
-            >>> qc = mct.QuantizationConfig(activation_error_method=mct.QuantizationErrorMethod.NOCLIPPING,weights_error_method=mct.QuantizationErrorMethod.MSE,relu_bound_to_power_of_2=True,weights_bias_correction=True,weights_per_channel_threshold=True)
+            >>> qc = mct.core.QuantizationConfig(activation_error_method=mct.core.QuantizationErrorMethod.NOCLIPPING,weights_error_method=mct.core.QuantizationErrorMethod.MSE,relu_bound_to_power_of_2=True,weights_bias_correction=True,weights_per_channel_threshold=True)
 
 
             The QuantizationConfig instanse can then be passed to
             :func:`~model_compression_toolkit.ptq.keras_post_training_quantization`
 
         """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from collections.abc import Callable
 from functools import partial
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.core.common.quantization.quantizers.kmeans_quantizer import kmeans_quantizer
 from model_compression_toolkit.core.common.quantization.quantizers.lut_kmeans_quantizer import lut_kmeans_quantizer
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import power_of_two_quantizer, \
     symmetric_quantizer, uniform_quantizer
 
 
 def get_weights_quantization_fn(weights_quantization_method: QuantizationMethod) -> Callable:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from collections.abc import Callable
 from functools import partial
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.kmeans_params import kmeans_tensor
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.lut_kmeans_params import \
     lut_kmeans_tensor, lut_kmeans_histogram
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.symmetric_selection import \
     symmetric_selection_tensor, symmetric_selection_histogram
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.uniform_selection import \
     uniform_selection_histogram, uniform_selection_tensor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # limitations under the License.
 # ==============================================================================
 from copy import deepcopy
 from typing import Tuple, Callable
 import numpy as np
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse, compute_mae, compute_lp_norm
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.core.common.constants import FLOAT_32
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FLOAT_32
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor
 
+
 def _mse_error_histogram(q_bins: np.ndarray,
                          q_count: np.ndarray,
                          bins: np.ndarray,
                          counts: np.ndarray) -> np.float32:
     """
     Compute the error function between a histogram to its quantized version.
     The error is computed based on the mean square error the distributions have.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 from sklearn.cluster import KMeans
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.core.common.constants import CLUSTER_CENTERS, SCALE_PER_CHANNEL, MIN_THRESHOLD, EPS
+from model_compression_toolkit.constants import CLUSTER_CENTERS, SCALE_PER_CHANNEL, MIN_THRESHOLD, EPS
 
 
 def kmeans_tensor(tensor_data: np.ndarray,
                   p: int,
                   n_bits: int,
                   per_channel: bool = False,
                   channel_axis: int = 1,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 from sklearn.cluster import KMeans
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.core.common.constants import CLUSTER_CENTERS, MIN_THRESHOLD, SCALE_PER_CHANNEL, \
+from model_compression_toolkit.constants import CLUSTER_CENTERS, MIN_THRESHOLD, SCALE_PER_CHANNEL, \
     MULTIPLIER_N_BITS, THRESHOLD
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     max_power_of_two, int_quantization_with_threshold
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.symmetric_selection import \
     symmetric_selection_tensor
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.power_of_two_selection import \
     power_of_two_selection_tensor
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def lut_kmeans_tensor(tensor_data: np.ndarray,
                       p: int,
                       n_bits: int,
                       per_channel: bool = False,
                       channel_axis: int = 1,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_selection_tensor_search, qparams_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import max_power_of_two, get_tensor_max
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 def power_of_two_selection_tensor(tensor_data: np.ndarray,
                                   p: int,
                                   n_bits: int,
                                   per_channel: bool = False,
                                   channel_axis: int = 1,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
-from typing import Tuple, Dict
+from typing import Dict
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
-from model_compression_toolkit.core.common.constants import SIGNED
+from model_compression_toolkit.constants import SIGNED
 from model_compression_toolkit.core.common.quantization import quantization_params_generation
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeActivationQuantizationConfig
 
 
 def get_activations_qparams(activation_quant_cfg: NodeActivationQuantizationConfig,
                             nodes_prior_info: NodePriorInfo,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.core.common import Graph, BaseNode, Logger
+from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_activations_computation \
     import get_activations_qparams
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_weights_computation import \
     get_weights_qparams, get_channels_axis
 
 
 def calculate_quantization_params(graph: Graph,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 import itertools
 from collections.abc import Callable
 from typing import Any, Tuple, Dict
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD, DEFAULT_TOL, DEFAULT_DEC_FACTOR, \
+from model_compression_toolkit.constants import MIN_THRESHOLD, DEFAULT_TOL, DEFAULT_DEC_FACTOR, \
     SYMMETRIC_TENSOR_PER_CHANNEL_N_INTERVALS, SYMMETRIC_TENSOR_PER_CHANNEL_N_ITER, SYMMETRIC_TENSOR_DEC_FREQ, \
     SYMMETRIC_TENSOR_PER_CHANNEL_DEC_FREQ, SYMMETRIC_TENSOR_N_INTERVALS, SYMMETRIC_TENSOR_N_ITER, \
     UNIFORM_TENSOR_PER_CHANNEL_N_ITER, UNIFORM_TENSOR_N_ITER, SYMMETRIC_HISTOGRAM_DEC_FREQ, SYMMETRIC_HISTOGRAM_N_ITER, \
     SYMMETRIC_HISTOGRAM_N_INTERVALS, UNIFORM_HISTOGRAM_N_ITER, BOTTOM_FACTOR, UPPER_FACTOR, UNIFORM_TENSOR_N_SAMPLES, \
     UNIFORM_HISTOGRAM_N_SAMPLES, DEC_RANGE_UPPER, DEC_RANGE_BOTTOM
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import quantize_tensor, \
     reshape_tensor_for_per_channel_search, uniform_quantize_tensor, get_output_shape
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any, Tuple
 
 import numpy as np
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeWeightsQuantizationConfig
 
 
 # If the quantization config does not contain kernel channel mapping or the weights
 # quantization is not per-channel, we use a dummy channel mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function, _kl_error_histogram
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_symmetric_selection_tensor_search, \
     qparams_symmetric_selection_histogram_search, kl_qparams_symmetric_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     get_tensor_max
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 def symmetric_selection_tensor(tensor_data: np.ndarray,
                                p: int,
                                n_bits: int,
                                per_channel: bool = False,
                                channel_axis: int = 1,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_uniform_selection_tensor_search, qparams_uniform_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import get_tensor_max, \
     get_tensor_min
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 def uniform_selection_tensor(tensor_data: np.ndarray,
                              p: int,
                              n_bits: int,
                              per_channel: bool = False,
                              channel_axis: int = 1,
                              n_iter: int = 10,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,43 @@
 import copy
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.quantize_node import get_quantized_kernel_by_weights_qc
+from model_compression_toolkit.logger import Logger
 
 
-def quantize_graph_weights(graph_to_quantize: Graph,
+def quantize_graph_weights(graph: Graph,
                            fw_info: FrameworkInfo,
                            fw_impl: FrameworkImplementation) -> Graph:
     """
     Get a graph representing a model, and quantize its nodes' weights.
     Each node is quantized according to the passed framework info and quantization configuration.
     If weights bias correction is enabled in the quantization configuration, a bias correction term
     is calculated and subtracted from the original node's bias. The graph is quantized in-place.
 
     Args:
-        graph_to_quantize: Graph to quantize its nodes.
+        graph: Graph to quantize its nodes.
         fw_info: Framework information needed for quantizing the graph's nodes' weights and activations.
         fw_impl: FrameworkImplementation with specific framework implementations.
 
     """
-    graph = copy.deepcopy(graph_to_quantize)
     # Iterate over nodes in the graph and quantize each node's weights and activations
     # (according to operators groups in framework info).
     for n in graph.nodes():
 
         if n.is_weights_quantization_enabled():
             quantized_kernel, io_channels_axes = get_quantized_kernel_by_weights_qc(fw_info,
                                                                                     n,
                                                                                     n.final_weights_quantization_cfg,
                                                                                     fw_impl=fw_impl)
 
-            common.Logger.debug(
+            Logger.debug(
                 f'Node name: {n.name} has the following quantization params: '
                 f'{str(n.final_weights_quantization_cfg.weights_quantization_params)}')
 
             # Set the kernel node to be the quantized kernel.
             n.set_weights_by_keys(fw_impl.constants.KERNEL, quantized_kernel)
 
     return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeWeightsQuantizationConfig
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_weights_computation \
     import \
     get_channels_axis
@@ -42,15 +42,15 @@
     Returns:
         A quantized kernel of the node using a weights quantization configuration.
     """
 
     # If weights should be quantized per-channel but a kernel channels mapping is missing.
     if weights_qc.weights_per_channel_threshold and fw_info.kernel_channels_mapping is \
             None:
-        common.Logger.warning(
+        Logger.warning(
             'Weights Per Channel Quantization requires channel mapping function but framework info '
             'does not contain one')
     output_channels_axis, input_channels_axis = get_channels_axis(weights_qc,
                                                                   fw_info,
                                                                   n.type)
 
     Logger.debug(f'quantizing {n.name} with {weights_qc.weights_n_bits} bits')
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from sklearn.cluster import KMeans
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import CLUSTER_CENTERS, MIN_THRESHOLD, SCALE_PER_CHANNEL
+from model_compression_toolkit.constants import CLUSTER_CENTERS, MIN_THRESHOLD, SCALE_PER_CHANNEL
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import kmeans_assign_clusters
 
 
 def kmeans_quantizer(tensor_data: np.ndarray,
                         n_bits: int,
                         signed: bool,
                         quantization_params: dict,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import CLUSTER_CENTERS, SCALE_PER_CHANNEL, \
+from model_compression_toolkit.constants import CLUSTER_CENTERS, SCALE_PER_CHANNEL, \
     MULTIPLIER_N_BITS
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import kmeans_assign_clusters, \
     get_quantized_tensor, int_quantization_with_threshold
 
 
 def lut_kmeans_quantizer(tensor_data: np.ndarray,
                         n_bits: int,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 
 
 from typing import Tuple, List
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD, EPS
+from model_compression_toolkit.constants import MIN_THRESHOLD, EPS
 from model_compression_toolkit.core import common
+from model_compression_toolkit.logger import Logger
+
 
 def max_power_of_two(x: np.ndarray,
                      min_threshold: float = MIN_THRESHOLD) -> np.ndarray:
     """
     Compute the max power-of-two threshold for quantizing a tensor x. The threshold
     is determined by the maximal value of the tensor (or min_threshold, the greater one, if a
     minimal value needed to be enforced for the threshold calculation).
@@ -232,15 +234,15 @@
         n_bits: number of bits the tensor will be quantized with
         is_uniform_quantization (bool): Whether the tensor will be quantized with uniform quantization (min-max)
 
     Returns: maximal value (or values).
 
     """
     if n_bits < 1:
-        common.Logger.error("n_bits must be positive")
+        Logger.error("n_bits must be positive")
     if is_uniform_quantization:
         expansion_factor = 1.0
     elif n_bits == 1:
         expansion_factor = 0.0
     else:
         expansion_factor = np.power(2.0, n_bits - 1) / (np.power(2.0, n_bits - 1) - 1)
     if per_channel:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import RANGE_MIN, RANGE_MAX, THRESHOLD
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import RANGE_MIN, RANGE_MAX, THRESHOLD
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor, \
     quantize_tensor
 
 
 def threshold_is_power_of_two(threshold: np.ndarray, per_channel: bool) -> bool:
     if per_channel:
         thresholds_per_channel = threshold.flatten()
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import copy
 from typing import List
 
-from model_compression_toolkit.core.common import Logger, BaseNode
+from model_compression_toolkit.core.common import BaseNode
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeActivationQuantizationConfig
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
 from model_compression_toolkit.core.common.quantization.quantization_params_fn_selection import \
     get_activation_quantization_params_fn, get_weights_quantization_params_fn
 from model_compression_toolkit.core.common.quantization.quantization_fn_selection import \
     get_weights_quantization_fn
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import OpQuantizationConfig, \
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
     QuantizationConfigOptions
 
 
 def set_quantization_configuration_to_graph(graph: Graph,
                                             quant_config: QuantizationConfig,
                                             mixed_precision_enable: bool = False) -> Graph:
     """
@@ -44,22 +45,21 @@
         quant_config: Quantization configuration containing parameters for how the graph should be quantized.
         mixed_precision_enable: is mixed precision enabled
 
     Returns:
         The graph with quantization configurations attached to each node in it.
     """
 
-    graph_with_qcs = copy.deepcopy(graph)
-    for n in graph_with_qcs.nodes:
+    for n in graph.nodes:
         set_quantization_configs_to_node(node=n,
                                          quant_config=quant_config,
                                          fw_info=graph.fw_info,
                                          tpc=graph.tpc,
                                          mixed_precision_enable=mixed_precision_enable)
-    return graph_with_qcs
+    return graph
 
 
 def set_quantization_configs_to_node(node: BaseNode,
                                      quant_config: QuantizationConfig,
                                      fw_info: FrameworkInfo,
                                      tpc: TargetPlatformCapabilities,
                                      mixed_precision_enable: bool = False):
@@ -69,15 +69,15 @@
     Args:
         node: Node to set its quantization configurations.
         quant_config: Quantization configuration to generate the node's configurations from.
         fw_info: Information needed for quantization about the specific framework.
         tpc: TargetPlatformCapabilities to get default OpQuantizationConfig.
         mixed_precision_enable: is mixed precision enabled
     """
-    node_qc_options = tpc.get_qco_by_node(node)
+    node_qc_options = node.get_qco(tpc)
 
     # Create QC candidates for weights and activation combined
     weight_channel_axis = fw_info.kernel_channels_mapping.get(node.type)[0]
     node.candidates_quantization_cfg = _create_node_candidates_qc(quant_config,
                                                                   fw_info,
                                                                   weight_channel_axis,
                                                                   node_qc_options,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import Any, Tuple
+from typing import Any
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import EPS
+from model_compression_toolkit.constants import EPS
 
 #########################
 #  Helpful functions
 #########################
 
 
 def validate_before_compute_similarity(float_tensor: Any, fxp_tensor: Any):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 
 
 def apply_bias_correction_to_graph(graph_to_apply_bias_correction: Graph,
                                    core_config: CoreConfig,
                                    fw_impl: FrameworkImplementation) -> Graph:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import copy
 from typing import Callable, Any
 
 from tqdm import tqdm
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common import Graph
@@ -88,32 +87,31 @@
 
     quantized_model, user_info = fw_impl.model_builder(quantized_tg,
                                                        mode=ModelBuilderMode.FLOAT,
                                                        fw_info=fw_info)
     return quantized_model
 
 
-def apply_second_moment_correction_to_graph(graph_to_apply_second_moment_correction: Graph,
+def apply_second_moment_correction_to_graph(graph: Graph,
                                             representative_data_gen: Callable,
                                             core_config: CoreConfig,
                                             fw_info: FrameworkInfo,
                                             fw_impl: FrameworkImplementation) -> Graph:
     """
      Apply second moment correction on graph.
      Args:
-        graph_to_apply_second_moment_correction: Graph to apply second moment correction.
+        graph: Graph to apply second moment correction.
         representative_data_gen (Callable): Dataset used for calibration.
         core_config (CoreConfig): Configuration object containing parameters of how the model should be
          quantized, including mixed precision parameters.
         fw_info: FrameworkInfo object with information about the specific framework's model.
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
 
      Returns:
          Graph after second moment correction.
      """
-    graph = copy.deepcopy(graph_to_apply_second_moment_correction)
     semi_quantized_model = quantized_model_builder_for_second_moment_correction(graph, fw_info, fw_impl)
     fw_impl.apply_second_moment_correction(semi_quantized_model, core_config, representative_data_gen, graph)
     graph = substitute(graph, fw_impl.get_substitutions_after_second_moment_correction(core_config.quantization_config))
     _collect_and_assign_act_threshold(graph, representative_data_gen, core_config, fw_info, fw_impl)
 
     return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,43 +14,43 @@
 # ==============================================================================
 
 import copy
 from typing import Any
 
 import numpy as np
 
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.core.common import BaseNode, Logger, Graph
+from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.quantization.quantize_node import get_quantized_kernel_by_weights_qc
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
+from model_compression_toolkit.logger import Logger
 
 
-def compute_bias_correction_of_graph(graph_co_compute_bias: Graph,
+def compute_bias_correction_of_graph(graph: Graph,
                                      core_config: CoreConfig,
                                      fw_info: FrameworkInfo,
                                      fw_impl: FrameworkImplementation) -> Graph:
     """
     For each node in a graph, and for each candidate weights quantization configuration,
     compute the bias-correction term, and store it in the candidate weights quantization configuration.
 
     Args:
-        graph_co_compute_bias: Graph with nodes to compute the bias correction for
+        graph: Graph with nodes to compute the bias correction for
         each node's weights quantization configuration candidates.
         core_config: CoreConfig containing parameters of how the model should be quantized.
         fw_info: Framework info like lists of nodes their kernel should quantized.
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
 
     Returns:
         Graph with bias correction for each weights quantization configuration candidate
         for each node.
     """
 
-    graph = copy.deepcopy(graph_co_compute_bias)
     for n in graph.nodes:
         if n.is_weights_quantization_enabled() and core_config.quantization_config.weights_bias_correction:
             _compute_bias_correction_per_candidate_qc(n,
                                                       fw_info,
                                                       graph.get_in_stats_collector(n),
                                                       fw_impl=fw_impl)
     return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-import copy
-
 from typing import List
 
 from model_compression_toolkit.core import common
 
 
-def substitute(graph_to_substitute: common.Graph,
+def substitute(graph: common.Graph,
                substitutions_list: List[common.BaseSubstitution]) -> common.Graph:
     """
     Apply a list of substitutions on a graph.
     Args:
         graph: Graph to transform.
         substitutions_list: List of substitutions to apply on the graph.
 
     Returns:
         Transformed graph after applying all substitutions in substitutions_list.
     """
 
-    graph = copy.deepcopy(graph_to_substitute)
     for substitution in substitutions_list:
         matched_nodes = graph.filter(substitution.matcher_instance)
         for idn in matched_nodes:
             graph = substitution.substitute(graph, idn)
-    return graph
+    return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 import copy
 from typing import Callable
 
 import numpy as np
 
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 class BatchNormalizationReconstruction(common.BaseSubstitution):
     """
     Reconstruct BatchNormalization after linear layers.
     """
     def __init__(self,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import numpy as np
 from typing import Tuple, Callable
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import EdgeMatcher, NodeOperationMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.core.common.constants import THRESHOLD, RANGE_MIN, RANGE_MAX
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import THRESHOLD, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.logger import Logger
 
 
 class BatchNormalizationRefusing(common.BaseSubstitution):
     """
     Re-fuse BatchNormalization into preceding linear layers.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import copy
 import numpy as np
 from typing import Tuple, Callable
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import EdgeMatcher, NodeOperationMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 class Conv2DCollapsing(common.BaseSubstitution):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-import copy
-
 from model_compression_toolkit.core import common
 
 
 def linear_collapsing_substitute(graph: common.Graph,
                                  linear_collapsing_substitution: common.BaseSubstitution) -> common.Graph:
     """
     Apply a list of linear collapsing substitutions on a graph.
@@ -28,15 +26,14 @@
     the matches are not valid anymore, and we can find new matches.
     Args:
         graph: Graph to transform.
         linear_collapsing_substitution: substitution to apply on the graph.
     Returns:
         Transformed graph after applying all linear collapsing substitutions.
     """
-    graph = copy.deepcopy(graph)
     matched_nodes = graph.filter(linear_collapsing_substitution.matcher_instance)
     matched_nodes_list = []
     match_indicator = True
     while len(matched_nodes) > 0 and match_indicator:
         match_indicator = False
         for matched_node in matched_nodes:
             if matched_node not in matched_nodes_list:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 import numpy as np
 from typing import List, Tuple, Any, Callable
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common import FrameworkInfo, Graph, BaseNode
-from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, SHIFT_NEGATIVE_NON_LINEAR_NUM_BITS
+from model_compression_toolkit.constants import THRESHOLD, SIGNED, SHIFT_NEGATIVE_NON_LINEAR_NUM_BITS
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.core.common.quantization.set_node_quantization_config import create_node_activation_qc, \
     set_quantization_configs_to_node
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_activations_computation \
     import get_activations_qparams
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     _mse_error_histogram
@@ -352,15 +352,15 @@
     if bypass_nodes:
         for bypass_node in bypass_nodes:
             for bypass_candidate_qc in bypass_node.candidates_quantization_cfg:
                 if bypass_candidate_qc.activation_quantization_cfg:
                     bypass_candidate_qc.activation_quantization_cfg.activation_quantization_params[SIGNED] = False
                     graph.shift_stats_collector(bypass_node, np.array(shift_value))
 
-    add_node_qco = graph.tpc.get_qco_by_node(add_node).quantization_config_list
+    add_node_qco = add_node.get_qco(graph.tpc).quantization_config_list
     for op_qc_idx, candidate_qc in enumerate(add_node.candidates_quantization_cfg):
         candidate_qc.weights_quantization_cfg.enable_weights_quantization = False
 
         candidate_qc.activation_quantization_cfg = create_node_activation_qc(core_config.quantization_config,
                                                                              fw_info,
                                                                              add_node_qco[op_qc_idx])
 
@@ -491,15 +491,15 @@
     Returns:
         Graph after applying shift negative on selected activations.
     """
 
     nodes = list(graph.nodes())
     for n in nodes:
         # Skip substitution if QuantizationMethod is uniform.
-        node_qco = graph.tpc.get_qco_by_node(n)
+        node_qco = n.get_qco(graph.tpc)
         if any([op_qc.activation_quantization_method is QuantizationMethod.UNIFORM
                 for op_qc in node_qco.quantization_config_list]):
             continue
 
         if snc_node_types.apply(n):
             linear_node, pad_node, bypass_nodes = get_next_nodes_to_correct(n,
                                                                             graph,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from model_compression_toolkit.core.common import BaseNode, Graph, BaseSubstitution
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.virtual_activation_weights_node import VirtualActivationWeightsNode
 
 
 class BaseVirtualActivationWeightsComposition(BaseSubstitution):
     def __init__(self, matcher_instance):
         super().__init__(matcher_instance=matcher_instance)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import itertools
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common import BaseNode, Graph, BaseSubstitution
 from model_compression_toolkit.core.common.graph.virtual_activation_weights_node import VirtualSplitWeightsNode, \
     VirtualSplitActivationNode
 from model_compression_toolkit.core.common.matchers.base_matcher import BaseMatcher
 
 
 class BaseWeightsActivationSplit(BaseSubstitution):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/current_tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 def get_current_tp_model():
     """
 
     Returns: The current TargetPlatformModel that is being used and accessed.
 
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/fusing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from typing import Any
 
-from model_compression_toolkit.core.common.target_platform.operators import OperatorSetConcat
-from model_compression_toolkit.core.common.target_platform.target_platform_model_component import TargetPlatformModelComponent
+from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorSetConcat
+from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model_component import TargetPlatformModelComponent
 
 
 class Fusing(TargetPlatformModelComponent):
 
     def __init__(self, operator_groups_list, name=None):
         assert isinstance(operator_groups_list,
                           list), f'List of operator groups should be of type list but is {type(operator_groups_list)}'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/op_quantization_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/operators.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any
 
-from model_compression_toolkit.core.common.constants import OPS_SET_LIST
-from model_compression_toolkit.core.common.target_platform.target_platform_model_component import TargetPlatformModelComponent
-from model_compression_toolkit.core.common.target_platform.current_tp_model import _current_tp_model
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import QuantizationConfigOptions
+from model_compression_toolkit.target_platform_capabilities.constants import OPS_SET_LIST
+from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model_component import TargetPlatformModelComponent
+from model_compression_toolkit.target_platform_capabilities.target_platform.current_tp_model import _current_tp_model
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import QuantizationConfigOptions
 
 
 class OperatorsSetBase(TargetPlatformModelComponent):
     """
     Base class to represent a set of operators.
     """
     def __init__(self, name: str):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import pprint
 from typing import Any, Dict
 
-from model_compression_toolkit.core.common.target_platform.current_tp_model import _current_tp_model, \
+from model_compression_toolkit.target_platform_capabilities.target_platform.current_tp_model import _current_tp_model, \
     get_current_tp_model
-from model_compression_toolkit.core.common.target_platform.fusing import Fusing
-from model_compression_toolkit.core.common.target_platform.target_platform_model_component import \
+from model_compression_toolkit.target_platform_capabilities.target_platform.fusing import Fusing
+from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model_component import \
     TargetPlatformModelComponent
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import OpQuantizationConfig, \
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
     QuantizationConfigOptions
-from model_compression_toolkit.core.common.target_platform.operators import OperatorsSetBase
-from model_compression_toolkit.core.common.immutable import ImmutableClass
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorsSetBase
+from model_compression_toolkit.target_platform_capabilities.immutable import ImmutableClass
+from model_compression_toolkit.logger import Logger
 
 
 def get_default_quantization_config_options() -> QuantizationConfigOptions:
     """
 
     Returns: The default QuantizationConfigOptions of the model. This is the options
     to use when a layer's options is queried and it wasn't specified in the TargetPlatformCapabilities.
@@ -219,7 +219,16 @@
     def show(self):
         """
 
         Display the TargetPlatformModel.
 
         """
         pprint.pprint(self.get_info(), sort_dicts=False)
+
+    def set_quantization_format(self,
+                                quantization_format: Any):
+        """
+        Set quantization format.
+        Args:
+            quantization_format: A quantization format (fake-quant, int8 etc.) from enum QuantizationFormat.
+        """
+        self.quantization_format = quantization_format
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any, Dict
 
-from model_compression_toolkit.core.common.target_platform.current_tp_model import _current_tp_model
+from model_compression_toolkit.target_platform_capabilities.target_platform.current_tp_model import _current_tp_model
 
 
 class TargetPlatformModelComponent:
     """
     Component of TargetPlatformModel (Fusing, OperatorsSet, etc.)
     """
     def __init__(self, name: str):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.current_tpc import get_current_tpc
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.target_platform_capabilities import TargetPlatformCapabilities
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.attribute_filter import \
-    Eq, GreaterEq, NotEq, SmallerEq, Greater, Smaller
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.layer_filter_params import \
-    LayerFilterParams
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.operations_to_layers import \
-    OperationsToLayers, OperationsSetToLayers
-
-
+from model_compression_toolkit.target_platform_capabilities.target_platform.fusing import Fusing
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import \
+    TargetPlatformCapabilities, OperationsSetToLayers, Smaller, SmallerEq, NotEq, Eq, GreaterEq, Greater, LayerFilterParams, OperationsToLayers, get_current_tpc
+
+from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model import \
+    get_default_quantization_config_options, TargetPlatformModel
+
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
+    QuantizationConfigOptions, QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorsSet, OperatorSetConcat
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import operator
 from typing import Any, Callable, Dict
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 class Filter:
     """
     Filter a layer configuration by its attributes.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import Any, Dict
-
-from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.attribute_filter import AttributeFilter
+from typing import Any
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.attribute_filter import AttributeFilter
 
 
 class LayerFilterParams:
     """
     Wrap a layer with filters to filter framework's layers by their attributes.
     """
 
@@ -83,38 +81,38 @@
         conditions and keyword arguments. Used for display and hashing.
 
         """
         params = [f'{k}={v}' for k,v in self.kwargs.items()]
         params.extend([str(c) for c in self.conditions])
         params_str = ', '.join(params)
         return f'{self.layer.__name__}({params_str})'
-
-    def match(self,
-              node: BaseNode) -> bool:
-        """
-        Check if a node matches the layer, conditions and keyword-arguments of
-        the LayerFilterParams.
-
-        Args:
-            node: Node to check if matches to the LayerFilterParams properties.
-
-        Returns:
-            Whether the node matches to the LayerFilterParams properties.
-        """
-        # Check the node has the same type as the layer in LayerFilterParams
-        if self.layer != node.type:
-            return False
-
-        # Get attributes from node to filter
-        layer_config = node.framework_attr
-        if hasattr(node, "op_call_kwargs"):
-            layer_config.update(node.op_call_kwargs)
-
-        for attr, value in self.kwargs.items():
-            if layer_config.get(attr) != value:
-                return False
-
-        for c in self.conditions:
-            if not c.match(layer_config):
-                return False
-
-        return True
+    #
+    # def match(self,
+    #           node: BaseNode) -> bool:
+    #     """
+    #     Check if a node matches the layer, conditions and keyword-arguments of
+    #     the LayerFilterParams.
+    #
+    #     Args:
+    #         node: Node to check if matches to the LayerFilterParams properties.
+    #
+    #     Returns:
+    #         Whether the node matches to the LayerFilterParams properties.
+    #     """
+    #     # Check the node has the same type as the layer in LayerFilterParams
+    #     if self.layer != node.type:
+    #         return False
+    #
+    #     # Get attributes from node to filter
+    #     layer_config = node.framework_attr
+    #     if hasattr(node, "op_call_kwargs"):
+    #         layer_config.update(node.op_call_kwargs)
+    #
+    #     for attr, value in self.kwargs.items():
+    #         if layer_config.get(attr) != value:
+    #             return False
+    #
+    #     for c in self.conditions:
+    #         if not c.match(layer_config):
+    #             return False
+    #
+    #     return True
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import List, Any
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.current_tpc import  _current_tpc
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.target_platform_capabilities_component import TargetPlatformCapabilitiesComponent
-from model_compression_toolkit.core.common.target_platform.operators import OperatorsSet, OperatorSetConcat, \
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.current_tpc import  _current_tpc
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.target_platform_capabilities_component import TargetPlatformCapabilitiesComponent
+from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorSetConcat, \
     OperatorsSetBase
 
 
 
 class OperationsSetToLayers(TargetPlatformCapabilitiesComponent):
     """
     Associate an OperatorsSet to a list of framework's layers.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 # ==============================================================================
 
 
 import itertools
 import pprint
 from typing import List, Any, Dict, Tuple
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.operations_to_layers import \
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.operations_to_layers import \
     OperationsToLayers, OperationsSetToLayers
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.target_platform_capabilities_component import TargetPlatformCapabilitiesComponent
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.layer_filter_params import LayerFilterParams
-from model_compression_toolkit.core.common.immutable import ImmutableClass
-from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import QuantizationConfigOptions, \
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.target_platform_capabilities_component import TargetPlatformCapabilitiesComponent
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.layer_filter_params import LayerFilterParams
+from model_compression_toolkit.target_platform_capabilities.immutable import ImmutableClass
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import QuantizationConfigOptions, \
     OpQuantizationConfig
-from model_compression_toolkit.core.common.target_platform.operators import OperatorsSet, OperatorsSetBase
-from model_compression_toolkit.core.common.target_platform.target_platform_model import TargetPlatformModel
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.current_tpc import _current_tpc
+from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorsSetBase
+from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model import TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.current_tpc import _current_tpc
 
 
 class TargetPlatformCapabilities(ImmutableClass):
     """
     Attach framework information to a modeled hardware.
     """
     def __init__(self,
@@ -159,34 +158,14 @@
 
         Returns: The default OpQuantizationConfig of the TargetPlatformModel that is attached
         to the TargetPlatformCapabilities.
 
         """
         return self.tp_model.get_default_op_quantization_config()
 
-    def get_qco_by_node(self,
-                        node: BaseNode) -> QuantizationConfigOptions:
-        """
-        Get the QuantizationConfigOptions of a node in a graph according
-        to the mappings from layers/LayerFilterParams to the OperatorsSet in the TargetPlatformModel.
-
-        Args:
-            node: Node from graph to get its QuantizationConfigOptions.
-
-        Returns:
-            QuantizationConfigOptions of the node.
-        """
-        if node is None:
-            Logger.error(f'Can not retrieve QC options for None node')  # pragma: no cover
-        for fl, qco in self.filterlayer2qco.items():
-            if fl.match(node):
-                return qco
-        if node.type in self.layer2qco:
-            return self.layer2qco.get(node.type)
-        return self.tp_model.default_qco
 
     def _get_config_options_mapping(self) -> Tuple[Dict[Any, QuantizationConfigOptions],
                                                    Dict[LayerFilterParams, QuantizationConfigOptions]]:
         """
         Build mapping from layers to their QuantizationConfigOptions (and from LayerFilterParams
         to their QuantizationConfigOptions).
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from enum import Enum
 
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.current_tpc import  _current_tpc
 
-
-class TargetPlatformCapabilitiesComponent:
-    def __init__(self, name: str):
-        self.name = name
-        _current_tpc.get().append_component(self)
-
-    def get_info(self):
-        return {}
+class QuantizationFormat(Enum):
+    FAKELY_QUANT = 0
+    INT8 = 1
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from tensorboard.compat.proto.step_stats_pb2 import StepStats, NodeExecStats, DeviceStepStats, AllocatorMemoryUsed
 from tensorboard.compat.proto.summary_pb2 import HistogramProto
 from tensorboard.compat.proto.summary_pb2 import Summary
 from tensorboard.compat.proto.tensor_shape_pb2 import TensorShapeProto
 from tensorboard.summary.writer.event_file_writer import EventFileWriter
 from typing import List, Any, Dict
 from networkx import topological_sort
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 
 DEVICE_STEP_STATS = "/device:CPU:0"
 
 
 def get_node_properties(node_dict_to_log: dict,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.keras.back2framework.float_model_builder import FloatKerasModelBuilder
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 from model_compression_toolkit.core.keras.back2framework.mixed_precision_model_builder import \
     MixedPrecisionKerasModelBuilder
 from model_compression_toolkit.core.keras.back2framework.quantized_model_builder import QuantizedKerasModelBuilder
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core import common
 from tensorflow.python.util.object_identity import Reference as TFReference
 
 class FloatKerasModelBuilder(KerasModelBuilder):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from abc import abstractmethod
-
 import tensorflow as tf
 from keras.engine.input_layer import InputLayer
 from keras.models import Model, clone_model
 from packaging import version
 
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.common.constants import INPUT_BASE_NAME
+from model_compression_toolkit.constants import INPUT_BASE_NAME
 
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Input
     from tensorflow.python.keras.layers.core import TFOpLambda
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
     from tensorflow.python.keras.layers import Layer
@@ -34,15 +32,14 @@
     from keras import Input
     from keras.layers.core import TFOpLambda
     from keras.engine.base_layer import TensorFlowOpLayer, Layer
 
 from typing import Any, Dict, List, Tuple, Callable
 from tensorflow.python.util.object_identity import Reference as TFReference
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
-from model_compression_toolkit.core.common.logger import Logger
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.keras.back2framework.instance_builder import OperationHandler
 from model_compression_toolkit.core.keras.reader.connectivity_handler import OutTensor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.layers.core import TFOpLambda, SlicingOpLambda  # pragma: no cover
 else:
     from keras.layers.core import TFOpLambda, SlicingOpLambda
 
 from tensorflow_model_optimization.python.core.quantization.keras.quantize_wrapper import QuantizeWrapper
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core.keras.quantizer.mixed_precision.quantization_config_factory import \
     quantization_config_builder_mixed_precision
 from tensorflow.python.util.object_identity import Reference as TFReference
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.layers import Layer  # pragma: no cover
 else:
     from keras.engine.base_layer import Layer
 
 from typing import Any, Dict, List, Tuple
 from tensorflow.python.util.object_identity import Reference as TFReference
-from model_compression_toolkit.core.common.constants import EPS, MIN_JACOBIANS_ITER, JACOBIANS_COMP_TOLERANCE
+from model_compression_toolkit.constants import EPS, MIN_JACOBIANS_ITER, JACOBIANS_COMP_TOLERANCE
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.keras.back2framework.instance_builder import OperationHandler
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def build_input_tensors_list(node: BaseNode,
                              graph: Graph,
                              node_to_output_tensors_dict: Dict[BaseNode, List[TFReference]]) -> List[List[TFReference]]:
     """
     Given a node, build a list of input tensors the node gets. The list is built
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from tensorflow.python.util.object_identity import Reference as TFReference
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,17 +95,10 @@
 V_BIAS = '/value/bias'
 OUTPUT_KERNEL = '/attention_output/kernel'
 OUTPUT_BIAS = '/attention_output/bias'
 
 # ReLU bound constants
 RELU_POT_BOUND = 8.0
 
-# Supported TP models names for Tensorflow:
-DEFAULT_TP_MODEL = 'default'
-IMX500_TP_MODEL = 'imx500'
-TFLITE_TP_MODEL = 'tflite'
-QNNPACK_TP_MODEL = 'qnnpack'
-
-
 # TFOpLambda functions:
 ADD = 'add'
 PAD = 'pad'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
 
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
-from model_compression_toolkit.core.common.framework_info import FrameworkInfo, ChannelAxis
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.core.common.constants import SOFTMAX_THRESHOLD
+from model_compression_toolkit.core.common.framework_info import FrameworkInfo
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import SOFTMAX_THRESHOLD
 from model_compression_toolkit.core.keras.constants import SOFTMAX, LINEAR, RELU, SWISH, SIGMOID, IDENTITY, TANH, SELU, \
     KERNEL, DEPTHWISE_KERNEL
 from model_compression_toolkit.core.keras.quantizer.fake_quant_builder import power_of_two_quantization, symmetric_quantization, uniform_quantization
 
 """
 Map each layer to a list of its' weights attributes that should get quantized.
 If a layer that is not listed here is queried, [None] is returned.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 
 from tensorflow.keras.layers import Dense, DepthwiseConv2D, Conv2D, Conv2DTranspose, Activation, SeparableConv2D
 
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common.constants import FLOAT_32, DATA_TYPE
+from model_compression_toolkit.constants import FLOAT_32, DATA_TYPE
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, \
     NodeFrameworkAttrMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.keras.constants import LINEAR, ACTIVATION, TRAINABLE, LAYER_NAME
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, EdgeMatcher, WalkMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
-from model_compression_toolkit.core.common.constants import THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD
 from model_compression_toolkit.core.keras.constants import KERNEL
 
 input_node = NodeOperationMatcher(InputLayer)
 zeropad_node = NodeOperationMatcher(ZeroPadding2D)
 op2d_node = NodeOperationMatcher(Dense) | \
             NodeOperationMatcher(Conv2D) | \
             NodeOperationMatcher(DepthwiseConv2D) | \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import tensorflow as tf
 from tensorflow.keras.layers import Conv2D
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, NodeFrameworkAttrMatcher
 from model_compression_toolkit.core.common.substitutions.linear_collapsing import Conv2DCollapsing
 from model_compression_toolkit.core.keras.constants import KERNEL, KERNEL_SIZE, STRIDES, DILATIONS, LINEAR, \
     ACTIVATION, BIAS, USE_BIAS, LAYER_NAME, FILTERS, PADDING, GROUPS, DATA_FORMAT
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def linear_collapsing_node_matchers() -> Tuple[NodeOperationMatcher, NodeOperationMatcher]:
     """
     Function generates matchers for matching:
     (Conv2D, Conv2D)[activation=linear] -> Conv2D.
     Returns:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.layers.core import TFOpLambda
     from tensorflow.keras.layers import MultiHeadAttention, Conv2D, Softmax, Concatenate, Reshape, Permute
 else:
     from keras.layers.core import TFOpLambda
     from keras.layers import MultiHeadAttention, Conv2D, Softmax, Concatenate, Reshape, Permute
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph, BaseNode, OutTensor
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
-from model_compression_toolkit.core.common.constants import REUSE, REUSE_GROUP
-from model_compression_toolkit.core.keras.reader.node_builder import REUSED_IDENTIFIER
+from model_compression_toolkit.constants import REUSE, REUSE_GROUP
 from model_compression_toolkit.core.keras.constants import KERNEL, BIAS, USE_BIAS, NUM_HEADS, KEY_DIM, VALUE_DIM, \
     QUERY_SHAPE, KEY_SHAPE, VALUE_SHAPE, OUTPUT_SHAPE, ATTENTION_AXES, ACTIVATION, LINEAR, FILTERS, \
     FUNCTION, DIMS, TARGET_SHAPE, F_STRIDED_SLICE, F_STACK, Q_KERNEL, Q_BIAS, K_KERNEL, K_BIAS, V_KERNEL, V_BIAS, \
-    OUTPUT_KERNEL, OUTPUT_BIAS, F_MATMUL, TRANSPOSE_B, KERNEL_SIZE, AXIS, F_STRIDED_SLICE_BEGIN, F_STRIDED_SLICE_END
+    OUTPUT_KERNEL, OUTPUT_BIAS, F_MATMUL, KERNEL_SIZE, AXIS, F_STRIDED_SLICE_BEGIN, F_STRIDED_SLICE_END
 
 
 class MHAParams:
     """
     A data class to hold all relevant parameters from the MHA node framework attributes
     """
     def __init__(self, mha_node):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numpy as np
 from tensorflow.keras.layers import ReLU, DepthwiseConv2D, Conv2DTranspose, Conv2D, Dense
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, WalkMatcher
 from model_compression_toolkit.core.keras.constants import KERNEL, BIAS, RELU_MAX_VALUE, RELU_POT_BOUND
+from model_compression_toolkit.logger import Logger
 
 
 class ReLUBoundToPowerOfTwo(common.BaseSubstitution):
     """
     Substitution to scale the weights of two linear nodes, and move the bound of non-linear between them
     (if bounded) in order to use the entire constrained range when activations are quantized.
     """
@@ -77,15 +78,15 @@
         # only act on bound relu with non POT max value
         if max_value is None or np.log2(max_value).astype(int) - np.log2(max_value) == 0:
             return graph
 
         scale_factor = max_value / self.threshold
 
         non_linear_node.framework_attr[RELU_MAX_VALUE] = np.float32(self.threshold)
-        common.Logger.debug(
+        Logger.debug(
             f"Node named:{non_linear_node.name} max value change "
             f"to:{non_linear_node.framework_attr[RELU_MAX_VALUE]}")
 
         w2_fixed = scale_factor * second_op2d_node.get_weights_by_keys(KERNEL)
         w1_fixed = first_op2d_node.get_weights_by_keys(KERNEL) / scale_factor
         b1_fixed = first_op2d_node.get_weights_by_keys(BIAS) / scale_factor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 from tensorflow.keras.layers import ReLU
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher,NodeFrameworkAttrMatcher
 from model_compression_toolkit.core.keras.constants import RELU_MAX_VALUE
-from model_compression_toolkit.core.common.constants import THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD
+from model_compression_toolkit.logger import Logger
 
 MATCHER = NodeOperationMatcher(ReLU) & NodeFrameworkAttrMatcher(RELU_MAX_VALUE, None).logic_not()
 
 
 class RemoveReLUUpperBound(common.BaseSubstitution):
     """
     Remove ReLU upper bound if its activation threshold bounds it anyway at
@@ -52,9 +53,9 @@
         Returns:
             Graph after applying the substitution.
         """
         if node.final_activation_quantization_cfg and \
                 node.final_activation_quantization_cfg.activation_quantization_params.get(THRESHOLD) == \
                 node.framework_attr.get(RELU_MAX_VALUE):
             node.framework_attr[RELU_MAX_VALUE] = None
-            common.Logger.info(f'Removing upper bound of {node.name}. Threshold and upper bound are equal.')
+            Logger.info(f'Removing upper bound of {node.name}. Threshold and upper bound are equal.')
         return graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import tensorflow as tf
 from tensorflow.keras.layers import Conv2D, Add
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, \
     NodeFrameworkAttrMatcher
 from model_compression_toolkit.core.common.substitutions.residual_collapsing import ResidualCollapsing
 from model_compression_toolkit.core.keras.constants import KERNEL, LINEAR, ACTIVATION, LAYER_NAME
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def residual_collapsing_node_matchers() -> Tuple[NodeOperationMatcher, NodeOperationMatcher]:
     """
     Function generates matchers for matching:
     (Conv2D, Add)[activation=linear] -> Conv2D.
     Returns:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 import tensorflow as tf
 
 from tensorflow.python.keras.layers.core import TFOpLambda
 from tensorflow.keras.layers import Activation, Conv2D, Dense, DepthwiseConv2D, ZeroPadding2D, Reshape, \
     GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU
 
-from model_compression_toolkit import CoreConfig, FrameworkInfo
+from model_compression_toolkit.core import CoreConfig, FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, \
     NodeFrameworkAttrMatcher
 from model_compression_toolkit.core.common.substitutions.shift_negative_activation import \
     apply_shift_negative_correction
 from model_compression_toolkit.core.keras.constants import KERNEL_SIZE, STRIDES, ACTIVATION, SWISH, \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import List, Any, Tuple, Callable, Type, Dict
+from typing import List, Any, Tuple, Callable, Dict
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras.models import Model
 from tensorflow.python.layers.base import Layer
 
 from model_compression_toolkit.core.common.mixed_precision.sensitivity_evaluation import SensitivityEvaluation
@@ -39,25 +39,23 @@
     from tensorflow.keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add
     from tensorflow.python.keras.layers.core import TFOpLambda
 else:
     from keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, \
         Concatenate, Add
     from keras.layers.core import TFOpLambda
 
-from model_compression_toolkit import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
-from model_compression_toolkit.gptq.common.gptq_training import GPTQTrainer
-from model_compression_toolkit.gptq.keras.gptq_training import KerasGPTQTrainer
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.activation_decomposition import \
     ActivationDecomposition
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.softmax_shift import \
     keras_softmax_shift
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_folding import \
     keras_batchnorm_folding
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_refusing import \
@@ -344,20 +342,14 @@
             A list of the framework substitutions used after we apply second moment statistics.
         """
         substitutions_list = []
         if quant_config.weights_second_moment_correction:
             substitutions_list.append(keras_batchnorm_refusing())
         return substitutions_list
 
-    def get_gptq_trainer_obj(self) -> Type[GPTQTrainer]:
-        """
-        Returns:  Keras object of GPTQTrainer
-        """
-        return KerasGPTQTrainer
-
     def get_sensitivity_evaluator(self,
                                   graph: Graph,
                                   quant_config: MixedPrecisionQuantizationConfigV2,
                                   representative_data_gen: Callable,
                                   fw_info: FrameworkInfo,
                                   disable_activation_for_metric: bool = False) -> SensitivityEvaluation:
         """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tensorflow.keras.models import Model
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common.framework_info import ChannelAxis
 from model_compression_toolkit.core.common.model_validation import ModelValidation
 from model_compression_toolkit.core.keras.constants import CHANNELS_FORMAT, CHANNELS_FORMAT_LAST, CHANNELS_FORMAT_FIRST
 
 
 class KerasModelValidation(ModelValidation):
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from packaging import version
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Activation, ReLU, BatchNormalization
 else:
     from keras.layers import Activation, ReLU, BatchNormalization
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.keras.constants import ACTIVATION, RELU_MAX_VALUE, NEGATIVE_SLOPE, THRESHOLD, \
     GAMMA, BETA, MOVING_MEAN, MOVING_VARIANCE
 from model_compression_toolkit.core.common.graph.base_graph import Graph
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable
 
-from model_compression_toolkit import MixedPrecisionQuantizationConfig, CoreConfig, MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import MixedPrecisionQuantizationConfig, CoreConfig, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import TENSORFLOW
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import TENSORFLOW
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_data import compute_kpi_data
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     DEFAULT_MIXEDPRECISION_CONFIG
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.constants import FOUND_TF
 
 if FOUND_TF:
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from tensorflow.keras.models import Model
 
     from model_compression_toolkit import get_target_platform_capabilities
 
     KERAS_DEFAULT_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
@@ -47,15 +47,15 @@
         Builds the computation graph from the given model and target platform modeling, and uses it to compute the KPI data.
 
         Args:
             in_model (Model): Keras model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             quant_config (MixedPrecisionQuantizationConfig): MixedPrecisionQuantizationConfig containing parameters of how the model should be quantized.
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default Keras info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/keras/default_framework_info.py>`_
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to. `Default Keras TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/keras_tp_models/keras_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
 
         Returns:
             A KPI object with total weights parameters sum, max activation tensor and total kpi.
 
         Examples:
 
             Import a Keras model:
@@ -71,15 +71,15 @@
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 224, 224, 3))]
 
             Import MCT and call for KPI data calculation:
 
             >>> import model_compression_toolkit as mct
-            >>> kpi_data = mct.keras_kpi_data(model, repr_datagen)
+            >>> kpi_data = mct.core.keras_kpi_data(model, repr_datagen)
 
 
         """
 
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
             Logger.error("KPI data computation can't be executed without MixedPrecisionQuantizationConfig object."
                          "Given quant_config is not of type MixedPrecisionQuantizationConfig.")
@@ -108,15 +108,15 @@
         Builds the computation graph from the given model and hw modeling, and uses it to compute the KPI data.
 
         Args:
             in_model (Model): Keras model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             core_config (CoreConfig): CoreConfig containing parameters for quantization and mixed precision of how the model should be quantized.
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default Keras info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/keras/default_framework_info.py>`_
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to. `Default Keras TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/keras_tp_models/keras_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
 
         Returns:
 
             A KPI object with total weights parameters sum and max activation tensor.
 
         Examples:
 
@@ -129,15 +129,15 @@
 
             >>> import numpy as np
             >>> def repr_datagen(): yield [np.random.random((1, 224, 224, 3))]
 
             Import MCT and call for KPI data calculation:
 
             >>> import model_compression_toolkit as mct
-            >>> kpi_data = mct.keras_kpi_data(model, repr_datagen)
+            >>> kpi_data = mct.core.keras_kpi_data(model, repr_datagen)
 
         """
 
         if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
             Logger.error("KPI data computation can't be executed without MixedPrecisionQuantizationConfigV2 object."
                          "Given quant_config is not of type MixedPrecisionQuantizationConfigV2.")
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable, List, Tuple
 
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import TENSORFLOW
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import TENSORFLOW
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.gptq import GradientPTQConfig, GradientPTQConfigV2
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.network_editors.actions import EditRule
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig, DEFAULT_MIXEDPRECISION_CONFIG
@@ -31,23 +30,23 @@
 from model_compression_toolkit.core.common.quantization.quantization_config import DEFAULTCONFIG
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.gptq.runner import gptq_runner
 from model_compression_toolkit.ptq.runner import ptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
 
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.constants import FOUND_TF
 
 if FOUND_TF:
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from tensorflow.keras.models import Model
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
 
     from model_compression_toolkit import get_target_platform_capabilities
 
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
 
     def keras_post_training_quantization(in_model: Model,
@@ -77,15 +76,15 @@
             representative_data_gen (Callable): Dataset used for calibration.
             n_iter (int): Number of calibration iterations to run.
             quant_config (QuantizationConfig): QuantizationConfig containing parameters of how the model should be quantized. `Default configuration. <https://github.com/sony/model_optimization/blob/21e21c95ca25a31874a5be7af9dd2dd5da8f3a10/model_compression_toolkit/core/common/quantization/quantization_config.py#L154>`_
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default Keras info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/keras/default_framework_info.py>`_
             network_editor (List[EditRule]): List of EditRules. Each EditRule consists of a node filter and an action to change quantization settings of the filtered nodes.
             gptq_config (GradientPTQConfig): Configuration for using gptq (e.g. optimizer).
             analyze_similarity (bool): Whether to plot similarity figures within TensorBoard (when logger is enabled) or not.
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to. `Default Keras TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/keras_tp_models/keras_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
 
         Returns:
             A quantized model and information the user may need to handle the quantized model.
 
         Examples:
 
             Import a Keras model:
@@ -180,15 +179,15 @@
              target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
              n_iter (int): Number of calibration iterations to run.
              quant_config (MixedPrecisionQuantizationConfig): QuantizationConfig containing parameters of how the model should be quantized.
              fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default Keras info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/keras/default_framework_info.py>`_
              network_editor (List[EditRule]): List of EditRules. Each EditRule consists of a node filter and an action to change quantization settings of the filtered nodes.
              gptq_config (GradientPTQConfig): Configuration for using GPTQ (e.g. optimizer).
              analyze_similarity (bool): Whether to plot similarity figures within TensorBoard (when logger is enabled) or not.
-             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to. `Default Keras TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/keras_tp_models/keras_default.py>`_
+             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
 
 
          Returns:
              A quantized model and information the user may need to handle the quantized model.
 
          Examples:
 
@@ -205,39 +204,39 @@
 
              >>> import numpy as np
              >>> def repr_datagen(): return [np.random.random((1,224,224,3))]
 
              Create a mixed-precision configuration, to quantize a model with different bitwidths for different layers.
              The candidates bitwidth for quantization should be defined in the target platform model:
 
-             >>> config = mct.MixedPrecisionQuantizationConfig()
+             >>> config = mct.core.MixedPrecisionQuantizationConfig()
 
              Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
              that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
              while the bias will not):
 
-             >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+             >>> kpi = mct.core.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model:
 
              >>> quantized_model, quantization_info = mct.keras_post_training_quantization_mixed_precision(model,repr_datagen, target_kpi=kpi, n_iter=10, quant_config=config)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/experimental_api_docs/modules/mixed_precision_quantization_config.html#model_compression_toolkit.MixedPrecisionQuantizationConfigV2>`_.
 
          """
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
-            common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+            Logger.error("Given quantization config to mixed-precision facade is not of type "
                                 "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization API,"
                                 "or pass a valid mixed precision configuration.")
 
-        common.Logger.info("Using experimental mixed-precision quantization. "
+        Logger.info("Using experimental mixed-precision quantization. "
                            "If you encounter an issue please file a bug.")
 
         quantization_config, mp_config = quant_config.separate_configs()
         core_config = CoreConfig(quantization_config=quantization_config,
                                  mixed_precision_config=mp_config,
                                  debug_config=DebugConfig(analyze_similarity=analyze_similarity,
                                                           network_editor=network_editor)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 from typing import Tuple, Callable
 
 import tensorflow as tf
 import numpy as np
 from tensorflow.python.util.object_identity import Reference as TFReference
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 
 
 def quantizer_min_max_calculator(threshold: np.ndarray,
                                  num_bits: int,
                                  signed: bool) -> Tuple[float, float]:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from tensorflow_model_optimization.python.core.quantization.keras.default_8bit.default_8bit_transforms import \
     InputLayerQuantize
 from tensorflow_model_optimization.python.core.quantization.keras.graph_transformations import transforms
 from tensorflow_model_optimization.python.core.quantization.keras.quantize_config import QuantizeConfig
 
 
 from model_compression_toolkit.core.common import BaseNode
-from model_compression_toolkit.core.common.constants import INPUT_BASE_NAME
+from model_compression_toolkit.constants import INPUT_BASE_NAME
 
 
 class InputLayerWrapperTransform(InputLayerQuantize):
     """
     Allows to configure an input layer with QuantizeWrapper given a QuantizeConfig object to wrap it.
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Tuple, Dict, Any, Callable
+from typing import Tuple, Dict, Callable
 
 import numpy as np
 import tensorflow as tf
 from keras.layers import Layer
 from tensorflow.python.util.object_identity import Reference as TFReference
 
-from model_compression_toolkit.core.common.constants import SIGNED, CLUSTER_CENTERS, EPS, \
+from model_compression_toolkit.constants import SIGNED, CLUSTER_CENTERS, EPS, \
     MULTIPLIER_N_BITS, THRESHOLD
 
 
 def activation_lut_kmean_quantizer(activation_n_bits: int,
                                    quantization_params: Dict[str, np.ndarray]) -> Callable:
     """
     Builds a LUT quantizer for layer's activation using the provided params (threshold and clusters).
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import tensorflow as tf
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 from model_compression_toolkit.core.keras.quantizer.mixed_precision.selective_activation_quantizer import \
     SelectiveActivationQuantizer
 from packaging import version
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.layers import Layer  # pragma: no cover
 else:
     from keras.engine.base_layer import Layer
 from tensorflow.python.training.tracking.data_structures import ListWrapper
 from tensorflow_model_optimization.python.core.quantization.keras.quantize_config import QuantizeConfig
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     from tensorflow.python.keras.engine.sequential import Sequential
 else:
     from keras.engine.input_layer import InputLayer
     from keras.engine.node import Node as KerasNode
     from keras.engine.functional import Functional
     from keras.engine.sequential import Sequential
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 def is_node_an_input_layer(node: BaseNode) -> bool:
     """
     Checks if a node represents a Keras input layer.
     Args:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import copy
 from typing import Any, Callable
 
 from tensorflow.keras.layers import BatchNormalization
 from tqdm import tqdm
 
 import model_compression_toolkit.core.keras.constants as keras_constants
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core import common
 
 
 def keras_apply_second_moment_correction(quantized_model: Any,
                                          core_config: CoreConfig,
                                          representative_data_gen: Callable,
                                          graph: common.Graph):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.pytorch.back2framework.float_model_builder import FloatPyTorchModelBuilder
 from model_compression_toolkit.core.pytorch.back2framework.mixed_precision_model_builder import \
     MixedPrecisionPyTorchModelBuilder
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
 from model_compression_toolkit.core.pytorch.back2framework.quantized_model_builder import QuantizedPyTorchModelBuilder
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 from typing import List, Tuple
 
 import torch
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder, \
     PytorchModel
 
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 from typing import List, Any, Tuple
 
 import torch
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder, \
     PytorchModel
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 import torch.autograd as autograd
 from networkx import topological_sort
 from tqdm import tqdm
 import numpy as np
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
-from model_compression_toolkit.core.common.constants import EPS, MIN_JACOBIANS_ITER, JACOBIANS_COMP_TOLERANCE
+from model_compression_toolkit.constants import EPS, MIN_JACOBIANS_ITER, JACOBIANS_COMP_TOLERANCE
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
 from model_compression_toolkit.core.pytorch.constants import BUFFER
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder, BufferHolder
 from model_compression_toolkit.core.pytorch.utils import torch_tensor_to_numpy, get_working_device
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def build_input_tensors_list(node: BaseNode,
                              graph: Graph,
                              inputs: Dict[BaseNode, List],
                              node_to_output_tensors_dict: Dict[BaseNode, List]) -> List[List]:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 from abc import abstractmethod
 from typing import Tuple, Any, Dict, List, Union, Callable
 
 import torch
 from networkx import topological_sort
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder, identity_wrapper
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 from typing import List, Tuple
 
 import torch
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder, \
     PytorchModel
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,20 +65,14 @@
 # torch devices
 CUDA = 'cuda'
 CPU = 'cpu'
 
 # ReLU bound constants
 RELU_POT_BOUND = 8.0
 
-# Supported TP models names for Pytorch:
-DEFAULT_TP_MODEL = 'default'
-IMX500_TP_MODEL = 'imx500'
-TFLITE_TP_MODEL = 'tflite'
-QNNPACK_TP_MODEL = 'qnnpack'
-
 # MultiHeadAttention layer attributes:
 EMBED_DIM = 'embed_dim'
 NUM_HEADS = 'num_heads'
 DROPOUT = 'dropout'
 ADD_ZERO_ATTN = 'add_zero_attn'
 KEY_DIM = "kdim"
 VALUE_DIM = 'vdim'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from torch.nn import Hardsigmoid, ReLU, ReLU6, Softmax, Sigmoid
 from torch.nn.functional import hardsigmoid, relu, relu6, softmax
 from torch.nn import Conv2d, ConvTranspose2d, Linear
 from torch import sigmoid
 
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo, ChannelAxis
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.core.common.constants import SOFTMAX_THRESHOLD
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import SOFTMAX_THRESHOLD
 from model_compression_toolkit.core.pytorch.constants import KERNEL
 from model_compression_toolkit.core.pytorch.quantizer.fake_quant_builder import power_of_two_quantization, \
     symmetric_quantization, uniform_quantization
 from model_compression_toolkit.core.pytorch.quantizer.lut_fake_quant import activation_lut_kmean_quantizer
 
 """
 Map each layer to a list of its' weights attributes that should get quantized.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from torch.nn import Conv2d
 import torch.nn.functional as F
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.substitutions.linear_collapsing import Conv2DCollapsing
 from model_compression_toolkit.core.pytorch.constants import KERNEL, KERNEL_SIZE, STRIDES, DILATIONS, BIAS, USE_BIAS, FILTERS, PADDING, GROUPS
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def linear_collapsing_node_matchers() -> Tuple[NodeOperationMatcher, NodeOperationMatcher]:
     """
     Function generates matchers for matching:
     (Conv2D, Conv2D)[activation=linear] -> Conv2D.
     Returns:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 import operator
 from typing import List
 
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph, BaseNode, OutTensor
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
 from model_compression_toolkit.core.pytorch.constants import KERNEL, BIAS, NUM_HEADS, KEY_DIM, VALUE_DIM, \
     EMBED_DIM, BIAS_K, BIAS_V, ADD_ZERO_ATTN, BATCH_FIRST, OUT_PROJ_WEIGHT, OUT_PROJ_BIAS, \
     V_PROJ_WEIGHT, K_PROJ_WEIGHT, Q_PROJ_WEIGHT, IN_PROJ_WEIGHT, IN_PROJ_BIAS, DIM, KERNEL_SIZE, \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher, WalkMatcher
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.pytorch.constants import KERNEL, BIAS, INPLACE, HARDTANH_MIN_VAL, HARDTANH_MAX_VAL, \
     RELU_POT_BOUND
+from model_compression_toolkit.logger import Logger
 
 
 class ReLUBoundToPowerOfTwo(common.BaseSubstitution):
     """
     Substitution to scale the weights of two linear nodes, and move the bound of non-linear between them
     (if bounded) in order to use the entire constrained range when activations are quantized.
     """
@@ -98,16 +99,16 @@
                     (np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]).astype(int) -
                      np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]) == 0):
                 scale_factor = non_linear_node.framework_attr[HARDTANH_MAX_VAL] / self.threshold
                 non_linear_node.functional_op.__defaults__ = (0.0, self.threshold, non_linear_node.framework_attr[INPLACE])
             else:
                 return graph
         else:
-            common.Logger.error(f"In substitution with wrong matched pattern")
-        common.Logger.debug(
+            Logger.error(f"In substitution with wrong matched pattern")
+        Logger.debug(
             f"Node named:{non_linear_node.name} changed "
             f"to:{non_linear_node.type}")
 
         w2_fixed = scale_factor * second_op2d_node.get_weights_by_keys(KERNEL)
         w1_fixed = first_op2d_node.get_weights_by_keys(KERNEL) / scale_factor
         b1_fixed = first_op2d_node.get_weights_by_keys(BIAS) / scale_factor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from torch import reshape
 import torch
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.pytorch.constants import BATCH_DIM_VALUE
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import numpy as np
 import torch
 from torch.nn import Conv2d
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
 from model_compression_toolkit.core.common.substitutions.residual_collapsing import ResidualCollapsing
 from model_compression_toolkit.core.pytorch.constants import KERNEL
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def residual_collapsing_node_matchers() -> Tuple[NodeOperationMatcher, NodeOperationMatcher]:
     """
     Function generates matchers for matching:
     (Conv2D, Add)[activation=linear] -> Conv2D.
     Returns:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import torch.nn.functional
 from torch.nn import Conv2d, Linear, PReLU, ELU, Hardswish, Dropout, ZeroPad2d, SiLU
 from torch import reshape
 from torch.nn.functional import hardswish, silu, prelu, elu
 from torch.nn.functional import avg_pool2d
 
-from model_compression_toolkit import CoreConfig, FrameworkInfo
+from model_compression_toolkit.core import CoreConfig, FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.graph.graph_matchers import EdgeMatcher
 from model_compression_toolkit.core.common.graph.graph_matchers import NodeOperationMatcher
 from model_compression_toolkit.core.common.substitutions.shift_negative_activation import apply_shift_negative_correction
 from model_compression_toolkit.core.pytorch.constants import PAD, VALUE, PADDING, BIAS, USE_BIAS
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import PYTORCH
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import PYTORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_data import compute_kpi_data
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig, DEFAULT_MIXEDPRECISION_CONFIG, MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.constants import FOUND_TORCH
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
-    from model_compression_toolkit.core.pytorch.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from torch.nn import Module
 
     from model_compression_toolkit import get_target_platform_capabilities
 
     PYTORCH_DEFAULT_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
 
@@ -47,15 +47,15 @@
         Builds the computation graph from the given model and target platform capabilities, and uses it to compute the KPI data.
 
         Args:
             in_model (Model): PyTorch model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             quant_config (MixedPrecisionQuantizationConfig): MixedPrecisionQuantizationConfig containing parameters of how the model should be quantized.
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default PyTorch info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/pytorch/default_framework_info.py>`_
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to. `Default PyTorch TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/pytorch_tp_models/pytorch_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
 
         Returns:
             A KPI object with total weights parameters sum, max activation tensor and total kpi.
 
         Examples:
 
             Import a Pytorch model:
@@ -71,15 +71,15 @@
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 3, 224, 224))]
 
             Import mct and call for KPI data calculation:
 
             >>> import model_compression_toolkit as mct
-            >>> kpi_data = mct.pytorch_kpi_data(module, repr_datagen)
+            >>> kpi_data = mct.core.pytorch_kpi_data(module, repr_datagen)
 
         """
 
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
             Logger.error("KPI data computation can't be executed without MixedPrecisionQuantizationConfig object."
                          "Given quant_config is not of type MixedPrecisionQuantizationConfig.")
 
@@ -107,15 +107,15 @@
         Builds the computation graph from the given model and target platform capabilities, and uses it to compute the KPI data.
 
         Args:
             in_model (Model): PyTorch model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             core_config (CoreConfig): CoreConfig containing parameters for quantization and mixed precision
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default PyTorch info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/pytorch/default_framework_info.py>`_
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to. `Default PyTorch TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/pytorch_tp_models/pytorch_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
 
         Returns:
 
             A KPI object with total weights parameters sum and max activation tensor.
 
         Examples:
 
@@ -128,15 +128,15 @@
 
             >>> import numpy as np
             >>> def repr_datagen(): yield [np.random.random((1, 3, 224, 224))]
 
             Import mct and call for KPI data calculation:
 
             >>> import model_compression_toolkit as mct
-            >>> kpi_data = mct.pytorch_kpi_data(module, repr_datagen)
+            >>> kpi_data = mct.core.pytorch_kpi_data(module, repr_datagen)
 
         """
 
         if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
             Logger.error("KPI data computation can't be executed without MixedPrecisionQuantizationConfigV2 object."
                          "Given quant_config is not of type MixedPrecisionQuantizationConfigV2.")
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 
 from typing import Any, List
 
 import torch
 import copy
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.pytorch.utils import set_model, to_torch_tensor
 
 
 class PytorchMixedPrecisionWrapper(torch.nn.Module):
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import operator
+from copy import deepcopy
 from typing import List, Any, Tuple, Callable, Type, Dict
 
 import numpy as np
 import torch
 from torch import sigmoid, softmax, add, cat, argmax
 from torch.nn import Conv2d, ConvTranspose2d, Linear
 from torch.nn import Module, Sigmoid, Softmax
 
 import model_compression_toolkit.core.pytorch.constants as pytorch_constants
-from model_compression_toolkit import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.collectors.statistics_collector import BaseStatsCollector
 from model_compression_toolkit.core.common.collectors.statistics_collector_generator import \
     create_stats_collector_for_node
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.mixed_precision.sensitivity_evaluation import SensitivityEvaluation
@@ -70,18 +71,15 @@
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.weights_activation_split import \
     WeightsActivationSplit
 from model_compression_toolkit.core.pytorch.mixed_precision.set_layer_to_bitwidth import set_layer_to_bitwidth
 from model_compression_toolkit.core.pytorch.pytorch_node_prior_info import create_node_prior_info
 from model_compression_toolkit.core.pytorch.reader.reader import model_reader
 from model_compression_toolkit.core.pytorch.statistics_correction.apply_second_moment_correction import \
     pytorch_apply_second_moment_correction
-from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
-from model_compression_toolkit.core.pytorch.utils import torch_tensor_to_numpy
-from model_compression_toolkit.gptq.common.gptq_training import GPTQTrainer
-from model_compression_toolkit.gptq.pytorch.gptq_training import PytorchGPTQTrainer
+from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy, set_model
 
 
 class PytorchImplementation(FrameworkImplementation):
     """
     An class with implemented methods to support optimizing Pytorch models.
     """
 
@@ -123,15 +121,17 @@
         Convert a framework's module into a graph.
         Args:
             module: Framework's module.
             representative_data_gen (Callable): Dataset used for calibration.
         Returns:
             Graph representing the input module.
         """
-        return model_reader(module, representative_data_gen, self.to_numpy, self.to_tensor)
+        _module = deepcopy(module)
+        _module.eval()
+        return model_reader(_module, representative_data_gen, self.to_numpy, self.to_tensor)
 
     def model_builder(self,
                       graph: Graph,
                       mode: ModelBuilderMode,
                       append2output: List[Any] = None,
                       fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO,
                       return_float_outputs: bool = False) -> Tuple[Module, UserInformation]:
@@ -319,20 +319,14 @@
             A list of the framework substitutions used after we apply second moment statistics.
         """
         substitutions_list = []
         if quant_config.weights_second_moment_correction:
             substitutions_list.append(pytorch_batchnorm_refusing())
         return substitutions_list
 
-    def get_gptq_trainer_obj(self) -> Type[GPTQTrainer]:
-        """
-        Returns: GPTQTrainer object
-        """
-        return PytorchGPTQTrainer
-
     def get_sensitivity_evaluator(self,
                                   graph: Graph,
                                   quant_config: MixedPrecisionQuantizationConfigV2,
                                   representative_data_gen: Callable,
                                   fw_info: FrameworkInfo,
                                   disable_activation_for_metric: bool = False) -> SensitivityEvaluation:
         """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any, Tuple
 import numpy as np
 from torch.nn import BatchNorm2d
 
-from model_compression_toolkit import FrameworkInfo
+from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.pytorch.constants import MOVING_MEAN, MOVING_VARIANCE, GAMMA, BETA
 
 
 def create_node_prior_info(node: BaseNode,
                            fw_info: FrameworkInfo,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable, List, Tuple
 
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import PYTORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import PYTORCH
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, GradientPTQConfigV2
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.network_editors.actions import EditRule
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common.quantization.debug_config import DebugConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig, DEFAULT_MIXEDPRECISION_CONFIG
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
 from model_compression_toolkit.core.common.quantization.quantization_config import DEFAULTCONFIG
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.gptq.runner import gptq_runner
 from model_compression_toolkit.ptq.runner import ptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.constants import FOUND_TORCH
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
-    from model_compression_toolkit.core.pytorch.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from torch.nn import Module
 
     from model_compression_toolkit import get_target_platform_capabilities
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
     def pytorch_post_training_quantization(in_module: Module,
                                            representative_data_gen: Callable,
@@ -72,15 +71,15 @@
             representative_data_gen (Callable): Dataset used for calibration.
             n_iter (int): Number of calibration iterations to run.
             quant_config (QuantizationConfig): QuantizationConfig containing parameters of how the module should be quantized. `Default configuration. <https://github.com/sony/model_optimization/blob/21e21c95ca25a31874a5be7af9dd2dd5da8f3a10/model_compression_toolkit/core/common/quantization/quantization_config.py#L154>`_
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default PyTorch info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/pytorch/default_framework_info.py>`_
             network_editor (List[EditRule]): List of EditRules. Each EditRule consists of a node filter and an action to change quantization settings of the filtered nodes.
             gptq_config (GradientPTQConfig): Configuration for using gptq (e.g. optimizer).
             analyze_similarity (bool): Whether to plot similarity figures within TensorBoard (when logger is enabled) or not.
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to. `Default PyTorch TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/pytorch_tp_models/pytorch_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
 
 
         Returns:
             A quantized module and information the user may need to handle the quantized module.
 
         Examples:
 
@@ -171,15 +170,15 @@
              target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
              n_iter (int): Number of calibration iterations to run.
              quant_config (MixedPrecisionQuantizationConfig): QuantizationConfig containing parameters of how the model should be quantized.
              fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default PyTorch info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/pytorch/default_framework_info.py>`_
              network_editor (List[EditRule]): List of EditRules. Each EditRule consists of a node filter and an action to change quantization settings of the filtered nodes.
              gptq_config (GradientPTQConfig): Configuration for using GPTQ (e.g. optimizer).
              analyze_similarity (bool): Whether to plot similarity figures within TensorBoard (when logger is enabled) or not.
-             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to. `Default PyTorch TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/pytorch_tp_models/pytorch_default.py>`_
+             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
 
          Returns:
              A quantized model and information the user may need to handle the quantized model.
 
          Examples:
 
              Import MCT:
@@ -195,37 +194,37 @@
 
              >>> import numpy as np
              >>> def repr_datagen(): return [np.random.random((1,224,224,3))]
 
              Create a mixed-precision configuration, to quantize a model with different bitwidths for different layers.
              The candidates bitwidth for quantization should be defined in the target platform model:
 
-             >>> config = mct.MixedPrecisionQuantizationConfig()
+             >>> config = mct.core.MixedPrecisionQuantizationConfig()
 
              Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
              that should be quantized (for example, the kernel of Conv2D in PyTorch will be affected by this value,
              while the bias will not):
 
-             >>> kpi = mct.KPI(sum(p.numel() for p in module.parameters()) * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+             >>> kpi = mct.core.KPI(sum(p.numel() for p in module.parameters()) * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model:
 
              >>> quantized_model, quantization_info = mct.pytorch_post_training_quantization_mixed_precision(module, repr_datagen, n_iter=10, quant_config=config, target_kpi=kpi)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/experimental_api_docs/modules/mixed_precision_quantization_config.html#model_compression_toolkit.MixedPrecisionQuantizationConfigV2>`_.
 
          """
 
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
-            common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+            Logger.error("Given quantization config to mixed-precision facade is not of type "
                                 "MixedPrecisionQuantizationConfig. Please use pytorch_post_training_quantization API, "
                                 "or pass a valid mixed precision configuration.")
 
-        common.Logger.info("Using experimental mixed-precision quantization. "
+        Logger.info("Using experimental mixed-precision quantization. "
                            "If you encounter an issue please file a bug.")
 
         quantization_config, mp_config = quant_config.separate_configs()
         core_config = CoreConfig(quantization_config=quantization_config,
                                  mixed_precision_config=mp_config,
                                  debug_config=DebugConfig(analyze_similarity=analyze_similarity,
                                                           network_editor=network_editor))
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Tuple, Callable
+from typing import Callable
 import torch
 
-from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import fix_range_to_include_zero
 
 
 def get_symmetric_quantization_range_and_scale(activation_is_signed: bool,
                                                activation_n_bits: int,
                                                activation_threshold: float):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Callable
 
 import torch
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import SIGNED, CLUSTER_CENTERS, THRESHOLD, MULTIPLIER_N_BITS, EPS
+from model_compression_toolkit.constants import SIGNED, CLUSTER_CENTERS, THRESHOLD, MULTIPLIER_N_BITS, EPS
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 
 
 def activation_lut_kmean_quantizer(activation_n_bits: int,
                                    quantization_params: Dict[str, np.ndarray]) -> Callable:
     """
     Builds a LUT quantizer for layer's activation using the provided params (threshold and clusters).
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.base_graph import OutTensor
 from model_compression_toolkit.core.common.graph.edge import Edge
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.pytorch.constants import OUTPUT, PLACEHOLDER, TENSOR_META, CALL_FUNCTION, TYPE, \
     CALL_METHOD, BIAS, FUNCTIONAL_OP, OP_CALL_KWARGS, OP_CALL_ARGS, INPUTS_AS_LIST, GET_ATTR, CONSTANT, BUFFER
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder, ConstantHolder, BufferHolder
+from model_compression_toolkit.logger import Logger
 
 
 def extract_holder_weights(constant_name, node_target, model, weights, to_numpy):
     """
     Extract layer weights and named buffers for BufferHolder and ConstantHolder.
     Args:
         constant_name: name to write the parameters under, CONSTANT for ConstantHolder and
@@ -60,14 +61,15 @@
                   to_numpy: Callable) -> Tuple[List, List, List, Dict]:
     """
     Build a node from a fx node. A node contains all information to reconstruct the model module or call function
     it's representing in the model: operation, module configuration, weights, input/output shape.
     Args:
         model: Pytorch FX model.
         module_dict: A dictionary of the Pyotrch model's named modules.
+        to_numpy: A function to convert a Tensor to numpy array
 
     Returns:
         A list of Graph nodes that were built from the fx GraphModule nodes.
     """
     # init function variables:
     inputs = []
     outputs = []
@@ -87,15 +89,15 @@
             framework_attr = {k: v for k, v in framework_attr.items() if k in fullargspec}
             if hasattr(node_module, BIAS) and BIAS in fullargspec:
                 framework_attr[BIAS] = False if node_module.bias is None else True
         elif node.op == CALL_FUNCTION:
             node_type = node.target
             if node_type == getattr:
                 node_has_activation = False
-                common.Logger.warning(
+                Logger.warning(
                     'Pytorch model has a parameter or constant Tensor value. This can cause unexpected behaviour when '
                     'converting the model.')
         elif node.op == PLACEHOLDER:
             node_type = DummyPlaceHolder
         elif node.op == OUTPUT:
             output_nodes += node.all_input_nodes
             continue
@@ -108,15 +110,15 @@
                 raise Exception(f'Call method of type \'{node.target}\' is currently not supported.')
         elif node.op == GET_ATTR:
             if node.meta[TYPE] == torch.Tensor:
                 node_type = BufferHolder
             else:
                 node_type = ConstantHolder
             node_has_activation = False
-            common.Logger.warning(
+            Logger.warning(
                 'Pytorch model has a parameter or constant Tensor value. This can cause unexpected behaviour when '
                 'converting the model.')
         else:
             raise Exception(f'Unknown node type: {node.name}')
 
         # extract layer weights and named buffers
         weights = {}
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 import copy
 from typing import Any, Callable
 
 import torch
 from tqdm import tqdm
 
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.pytorch.constants import GAMMA, BETA, MOVING_MEAN, MOVING_VARIANCE
 from model_compression_toolkit.core.pytorch.utils import set_model, to_torch_tensor
 
 
 def pytorch_apply_second_moment_correction(quantized_model: Any,
                                            core_config: CoreConfig,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/runner.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Callable, Tuple, Any, List, Dict
 
 import numpy as np
 from tqdm import tqdm
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import FrameworkInfo
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.fusion.layer_fusing import fusion
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.mixed_precision.bit_width_setter import set_bit_widths
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI, KPITarget
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_aggregation_methods import MpKpiAggregation
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi_functions_mapping import kpi_functions_mapping
@@ -44,15 +44,15 @@
 from model_compression_toolkit.core.common.quantization.set_node_quantization_config import \
     set_quantization_configuration_to_graph
 from model_compression_toolkit.core.common.statistics_correction.statistics_correction import \
     statistics_correction_runner
 from model_compression_toolkit.core.common.substitutions.apply_substitutions import substitute
 from model_compression_toolkit.core.common.substitutions.linear_collapsing_substitution import \
     linear_collapsing_substitute
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.visualization.final_config_visualizer import \
     WeightsFinalBitwidthConfigVisualizer, \
     ActivationFinalBitwidthConfigVisualizer
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import TensorboardWriter
 
 
 def core_runner(in_model: Any,
@@ -139,17 +139,17 @@
                    fw_impl=fw_impl)
 
     if target_kpi is not None:
         # Retrieve lists of tuples (node, node's final weights/activation bitwidth)
         weights_conf_nodes_bitwidth = tg.get_final_weights_config()
         activation_conf_nodes_bitwidth = tg.get_final_activation_config()
 
-        common.Logger.info(
+        Logger.info(
             f'Final weights bit-width configuration: {[node_b[1] for node_b in weights_conf_nodes_bitwidth]}')
-        common.Logger.info(
+        Logger.info(
             f'Final activation bit-width configuration: {[node_b[1] for node_b in activation_conf_nodes_bitwidth]}')
 
         if tb_w is not None:
             if len(weights_conf_nodes_bitwidth) > 0:
                 visual = WeightsFinalBitwidthConfigVisualizer(weights_conf_nodes_bitwidth)
                 figure = visual.plot_config_bitwidth()
                 tb_w.add_figure(figure, f'Weights final bit-width config')
@@ -255,17 +255,17 @@
     Args:
         fw_info: FrameworkInfo object.
 
     Returns:
         A TensorBoardWriter object.
     """
     tb_w = None
-    if common.Logger.LOG_PATH is not None:
-        tb_log_dir = os.path.join(os.getcwd(), common.Logger.LOG_PATH, 'tensorboard_logs')
-        common.Logger.info(f'To use Tensorboard, please run: tensorboard --logdir {tb_log_dir}')
+    if Logger.LOG_PATH is not None:
+        tb_log_dir = os.path.join(os.getcwd(), Logger.LOG_PATH, 'tensorboard_logs')
+        Logger.info(f'To use Tensorboard, please run: tensorboard --logdir {tb_log_dir}')
         tb_w = TensorboardWriter(tb_log_dir, fw_info)
     return tb_w
 
 
 def read_model_to_graph(in_model: Any,
                         representative_data_gen: Callable,
                         tpc: TargetPlatformCapabilities,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH
-
-from model_compression_toolkit.core.tpc_models.default_tpc.v4.tp_model import get_tp_model, generate_tp_model, get_op_quantization_configs
-
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model, generate_tp_model, get_op_quantization_configs
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_keras import get_keras_tpc as get_keras_tpc_latest
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_keras import generate_keras_tpc
-
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_keras import generate_keras_tpc
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_latest
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_pytorch import generate_pytorch_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_pytorch import generate_pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH, LATEST
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH
+from model_compression_toolkit.target_platform_capabilities.constants import LATEST
+
 
 ###############################
 # Build Tensorflow TPC models
 ###############################
 keras_tpc_models_dict = None
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.default_tpc.latest import get_keras_tpc_latest
-    from model_compression_toolkit.core.tpc_models.default_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
-    from model_compression_toolkit.core.tpc_models.default_tpc.v2.tpc_keras import get_keras_tpc as get_keras_tpc_v2
-    from model_compression_toolkit.core.tpc_models.default_tpc.v3.tpc_keras import get_keras_tpc as get_keras_tpc_v3
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_keras import get_keras_tpc as get_keras_tpc_v4
-    from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v3_lut
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v4_lut
-    from model_compression_toolkit.core.tpc_models.default_tpc.v5.tpc_keras import get_keras_tpc as get_keras_tpc_v5
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.latest import get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2.tpc_keras import get_keras_tpc as get_keras_tpc_v2
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tpc_keras import get_keras_tpc as get_keras_tpc_v3
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_keras import get_keras_tpc as get_keras_tpc_v4
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v3_lut
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v4_lut
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v5.tpc_keras import get_keras_tpc as get_keras_tpc_v5
 
     # Keras: TPC versioning
     keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
                              'v2': get_keras_tpc_v2(),
                              'v3': get_keras_tpc_v3(),
                              'v3_lut': get_keras_tpc_v3_lut(),
                              'v4': get_keras_tpc_v4(),
@@ -40,28 +42,28 @@
                              LATEST: get_keras_tpc_latest()}
 
 ###############################
 # Build Pytorch TPC models
 ###############################
 pytorch_tpc_models_dict = None
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.default_tpc.latest import get_pytorch_tpc_latest
-    from model_compression_toolkit.core.tpc_models.default_tpc.v1.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.latest import get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v1
-    from model_compression_toolkit.core.tpc_models.default_tpc.v2.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v2
-    from model_compression_toolkit.core.tpc_models.default_tpc.v3.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v3
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v4
-    from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v3_lut
-    from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v4_lut
-    from model_compression_toolkit.core.tpc_models.default_tpc.v5.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v5.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v5
 
     # Pytorch: TPC versioning
     pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
                                'v2': get_pytorch_tpc_v2(),
                                'v3': get_pytorch_tpc_v3(),
                                'v3_lut': get_pytorch_tpc_v3_lut(),
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -102,14 +105,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                          tp.get_default_quantization_config_options().clone_and_edit(
                              enable_weights_quantization=False,
                              enable_activation_quantization=False))
 
         # Define operator sets that use mixed_precision_configuration_options:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Reshape, ZeroPadding2D, \
         Dropout, \
         MaxPooling2D, Activation, ReLU, Flatten, Cropping2D
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Reshape, ZeroPadding2D, \
         Dropout, MaxPooling2D, Activation, ReLU, Flatten, Cropping2D
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import torch
 from torch import flatten, reshape, split, unsqueeze, dropout, chunk
 from torch.nn import Conv2d, BatchNorm2d
 from torch.nn import Dropout, Flatten
 from torch.nn import ReLU, ReLU6
 from torch.nn.functional import relu, relu6
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -102,14 +105,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                          tp.get_default_quantization_config_options().clone_and_edit(
                              enable_weights_quantization=False,
                              enable_activation_quantization=False))
 
         conv = tp.OperatorsSet("Conv")
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, \
         MaxPooling2D, Activation, ReLU, PReLU, Flatten, Cropping2D
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, MaxPooling2D, Activation, ReLU, PReLU, Flatten, Cropping2D
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v2.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v2 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import torch
 from torch import flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk
 from torch.nn import Conv2d, Linear, BatchNorm2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v2.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v2 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v2 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -109,14 +112,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                          tp.get_default_quantization_config_options().clone_and_edit(
                              enable_weights_quantization=False,
                              enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import tensorflow as tf
 from packaging import version
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut import __version__ as TPC_VERSION
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v3 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Keras TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
-    default_tp_model = get_tp_model()
-    return generate_keras_tpc(name='default_keras_tpc', tp_model=default_tp_model)
+    lut_mp_tp_model = get_tp_model()
+    return generate_keras_tpc(name='default_keras_lut_mp_tpc', tp_model=lut_mp_tp_model)
 
 
 def generate_keras_tpc(name: str, tp_model: tp.TargetPlatformModel):
     """
     Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
 
     Args:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import torch
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind
 from torch.nn import Conv2d, Linear, BatchNorm2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v3 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel, \
-    QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel, QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -111,14 +113,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                         tp.get_default_quantization_config_options().clone_and_edit(
                             enable_weights_quantization=False,
                             enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import tensorflow as tf
 from packaging import version
-from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut import __version__ as TPC_VERSION
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, \
         Dropout, MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tp_model import get_tp_model
 import model_compression_toolkit as mct
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Keras TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
-    lut_mp_tp_model = get_tp_model()
-    return generate_keras_tpc(name='default_keras_lut_mp_tpc', tp_model=lut_mp_tp_model)
+    default_tp_model = get_tp_model()
+    return generate_keras_tpc(name='default_keras_tpc', tp_model=default_tp_model)
 
 
 def generate_keras_tpc(name: str, tp_model: tp.TargetPlatformModel):
     """
     Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
 
     Args:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import torch
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind
 from torch.nn import Conv2d, Linear, BatchNorm2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v3_lut import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3_lut import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -109,14 +112,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                          tp.get_default_quantization_config_options().clone_and_edit(
                              enable_weights_quantization=False,
                              enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,22 +20,21 @@
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v4.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
-
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Keras TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
     default_tp_model = get_tp_model()
     return generate_keras_tpc(name='default_keras_tpc', tp_model=default_tp_model)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind, \
     permute, transpose, equal, gather, topk
 from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish, LeakyReLU
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish, leaky_relu
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel, \
-    QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel, QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -111,14 +113,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                         tp.get_default_quantization_config_options().clone_and_edit(
                             enable_weights_quantization=False,
                             enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import tensorflow as tf
 from packaging import version
-from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut import __version__ as TPC_VERSION
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut.tp_model import get_tp_model
 import model_compression_toolkit as mct
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,34 +13,34 @@
 # limitations under the License.
 # ==============================================================================
 
 import operator
 
 import torch
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind, topk, \
-    gather, equal, permute, transpose
+    gather, equal, transpose, permute
 from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish, LeakyReLU
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish, leaky_relu
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v4_lut import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Pytorch TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
-    lut_mp_tp_model = get_tp_model()
-    return generate_pytorch_tpc(name='default_pytorch_lut_mp_tpc', tp_model=lut_mp_tp_model)
+    imx500_tpc_tp_model = get_tp_model()
+    return generate_pytorch_tpc(name='imx500_tpc_pytorch_tpc', tp_model=imx500_tpc_tp_model)
 
 
 def generate_pytorch_tpc(name: str, tp_model: tp.TargetPlatformModel):
     """
     Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
     Args:
         name: Name of the TargetPlatformModel.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -109,14 +112,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                          tp.get_default_quantization_config_options().clone_and_edit(
                              enable_weights_quantization=False,
                              enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v4.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind, topk, \
     gather, equal, transpose, permute
 from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish, LeakyReLU
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish, leaky_relu
 
-from model_compression_toolkit.core.tpc_models.default_tpc.v3.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v3.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,46 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH
+from model_compression_toolkit.target_platform_capabilities.constants import LATEST
+
+###############################
+# Build Tensorflow TPC models
+###############################
+keras_tpc_models_dict = None
+if FOUND_TF:
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.latest import get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
+
+    # Keras: TPC versioning
+    keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
+                             LATEST: get_keras_tpc_latest()}
+
+###############################
+# Build Pytorch TPC models
+###############################
+pytorch_tpc_models_dict = None
+if FOUND_TORCH:
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.latest import get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import \
+        get_pytorch_tpc as get_pytorch_tpc_v1
+
+    # Pytorch: TPC versioning
+    pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
+                               LATEST: get_pytorch_tpc_latest()}
+
+tpc_dict = {TENSORFLOW: keras_tpc_models_dict,
+            PYTORCH: pytorch_tpc_models_dict}
 
-from model_compression_toolkit.core.tpc_models.default_tpc.target_platform_capabilities import \
-    tpc_dict as default_tpc_dict
-from model_compression_toolkit.core.tpc_models.imx500_tpc.target_platform_capabilities import \
-    tpc_dict as imx500_tpc_dict
-from model_compression_toolkit.core.tpc_models.tflite_tpc.target_platform_capabilities import \
-    tpc_dict as tflite_tpc_dict
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.target_platform_capabilities import \
-    tpc_dict as qnnpack_tpc_dict
-from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL, IMX500_TP_MODEL, TFLITE_TP_MODEL, \
-    QNNPACK_TP_MODEL
-from model_compression_toolkit.core.common.constants import LATEST
-
-tpc_dict = {DEFAULT_TP_MODEL: default_tpc_dict,
-            IMX500_TP_MODEL: imx500_tpc_dict,
-            TFLITE_TP_MODEL: tflite_tpc_dict,
-            QNNPACK_TP_MODEL: qnnpack_tpc_dict}
-
-
-def get_target_platform_capabilities(fw_name: str,
-                                     target_platform_name: str,
-                                     target_platform_version: str = None) -> TargetPlatformCapabilities:
-    """
-    Get a TargetPlatformCapabilities by the target platform model name and the framework name.
-    For now, it supports frameworks 'tensorflow' and 'pytorch'. For both of them
-    the target platform model can be 'default', 'imx500', 'tflite', or 'qnnpack'.
-
-    Args:
-        fw_name: Framework name of the TargetPlatformCapabilities.
-        target_platform_name: Target platform model name the model will use for inference.
-        target_platform_version: Target platform capabilities version.
-    Returns:
-        A TargetPlatformCapabilities object that models the hardware and attaches
-        a framework information to it.
-    """
-    assert target_platform_name in tpc_dict, f'Target platform {target_platform_name} is not defined!'
-    fw_tpc = tpc_dict.get(target_platform_name)
-    assert fw_name in fw_tpc, f'Framework {fw_name} is not supported in {target_platform_name}. Please make sure the relevant ' \
-                              f'packages are installed when using MCT for optimizing a {fw_name} model. ' \
-                              f'For Tensorflow, please install tensorflow and tensorflow-model-optimization. ' \
-                              f'For PyTorch, please install torch.'
-    tpc_versions = fw_tpc.get(fw_name)
-    if target_platform_version is None:
-        target_platform_version = LATEST
-    else:
-        assert target_platform_version in tpc_versions, f'TPC version {target_platform_version} is not supported for framework {fw_name}'
-    return tpc_versions.get(target_platform_version)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH
-from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tp_model import get_tp_model, generate_tp_model, \
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tp_model import get_tp_model, generate_tp_model, \
     get_op_quantization_configs
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_keras import generate_keras_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import generate_keras_tpc
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_pytorch import get_pytorch_tpc as \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import get_pytorch_tpc as \
         get_pytorch_tpc_latest
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_pytorch import generate_pytorch_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import generate_pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH, LATEST
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH
+from model_compression_toolkit.target_platform_capabilities.constants import LATEST
+
 
 ###############################
 # Build Tensorflow TPC models
 ###############################
 keras_tpc_models_dict = None
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.latest import get_keras_tpc_latest
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.latest import get_keras_tpc_latest
 
     # Keras: TPC versioning
     keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
                              LATEST: get_keras_tpc_latest()}
 
 ###############################
 # Build Pytorch TPC models
 ###############################
 pytorch_tpc_models_dict = None
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.latest import get_pytorch_tpc_latest
-    from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v1
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.latest import get_pytorch_tpc_latest
 
     # Pytorch: TPC versioning
     pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
                                LATEST: get_pytorch_tpc_latest()}
 
 tpc_dict = {TENSORFLOW: keras_tpc_models_dict,
             PYTORCH: pytorch_tpc_models_dict}
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -109,14 +112,17 @@
     with generated_tpc:
         # Create an OperatorsSet to represent a set of operations.
         # Each OperatorsSet has a unique label.
         # If a quantization configuration options is passed, these options will
         # be used for operations that will be attached to this set's label.
         # Otherwise, it will be a configure-less set (used in fusing):
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
         # May suit for operations like: Dropout, Reshape, etc.
         tp.OperatorsSet("NoQuantization",
                         tp.get_default_quantization_config_options().clone_and_edit(
                             enable_weights_quantization=False,
                             enable_activation_quantization=False))
 
         # Create Mixed-Precision quantization configuration options from the given list of OpQuantizationConfig objects
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Dense, Reshape, ZeroPadding2D, Dropout, \
         MaxPooling2D, Activation, ReLU, Add, Subtract, Multiply, PReLU, Flatten, Cropping2D, LeakyReLU, Permute, \
         Conv2DTranspose
 
-from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.imx500_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,34 +13,34 @@
 # limitations under the License.
 # ==============================================================================
 
 import operator
 
 import torch
 from torch import add, sub, mul, div, flatten, reshape, split, unsqueeze, dropout, sigmoid, tanh, chunk, unbind, topk, \
-    gather, equal, transpose, permute
+    gather, equal, permute, transpose
 from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d
 from torch.nn import Dropout, Flatten, Hardtanh
 from torch.nn import ReLU, ReLU6, PReLU, SiLU, Sigmoid, Tanh, Hardswish, LeakyReLU
 from torch.nn.functional import relu, relu6, prelu, silu, hardtanh, hardswish, leaky_relu
 
-from model_compression_toolkit.core.tpc_models.imx500_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.imx500_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4_lut import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Pytorch TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
-    imx500_tpc_tp_model = get_tp_model()
-    return generate_pytorch_tpc(name='imx500_tpc_pytorch_tpc', tp_model=imx500_tpc_tp_model)
+    lut_mp_tp_model = get_tp_model()
+    return generate_pytorch_tpc(name='default_pytorch_lut_mp_tpc', tp_model=lut_mp_tp_model)
 
 
 def generate_pytorch_tpc(name: str, tp_model: tp.TargetPlatformModel):
     """
     Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
     Args:
         name: Name of the TargetPlatformModel.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model, generate_tp_model, get_op_quantization_configs
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tp_model import get_tp_model, generate_tp_model, get_op_quantization_configs
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_keras import generate_keras_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_keras import generate_keras_tpc
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_latest
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_pytorch import generate_pytorch_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tpc_pytorch import generate_pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH, LATEST
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH
+from model_compression_toolkit.target_platform_capabilities.constants import LATEST
 
 
 ###############################
 # Build Tensorflow TPC models
 ###############################
 keras_tpc_models_dict = None
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.latest import get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.latest import get_keras_tpc_latest
 
     # Keras: TPC versioning
     keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
                              LATEST: get_keras_tpc_latest()}
 
 ###############################
 # Build Pytorch TPC models
 ###############################
 pytorch_tpc_models_dict = None
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tpc_pytorch import \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v1
-    from model_compression_toolkit.core.tpc_models.qnnpack_tpc.latest import get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.latest import get_pytorch_tpc_latest
 
     # Pytorch: TPC versioning
     pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
                                LATEST: get_pytorch_tpc_latest()}
 
 tpc_dict = {TENSORFLOW: keras_tpc_models_dict,
             PYTORCH: pytorch_tpc_models_dict}
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -116,8 +119,11 @@
         # Fusions
         # ------------------- #
         tp.Fusing([conv, batchnorm, relu])
         tp.Fusing([conv, batchnorm])
         tp.Fusing([conv, relu])
         tp.Fusing([linear, relu])
 
+        # Set quantization format to fakely quant
+        generated_tpc.set_quantization_format(QuantizationFormat.FAKELY_QUANT)
+
     return generated_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import tensorflow as tf
 
 from packaging import version
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1 import __version__ as TPC_VERSION
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, BatchNormalization, ReLU, \
         Activation
 else:
     from keras.layers import Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, BatchNormalization, ReLU, Activation
 
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import torch
 from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d, Hardtanh, ReLU, ReLU6
 from torch.nn.functional import relu, relu6, hardtanh
 
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.qnnpack_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,39 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH
 
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH, TENSORFLOW, PYTORCH, LATEST
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tp_model import get_tp_model, generate_tp_model, get_op_quantization_configs
 
-
-###############################
-# Build Tensorflow TPC models
-###############################
-keras_tpc_models_dict = None
 if FOUND_TF:
-    from model_compression_toolkit.core.tpc_models.tflite_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
-    from model_compression_toolkit.core.tpc_models.tflite_tpc.latest import get_keras_tpc_latest
-
-    # Keras: TPC versioning
-    keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
-                             LATEST: get_keras_tpc_latest()}
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_keras import get_keras_tpc as get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_keras import generate_keras_tpc
 
-###############################
-# Build Pytorch TPC models
-###############################
-pytorch_tpc_models_dict = None
 if FOUND_TORCH:
-    from model_compression_toolkit.core.tpc_models.tflite_tpc.v1.tpc_pytorch import \
-        get_pytorch_tpc as get_pytorch_tpc_v1
-    from model_compression_toolkit.core.tpc_models.tflite_tpc.latest import get_pytorch_tpc_latest
-
-    # Pytorch: TPC versioning
-    pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
-                               LATEST: get_pytorch_tpc_latest()}
-
-tpc_dict = {TENSORFLOW: keras_tpc_models_dict,
-            PYTORCH: pytorch_tpc_models_dict}
-
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v4.tpc_pytorch import generate_pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Tuple
 
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.common.target_platform import OpQuantizationConfig, TargetPlatformModel
-from model_compression_toolkit.core.common.target_platform.op_quantization_config import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import OpQuantizationConfig, \
+    TargetPlatformModel
+from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import \
+    QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform.quantization_format import \
+    QuantizationFormat
 
 tp = mct.target_platform
 
 
 def get_tp_model() -> TargetPlatformModel:
     """
     A method that generates a default target platform model, with base 8-bit quantization configuration and 8, 4, 2
@@ -61,15 +65,15 @@
         enable_activation_quantization=True,
         quantization_preserving=False,
         fixed_scale=None,
         fixed_zero_point=None,
         weights_multiplier_nbits=None
     )
 
-    mixed_precision_cfg_list = [] # No mixed precision
+    mixed_precision_cfg_list = []  # No mixed precision
 
     return eight_bits, mixed_precision_cfg_list
 
 
 def generate_tp_model(default_config: OpQuantizationConfig,
                       base_config: OpQuantizationConfig,
                       mixed_precision_cfg_list: List[OpQuantizationConfig],
@@ -102,54 +106,58 @@
     # To start defining the model's components (such as operator sets, and fusing patterns),
     # use 'with' the TargetPlatformModel instance, and create them as below:
     with generated_tpc:
         # In TFLite, the quantized operator specifications constraint operators quantization
         # differently. For more details:
         # https://www.tensorflow.org/lite/performance/quantization_spec#int8_quantized_operator_specifications
         tp.OperatorsSet("NoQuantization",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  quantization_preserving=True))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            quantization_preserving=True))
 
         fc = tp.OperatorsSet("FullyConnected",
-                              tp.get_default_quantization_config_options().clone_and_edit(
-                                       weights_per_channel_threshold=False))
+                             tp.get_default_quantization_config_options().clone_and_edit(
+                                 weights_per_channel_threshold=False))
 
         tp.OperatorsSet("L2Normalization",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  fixed_zero_point=0, fixed_scale=1 / 128))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            fixed_zero_point=0, fixed_scale=1 / 128))
         tp.OperatorsSet("LogSoftmax",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  fixed_zero_point=127, fixed_scale=16 / 256))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            fixed_zero_point=127, fixed_scale=16 / 256))
         tp.OperatorsSet("Tanh",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  fixed_zero_point=0, fixed_scale=1 / 128))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            fixed_zero_point=0, fixed_scale=1 / 128))
         tp.OperatorsSet("Softmax",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  fixed_zero_point=-128, fixed_scale=1 / 256))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            fixed_zero_point=-128, fixed_scale=1 / 256))
         tp.OperatorsSet("Logistic",
-                         tp.get_default_quantization_config_options().clone_and_edit(
-                                  fixed_zero_point=-128, fixed_scale=1 / 256))
+                        tp.get_default_quantization_config_options().clone_and_edit(
+                            fixed_zero_point=-128, fixed_scale=1 / 256))
 
         conv2d = tp.OperatorsSet("Conv2d")
         kernel = tp.OperatorSetConcat(conv2d, fc)
 
         relu = tp.OperatorsSet("Relu")
         elu = tp.OperatorsSet("Elu")
         activations_to_fuse = tp.OperatorSetConcat(relu, elu)
 
         batch_norm = tp.OperatorsSet("BatchNorm")
         bias_add = tp.OperatorsSet("BiasAdd")
         add = tp.OperatorsSet("Add")
         squeeze = tp.OperatorsSet("Squeeze",
-                                   qc_options=tp.get_default_quantization_config_options().clone_and_edit(quantization_preserving=True))
+                                  qc_options=tp.get_default_quantization_config_options().clone_and_edit(
+                                      quantization_preserving=True))
         # ------------------- #
         # Fusions
         # ------------------- #
         # Source: https://github.com/tensorflow/tensorflow/blob/master/tensorflow/core/grappler/optimizers/remapper
         tp.Fusing([kernel, bias_add])
         tp.Fusing([kernel, bias_add, activations_to_fuse])
         tp.Fusing([conv2d, batch_norm, activations_to_fuse])
         tp.Fusing([conv2d, squeeze, activations_to_fuse])
         tp.Fusing([batch_norm, activations_to_fuse])
         tp.Fusing([batch_norm, add, activations_to_fuse])
 
+        # Set quantization format to int8
+        generated_tpc.set_quantization_format(QuantizationFormat.INT8)
+
     return generated_tpc
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         DepthwiseConv2D, MaxPooling2D, ReLU, Add, Softmax, Concatenate, Multiply, Maximum, Minimum, BatchNormalization
 else:
     from keras.layers import Conv2D, Dense, Reshape, ZeroPadding2D, AveragePooling2D, Activation, DepthwiseConv2D, \
         MaxPooling2D, ReLU, Add, Softmax, Concatenate, Multiply, Maximum, Minimum, BatchNormalization
 
 from tensorflow.python.keras.layers.core import SlicingOpLambda
 from tensorflow.python.ops.image_ops_impl import ResizeMethod
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.attribute_filter import Eq
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.attribute_filter import Eq
 
-from model_compression_toolkit.core.tpc_models.tflite_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.tflite_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_keras_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Keras TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import torch
 from torch.nn import AvgPool2d, MaxPool2d
 from torch.nn.functional import avg_pool2d, max_pool2d, interpolate
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework.attribute_filter import Eq
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.attribute_filter import Eq
 
-from model_compression_toolkit.core.tpc_models.tflite_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.core.tpc_models.tflite_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.tflite_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 
 
 from abc import abstractmethod
 from typing import Any, Callable
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 
 
 class Exporter:
     """
     Base class to define API for an Exporter class that exports and saves models.
     At initiation, it gets a model to export. This model must be an exportable model.
     Each exporter needs to implement a method called 'export' which export the model
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Dict, Callable
 
 import keras.models
 import keras.models
 import tensorflow as tf
 from keras.engine.base_layer import Layer
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.exporter.model_exporter.keras.base_keras_exporter import \
     BaseKerasExporter
 from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
 
 
 
 class FakelyQuantKerasExporter(BaseKerasExporter):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from enum import Enum
 from typing import Callable, Dict
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
 
 class KerasExportMode(Enum):
     FAKELY_QUANT = 0
 
 
 if FOUND_TF:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,26 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
 
 import torch.nn
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
-from packaging import version
 
-# ONNX opset version 16 is supported from PyTorch 1.12
-if version.parse(torch.__version__) < version.parse("1.12"):
-    OPSET_VERSION = 15
-else:
-    OPSET_VERSION = 16
 
-class FakelyQuantONNXPyTorchExporter(BasePyTorchExporter):
+class FakelyQuantTorchScriptPyTorchExporter(BasePyTorchExporter):
     """
     Exporter for fakely-quant PyTorch models.
     The exporter expects to receive an exportable model (where each layer's full quantization parameters
     can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
     format) and fake-quant layers for the activations.
     """
 
@@ -50,32 +44,26 @@
         """
 
         super().__init__(model,
                          is_layer_exportable_fn,
                          save_model_path,
                          repr_dataset)
 
-
     def export(self) -> None:
         """
         Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
         (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
         Returns:
             Fake-quant PyTorch model.
         """
         for layer in self.model.children():
-            assert self.is_layer_exportable_fn(layer), f'Layer {layer.name} is not exportable.'
+            assert self.is_layer_exportable_fn(layer), f'Layer {layer} is not exportable.'
 
-        model_input = to_torch_tensor(next(self.repr_dataset())[0])
+        torch_traced = torch.jit.trace(self.model,
+                                       to_torch_tensor(next(self.repr_dataset())),
+                                       check_trace=True)
+        self.exported_model = torch.jit.script(torch_traced)
+        Logger.info(f"Exporting PyTorch torch script Model: {self.save_model_path}")
+        torch.jit.save(self.exported_model, self.save_model_path)
 
-        Logger.info(f"Exporting PyTorch fake quant onnx model: {self.save_model_path}")
 
-        torch.onnx.export(self.model,
-                          model_input,
-                          self.save_model_path,
-                          opset_version=OPSET_VERSION,
-                          verbose=False,
-                          input_names=['input'],
-                          output_names=['output'],
-                          dynamic_axes={'input': {0: 'batch_size'},
-                                        'output': {0: 'batch_size'}})
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,62 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import os
+import tempfile
 from typing import Callable
 
-import torch.nn
+import keras.models
+import tensorflow as tf
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
-from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.load_model import keras_load_quantized_model
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
 
 
-class FakelyQuantTorchScriptPyTorchExporter(BasePyTorchExporter):
+class FakelyQuantTFLiteExporter(FakelyQuantKerasExporter):
     """
-    Exporter for fakely-quant PyTorch models.
+    Exporter for fakely-quant TFLite models.
     The exporter expects to receive an exportable model (where each layer's full quantization parameters
     can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
     format) and fake-quant layers for the activations.
     """
 
     def __init__(self,
-                 model: torch.nn.Module,
+                 model: keras.models.Model,
                  is_layer_exportable_fn: Callable,
-                 save_model_path: str,
-                 repr_dataset: Callable):
+                 save_model_path: str):
         """
 
         Args:
             model: Model to export.
             is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
             save_model_path: Path to save the exported model.
-            repr_dataset: Representative dataset (needed for creating torch script).
         """
-
         super().__init__(model,
                          is_layer_exportable_fn,
-                         save_model_path,
-                         repr_dataset)
+                         save_model_path)
+
+        self.exported_model = None
 
-    def export(self) -> None:
+    def export(self):
         """
-        Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
+        Convert an exportable (fully-quantized) Keras model to a fakely-quant TFLite model
         (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
-        Returns:
-            Fake-quant PyTorch model.
         """
-        for layer in self.model.children():
-            assert self.is_layer_exportable_fn(layer), f'Layer {layer} is not exportable.'
-
-        torch_traced = torch.jit.trace(self.model,
-                                       to_torch_tensor(next(self.repr_dataset())),
-                                       check_trace=True)
-        self.exported_model = torch.jit.script(torch_traced)
-        Logger.info(f"Exporting PyTorch torch script Model: {self.save_model_path}")
-        torch.jit.save(self.exported_model, self.save_model_path)
-
-
+        # Use Keras exporter to quantize model's weights before converting it to TFLite.
+        # Since exporter saves the model, we use a tmp path for saving, and then we delete it.
+        _, tmp_h5_file = tempfile.mkstemp('.h5')
+        custom_objects = FakelyQuantKerasExporter(self.model,
+                                                  self.is_layer_exportable_fn,
+                                                  tmp_h5_file).export()
+
+        model = keras_load_quantized_model(tmp_h5_file)
+        os.remove(tmp_h5_file)
+
+        self.exported_model = tf.lite.TFLiteConverter.from_keras_model(model).convert()
+        Logger.info(f'Exporting FQ tflite model to: {self.save_model_path}')
+        with open(self.save_model_path, 'wb') as f:
+            f.write(self.exported_model)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from enum import Enum
 from typing import Callable
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
 
 
 class PyTorchExportMode(Enum):
     FAKELY_QUANT_TORCHSCRIPT = 0
     FAKELY_QUANT_ONNX = 1
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,64 +8,66 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-import os
-import tempfile
+from enum import Enum
 from typing import Callable
 
-import keras.models
-import tensorflow as tf
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.load_model import keras_load_quantized_model
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
-
-
-class FakelyQuantTFLiteExporter(FakelyQuantKerasExporter):
-    """
-    Exporter for fakely-quant TFLite models.
-    The exporter expects to receive an exportable model (where each layer's full quantization parameters
-    can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
-    format) and fake-quant layers for the activations.
-    """
-
-    def __init__(self,
-                 model: keras.models.Model,
-                 is_layer_exportable_fn: Callable,
-                 save_model_path: str):
+
+class TFLiteExportMode(Enum):
+    FAKELY_QUANT = 0
+    INT8 = 1
+
+if FOUND_TF:
+    import keras
+    from model_compression_toolkit.exporter.model_exporter.tflite.fakely_quant_tflite_exporter import FakelyQuantTFLiteExporter
+    from model_compression_toolkit.exporter.model_exporter.tflite.int8_tflite_exporter import INT8TFLiteExporter
+    from model_compression_toolkit.exporter.model_wrapper.keras.validate_layer import is_keras_layer_exportable
+
+    def tflite_export_model(model: keras.models.Model,
+                            save_model_path: str,
+                            mode: TFLiteExportMode = TFLiteExportMode.FAKELY_QUANT,
+                            is_layer_exportable_fn: Callable = is_keras_layer_exportable
+                            ):
         """
+        Export a Keras quantized model to a tflite model.
+        The model will be saved to the path in save_model_path.
+        Mode can be used for different exported files. Currently, tflite_export_model
+        supports TFLiteExportMode.FAKELY_QUANT (where weights and activations are
+        float fakely-quantized values), and TFLiteExportMode.INT8 (where weights
+        and activations are represented using 8bits integers).
 
         Args:
             model: Model to export.
             is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
-            save_model_path: Path to save the exported model.
-        """
-        super().__init__(model,
-                         is_layer_exportable_fn,
-                         save_model_path)
+            mode: Mode to export the model according to.
+            save_model_path: Path to save the model.
 
-        self.exported_model = None
-
-    def export(self):
         """
-        Convert an exportable (fully-quantized) Keras model to a fakely-quant TFLite model
-        (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
-        """
-        # Use Keras exporter to quantize model's weights before converting it to TFLite.
-        # Since exporter saves the model, we use a tmp path for saving, and then we delete it.
-        _, tmp_h5_file = tempfile.mkstemp('.h5')
-        custom_objects = FakelyQuantKerasExporter(self.model,
-                                                  self.is_layer_exportable_fn,
-                                                  tmp_h5_file).export()
-
-        model = keras_load_quantized_model(tmp_h5_file)
-        os.remove(tmp_h5_file)
-
-        self.exported_model = tf.lite.TFLiteConverter.from_keras_model(model).convert()
-        Logger.info(f'Exporting FQ tflite model to: {self.save_model_path}')
-        with open(self.save_model_path, 'wb') as f:
-            f.write(self.exported_model)
+        if mode == TFLiteExportMode.FAKELY_QUANT:
+            exporter = FakelyQuantTFLiteExporter(model,
+                                                 is_layer_exportable_fn,
+                                                 save_model_path)
+        elif mode == TFLiteExportMode.INT8:
+            exporter = INT8TFLiteExporter(model,
+                                          is_layer_exportable_fn,
+                                          save_model_path)
+
+        else:
+            Logger.critical(
+                f'Unsupported mode was used {mode.name} to export TFLite model.'
+                f' Please see API for supported modes.')  # pragma: no cover
+
+        exporter.export()
+
+else:
+    def tflite_export_model(*args, **kwargs):
+        Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+                     'when using tflite_export_model. '
+                     'Could not find some or all of TensorFlow packages.')  # pragma: no cover
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import numpy as np
 import tensorflow as tf
 from keras import Sequential
 from keras.layers import Dense, Conv2D, Reshape
 from keras.models import clone_model
 
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
     constants as keras_inferable_constants
 
 BIAS_INITIALIZER = 'bias_initializer'
 BIAS_REGULARIZER = 'bias_regularizer'
 BIAS_CONSTRAINT = 'bias_constraint'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 from typing import Tuple
 
 
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Graph, Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.core.common import Graph
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.core.common.user_info import UserInformation
+from model_compression_toolkit.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.keras.layers import Layer
     from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
     from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizers import get_quantization_quantizers
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any
 
-from model_compression_toolkit.core.common import BaseNode, Logger
-from model_compression_toolkit.core.common.constants import THRESHOLD, RANGE_MIN, RANGE_MAX, SIGNED, CLUSTER_CENTERS, SCALE_PER_CHANNEL
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.core.common import BaseNode
+from model_compression_toolkit.constants import THRESHOLD, RANGE_MIN, RANGE_MAX, SIGNED, CLUSTER_CENTERS, SCALE_PER_CHANNEL
+
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import get_inferable_quantizer_class
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import constants as qi_keras_consts
 
 def get_inferable_quantizer_kwargs(node: BaseNode,
                                    quantization_target: QuantizationTarget) -> Dict[str, Any]:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer
 
 
 if FOUND_TF:
     from keras.engine.input_layer import InputLayer
     from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Graph, Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.core.common import Graph
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
 
 if FOUND_TORCH:
     import torch
     from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
     from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.node_to_quantizers import \
         get_quantization_quantizers
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Dict, Any
 
-from model_compression_toolkit.core.common import BaseNode, Logger
-from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX, \
+from model_compression_toolkit.core.common import BaseNode
+from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX, \
     SCALE_PER_CHANNEL, CLUSTER_CENTERS
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
     get_inferable_quantizer_class
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     constants as qi_inferable_quantizers_constants, BasePyTorchInferableQuantizer
 import numpy as np
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
         BasePyTorchInferableQuantizer
     def is_pytorch_layer_exportable(layer: Any) -> bool:
         """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Tuple, List
 
-from model_compression_toolkit import FrameworkInfo
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.core import FrameworkInfo
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 def get_compare_points(input_graph: Graph) -> Tuple[List[BaseNode], List[str], List, List]:
     """
     Create a list of nodes with weights in a graph and a corresponding list
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # limitations under the License.
 # ==============================================================================
 import copy
 from abc import ABC, abstractmethod
 import numpy as np
 from typing import Callable, List, Any
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
-from model_compression_toolkit.core.common import Graph, Logger, BaseNode
+from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.gptq.common.gptq_constants import QUANT_PARAM_LEARNING_STR
 from model_compression_toolkit.gptq.common.gptq_graph import get_compare_points
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
+from model_compression_toolkit.logger import Logger
 
 
 class GPTQTrainer(ABC):
     """
     Abstract GPTQ training class for fine-tuning a quantized model
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 from packaging import version
 
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.keras.quantizer.quantization_builder import quantization_builder
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
 else:
     from keras.engine.base_layer import TensorFlowOpLayer
 
@@ -101,15 +102,15 @@
         self.optimizer_with_param = self.get_optimizer_with_param(flattened_trainable_weights,
                                                                   flattened_bias_weights,
                                                                   trainable_quantization_parameters)
         self.has_params_to_train = np.sum(
             [len(optimizer_params_tuple[1]) for optimizer_params_tuple in self.optimizer_with_param]) > 0
 
         if self.float_user_info.input_scale != self.gptq_user_info.input_scale:
-            common.Logger.error("Input scale mismatch between float and GPTQ networks")  # pragma: no cover
+            Logger.error("Input scale mismatch between float and GPTQ networks")  # pragma: no cover
         else:
             self.input_scale = self.gptq_user_info.input_scale
 
         self.weights_for_average_loss = self.compute_hessian_based_weights(representative_data_gen)
 
         self.reg_func = get_regularization(self.gptq_config, representative_data_gen)
 
@@ -122,15 +123,15 @@
             node (BaseNode): Node for quantization decision
 
         Returns:
             A boolean whether the layer is to be wrapped with a QuantizeWrapper
         """
 
         if node.is_weights_quantization_enabled() and not self.fw_info.is_kernel_op(node.type):
-            common.Logger.error(f"GPTQ Error: Quantizing node {node.name} of type {node.type} "
+            Logger.error(f"GPTQ Error: Quantizing node {node.name} of type {node.type} "
                                 f"without a kernel isn't supported")
         return node.is_weights_quantization_enabled()
 
     def gptq_wrapper(self, n: common.BaseNode, layer: Layer) -> Union[qi.KerasQuantizationWrapper, Layer]:
         """
         A function which takes a computational graph node and a keras layer and perform the quantization wrapping.
 
@@ -276,15 +277,15 @@
                 # the value of the variables to minimize the loss.
                 for i, (o, p) in enumerate(in_optimizer_with_param):
                     o.apply_gradients(zip(grads[i], p))
                 if self.gptq_config.log_function is not None:
                     self.gptq_config.log_function(loss_value_step, grads[0], in_optimizer_with_param[0][-1],
                                                   self.compare_points)
                 self.loss_list.append(loss_value_step.numpy())
-                common.Logger.debug(f'last loss value: {self.loss_list[-1]}')
+                Logger.debug(f'last loss value: {self.loss_list[-1]}')
 
     def update_graph(self):
         """
         Update a graph using GPTQ after minimizing the loss between the float model's output
         and the quantized model's outputs.
         Returns:
             Updated graph after GPTQ.
@@ -293,15 +294,15 @@
 
         for layer in self.fxp_model.layers:
             if isinstance(layer, KerasQuantizationWrapper):
                 node = graph.find_node_by_name(layer.layer.name)
                 if len(node) == 0 and isinstance(layer.layer, TensorFlowOpLayer):
                     node = graph.find_node_by_name('_'.join(layer.layer.name.split('_')[3:]))
                 if len(node) != 1:
-                    common.Logger.error(f"Can't update GPTQ graph due to missing layer named: {layer.layer.name}")
+                    Logger.error(f"Can't update GPTQ graph due to missing layer named: {layer.layer.name}")
                 node = node[0]
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=node.type,
                                                                       fw_info=self.fw_info)
                 weights, weight_quant_config, activation_quant_config = \
                     layer.weights_quantizers[kernel_attribute].update_layer_quantization_params(layer)
                 for weight_attr, weight in weights.items():
                     node.set_weights_by_keys(weight_attr, weight.numpy())
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,44 +12,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable, Tuple
 from packaging import version
 
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import TENSORFLOW
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
-    MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import MixedPrecisionQuantizationConfigV2
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.gptq.runner import gptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 
 LR_DEFAULT = 0.15
 LR_REST_DEFAULT = 1e-4
 LR_BIAS_DEFAULT = 1e-4
 LR_QUANTIZATION_PARAM_DEFAULT = 1e-3
 GPTQ_MOMENTUM = 0.9
 
-if common.constants.FOUND_TF:
+if FOUND_TF:
     import tensorflow as tf
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
-    from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
+    from model_compression_toolkit.gptq.keras.gptq_keras_implementation import GPTQKerasImplemantation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from tensorflow.keras.models import Model
     from model_compression_toolkit.gptq.keras.gptq_loss import GPTQMultipleTensorsLoss
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.exporter.model_wrapper import get_exportable_keras_model
     from model_compression_toolkit import get_target_platform_capabilities
 
     # As from TF2.9 optimizers package is changed
     if version.parse(tf.__version__) < version.parse("2.9"):
         from keras.optimizer_v2.optimizer_v2 import OptimizerV2
     else:
@@ -58,24 +56,26 @@
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
 
     def get_keras_gptq_config(n_epochs: int,
                               optimizer: OptimizerV2 = tf.keras.optimizers.Adam(learning_rate=LR_DEFAULT),
                               optimizer_rest: OptimizerV2 = tf.keras.optimizers.Adam(learning_rate=LR_REST_DEFAULT),
                               loss: Callable = GPTQMultipleTensorsLoss(),
-                              log_function: Callable = None) -> GradientPTQConfigV2:
+                              log_function: Callable = None,
+                              use_hessian_based_weights: bool = True) -> GradientPTQConfigV2:
         """
         Create a GradientPTQConfigV2 instance for Keras models.
 
         args:
             n_epochs (int): Number of epochs for running the representative dataset for fine-tuning.
             optimizer (OptimizerV2): Keras optimizer to use for fine-tuning for auxiliry variable with a default learning rate set to 0.2.
             optimizer_rest (OptimizerV2): Keras optimizer to use for fine-tuning of the bias variable.
             loss (Callable): loss to use during fine-tuning. should accept 4 lists of tensors. 1st list of quantized tensors, the 2nd list is the float tensors, the 3rd is a list of quantized weights and the 4th is a list of float weights.
             log_function (Callable): Function to log information about the gptq process.
+            use_hessian_based_weights (bool): Whether to use Hessian-based weights for weighted average loss.
 
         returns:
             a GradientPTQConfigV2 object to use when fine-tuning the quantized model using gptq.
 
         Examples:
 
             Import MCT and TensorFlow:
@@ -90,17 +90,24 @@
             Other Tensorflow optimizers can be passed:
 
             >>> gptq_conf = mct.gptq.get_keras_gptq_config(n_epochs=3, optimizer=tf.keras.optimizers.Nadam())
 
             The configuration can be passed to :func:`~model_compression_toolkit.keras_post_training_quantization` in order to quantize a keras model using gptq.
 
         """
-        bias_optimizer = tf.keras.optimizers.SGD(learning_rate=LR_BIAS_DEFAULT, momentum=GPTQ_MOMENTUM)
-        return GradientPTQConfigV2(n_epochs, optimizer, optimizer_rest=optimizer_rest, loss=loss,
-                                   log_function=log_function, train_bias=True, optimizer_bias=bias_optimizer)
+        bias_optimizer = tf.keras.optimizers.SGD(learning_rate=LR_BIAS_DEFAULT,
+                                                 momentum=GPTQ_MOMENTUM)
+        return GradientPTQConfigV2(n_epochs,
+                                   optimizer,
+                                   optimizer_rest=optimizer_rest,
+                                   loss=loss,
+                                   log_function=log_function,
+                                   train_bias=True,
+                                   optimizer_bias=bias_optimizer,
+                                   use_hessian_based_weights=use_hessian_based_weights)
 
 
     def keras_gradient_post_training_quantization_experimental(in_model: Model,
                                                                representative_data_gen: Callable,
                                                                gptq_config: GradientPTQConfigV2,
                                                                gptq_representative_data_gen: Callable = None,
                                                                target_kpi: KPI = None,
@@ -154,28 +161,28 @@
             >>> num_calibration_batches = 10
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 224, 224, 3))]
 
             Create an MCT core config, containing the quantization configuration:
 
-            >>> config = mct.CoreConfig()
+            >>> config = mct.core.CoreConfig()
 
             If mixed precision is desired, create an MCT core config with a mixed-precision configuration, to quantize a model
             with different bitwidths for different layers.
             The candidates bitwidth for quantization should be defined in the target platform model:
 
-            >>> config = mct.CoreConfig(mixed_precision_config=mct.MixedPrecisionQuantizationConfigV2(num_of_images=1))
+            >>> config = mct.core.CoreConfig(mixed_precision_config=mct.core.MixedPrecisionQuantizationConfigV2(num_of_images=1))
 
             For mixed-precision set a target KPI object:
             Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
             that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
             while the bias will not):
 
-            >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+            >>> kpi = mct.core.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
             Create GPTQ config:
 
             >>> gptq_config = mct.gptq.get_keras_gptq_config(n_epochs=1)
 
             Pass the model with the representative dataset generator to get a quantized model:
 
@@ -183,23 +190,23 @@
 
         """
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization "
                                     "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
         tb_w = _init_tensorboard_writer(fw_info)
 
-        fw_impl = KerasImplementation()
+        fw_impl = GPTQKerasImplemantation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
                                             representative_data_gen=representative_data_gen,
                                             core_config=core_config,
                                             fw_info=fw_info,
                                             fw_impl=fw_impl,
                                             tpc=target_platform_capabilities,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import model_compression_toolkit.gptq.keras.quantizer.ste_rounding.symmetric_ste
 import model_compression_toolkit.gptq.keras.quantizer.soft_rounding.symmetric_soft_quantizer
+import model_compression_toolkit.gptq.keras.quantizer.soft_rounding.uniform_soft_quantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import abstractmethod
 from typing import Union, Dict, List
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.gptq.common.gptq_constants import WEIGHTS_QUANTIZATION_PARAMS
 
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer
 
 if FOUND_TF:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import tensorflow as tf
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD
 from typing import Tuple
 
 
 def ste_ceil(x: tf.Tensor) -> tf.Tensor:
     """
     Return the ceil values of a tensor.
     """
     error = tf.stop_gradient(tf.math.ceil(x) - x)
     return error + x
 
 
+def ste_floor(x: tf.Tensor) -> tf.Tensor:
+    """
+    Return the floor values of a tensor.
+    """
+    error = tf.stop_gradient(tf.math.floor(x) - x)
+    return error + x
+
+
 def safe_log(x: tf.Tensor, eps: float) -> tf.Tensor:
     """
     Computes log function of x unless x is smaller than some small value, so the log function would not fail.
 
     Args:
         x: input variable.
         eps: limit value.
@@ -68,14 +76,23 @@
                     signed: bool) -> tf.Tensor:
     """
     Compute the step size for the quantization.
     """
     return max_tensor / (2 ** (num_bits - int(signed)))
 
 
+def calculate_delta_uniform(min_tensor: tf.Tensor,
+                            max_tensor: tf.Tensor,
+                            num_bits: int) -> tf.Tensor:
+    """
+    Compute the step size for the uniform quantization.
+    """
+    return (max_tensor-min_tensor) / (2 ** num_bits - 1)
+
+
 def ste_clip(x: [tf.Tensor, tf.Variable], max_val=1, min_val=None) -> tf.Tensor:
     """
     clip a variable between fixed values such that min_val<=output<=max_val
     Args:
         x: input variable
         max_val: maximum value for clipping
         min_val: minimum value for clipping (defaults to -max_val)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,40 +73,38 @@
 
         Args:
             total_gradient_steps: The number of gradient steps during optimization.
         """
         # Initializing the temperature decay according to the number of expected gradient steps
         self.linear_decay = LinearTempDecay(total_gradient_steps)
 
-        self.count_iter = 0
+        self.count_iter = tf.Variable(0.)
 
 
     def __call__(self, model: Model, entropy_reg: float):
         """
         Returns the soft quantizer regularization value for SoftRounding.
 
         Args:
             model: A model to be quantized with SoftRounding.
             entropy_reg: Entropy value to scale the quantizer regularization.
 
         Returns: Regularization value.
         """
-
         soft_reg_aux: List[tf.Tensor] = []
+        b = self.linear_decay(self.count_iter.value())
         for layer in model.layers:
             if isinstance(layer, KerasQuantizationWrapper):
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
                                                                       fw_info=DEFAULT_KERAS_INFO)
 
                 st = layer.weights_quantizers[kernel_attribute].get_soft_targets()
-                b = self.linear_decay(self.count_iter)
-
                 soft_reg_aux.append(tf.reduce_sum(1 - tf.pow(tf.math.abs(st - .5) * 2, b)))
 
         reg = 0
 
         for sq in soft_reg_aux:
             reg += sq
 
-        self.count_iter += 1
+        self.count_iter.assign_add(1.0)
 
         return entropy_reg * reg
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import tensorflow as tf
 import numpy as np
 
 from model_compression_toolkit.gptq import RoundingType
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common import max_power_of_two
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
     SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
 from typing import Dict, Any
-from model_compression_toolkit.core.common.constants import THRESHOLD, MIN_THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD, MIN_THRESHOLD
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.gptq.keras.quantizer.quant_utils import power_of_two_max, clip, calculate_delta
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from typing import Dict, Any
 
 import numpy as np
 import tensorflow as tf
 
 from model_compression_toolkit.gptq import RoundingType
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
-from model_compression_toolkit.core.common.constants import THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Callable, List, Tuple, Union
 
 import numpy as np
 from torch.nn import Module
 from tqdm import tqdm
 import copy
 import torch
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.common.gptq_training import GPTQTrainer
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import PYTORCH
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import PYTORCH
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.gptq.keras.quantization_facade import GPTQ_MOMENTUM
 from model_compression_toolkit.gptq.runner import gptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
 
 LR_DEFAULT = 1e-4
 LR_REST_DEFAULT = 1e-4
 LR_BIAS_DEFAULT = 1e-4
 LR_QUANTIZATION_PARAM_DEFAULT = 1e-4
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
-    from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
-    from model_compression_toolkit.core.pytorch.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.gptq.pytorch.gptq_pytorch_implementation import GPTQPytorchImplemantation
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.gptq.pytorch.gptq_loss import multiple_tensors_mse_loss
     from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
     import torch
     from torch.nn import Module
     from torch.optim import Adam, Optimizer
     from model_compression_toolkit import get_target_platform_capabilities
 
@@ -114,15 +114,15 @@
         Args:
             model (Module): Pytorch model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
             core_config (CoreConfig): Configuration object containing parameters of how the model should be quantized, including mixed precision parameters.
             gptq_config (GradientPTQConfigV2): Configuration for using gptq (e.g. optimizer).
             gptq_representative_data_gen (Callable): Dataset used for GPTQ training. If None defaults to representative_data_gen
-            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to. `Default PyTorch TPC <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/tpc_models/pytorch_tp_models/pytorch_default.py>`_
+            target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
             new_experimental_exporter (bool): Whether exporting the quantized model using new exporter or not (in progress. Avoiding it for now is recommended).
 
         Returns:
             A quantized module and information the user may need to handle the quantized module.
 
         Examples:
 
@@ -138,34 +138,34 @@
             >>> num_calibration_batches = 10
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 3, 224, 224))]
 
             Create MCT core configurations with number of calibration iterations set to 1:
 
-            >>> config = mct.CoreConfig()
+            >>> config = mct.core.CoreConfig()
 
             Pass the module, the representative dataset generator and the configuration (optional) to get a quantized module
 
             >>> quantized_module, quantization_info = mct.gptq.pytorch_gradient_post_training_quantization_experimental(module, repr_datagen, core_config=config, gptq_config=gptq_conf)
 
         """
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization "
                                     "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(DEFAULT_PYTORCH_INFO)
 
-        fw_impl = PytorchImplementation()
+        fw_impl = GPTQPytorchImplemantation()
 
         # ---------------------- #
         # Core Runner
         # ---------------------- #
         graph, bit_widths_config = core_runner(in_model=model,
                                                representative_data_gen=representative_data_gen,
                                                core_config=core_config,
@@ -188,15 +188,15 @@
         # ---------------------- #
         # Export
         # ---------------------- #
         if new_experimental_exporter:
             Logger.warning('Using new experimental exported models. '
                            'Please do not use unless you are familiar with what you are doing')
 
-            return get_fully_quantized_pytorch_model(graph_gptq)
+            return get_exportable_pytorch_model(graph_gptq)
 
         return export_model(graph_gptq,
                             DEFAULT_PYTORCH_INFO,
                             fw_impl,
                             tb_w,
                             bit_widths_config)
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import abstractmethod
-from typing import Union, Dict, List
+from typing import Union, Dict
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.gptq.common.gptq_constants import WEIGHTS_QUANTIZATION_PARAMS
 
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import \
     BaseTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union, Tuple
 import torch
-from torch.nn.functional import softmax, log_softmax, one_hot
-from model_compression_toolkit.core.common.constants import MIN_THRESHOLD
-from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
+from model_compression_toolkit.constants import MIN_THRESHOLD
 
 
 def power_of_two_max(max_tensor: torch.Tensor) -> torch.Tensor:
     """
     Compute the power of two threshold for a tensor.
     """
     return torch.pow(2, ste_ceil(torch.log2(torch.clip(max_tensor, min=MIN_THRESHOLD, max=torch.inf))))
@@ -47,14 +45,21 @@
 def ste_ceil(x: torch.Tensor) -> torch.Tensor:
     """
     Return the ceil values of a tensor.
     """
     return (torch.ceil(x) - x).detach() + x
 
 
+def ste_floor(x: torch.Tensor) -> torch.Tensor:
+    """
+    Return the floor values of a tensor.
+    """
+    return (torch.floor(x) - x).detach() + x
+
+
 def ste_round(x: torch.Tensor) -> torch.Tensor:
     """
     Calculate the rounded values of a tensor
     Args:
         x: input variable
     Returns:
         rounded value
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,22 +91,21 @@
             model: A model to be quantized with SoftRounding.
             entropy_reg: Entropy value to scale the quantizer regularization.
 
         Returns: Regularization value.
         """
 
         soft_reg_aux: List[torch.Tensor] = []
+        b = self.linear_decay(self.count_iter)
         for layer in model.modules():
             if isinstance(layer, PytorchQuantizationWrapper):
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
                                                                       fw_info=DEFAULT_PYTORCH_INFO)
 
                 st = layer.weights_quantizers[kernel_attribute].get_soft_targets()
-                b = self.linear_decay(self.count_iter)
-
                 soft_reg_aux.append((1 - torch.pow(torch.abs(st - .5) * 2, b)).sum())
 
         reg = 0
 
         for sq in soft_reg_aux:
             reg += sq
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 
 from model_compression_toolkit.core.common import max_power_of_two
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
     SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
-from model_compression_toolkit.core.common.constants import THRESHOLD, MIN_THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD, MIN_THRESHOLD
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 # ==============================================================================
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.pytorch.quantizer.quant_utils import fix_range_to_include_zero
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
     mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import \
     VariableGroup
-from model_compression_toolkit.core.common.constants import RANGE_MAX, RANGE_MIN
-from model_compression_toolkit.qat.common.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.constants import RANGE_MAX, RANGE_MIN
+
 
 def soft_rounding_unifrom_quantizer(input_tensor: torch.Tensor,
                                     auxvar_tensor: torch.Tensor,
                                     min_range: torch.Tensor,
                                     max_range: torch.Tensor,
                                     num_bits: int) -> torch.Tensor:
     """
@@ -50,21 +51,20 @@
         num_bits: Num of bits to use.
 
     Returns:
         A quantized tensor.
     """
     # adjusts the quantization range so the quantization grid includes zero.
     min_range, max_range = fix_range_to_include_zero(min_range, max_range, num_bits)
-    delta = qutils.calculate_delta_uniform(max_range, min_range, num_bits)
-    with torch.no_grad():
-        input_tensor_int = torch.floor(input_tensor / delta)
+    delta = qutils.calculate_delta_uniform(min_range, max_range, num_bits)
+    input_tensor_int = qutils.ste_floor((input_tensor - min_range) / delta)
     tensor_q = input_tensor_int + auxvar_tensor
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=0,
-                                   max_val=2 ** num_bits - 1)
+                                   max_val=2 ** num_bits - 1) + min_range
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=RoundingType.SoftQuantizer)
 class UniformSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
@@ -118,26 +118,25 @@
             min_values = torch.tensor(self.min_values)
             max_values = torch.tensor(self.max_values)
 
         layer.register_parameter(name+"_"+FQ_MIN, nn.Parameter(min_values, requires_grad=self.quantization_parameter_learning))
         layer.register_parameter(name+"_"+FQ_MAX, nn.Parameter(max_values, requires_grad=self.quantization_parameter_learning))
 
         w = layer.layer.weight
-        delta = qutils.calculate_delta_uniform(max_values, min_values, self.num_bits)
-        w_clipped_normed = torch.clip(w / delta, 0, 2 ** self.num_bits - 1)
+        delta = qutils.calculate_delta_uniform(min_values, max_values, self.num_bits)
+        w_clipped_normed = torch.clip((w - min_values) / delta, 0, 2 ** self.num_bits - 1)
         rest = w_clipped_normed - torch.floor(w_clipped_normed)  # rest of rounding [0, 1)
         alpha = -torch.log((self.zeta - self.gamma) / (rest - self.gamma) - 1)  # => sigmoid(alpha) = rest
         layer.register_parameter(f"{name}_{AUXVAR}", nn.Parameter(alpha, requires_grad=True))
 
         # Save the quantizer parameters
         self.add_quantizer_variable(FQ_MIN, layer.get_parameter(name+"_"+FQ_MIN), VariableGroup.QPARAMS)
         self.add_quantizer_variable(FQ_MAX, layer.get_parameter(name+"_"+FQ_MAX), VariableGroup.QPARAMS)
         self.add_quantizer_variable(AUXVAR, layer.get_parameter(f"{name}_{AUXVAR}"), VariableGroup.WEIGHTS)
 
-
     def get_soft_targets(self) -> torch.Tensor:
         """
         Computes the rectified sigmoid function for the quantization target parameters.
 
         Returns:
             A tensor with the soft rounding targets values.
 
@@ -188,9 +187,8 @@
         #####################################################
         q_tensor = soft_rounding_unifrom_quantizer(input_tensor=inputs,
                                                    auxvar_tensor=aux_var,
                                                    min_range=min_range,
                                                    max_range=max_range,
                                                    num_bits=self.num_bits)
 
-
         return q_tensor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD, MAX_LSB_CHANGE
-from model_compression_toolkit.core.common.constants import THRESHOLD
+from model_compression_toolkit.constants import THRESHOLD
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
     mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable
 
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.statistics_correction.statistics_correction import \
     apply_statistics_correction
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.gptq.common.gptq_training import gptq_training
 
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import TensorboardWriter
 from model_compression_toolkit.core.common.statistics_correction.apply_bias_correction_to_graph import \
     apply_bias_correction_to_graph
+from model_compression_toolkit.logger import Logger
 
 
 def _apply_gptq(gptq_config: GradientPTQConfigV2,
                 representative_data_gen: Callable,
                 tb_w: TensorboardWriter,
                 tg: Graph,
                 tg_bias: Graph,
@@ -51,15 +52,15 @@
         tg_bias: Graph of quantized model.
         fw_info: Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.).
         fw_impl: Framework implementation per framework
     Returns:
 
     """
     if gptq_config is not None and gptq_config.n_epochs > 0:
-        common.Logger.info("Using experimental Gradient Based PTQ: If you encounter an issue "
+        Logger.info("Using experimental Gradient Based PTQ: If you encounter an issue "
                            "please file a bug. To disable it, do not pass a gptq configuration.")
 
         tg_bias = gptq_training(tg,
                                 tg_bias,
                                 gptq_config,
                                 representative_data_gen,
                                 fw_impl,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable
 
-from model_compression_toolkit import CoreConfig
-from model_compression_toolkit.core import common
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import TENSORFLOW, FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 
 if FOUND_TF:
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from tensorflow.keras.models import Model
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.exporter.model_wrapper import get_exportable_keras_model
 
     from model_compression_toolkit import get_target_platform_capabilities
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
 
     def keras_post_training_quantization_experimental(in_model: Model,
@@ -89,50 +88,50 @@
             >>> num_calibration_batches = 10
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 224, 224, 3))]
 
             Create a MCT core config, containing the quantization configuration:
 
-            >>> config = mct.CoreConfig()
+            >>> config = mct.core.CoreConfig()
 
             If mixed precision is desired, create a MCT core config with a mixed-precision configuration, to quantize a model with different bitwidths for different layers.
             The candidates bitwidth for quantization should be defined in the target platform model.
             In this example we use 1 image to search mixed-precision configuration:
 
-            >>> config = mct.CoreConfig(mixed_precision_config=mct.MixedPrecisionQuantizationConfigV2(num_of_images=1))
+            >>> config = mct.core.CoreConfig(mixed_precision_config=mct.core.MixedPrecisionQuantizationConfigV2(num_of_images=1))
 
             For mixed-precision set a target KPI object:
             Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
             that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
             while the bias will not):
 
-            >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+            >>> kpi = mct.core.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
             Pass the model, the representative dataset generator, the configuration and the target KPI to get a
             quantized model:
 
-            >>> quantized_model, quantization_info = mct.keras_post_training_quantization_experimental(model, repr_datagen, kpi, core_config=config)
+            >>> quantized_model, quantization_info = mct.ptq.keras_post_training_quantization_experimental(model, repr_datagen, kpi, core_config=config)
 
             For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/api_docs/modules/mixed_precision_quantization_config.html>`_.
 
          """
 
         fw_info = DEFAULT_KERAS_INFO
 
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization "
                                     "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(fw_info)
 
         fw_impl = KerasImplementation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
 
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import PYTORCH, FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import PYTORCH, FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
 
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
-    from model_compression_toolkit.core.pytorch.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from torch.nn import Module
     from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
     from model_compression_toolkit import get_target_platform_capabilities
 
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
     def pytorch_post_training_quantization_experimental(in_module: Module,
@@ -84,26 +84,26 @@
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 3, 224, 224))]
 
             Import MCT and pass the module with the representative dataset generator to get a quantized module
             Set number of clibration iterations to 1:
 
             >>> import model_compression_toolkit as mct
-            >>> quantized_module, quantization_info = mct.pytorch_post_training_quantization_experimental(module, repr_datagen)
+            >>> quantized_module, quantization_info = mct.ptq.pytorch_post_training_quantization_experimental(module, repr_datagen)
 
         """
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use "
                                     "pytorch_post_training_quantization API, or pass a valid mixed precision "
                                     "configuration.")  # pragma: no cover
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(DEFAULT_PYTORCH_INFO)
 
         fw_impl = PytorchImplementation()
 
         tg, bit_widths_config = core_runner(in_model=in_module,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,27 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.qat.common.constants import THRESHOLD_TENSOR, WEIGHTS_QUANTIZATION_PARAMS
+# TP Model constants
+OPS_SET_LIST = 'ops_set_list'
+
+# Version
+LATEST = 'latest'
+
+
+# Supported TP models names:
+DEFAULT_TP_MODEL = 'default'
+IMX500_TP_MODEL = 'imx500'
+TFLITE_TP_MODEL = 'tflite'
+QNNPACK_TP_MODEL = 'qnnpack'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,13 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
-
-FQ_MIN = "min"
-FQ_MAX = "max"
-THRESHOLD_TENSOR = "ptq_threshold_tensor"
-WEIGHTS_QUANTIZATION_PARAMS = 'weights_quantization_params'
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/qat_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 # limitations under the License.
 # ==============================================================================
 
 from typing import Dict
 from enum import Enum
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
+from model_compression_toolkit.logger import Logger
+
 
 def _is_qat_applicable(node: common.BaseNode,
                        fw_info: FrameworkInfo) -> bool:
     """
     A function for deciding if a layer should be fine-tuned during QAT
     Args:
         node (BaseNode): Node for quantization decision
         fw_info (FrameworkInfo): Pytorch quantization information
 
     Returns:
         A boolean whether the layer is to be wrapped with a QuantizeWrapper
     """
 
     if node.is_weights_quantization_enabled() and not fw_info.is_kernel_op(node.type):
-        common.Logger.error("QAT Error: Quantizing a node without a kernel isn't supported")
+        Logger.error("QAT Error: Quantizing a node without a kernel isn't supported")
     return node.is_weights_quantization_enabled() or node.is_activation_quantization_enabled()
 
 
 class TrainingMethod(Enum):
     """
     An enum for selecting a QAT training method
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,48 +12,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Callable
 from functools import partial
 
-from model_compression_toolkit import CoreConfig
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import TENSORFLOW, FOUND_TF
-from model_compression_toolkit.core.common.framework_info import FrameworkInfo
+from model_compression_toolkit.core import CoreConfig
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.keras.layers import Layer
     from tensorflow.keras.models import Model
 
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
 
     from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 
     from model_compression_toolkit import get_target_platform_capabilities
     from model_compression_toolkit import quantizers_infrastructure as qi
 
     from model_compression_toolkit import get_target_platform_capabilities
     from model_compression_toolkit.core import common
     from model_compression_toolkit.core.common import BaseNode
-    from model_compression_toolkit.core.common.constants import TENSORFLOW
+    from model_compression_toolkit.constants import TENSORFLOW
     from model_compression_toolkit.core.common.framework_info import FrameworkInfo
     from model_compression_toolkit.qat.common.qat_config import _is_qat_applicable
-    from model_compression_toolkit.core.keras.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.qat.keras.quantizer.quantization_builder import quantization_builder
     from model_compression_toolkit.qat.common.qat_config import QATConfig
     from model_compression_toolkit import quantizers_infrastructure as qi
 
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
@@ -130,50 +128,50 @@
              >>> num_calibration_batches = 10
              >>> def repr_datagen():
              >>>     for _ in range(num_calibration_batches):
              >>>         yield [np.random.random((4, 224, 224, 3))]
 
              Create a MCT core config, containing the quantization configuration:
 
-             >>> config = mct.CoreConfig()
+             >>> config = mct.core.CoreConfig()
 
              If mixed precision is desired, create a MCT core config with a mixed-precision configuration, to quantize a model with different bitwidths for different layers.
              The candidates bitwidth for quantization should be defined in the target platform model:
 
-             >>> config = mct.CoreConfig(mixed_precision_config=MixedPrecisionQuantizationConfigV2())
+             >>> config = mct.core.CoreConfig(mixed_precision_config=MixedPrecisionQuantizationConfigV2())
 
              For mixed-precision set a target KPI object:
              Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
              that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
              while the bias will not):
 
-             >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+             >>> kpi = mct.core.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model:
 
-             >>> quantized_model, quantization_info, custom_objects = mct.keras_quantization_aware_training_init(model, repr_datagen, kpi, core_config=config)
+             >>> quantized_model, quantization_info, custom_objects = mct.qat.keras_quantization_aware_training_init(model, repr_datagen, kpi, core_config=config)
 
              Use the quantized model for fine-tuning. For loading the model from file, use the custom_objects dictionary:
 
              >>> quantized_model = tf.keras.models.load_model(model_file, custom_objects=custom_objects)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/api_docs/modules/mixed_precision_quantization_config.html>`_.
 
          """
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization API,"
                                     "or pass a valid mixed precision configuration.")
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(fw_info)
 
         fw_impl = KerasImplementation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
@@ -219,37 +217,37 @@
              Create a random dataset generator:
 
              >>> import numpy as np
              >>> def repr_datagen(): yield [np.random.random((1, 224, 224, 3))]
 
              Create a MCT core config, containing the quantization configuration:
 
-             >>> config = mct.CoreConfig()
+             >>> config = mct.core.CoreConfig()
 
              If mixed precision is desired, create a MCT core config with a mixed-precision configuration, to quantize a model with different bitwidths for different layers.
              The candidates bitwidth for quantization should be defined in the target platform model:
 
-             >>> config = mct.CoreConfig(mixed_precision_config=MixedPrecisionQuantizationConfigV2())
+             >>> config = mct.core.CoreConfig(mixed_precision_config=MixedPrecisionQuantizationConfigV2())
 
              For mixed-precision set a target KPI object:
              Create a KPI object to limit our returned model's size. Note that this value affects only coefficients
              that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
              while the bias will not):
 
-             >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
+             >>> kpi = mct.core.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model:
 
-             >>> quantized_model, quantization_info, custom_objects = mct.keras_quantization_aware_training_init(model, repr_datagen, kpi, core_config=config)
+             >>> quantized_model, quantization_info, custom_objects = mct.qat.keras_quantization_aware_training_init(model, repr_datagen, kpi, core_config=config)
 
              Use the quantized model for fine-tuning. For loading the model from file, use the custom_objects dictionary:
 
              >>> quantized_model = tf.keras.models.load_model(model_file, custom_objects=custom_objects)
-             >>> quantized_model = mct.keras_quantization_aware_training_finalize(quantized_model)
+             >>> quantized_model = mct.qat.keras_quantization_aware_training_finalize(quantized_model)
 
          """
         def _export(layer):
             if isinstance(layer, qi.KerasQuantizationWrapper):
                 layer.convert_to_inferable_quantizers()
             return layer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig, BaseKerasTrainableQuantizer
 
 if FOUND_TF:
 
     class BaseKerasQATTrainableQuantizer(BaseKerasTrainableQuantizer):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 # ==============================================================================
 
 from typing import Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
-from model_compression_toolkit.core.common.constants import SIGNED
+from model_compression_toolkit.constants import SIGNED
+from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.qat import TrainingMethod
+
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.qat.common import THRESHOLD_TENSOR
-from model_compression_toolkit.qat.common.constants import FQ_MIN, FQ_MAX
-from model_compression_toolkit import quantizers_infrastructure as qi, TrainingMethod
-from model_compression_toolkit.core.common import constants as C
+from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
     WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
     ActivationSymmetricInferableQuantizer
@@ -49,19 +51,19 @@
         for the quantization.
 
         Args:
             quantization_config: trainable quantizer config class
         """
         super().__init__(quantization_config)
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
-        self.threshold_values = quantization_config.weights_quantization_params[C.THRESHOLD]
+        self.threshold_values = np.array(quantization_config.weights_quantization_params[C.THRESHOLD])
         self.threshold_shape = np.asarray(self.threshold_values).shape
         self.per_channel = self.quantization_config.weights_per_channel_threshold
         self.channel_axis = self.quantization_config.weights_channels_axis
-        self.np_threshold_values = np.reshape(np.asarray(self.threshold_values),[-1]) if self.channel_axis else float(self.threshold_values)
+        self.np_threshold_values = np.reshape(np.asarray(self.threshold_values),[-1]) if self.per_channel else float(self.threshold_values)
 
         if self.per_channel and self.channel_axis not in [-1, len(self.threshold_shape) - 1]:
             # Tensorflow's fake_quant_with_min_max_vars_per_channel only works on last axis, so
             # need to move the quantization axis to the last axis
             self.perm_vec = list(np.arange(len(self.threshold_shape)))
             self.perm_vec[self.channel_axis] = len(self.threshold_shape) - 1
             self.perm_vec[len(self.threshold_shape) - 1] = self.channel_axis
@@ -89,29 +91,29 @@
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
         """
         ptq_threshold_tensor = layer.add_weight(
             name + THRESHOLD_TENSOR,
-            shape=len(self.np_threshold_values) if self.channel_axis else (),
+            shape=len(self.np_threshold_values) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         ptq_threshold_tensor.assign(self.np_threshold_values)
 
         fq_min = layer.add_weight(
             name + FQ_MIN,
-            shape=len(self.min) if self.channel_axis else (),
+            shape=len(self.min) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(-1.0),
             trainable=False)
         fq_min.assign(self.min)
 
         fq_max = layer.add_weight(
             name + FQ_MAX,
-            shape=len(self.max) if self.channel_axis else (),
+            shape=len(self.max) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         fq_max.assign(self.max)
 
         # save the quantizer added parameters for later calculations
         self.add_quantizer_variable(THRESHOLD_TENSOR, ptq_threshold_tensor, VariableGroup.QPARAMS)
         self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
@@ -130,15 +132,15 @@
 
         Returns:
             The quantized tensor.
         """
 
         _min = self.get_quantizer_variable(FQ_MIN)
         _max = self.get_quantizer_variable(FQ_MAX)
-        if self.channel_axis:
+        if self.per_channel:
             if self.perm_vec:
                 inputs = tf.transpose(inputs, perm=self.perm_vec)
             q_tensor = tf.quantization.fake_quant_with_min_max_vars_per_channel(inputs, _min, _max,
                                                                                 num_bits=self.num_bits)
             if self.perm_vec:
                 q_tensor = tf.transpose(q_tensor, perm=self.perm_vec)
         else:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
-from model_compression_toolkit.core.common.constants import RANGE_MIN, RANGE_MAX
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.qat.common.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.constants import RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.qat import TrainingMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+
 from model_compression_toolkit.qat.keras.quantizer.quant_utils import adjust_range_to_include_zero
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import fix_range_to_include_zero
-from model_compression_toolkit import quantizers_infrastructure as qi, TrainingMethod
-from model_compression_toolkit.core.common import constants as C
+from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
     mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
     BaseKerasInferableQuantizer, WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
@@ -46,16 +48,16 @@
         for the quantization.
 
         Args:
             quantization_config: a trainable quantizer config class with attributes for the quantization.
 
         """
         super().__init__(quantization_config)
-        self.max_values = quantization_config.weights_quantization_params[RANGE_MAX]
-        self.min_values = quantization_config.weights_quantization_params[RANGE_MIN]
+        self.max_values = np.array(quantization_config.weights_quantization_params[RANGE_MAX])
+        self.min_values = np.array(quantization_config.weights_quantization_params[RANGE_MIN])
         self.num_bits = self.quantization_config.weights_n_bits
         self.per_channel = self.quantization_config.weights_per_channel_threshold
         self.channel_axis = self.quantization_config.weights_channels_axis
         self.min_max_shape = np.asarray(self.max_values).shape
         self.max = np.reshape(self.max_values, [-1]) if self.per_channel else float(self.max_values)
         self.min = np.reshape(self.min_values, [-1]) if self.per_channel else float(self.min_values)
 
@@ -94,15 +96,14 @@
             trainable=False)
         fq_max.assign(self.max)
 
         # save the quantizer added parameters for later calculations
         self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
         self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
 
-
     def __call__(self, inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
@@ -195,15 +196,14 @@
             trainable=False)
         fq_max.assign(self.max_range)
 
         # save the quantizer added parameters for later calculations
         self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
         self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
 
-
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from typing import Callable
 from functools import partial
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH, PYTORCH
+from model_compression_toolkit.constants import FOUND_TORCH, PYTORCH
 
-from model_compression_toolkit import CoreConfig
+from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.core.common.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 
 
 if FOUND_TORCH:
     import torch.nn as nn
     from torch.nn import Module
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
-    from model_compression_toolkit.core.pytorch.constants import DEFAULT_TP_MODEL
+    from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
     from model_compression_toolkit.qat.common.qat_config import _is_qat_applicable
     from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
     from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
     from model_compression_toolkit import quantizers_infrastructure as qi
     from model_compression_toolkit import get_target_platform_capabilities
     from model_compression_toolkit.qat.common.qat_config import QATConfig
@@ -117,32 +117,32 @@
             >>> num_calibration_batches = 10
             >>> def repr_datagen():
             >>>     for _ in range(num_calibration_batches):
             >>>         yield [np.random.random((4, 3, 224, 224))]
 
              Create a MCT core config, containing the quantization configuration:
 
-             >>> config = mct.CoreConfig()
+             >>> config = mct.core.CoreConfig()
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model. Now the model contains quantizer wrappers for fine tunning the weights:
 
              >>> quantized_model, quantization_info = pytorch_quantization_aware_training_init(model, repr_datagen, core_config=config)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/api_docs/modules/mixed_precision_quantization_config.html>`_.
 
          """
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
-                common.Logger.error("Given quantization config to mixed-precision facade is not of type "
+                Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use pytorch_post_training_quantization API,"
                                     "or pass a valid mixed precision configuration.")
 
-            common.Logger.info("Using experimental mixed-precision quantization. "
+            Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(fw_info)
 
         fw_impl = PytorchImplementation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
@@ -189,15 +189,15 @@
              Create a random dataset generator:
 
              >>> import numpy as np
              >>> def repr_datagen(): yield [np.random.random((1, 224, 224, 3))]
 
              Create a MCT core config, containing the quantization configuration:
 
-             >>> config = mct.CoreConfig()
+             >>> config = mct.core.CoreConfig()
 
              Pass the model, the representative dataset generator, the configuration and the target KPI to get a
              quantized model:
 
              >>> quantized_model, quantization_info = pytorch_quantization_aware_training_init(model, repr_datagen, core_config=config)
 
              Use the quantized model for fine-tuning. Finally, remove the quantizer wrappers and keep a quantize model ready for inference.
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
 
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
     BasePytorchTrainableQuantizer
 
 if FOUND_TORCH:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # ==============================================================================
 from typing import Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.qat import TrainingMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.qat.common import THRESHOLD_TENSOR
-from model_compression_toolkit import quantizers_infrastructure as qi, TrainingMethod
+from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
 from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.core.common import constants as C
+
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import ste_round, ste_clip, symmetric_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
     ActivationSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import Tensor
 
-from model_compression_toolkit.core.common.constants import RANGE_MAX, RANGE_MIN
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.qat.common.constants import FQ_MIN, FQ_MAX
-from model_compression_toolkit.core.common import constants as C
-from model_compression_toolkit import quantizers_infrastructure as qi, TrainingMethod
+from model_compression_toolkit.constants import RANGE_MAX, RANGE_MIN
+from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+
+from model_compression_toolkit.qat import TrainingMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+
 from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import uniform_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from enum import Enum
 from typing import Any, Dict, List
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 class QuantizationTarget(Enum):
     Activation = "Activation"
     Weights = "Weights"
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import QUANTIZATION_TARGET, \
     QUANTIZATION_METHOD
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses import get_all_subclasses
 
 
 def get_inferable_quantizer_class(quant_target: QuantizationTarget,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses import get_all_subclasses
 
 if FOUND_TF:
     import tensorflow as tf
     from model_compression_toolkit import quantizers_infrastructure as qi
     from model_compression_toolkit.quantizers_infrastructure import BaseKerasTrainableQuantizer
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, List, Any, Tuple
 from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.quantizers_infrastructure import BaseInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import WEIGHTS_QUANTIZERS, ACTIVATION_QUANTIZERS, LAYER, STEPS, TRAINING
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.util import tf_inspect
     from tensorflow_model_optimization.python.core.keras import utils
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 # ==============================================================================
 import warnings
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TF:
     import tensorflow as tf
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 
 
 if FOUND_TF:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer \
         import ActivationSymmetricInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 
 if FOUND_TF:
     import tensorflow as tf
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_uniform_inferable_quantizer \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.quant_utils import \
     adjust_range_to_include_zero
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.validation_functions import \
     validate_uniform_min_max_ranges, validate_adjusted_min_max_ranges
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import abstractmethod
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.quantizers_infrastructure import BaseInferableQuantizer
 
 if FOUND_TF:
     import tensorflow as tf
 
     class BaseKerasInferableQuantizer(BaseInferableQuantizer):
         def __init__(self):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TF:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.\
         weights_lut_symmetric_inferable_quantizer import WeightsLUTSymmetricInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 # ==============================================================================
 import warnings
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TF:
     import tensorflow as tf
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
 
 if FOUND_TF:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer \
         import WeightsSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
 
 if FOUND_TF:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_uniform_inferable_quantizer \
         import WeightsUniformInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TF
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.quant_utils import \
     adjust_range_to_include_zero
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.validation_functions import \
     validate_uniform_min_max_ranges, validate_adjusted_min_max_ranges
 
 if FOUND_TF:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
 import numpy as np
 
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 
 
 def validate_uniform_min_max_ranges(min_range: Any, max_range: Any) -> None:
     """
     Validate min/max ranges in uniform quantizers are valid
 
     Args:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================f
 from typing import List, Union, Any, Dict, Tuple
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.quantizers_infrastructure import BaseInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import LAYER, TRAINING
 import inspect
 
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
     BasePytorchTrainableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer \
     import mark_quantizer, QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
     import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TORCH:
     import torch
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer import \
         ActivationSymmetricInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 if FOUND_TORCH:
     import torch
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.base_symmetric_inferable_quantizer import \
         BaseSymmetricInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 if FOUND_TORCH:
     import torch
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.base_uniform_inferable_quantizer import \
         BaseUniformInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 import warnings
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer \
     import mark_quantizer
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers \
         .base_pytorch_inferable_quantizer import BasePyTorchInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import abstractmethod
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.quantizers_infrastructure import BaseInferableQuantizer
 
 if FOUND_TORCH:
     import torch
 
 
     class BasePyTorchInferableQuantizer(BaseInferableQuantizer):
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.base_pytorch_inferable_quantizer import \
         BasePyTorchInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.base_pytorch_inferable_quantizer import \
         BasePyTorchInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer \
     import mark_quantizer, QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
     import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers \
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer \
     import mark_quantizer, \
     QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
     import MULTIPLIER_N_BITS, EPS
 
 if FOUND_TORCH:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 if FOUND_TORCH:
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer import \
         WeightsSymmetricInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer, \
     QuantizationTarget
 
 if FOUND_TORCH:
     import torch
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizer_utils import to_torch_tensor, \
         get_working_device
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import QuantizationTarget, \
     mark_quantizer
 
 if FOUND_TORCH:
     import torch
     from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizer_utils import get_working_device, \
     fix_range_to_include_zero, to_torch_tensor
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+from model_compression_toolkit.quantizers_infrastructure.constants import THRESHOLD_TENSOR, WEIGHTS_QUANTIZATION_PARAMS
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 from abc import abstractmethod
 from enum import Enum
 from typing import Union, List, Any
 from inspect import signature
 
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.logger import Logger
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer, \
     QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import QUANTIZATION_METHOD, \
     QUANTIZATION_TARGET
@@ -51,17 +51,17 @@
             quantization_config: quantizer config class contains all the information about the quantizer configuration.
         """
 
         # verify the quantizer class that inherits this class only has a config argument and key-word arguments
         for i, (k, v) in enumerate(self.get_sig().parameters.items()):
             if i == 0:
                 if v.annotation not in [TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]:
-                    common.Logger.error(f"First parameter must be either TrainableQuantizerWeightsConfig or TrainableQuantizerActivationConfig")  # pragma: no cover
+                    Logger.error(f"First parameter must be either TrainableQuantizerWeightsConfig or TrainableQuantizerActivationConfig")  # pragma: no cover
             elif v.default is v.empty:
-                common.Logger.error(f"Parameter {k} doesn't have a default value")  # pragma: no cover
+                Logger.error(f"Parameter {k} doesn't have a default value")  # pragma: no cover
 
         super(BaseTrainableQuantizer, self).__init__()
         self.quantization_config = quantization_config
 
         # Inherited class should be decorated with @mark_quantizer decorator, and define the following static properties
         static_quantization_method = getattr(self, QUANTIZATION_METHOD, None)
         static_quantization_target = getattr(self, QUANTIZATION_TARGET, None)
@@ -69,23 +69,23 @@
         if static_quantization_method is None or static_quantization_target is None:
             Logger.error("A quantizer class that inherit from BaseTrainableQuantizer is not defined appropriately."
                          "Either it misses the @mark_quantizer decorator or the decorator is not used correctly.")
 
         if static_quantization_target == QuantizationTarget.Weights:
             self.validate_weights()
             if self.quantization_config.weights_quantization_method not in static_quantization_method:
-                common.Logger.error(
+                Logger.error(
                     f'Quantization method mismatch expected: {static_quantization_method} and got  {self.quantization_config.weights_quantization_method}')
         elif static_quantization_target == QuantizationTarget.Activation:
             self.validate_activation()
             if self.quantization_config.activation_quantization_method not in static_quantization_method:
-                common.Logger.error(
+                Logger.error(
                     f'Quantization method mismatch expected: {static_quantization_method} and got  {self.quantization_config.activation_quantization_method}')
         else:
-            common.Logger.error(
+            Logger.error(
                 f'Unknown Quantization Part:{static_quantization_target}')  # pragma: no cover
 
         self.quantizer_parameters = {}
 
     @classmethod
     def get_sig(cls):
         return signature(cls)
@@ -141,23 +141,23 @@
     def validate_weights(self) -> None:
         """
         This function validates the quantization config compared with its parameters.
 
 
         """
         if self.activation_quantization() or not self.weights_quantization():
-            common.Logger.error(f'Expect weight quantization got activation')
+            Logger.error(f'Expect weight quantization got activation')
 
     def validate_activation(self) -> None:
         """
         This function validates the quantization config compared with its parameters.
 
         """
         if not self.activation_quantization() or self.weights_quantization():
-            common.Logger.error(f'Expect activation quantization got weight')
+            Logger.error(f'Expect activation quantization got weight')
 
     def convert2inferable(self) -> BaseInferableQuantizer:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseInferableQuantizer object.
@@ -179,15 +179,15 @@
 
         Returns:
             trainable variable
         """
         if name in self.quantizer_parameters:
             return self.quantizer_parameters[name][VAR]
         else:
-            common.Logger.error(f'Variable {name} is not exist in quantizers parameters!') # pragma: no cover
+            Logger.error(f'Variable {name} is not exist in quantizers parameters!') # pragma: no cover
 
 
     @abstractmethod
     def get_trainable_variables(self, group: VariableGroup) -> List[Any]:
         """
         Get trainable parameters with specific group from quantizer
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
-from model_compression_toolkit.core.common import BaseNode, Logger
+from model_compression_toolkit.core.common import BaseNode
+from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig, TrainableQuantizerCandidateConfig
 
 
 def get_trainable_quantizer_weights_config(
         n: BaseNode,
         weights_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Union
+from typing import Union, Any
 
-from model_compression_toolkit.gptq import RoundingType
-from model_compression_toolkit import TrainingMethod
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
     import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_TYPE
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses \
     import get_all_subclasses
 
 
 def get_trainable_quantizer_class(quant_target: QuantizationTarget,
-                                  quantizer_type: Union[TrainingMethod, RoundingType],
+                                  quantizer_type: Union[Any, Any],
                                   quant_method: QuantizationMethod,
                                   quantizer_base_class: type) -> type:
     """
     Searches for a trainable quantizer class that matches the requested QuantizationTarget and QuantizationMethod and
     a task dedicated quantizer type. Exactly one class should be found.
 
     Args:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import ABC
 from typing import Dict, List
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 class TrainableQuantizerCandidateConfig:
 
     def __init__(self,
                  n_bits: int,
                  quantization_params: Dict,
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any, Union, List
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 
 if FOUND_TF:
     QUANTIZATION_CONFIG = 'quantization_config'
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 import copy
 
 from typing import Any, Union
 from enum import Enum
 
-from model_compression_toolkit.core.common.target_platform import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common import constants as C
 
 
 def transform_enum(v: Any):
     """
```

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union, List
 
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 
 
 if FOUND_TORCH:
```

### Comparing `mct-nightly-1.8.0.9042023.post411/setup.py` & `mct-nightly-1.8.0.9052023.post348/setup.py`

 * *Files identical despite different names*

