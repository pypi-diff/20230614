# Comparing `tmp/arize-7.0.4.tar.gz` & `tmp/arize-7.0.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.4.tar", last modified: Tue Jun 13 00:39:02 2023, max compression
+gzip compressed data, was "arize-7.0.5rc0.tar", last modified: Tue Jun 13 23:05:38 2023, max compression
```

## Comparing `arize-7.0.4.tar` & `arize-7.0.5rc0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.666999 arize-7.0.4/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-12 17:30:40.000000 arize-7.0.4/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-12 17:30:40.000000 arize-7.0.4/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-13 00:39:02.667268 arize-7.0.4/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-12 17:30:40.000000 arize-7.0.4/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.556183 arize-7.0.4/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-13 00:36:59.000000 arize-7.0.4/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    28890 2023-06-12 17:30:40.000000 arize-7.0.4/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-12 17:30:40.000000 arize-7.0.4/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.590385 arize-7.0.4/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.591889 arize-7.0.4/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.599370 arize-7.0.4/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10306 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)      470 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/endpoint.py
--rw-r--r--   0 kiko       (501) staff       (20)     1111 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3956 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/session.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.606759 arize-7.0.4/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)       99 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      552 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.608874 arize-7.0.4/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.640738 arize-7.0.4/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.642069 arize-7.0.4/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.645927 arize-7.0.4/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    23005 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.648990 arize-7.0.4/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5058 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.653613 arize-7.0.4/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    69574 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-12 19:46:43.000000 arize-7.0.4/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.662460 arize-7.0.4/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24227 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.563788 arize-7.0.4/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      433 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-12 17:30:40.000000 arize-7.0.4/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-06-13 00:39:02.669456 arize-7.0.4/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.666134 arize-7.0.4/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49447 2023-06-12 17:30:40.000000 arize-7.0.4/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-12 17:30:40.000000 arize-7.0.4/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.671826 arize-7.0.5rc0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-12 17:30:40.000000 arize-7.0.5rc0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-12 17:30:40.000000 arize-7.0.5rc0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-13 23:05:38.672087 arize-7.0.5rc0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-12 17:30:40.000000 arize-7.0.5rc0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.573876 arize-7.0.5rc0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    28890 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.605977 arize-7.0.5rc0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.607396 arize-7.0.5rc0/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.612206 arize-7.0.5rc0/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10541 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)      470 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/core/endpoint.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1285 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3931 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/session.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.616857 arize-7.0.5rc0/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)       99 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      552 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.618761 arize-7.0.5rc0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.629714 arize-7.0.5rc0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.630616 arize-7.0.5rc0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.633999 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    23005 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.635777 arize-7.0.5rc0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5058 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.656288 arize-7.0.5rc0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    69574 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-12 19:46:43.000000 arize-7.0.5rc0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.666095 arize-7.0.5rc0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24227 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.580009 arize-7.0.5rc0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      433 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-12 17:30:40.000000 arize-7.0.5rc0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-06-13 23:05:38.673446 arize-7.0.5rc0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.670941 arize-7.0.5rc0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49447 2023-06-12 17:30:40.000000 arize-7.0.5rc0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-12 17:30:40.000000 arize-7.0.5rc0/tests/test_utils.py
```

### Comparing `arize-7.0.4/LICENSE.md` & `arize-7.0.5rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/PKG-INFO` & `arize-7.0.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.4
+Version: 7.0.5rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.4/README.md` & `arize-7.0.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/api.py` & `arize-7.0.5rc0/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/bounded_executor.py` & `arize-7.0.5rc0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/bulk_client.py` & `arize-7.0.5rc0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/bulk_client_shap.py` & `arize-7.0.5rc0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/client_shap_values.py` & `arize-7.0.5rc0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/log_client.py` & `arize-7.0.5rc0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/log_pandas_dataframe.py` & `arize-7.0.5rc0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/examples/preproduction_client.py` & `arize-7.0.5rc0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/exporter/core/client.py` & `arize-7.0.5rc0/arize/exporter/core/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import itertools
-import sys
-import threading
-import time
 from datetime import datetime
-from typing import Optional
+from typing import Optional, Tuple
 
 import pandas as pd
 import pyarrow.parquet as pq
 from arize.utils.types import Environments
 from pyarrow import flight
+from tqdm import tqdm
 
 from ..utils.validation import Validator
 from .endpoint import Endpoint
 from .session import Session
 
 
 class ArizeExportClient:
@@ -87,36 +84,39 @@
                 Batches only apply to the Validation environment, and can be found in the Datasets tab on
                 the model page in the Arize UI.
 
         Returns:
         --------
             A pandas dataframe
         """
-        stream_reader = self.get_model_stream_reader(
+        stream_reader, num_recs = self.get_model_stream_reader(
             space_id=space_id,
             model_id=model_id,
             environment=environment,
             start_time=start_time,
             end_time=end_time,
             include_actuals=include_actuals,
             model_version=model_version,
             batch_id=batch_id,
         )
-        t = threading.Thread(target=self.animate)
-        t.start()
+        if stream_reader is None:
+            return pd.DataFrame()
+        progress_bar = self.get_progress_bar(num_recs)
         list_of_df = []
         while True:
             try:
                 flight_batch = stream_reader.read_chunk()
                 record_batch = flight_batch.data
                 data_to_pandas = record_batch.to_pandas()
                 list_of_df.append(data_to_pandas)
+                progress_bar.update(data_to_pandas.shape[0])
             except StopIteration:
                 self.done = True
                 break
+        progress_bar.close()
         return pd.concat(list_of_df)
 
     def export_model_to_parquet(
         self,
         path: str,
         space_id: str,
         model_id: str,
@@ -156,47 +156,50 @@
                 the model page in the Arize UI.
 
         Returns:
         --------
             None
         """
         Validator.validate_input_type(path, "path", str)
-        stream_reader = self.get_model_stream_reader(
+        stream_reader, num_recs = self.get_model_stream_reader(
             space_id=space_id,
             model_id=model_id,
             environment=environment,
             start_time=start_time,
             end_time=end_time,
             include_actuals=include_actuals,
             model_version=model_version,
             batch_id=batch_id,
         )
-        t = threading.Thread(target=self.animate)
-        t.start()
+        if stream_reader is None:
+            return None
+        progress_bar = self.get_progress_bar(num_recs)
         with pq.ParquetWriter(path, schema=stream_reader.schema) as writer:
             while True:
                 try:
                     flight_batch = stream_reader.read_chunk()
                     record_batch = flight_batch.data
                     writer.write_batch(record_batch)
+                    progress_bar.update(record_batch.num_rows)
                 except StopIteration:
                     self.done = True
                     break
+        progress_bar.close()
 
     def get_model_stream_reader(
         self,
         space_id: str,
         model_id: str,
         environment: Environments,
         start_time: datetime,
         end_time: datetime,
         include_actuals: Optional[bool] = False,
         model_version: Optional[str] = "",
         batch_id: Optional[str] = "",
-    ) -> flight.FlightStreamReader:
+    ) -> Tuple[flight.FlightStreamReader, int]:
         Validator.validate_input_type(space_id, "space_id", str)
         Validator.validate_input_type(model_id, "model_id", str)
         Validator.validate_input_type(environment, "environment", Environments)
         Validator.validate_input_type(include_actuals, "include_actuals", bool)
         Validator.validate_input_type(start_time, "start_time", datetime)
         Validator.validate_input_type(end_time, "end_time", datetime)
         Validator.validate_input_type(model_version, "model_version", str)
@@ -214,19 +217,18 @@
         start_time_str = start_time.strftime("%Y-%m-%dT%H:%M:%SZ")
         end_time_str = end_time.strftime("%Y-%m-%dT%H:%M:%SZ")
         cmd = (
             f'{{"spaceId":"{space_id}","modelId":"{model_id}", "environment":"{env}", '
             f'"modelVersion":"{model_version}", "batchId":"{batch_id}", "startTime":"{start_time_str}", '
             f'"endTime":"{end_time_str}", "includeActuals": {str(include_actuals).lower()}}}'
         )
-        stream_reader = self(query=cmd)
-        return stream_reader
+        return self(query=cmd)
 
-    def animate(self) -> None:
-        self.done = False
-        for c in itertools.cycle(["," "/", "-", "\\"]):
-            if self.done:
-                break
-            sys.stdout.write("\rexporting in progress " + c)
-            sys.stdout.flush()
-            time.sleep(0.1)
-        sys.stdout.write("\rexport complete!     ")
+    def get_progress_bar(self, num_recs):
+        return tqdm(
+            total=num_recs,
+            desc=f"  exporting {num_recs} rows",
+            bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}, {rate_fmt}{postfix}]",
+            ncols=80,
+            colour="#008000",
+            unit=" row",
+        )
```

### Comparing `arize-7.0.4/arize/exporter/core/session.py` & `arize-7.0.5rc0/arize/exporter/core/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
-import logging
 import os
 import uuid
 from dataclasses import InitVar, dataclass, field
 
+from arize.utils.logging import logger
 from pyarrow import flight
 
 from ..utils.constants import (
     ARIZE_API_KEY,
     ARIZE_PROFILE,
     DEFAULT_ARIZE_API_KEY_CONFIG_KEY,
     DEFAULT_ARIZE_FLIGHT_HOST,
@@ -15,16 +15,14 @@
     DEFAULT_CONFIG_PATH,
     DEFAULT_PACKAGE_NAME,
     DEFAULT_PROFILE_NAME,
     PROFILE_FILE_NAME,
 )
 from ..utils.errors import InvalidConfigFileError, InvalidSessionError
 
-logging.basicConfig(level=logging.INFO)
-
 
 @dataclass
 class Session:
     api_key: InitVar[str] = None
     arize_profile: InitVar[str] = None
     arize_config_path: InitVar[str] = DEFAULT_CONFIG_PATH
     host: InitVar[str] = DEFAULT_ARIZE_FLIGHT_HOST
@@ -34,15 +32,15 @@
 
     def __post_init__(
         self, api_key: str, arize_profile: str, arize_config_path: str, host: str, port: int
     ):
         self.headers = []
         self.call_options = None
         self.session_name = f"python-sdk-{DEFAULT_PACKAGE_NAME}-{uuid.uuid4()}"
-        logging.info(f"Creating named session as '{self.session_name}'.")
+        logger.info(f"Creating named session as '{self.session_name}'.")
         api_key = api_key or ARIZE_API_KEY
         if api_key:
             self.arize_api_key = api_key
         else:
             self._read_config(arize_profile, arize_config_path)
 
         if host:
@@ -51,25 +49,25 @@
             self.host = DEFAULT_ARIZE_FLIGHT_HOST
 
         if port:
             self.port = port
         else:
             self.port = DEFAULT_ARIZE_FLIGHT_PORT
 
-        logging.debug(
+        logger.debug(
             f"Created session with Arize API Token '{self.arize_api_key}' at '{self.host}':'{self.port}'"
         )
 
     def _read_config(self, arize_profile: str, arize_config_path: str):
         arize_profile = arize_profile or ARIZE_PROFILE or DEFAULT_PROFILE_NAME
         arize_config_path = arize_config_path or DEFAULT_CONFIG_PATH
 
         config_parser = Session._get_config_parser()
         file_path = os.path.join(arize_config_path, PROFILE_FILE_NAME)
-        logging.debug(
+        logger.debug(
             f"No provided connection details. Looking up session values from '{arize_profile}' in "
             f"'{file_path}'."
         )
         try:
             config_parser.read(file_path)
             self.arize_api_key = config_parser.get(arize_profile, DEFAULT_ARIZE_API_KEY_CONFIG_KEY)
         except configparser.NoSectionError:
@@ -100,9 +98,9 @@
                     disable_server_verification=disable_cert,
                 )
                 self.headers.append((b"auth-token-bin", f"{self.arize_api_key}".encode("utf-8")))
                 self.call_options = flight.FlightCallOptions(timeout=600, headers=self.headers)
                 return client
             raise ConnectionError("arize api key must be supplied.")
         except Exception:
-            logging.exception("There was an error trying to connect to the Arize Flight Endpoint")
+            logger.error("There was an error trying to connect to the Arize Flight Endpoint")
             raise
```

### Comparing `arize-7.0.4/arize/exporter/utils/constants.py` & `arize-7.0.5rc0/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/exporter/utils/schema_parser.py` & `arize-7.0.5rc0/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/exporter/utils/validation.py` & `arize-7.0.5rc0/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.5rc0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/base_generators.py` & `arize-7.0.5rc0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.5rc0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/errors.py` & `arize-7.0.5rc0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/models.py` & `arize-7.0.5rc0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.5rc0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.5rc0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/logger.py` & `arize-7.0.5rc0/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.5rc0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/validation/errors.py` & `arize-7.0.5rc0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/pandas/validation/validator.py` & `arize-7.0.5rc0/arize/pandas/validation/validator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/public_pb2.py` & `arize-7.0.5rc0/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/utils/constants.py` & `arize-7.0.5rc0/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/utils/logging.py` & `arize-7.0.5rc0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/utils/model_mapping.json` & `arize-7.0.5rc0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/utils/types.py` & `arize-7.0.5rc0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize/utils/utils.py` & `arize-7.0.5rc0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/arize.egg-info/PKG-INFO` & `arize-7.0.5rc0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.4
+Version: 7.0.5rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.4/arize.egg-info/SOURCES.txt` & `arize-7.0.5rc0/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/setup.cfg` & `arize-7.0.5rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/tests/test_api.py` & `arize-7.0.5rc0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.4/tests/test_utils.py` & `arize-7.0.5rc0/tests/test_utils.py`

 * *Files identical despite different names*

