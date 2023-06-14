# Comparing `tmp/gpt_index-0.6.8.tar.gz` & `tmp/gpt_index-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.8.tar", last modified: Tue May 16 04:14:08 2023, max compression
+gzip compressed data, was "gpt_index-0.6.9.tar", last modified: Fri May 19 20:29:42 2023, max compression
```

## Comparing `gpt_index-0.6.8.tar` & `gpt_index-0.6.9.tar`

### file list

```diff
@@ -1,476 +1,496 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 04:13:54.000000 gpt_index-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 04:13:54.000000 gpt_index-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-16 04:14:08.337147 gpt_index-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-16 04:13:54.000000 gpt_index-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/gpt_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/docs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/epub_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/slides_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/video_audio_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 04:13:54.000000 gpt_index-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:14:08.337147 gpt_index-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-16 04:13:54.000000 gpt_index-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/test_llm_rerank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.423003 gpt_index-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 20:29:22.000000 gpt_index-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-19 20:29:22.000000 gpt_index-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-19 20:29:42.423003 gpt_index-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-19 20:29:22.000000 gpt_index-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.319002 gpt_index-0.6.9/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-19 20:29:42.000000 gpt_index-0.6.9/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-05-19 20:29:42.000000 gpt_index-0.6.9/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:29:42.000000 gpt_index-0.6.9/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 20:29:42.000000 gpt_index-0.6.9/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 20:29:42.000000 gpt_index-0.6.9/gpt_index.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.319002 gpt_index-0.6.9/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.323002 gpt_index-0.6.9/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.323002 gpt_index-0.6.9/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.323002 gpt_index-0.6.9/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.323002 gpt_index-0.6.9/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.323002 gpt_index-0.6.9/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.327003 gpt_index-0.6.9/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.331003 gpt_index-0.6.9/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.335003 gpt_index-0.6.9/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.335003 gpt_index-0.6.9/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.339003 gpt_index-0.6.9/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.339003 gpt_index-0.6.9/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.339003 gpt_index-0.6.9/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.343003 gpt_index-0.6.9/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/base_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/compact_and_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/simple_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/tree_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.343003 gpt_index-0.6.9/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.347003 gpt_index-0.6.9/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.347003 gpt_index-0.6.9/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-19 20:29:22.000000 gpt_index-0.6.9/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.347003 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.347003 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.347003 gpt_index-0.6.9/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.351003 gpt_index-0.6.9/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.351003 gpt_index-0.6.9/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/llm_predictor/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.351003 gpt_index-0.6.9/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.351003 gpt_index-0.6.9/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.355003 gpt_index-0.6.9/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.355003 gpt_index-0.6.9/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/output_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.355003 gpt_index-0.6.9/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.359003 gpt_index-0.6.9/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/default_choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.359003 gpt_index-0.6.9/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.363003 gpt_index-0.6.9/llama_index/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/question_gen/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/question_gen/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/question_gen/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.367003 gpt_index-0.6.9/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.367003 gpt_index-0.6.9/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.371003 gpt_index-0.6.9/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.371003 gpt_index-0.6.9/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.375003 gpt_index-0.6.9/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.379003 gpt_index-0.6.9/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.379003 gpt_index-0.6.9/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.379003 gpt_index-0.6.9/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.379003 gpt_index-0.6.9/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.383003 gpt_index-0.6.9/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.383003 gpt_index-0.6.9/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.383003 gpt_index-0.6.9/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.387003 gpt_index-0.6.9/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.387003 gpt_index-0.6.9/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.387003 gpt_index-0.6.9/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.395003 gpt_index-0.6.9/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-19 20:29:23.000000 gpt_index-0.6.9/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 20:29:23.000000 gpt_index-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:29:42.423003 gpt_index-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-19 20:29:23.000000 gpt_index-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.395003 gpt_index-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.395003 gpt_index-0.6.9/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.395003 gpt_index-0.6.9/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.399003 gpt_index-0.6.9/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.399003 gpt_index-0.6.9/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.399003 gpt_index-0.6.9/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.399003 gpt_index-0.6.9/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.403003 gpt_index-0.6.9/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.403003 gpt_index-0.6.9/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.403003 gpt_index-0.6.9/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.403003 gpt_index-0.6.9/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/postprocessor/test_llm_rerank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.407003 gpt_index-0.6.9/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.407003 gpt_index-0.6.9/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.407003 gpt_index-0.6.9/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.407003 gpt_index-0.6.9/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.411003 gpt_index-0.6.9/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.411003 gpt_index-0.6.9/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.411003 gpt_index-0.6.9/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.411003 gpt_index-0.6.9/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.415003 gpt_index-0.6.9/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.415003 gpt_index-0.6.9/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.415003 gpt_index-0.6.9/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.415003 gpt_index-0.6.9/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.415003 gpt_index-0.6.9/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/question_gen/test_llm_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.419003 gpt_index-0.6.9/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.423003 gpt_index-0.6.9/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:42.423003 gpt_index-0.6.9/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-19 20:29:23.000000 gpt_index-0.6.9/tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.6.8/LICENSE` & `gpt_index-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/PKG-INFO` & `gpt_index-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.6.8
+Version: 0.6.9
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.8/README.md` & `gpt_index-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.6.9/gpt_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.6.8
+Version: 0.6.9
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.8/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.6.9/gpt_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,23 @@
 llama_index/indices/query/embedding_utils.py
 llama_index/indices/query/response_synthesis.py
 llama_index/indices/query/schema.py
 llama_index/indices/query/query_transform/__init__.py
 llama_index/indices/query/query_transform/base.py
 llama_index/indices/query/query_transform/prompts.py
 llama_index/indices/response/__init__.py
+llama_index/indices/response/accumulate.py
+llama_index/indices/response/base_builder.py
+llama_index/indices/response/compact_and_refine.py
+llama_index/indices/response/factory.py
+llama_index/indices/response/generation.py
+llama_index/indices/response/refine.py
 llama_index/indices/response/response_builder.py
+llama_index/indices/response/simple_summarize.py
+llama_index/indices/response/tree_summarize.py
 llama_index/indices/response/type.py
 llama_index/indices/struct_store/__init__.py
 llama_index/indices/struct_store/base.py
 llama_index/indices/struct_store/container_builder.py
 llama_index/indices/struct_store/pandas.py
 llama_index/indices/struct_store/pandas_query.py
 llama_index/indices/struct_store/sql.py
@@ -140,14 +148,15 @@
 llama_index/optimization/__init__.py
 llama_index/optimization/optimizer.py
 llama_index/output_parsers/__init__.py
 llama_index/output_parsers/base.py
 llama_index/output_parsers/guardrails.py
 llama_index/output_parsers/langchain.py
 llama_index/output_parsers/selection.py
+llama_index/output_parsers/utils.py
 llama_index/playground/__init__.py
 llama_index/playground/base.py
 llama_index/prompts/__init__.py
 llama_index/prompts/base.py
 llama_index/prompts/chat_prompts.py
 llama_index/prompts/choice_select.py
 llama_index/prompts/default_choice_select.py
@@ -156,15 +165,21 @@
 llama_index/prompts/prompt_type.py
 llama_index/prompts/prompts.py
 llama_index/query_engine/__init__.py
 llama_index/query_engine/graph_query_engine.py
 llama_index/query_engine/multistep_query_engine.py
 llama_index/query_engine/retriever_query_engine.py
 llama_index/query_engine/router_query_engine.py
+llama_index/query_engine/sub_question_query_engine.py
 llama_index/query_engine/transform_query_engine.py
+llama_index/question_gen/__init__.py
+llama_index/question_gen/llm_generators.py
+llama_index/question_gen/output_parser.py
+llama_index/question_gen/prompts.py
+llama_index/question_gen/types.py
 llama_index/readers/__init__.py
 llama_index/readers/base.py
 llama_index/readers/chroma.py
 llama_index/readers/database.py
 llama_index/readers/deeplake.py
 llama_index/readers/discord_reader.py
 llama_index/readers/download.py
@@ -244,14 +259,15 @@
 llama_index/storage/index_store/keyval_index_store.py
 llama_index/storage/index_store/mongo_index_store.py
 llama_index/storage/index_store/simple_index_store.py
 llama_index/storage/index_store/types.py
 llama_index/storage/index_store/utils.py
 llama_index/storage/kvstore/__init__.py
 llama_index/storage/kvstore/mongodb_kvstore.py
+llama_index/storage/kvstore/s3_kvstore.py
 llama_index/storage/kvstore/simple_kvstore.py
 llama_index/storage/kvstore/types.py
 llama_index/token_counter/__init__.py
 llama_index/token_counter/mock_chain_wrapper.py
 llama_index/token_counter/mock_embed_model.py
 llama_index/token_counter/token_counter.py
 llama_index/token_counter/utils.py
@@ -361,14 +377,16 @@
 tests/output_parsers/__init__.py
 tests/output_parsers/test_base.py
 tests/output_parsers/test_selection.py
 tests/playground/__init__.py
 tests/playground/test_base.py
 tests/prompts/__init__.py
 tests/prompts/test_base.py
+tests/question_gen/__init__.py
+tests/question_gen/test_llm_generators.py
 tests/readers/__init__.py
 tests/readers/test_file.py
 tests/readers/test_json.py
 tests/readers/test_mongo.py
 tests/readers/test_string_iterable.py
 tests/selectors/__init__.py
 tests/selectors/test_llm_selectors.py
```

### Comparing `gpt_index-0.6.8/llama_index/__init__.py` & `gpt_index-0.6.9/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/callbacks/aim.py` & `gpt_index-0.6.9/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/callbacks/base.py` & `gpt_index-0.6.9/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/callbacks/llama_debug.py` & `gpt_index-0.6.9/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/callbacks/schema.py` & `gpt_index-0.6.9/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/composability/joint_qa_summary.py` & `gpt_index-0.6.9/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/data_structs.py` & `gpt_index-0.6.9/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/document_summary.py` & `gpt_index-0.6.9/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/node.py` & `gpt_index-0.6.9/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/registry.py` & `gpt_index-0.6.9/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/struct_type.py` & `gpt_index-0.6.9/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/data_structs/table.py` & `gpt_index-0.6.9/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/embeddings/base.py` & `gpt_index-0.6.9/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/embeddings/google.py` & `gpt_index-0.6.9/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/embeddings/langchain.py` & `gpt_index-0.6.9/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/embeddings/openai.py` & `gpt_index-0.6.9/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/embeddings/utils.py` & `gpt_index-0.6.9/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/evaluation/base.py` & `gpt_index-0.6.9/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/evaluation/dataset_generation.py` & `gpt_index-0.6.9/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/img_utils.py` & `gpt_index-0.6.9/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/__init__.py` & `gpt_index-0.6.9/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/base.py` & `gpt_index-0.6.9/llama_index/indices/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,23 @@
     def service_context(self) -> ServiceContext:
         return self._service_context
 
     @property
     def storage_context(self) -> StorageContext:
         return self._storage_context
 
+    @property
+    def summary(self) -> str:
+        return str(self._index_struct.summary)
+
+    @summary.setter
+    def summary(self, new_summary: str) -> None:
+        self._index_struct.summary = new_summary
+        self._storage_context.index_store.add_index_struct(self._index_struct)
+
     @abstractmethod
     def _build_index_from_nodes(self, nodes: Sequence[Node]) -> IS:
         """Build the index from nodes."""
 
     @llm_token_counter("build_index_from_nodes")
     def build_index_from_nodes(self, nodes: Sequence[Node]) -> IS:
         """Build the index from nodes."""
```

### Comparing `gpt_index-0.6.8/llama_index/indices/base_retriever.py` & `gpt_index-0.6.9/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/common/struct_store/base.py` & `gpt_index-0.6.9/llama_index/indices/common/struct_store/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
 from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import Node
 from llama_index.data_structs.table import StructDatapoint
-from llama_index.indices.response.response_builder import get_response_builder
+from llama_index.indices.response import get_response_builder
 from llama_index.indices.service_context import ServiceContext
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.langchain_helpers.text_splitter import TextSplitter
 from llama_index.prompts.default_prompt_selectors import (
     DEFAULT_REFINE_TABLE_CONTEXT_PROMPT_SEL,
 )
```

### Comparing `gpt_index-0.6.8/llama_index/indices/common/struct_store/schema.py` & `gpt_index-0.6.9/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/common/struct_store/sql.py` & `gpt_index-0.6.9/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/common_tree/base.py` & `gpt_index-0.6.9/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/composability/graph.py` & `gpt_index-0.6.9/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/document_summary/base.py` & `gpt_index-0.6.9/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/document_summary/retrievers.py` & `gpt_index-0.6.9/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/empty/base.py` & `gpt_index-0.6.9/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/empty/retrievers.py` & `gpt_index-0.6.9/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/__init__.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/base.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/rake_base.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/retrievers.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/simple_base.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/keyword_table/utils.py` & `gpt_index-0.6.9/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/knowledge_graph/base.py` & `gpt_index-0.6.9/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/knowledge_graph/retrievers.py` & `gpt_index-0.6.9/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/list/base.py` & `gpt_index-0.6.9/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/list/retrievers.py` & `gpt_index-0.6.9/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/loading.py` & `gpt_index-0.6.9/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/__init__.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/cohere_rerank.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/llm_rerank.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/node.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Node postprocessor."""
 
+import logging
 import re
 from abc import abstractmethod
 from typing import Dict, List, Optional, cast
 
 from pydantic import BaseModel, Field, validator
 
-import logging
+from llama_index.data_structs.node import DocumentRelationship, NodeWithScore
 from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.schema import QueryBundle
+from llama_index.indices.response import get_response_builder
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.prompts import QuestionAnswerPrompt, RefinePrompt
 from llama_index.storage.docstore import BaseDocumentStore
-from llama_index.data_structs.node import DocumentRelationship, NodeWithScore
-from llama_index.indices.response.response_builder import get_response_builder
 
 logger = logging.getLogger(__name__)
 
 
 class BasePydanticNodePostprocessor(BaseModel, BaseNodePostprocessor):
     """Node postprocessor."""
```

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/node_recency.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/node_recency.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,17 @@
 
     This post-processor does the following steps:
 
     - Decides if we need to use the post-processor given the query
       (is it temporal-related?)
     - If yes, sorts nodes by date.
     - For each node, look at subsequent nodes and filter out nodes
-        that have high embedding similarity with the current node.
-        (because this means )
-
+      that have high embedding similarity with the current node.
+      Because this means the subsequent node may have overlapping content
+      with the current node but is also out of date
     """
 
     service_context: ServiceContext
     # infer_recency_tmpl: str = Field(default=DEFAULT_INFER_RECENCY_TMPL)
     date_key: str = "date"
     # if false, then search node info
     in_extra_info: bool = True
```

### Comparing `gpt_index-0.6.8/llama_index/indices/postprocessor/pii.py` & `gpt_index-0.6.9/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/prompt_helper.py` & `gpt_index-0.6.9/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/query/base.py` & `gpt_index-0.6.9/llama_index/indices/query/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Base query engine."""
 
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional, Sequence
-from llama_index.data_structs.node import NodeWithScore
 
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.query.schema import QueryBundle, QueryType
-from llama_index.response.schema import (
-    RESPONSE_TYPE,
-)
+from llama_index.response.schema import RESPONSE_TYPE
 
 logger = logging.getLogger(__name__)
 
 
 class BaseQueryEngine(ABC):
     def query(self, str_or_query_bundle: QueryType) -> RESPONSE_TYPE:
         if isinstance(str_or_query_bundle, str):
```

### Comparing `gpt_index-0.6.8/llama_index/indices/query/embedding_utils.py` & `gpt_index-0.6.9/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/query/query_transform/base.py` & `gpt_index-0.6.9/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/query/query_transform/prompts.py` & `gpt_index-0.6.9/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/query/response_synthesis.py` & `gpt_index-0.6.9/llama_index/indices/query/response_synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Any, Dict, Generator, List, Optional, Sequence
 
 from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.response.response_builder import (
+from llama_index.indices.response import (
     BaseResponseBuilder,
     ResponseMode,
     get_response_builder,
 )
 from llama_index.indices.service_context import ServiceContext
 from llama_index.optimization.optimizer import BaseTokenUsageOptimizer
 from llama_index.prompts.prompts import (
```

### Comparing `gpt_index-0.6.8/llama_index/indices/query/schema.py` & `gpt_index-0.6.9/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/registry.py` & `gpt_index-0.6.9/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/service_context.py` & `gpt_index-0.6.9/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/__init__.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/base.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/container_builder.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/pandas.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/pandas_query.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/sql.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/struct_store/sql_query.py` & `gpt_index-0.6.9/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/__init__.py` & `gpt_index-0.6.9/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.6.9/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/base.py` & `gpt_index-0.6.9/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/inserter.py` & `gpt_index-0.6.9/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.6.9/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.6.9/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, List, Optional, cast
 
 from langchain.input import print_text
 
 from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.response.response_builder import get_response_builder
+from llama_index.indices.response import get_response_builder
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.indices.utils import (
     extract_numbers_given_response,
     get_sorted_node_list,
 )
 from llama_index.prompts.default_prompt_selectors import DEFAULT_REFINE_PROMPT_SEL
 from llama_index.prompts.default_prompts import (
```

### Comparing `gpt_index-0.6.8/llama_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.6.9/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/utils.py` & `gpt_index-0.6.9/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/vector_store/base.py` & `gpt_index-0.6.9/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/retriever.py` & `gpt_index-0.6.9/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/agents/__init__.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/agents/agents.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/agents/tools.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/streaming.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/langchain_helpers/text_splitter.py` & `gpt_index-0.6.9/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/llm_predictor/base.py` & `gpt_index-0.6.9/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/llm_predictor/chatgpt.py` & `gpt_index-0.6.9/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/llm_predictor/huggingface.py` & `gpt_index-0.6.9/llama_index/llm_predictor/huggingface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/llm_predictor/structured.py` & `gpt_index-0.6.9/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/logger/base.py` & `gpt_index-0.6.9/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/node_parser/interface.py` & `gpt_index-0.6.9/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/node_parser/node_utils.py` & `gpt_index-0.6.9/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/node_parser/simple.py` & `gpt_index-0.6.9/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/optimization/optimizer.py` & `gpt_index-0.6.9/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/output_parsers/base.py` & `gpt_index-0.6.9/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/output_parsers/guardrails.py` & `gpt_index-0.6.9/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/output_parsers/langchain.py` & `gpt_index-0.6.9/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/output_parsers/selection.py` & `gpt_index-0.6.9/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/playground/base.py` & `gpt_index-0.6.9/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/base.py` & `gpt_index-0.6.9/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/chat_prompts.py` & `gpt_index-0.6.9/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/choice_select.py` & `gpt_index-0.6.9/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/default_choice_select.py` & `gpt_index-0.6.9/llama_index/prompts/default_choice_select.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/default_prompt_selectors.py` & `gpt_index-0.6.9/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/default_prompts.py` & `gpt_index-0.6.9/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/prompts/prompt_type.py` & `gpt_index-0.6.9/llama_index/prompts/prompt_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,12 @@
     SINGLE_SELECT = "single_select"
 
     # Multiple select prompt
     MULTI_SELECT = "multi_select"
 
     VECTOR_STORE_QUERY = "vector_store_query"
 
+    # Sub question prompt
+    SUB_QUESTION = "sub_question"
+
     # custom (by default)
     CUSTOM = "custom"
```

### Comparing `gpt_index-0.6.8/llama_index/prompts/prompts.py` & `gpt_index-0.6.9/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/query_engine/__init__.py` & `gpt_index-0.6.9/llama_index/query_engine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from llama_index.query_engine.graph_query_engine import ComposableGraphQueryEngine
-from llama_index.query_engine.retriever_query_engine import RetrieverQueryEngine
-from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.query_engine.multistep_query_engine import MultiStepQueryEngine
+from llama_index.query_engine.retriever_query_engine import RetrieverQueryEngine
 from llama_index.query_engine.router_query_engine import (
-    RouterQueryEngine,
     RetrieverRouterQueryEngine,
+    RouterQueryEngine,
 )
-
+from llama_index.query_engine.sub_question_query_engine import SubQuestionQueryEngine
+from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 
 __all__ = [
     "ComposableGraphQueryEngine",
     "RetrieverQueryEngine",
     "TransformQueryEngine",
     "MultiStepQueryEngine",
     "RouterQueryEngine",
     "RetrieverRouterQueryEngine",
+    "SubQuestionQueryEngine",
 ]
```

### Comparing `gpt_index-0.6.8/llama_index/query_engine/graph_query_engine.py` & `gpt_index-0.6.9/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/query_engine/multistep_query_engine.py` & `gpt_index-0.6.9/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/query_engine/retriever_query_engine.py` & `gpt_index-0.6.9/llama_index/query_engine/retriever_query_engine.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from llama_index.callbacks.base import CallbackManager
 from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.base import BaseQueryEngine
-from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.query.response_synthesis import ResponseSynthesizer
+from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.optimization.optimizer import BaseTokenUsageOptimizer
 from llama_index.prompts.prompts import (
     QuestionAnswerPrompt,
     RefinePrompt,
     SimpleInputPrompt,
```

### Comparing `gpt_index-0.6.8/llama_index/query_engine/router_query_engine.py` & `gpt_index-0.6.9/llama_index/query_engine/router_query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
-from typing import Optional, Sequence
+from typing import Callable, Optional, Sequence
+
+from llama_index.data_structs.node import Node
+from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.response.schema import RESPONSE_TYPE
 from llama_index.selectors.llm_selectors import LLMSingleSelector
 from llama_index.selectors.types import BaseSelector
-from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.tools.query_engine import QueryEngineTool
-from llama_index.data_structs.node import Node
 from llama_index.tools.types import ToolMetadata
-from typing import Callable
 
 logger = logging.getLogger(__name__)
 
 
 class RouterQueryEngine(BaseQueryEngine):
     """Router query engine.
```

### Comparing `gpt_index-0.6.8/llama_index/query_engine/transform_query_engine.py` & `gpt_index-0.6.9/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/__init__.py` & `gpt_index-0.6.9/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/base.py` & `gpt_index-0.6.9/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.6.9/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/chroma.py` & `gpt_index-0.6.9/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/database.py` & `gpt_index-0.6.9/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/deeplake.py` & `gpt_index-0.6.9/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/discord_reader.py` & `gpt_index-0.6.9/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/download.py` & `gpt_index-0.6.9/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/elasticsearch.py` & `gpt_index-0.6.9/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/faiss.py` & `gpt_index-0.6.9/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/base.py` & `gpt_index-0.6.9/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/docs_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/epub_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/image_caption_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/image_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/image_vision_llm_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/ipynb_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/markdown_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/mbox_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/slides_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/tabular_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/file/video_audio_reader.py` & `gpt_index-0.6.9/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/github_readers/github_api_client.py` & `gpt_index-0.6.9/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.6.9/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/github_readers/utils.py` & `gpt_index-0.6.9/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/google_readers/gdocs.py` & `gpt_index-0.6.9/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/google_readers/gsheets.py` & `gpt_index-0.6.9/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/json.py` & `gpt_index-0.6.9/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/make_com/wrapper.py` & `gpt_index-0.6.9/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/mbox.py` & `gpt_index-0.6.9/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/metal.py` & `gpt_index-0.6.9/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/milvus.py` & `gpt_index-0.6.9/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/mongo.py` & `gpt_index-0.6.9/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/myscale.py` & `gpt_index-0.6.9/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/notion.py` & `gpt_index-0.6.9/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/obsidian.py` & `gpt_index-0.6.9/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/pinecone.py` & `gpt_index-0.6.9/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/qdrant.py` & `gpt_index-0.6.9/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/redis/utils.py` & `gpt_index-0.6.9/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/schema/base.py` & `gpt_index-0.6.9/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/slack.py` & `gpt_index-0.6.9/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/steamship/file_reader.py` & `gpt_index-0.6.9/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/string_iterable.py` & `gpt_index-0.6.9/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/twitter.py` & `gpt_index-0.6.9/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/weaviate/client.py` & `gpt_index-0.6.9/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/weaviate/reader.py` & `gpt_index-0.6.9/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/weaviate/utils.py` & `gpt_index-0.6.9/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/web.py` & `gpt_index-0.6.9/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/wikipedia.py` & `gpt_index-0.6.9/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/readers/youtube_transcript.py` & `gpt_index-0.6.9/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/response/notebook_utils.py` & `gpt_index-0.6.9/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/response/pprint_utils.py` & `gpt_index-0.6.9/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/response/schema.py` & `gpt_index-0.6.9/llama_index/response/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         return Response(self.response_txt, self.source_nodes, self.extra_info)
 
     def print_response_stream(self) -> None:
         """Print the response stream."""
         if self.response_txt is None and self.response_gen is not None:
             response_txt = ""
             for text in self.response_gen:
-                print(text, end="")
+                print(text, end="", flush=True)
             self.response_txt = response_txt
         else:
             print(self.response_txt)
 
     def get_formatted_sources(self, length: int = 100) -> str:
         """Get formatted sources text."""
         texts = []
```

### Comparing `gpt_index-0.6.8/llama_index/retrievers/__init__.py` & `gpt_index-0.6.9/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/retrievers/transform_retriever.py` & `gpt_index-0.6.9/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/schema.py` & `gpt_index-0.6.9/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/selectors/llm_selectors.py` & `gpt_index-0.6.9/llama_index/selectors/llm_selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from typing import Any, List, Optional, Sequence, cast
+
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
-
-
 from llama_index.llm_predictor.base import LLMPredictor
 from llama_index.output_parsers.base import BaseOutputParser, StructuredOutput
-from llama_index.output_parsers.selection import (
-    Answer,
-    SelectionOutputParser,
-)
+from llama_index.output_parsers.selection import Answer, SelectionOutputParser
 from llama_index.selectors.prompts import (
     DEFAULT_MULTI_SELECT_PROMPT_TMPL,
     DEFAULT_SINGLE_SELECT_PROMPT_TMPL,
     MultiSelectPrompt,
     SingleSelectPrompt,
 )
 from llama_index.selectors.types import BaseSelector, SelectorResult
```

### Comparing `gpt_index-0.6.8/llama_index/selectors/prompts.py` & `gpt_index-0.6.9/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/selectors/types.py` & `gpt_index-0.6.9/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/__init__.py` & `gpt_index-0.6.9/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.6.9/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.6.9/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/registry.py` & `gpt_index-0.6.9/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/simple_docstore.py` & `gpt_index-0.6.9/llama_index/storage/docstore/simple_docstore.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import fsspec
 from typing import Optional
 from llama_index.storage.docstore.keyval_docstore import KVDocumentStore
 from llama_index.storage.kvstore.simple_kvstore import SimpleKVStore
 from llama_index.storage.kvstore.types import BaseInMemoryKVStore
 from llama_index.storage.docstore.types import (
     DEFAULT_PERSIST_PATH,
     DEFAULT_PERSIST_DIR,
@@ -31,50 +32,55 @@
         super().__init__(simple_kvstore, name_space)
 
     @classmethod
     def from_persist_dir(
         cls,
         persist_dir: str = DEFAULT_PERSIST_DIR,
         namespace: Optional[str] = None,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> "SimpleDocumentStore":
         """Create a SimpleDocumentStore from a persist directory.
 
         Args:
             persist_dir (str): directory to persist the store
             namespace (Optional[str]): namespace for the docstore
+            fs (Optional[fsspec.AbstractFileSystem]): filesystem to use
 
         """
 
         persist_path = os.path.join(persist_dir, DEFAULT_PERSIST_FNAME)
-        return cls.from_persist_path(persist_path, namespace=namespace)
+        return cls.from_persist_path(persist_path, namespace=namespace, fs=fs)
 
     @classmethod
     def from_persist_path(
         cls,
         persist_path: str,
         namespace: Optional[str] = None,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> "SimpleDocumentStore":
         """Create a SimpleDocumentStore from a persist path.
 
         Args:
             persist_path (str): Path to persist the store
             namespace (Optional[str]): namespace for the docstore
+            fs (Optional[fsspec.AbstractFileSystem]): filesystem to use
 
         """
 
-        simple_kvstore = SimpleKVStore.from_persist_path(persist_path)
+        simple_kvstore = SimpleKVStore.from_persist_path(persist_path, fs=fs)
         return cls(simple_kvstore, namespace)
 
     def persist(
         self,
         persist_path: str = DEFAULT_PERSIST_PATH,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> None:
         """Persist the store."""
         if isinstance(self._kvstore, BaseInMemoryKVStore):
-            self._kvstore.persist(persist_path)
+            self._kvstore.persist(persist_path, fs=fs)
 
     @classmethod
     def from_dict(
         cls, save_dict: dict, namespace: Optional[str] = None
     ) -> "SimpleDocumentStore":
         simple_kvstore = SimpleKVStore.from_dict(save_dict)
         return cls(simple_kvstore, namespace)
```

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/types.py` & `gpt_index-0.6.9/llama_index/storage/docstore/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import os
+import fsspec
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional, Sequence
 from llama_index.data_structs.node import Node
 
 from llama_index.schema import BaseDocument
-import os
 
 
 DEFAULT_PERSIST_FNAME = "docstore.json"
 DEFAULT_PERSIST_DIR = "./storage"
 DEFAULT_PERSIST_PATH = os.path.join(DEFAULT_PERSIST_DIR, DEFAULT_PERSIST_FNAME)
 
 
 class BaseDocumentStore(ABC):
     # ===== Save/load =====
-    def persist(self, persist_path: str = DEFAULT_PERSIST_PATH) -> None:
+    def persist(
+        self,
+        persist_path: str = DEFAULT_PERSIST_PATH,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
+    ) -> None:
+        """Persist the docstore to a file."""
         pass
 
     # ===== Main interface =====
     @property
     @abstractmethod
     def docs(self) -> Dict[str, BaseDocument]:
         ...
```

### Comparing `gpt_index-0.6.8/llama_index/storage/docstore/utils.py` & `gpt_index-0.6.9/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.6.9/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.6.9/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/index_store/simple_index_store.py` & `gpt_index-0.6.9/llama_index/storage/index_store/simple_index_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from typing import Optional
+import fsspec
 from llama_index.storage.index_store.keyval_index_store import KVIndexStore
 from llama_index.storage.kvstore.simple_kvstore import SimpleKVStore
 from llama_index.storage.kvstore.types import BaseInMemoryKVStore
 from llama_index.storage.index_store.types import (
     DEFAULT_PERSIST_DIR,
     DEFAULT_PERSIST_FNAME,
     DEFAULT_PERSIST_PATH,
@@ -14,36 +15,51 @@
     """Simple in-memory Index store.
 
     Args:
         simple_kvstore (SimpleKVStore): simple key-value store
 
     """
 
-    def __init__(self, simple_kvstore: Optional[SimpleKVStore] = None) -> None:
+    def __init__(
+        self,
+        simple_kvstore: Optional[SimpleKVStore] = None,
+    ) -> None:
+        """Init a SimpleIndexStore."""
         simple_kvstore = simple_kvstore or SimpleKVStore()
         super().__init__(simple_kvstore)
 
     @classmethod
     def from_persist_dir(
-        cls, persist_dir: str = DEFAULT_PERSIST_DIR
+        cls,
+        persist_dir: str = DEFAULT_PERSIST_DIR,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> "SimpleIndexStore":
         """Create a SimpleIndexStore from a persist directory."""
         persist_path = os.path.join(persist_dir, DEFAULT_PERSIST_FNAME)
-        return cls.from_persist_path(persist_path)
+        return cls.from_persist_path(persist_path, fs=fs)
 
     @classmethod
-    def from_persist_path(cls, persist_path: str) -> "SimpleIndexStore":
+    def from_persist_path(
+        cls,
+        persist_path: str,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
+    ) -> "SimpleIndexStore":
         """Create a SimpleIndexStore from a persist path."""
-        simple_kvstore = SimpleKVStore.from_persist_path(persist_path)
+        fs = fs or fsspec.filesystem("file")
+        simple_kvstore = SimpleKVStore.from_persist_path(persist_path, fs=fs)
         return cls(simple_kvstore)
 
-    def persist(self, persist_path: str = DEFAULT_PERSIST_PATH) -> None:
+    def persist(
+        self,
+        persist_path: str = DEFAULT_PERSIST_PATH,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
+    ) -> None:
         """Persist the store."""
         if isinstance(self._kvstore, BaseInMemoryKVStore):
-            self._kvstore.persist(persist_path)
+            self._kvstore.persist(persist_path, fs=fs)
 
     @classmethod
     def from_dict(cls, save_dict: dict) -> "SimpleIndexStore":
         simple_kvstore = SimpleKVStore.from_dict(save_dict)
         return cls(simple_kvstore)
 
     def to_dict(self) -> dict:
```

### Comparing `gpt_index-0.6.8/llama_index/storage/index_store/utils.py` & `gpt_index-0.6.9/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.6.9/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.6.9/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
+import logging
 import os
 from typing import Dict, Optional
-import logging
 
-from llama_index.storage.kvstore.types import (
-    DEFAULT_COLLECTION,
-    BaseInMemoryKVStore,
-)
+import fsspec
 
+from llama_index.storage.kvstore.types import DEFAULT_COLLECTION, BaseInMemoryKVStore
 
 logger = logging.getLogger(__name__)
 
 DATA_TYPE = Dict[str, Dict[str, dict]]
 
 
 class SimpleKVStore(BaseInMemoryKVStore):
     """Simple in-memory Key-Value store.
 
     Args:
-        persist_path (str): path to persist the store
-
+        data (Optional[DATA_TYPE]): data to initialize the store with
     """
 
-    def __init__(self, data: Optional[DATA_TYPE] = None) -> None:
+    def __init__(
+        self,
+        data: Optional[DATA_TYPE] = None,
+    ) -> None:
         """Init a SimpleKVStore."""
         self._data: DATA_TYPE = data or {}
 
     def put(self, key: str, val: dict, collection: str = DEFAULT_COLLECTION) -> None:
         """Put a key-value pair into the store."""
         if collection not in self._data:
             self._data[collection] = {}
@@ -49,31 +49,34 @@
         """Delete a value from the store."""
         try:
             self._data[collection].pop(key)
             return True
         except KeyError:
             return False
 
-    def persist(self, persist_path: str) -> None:
+    def persist(
+        self, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
+    ) -> None:
         """Persist the store."""
+        fs = fs or fsspec.filesystem("file")
         dirpath = os.path.dirname(persist_path)
-        if not os.path.exists(dirpath):
-            os.makedirs(dirpath)
+        if not fs.exists(dirpath):
+            fs.makedirs(dirpath)
 
-        with open(persist_path, "w+") as f:
-            json.dump(self._data, f)
+        with fs.open(persist_path, "w") as f:
+            f.write(json.dumps(self._data))
 
     @classmethod
-    def from_persist_path(cls, persist_path: str) -> "SimpleKVStore":
-        """Load a SimpleKVStore from a persist path."""
-        if not os.path.exists(persist_path):
-            raise ValueError(f"No existing {__name__} found at {persist_path}.")
-
+    def from_persist_path(
+        cls, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
+    ) -> "SimpleKVStore":
+        """Load a SimpleKVStore from a persist path and filesystem."""
+        fs = fs or fsspec.filesystem("file")
         logger.debug(f"Loading {__name__} from {persist_path}.")
-        with open(persist_path, "r+") as f:
+        with fs.open(persist_path, "rb") as f:
             data = json.load(f)
         return cls(data)
 
     def to_dict(self) -> dict:
         """Save the store as dict."""
         return self._data
```

### Comparing `gpt_index-0.6.8/llama_index/storage/kvstore/types.py` & `gpt_index-0.6.9/llama_index/storage/kvstore/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Optional
+import fsspec
 
 DEFAULT_COLLECTION = "data"
 
 
 class BaseKVStore(ABC):
     """Base key-value store."""
 
@@ -24,14 +25,16 @@
         pass
 
 
 class BaseInMemoryKVStore(BaseKVStore):
     """Base in-memory key-value store."""
 
     @abstractmethod
-    def persist(self, persist_path: str) -> None:
+    def persist(
+        self, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
+    ) -> None:
         pass
 
     @classmethod
     @abstractmethod
     def from_persist_path(cls, persist_path: str) -> "BaseInMemoryKVStore":
         """Create a BaseInMemoryKVStore from a persist directory."""
```

### Comparing `gpt_index-0.6.8/llama_index/storage/storage_context.py` & `gpt_index-0.6.9/llama_index/storage/storage_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from dataclasses import dataclass
-from typing import Optional
 from pathlib import Path
+from typing import Optional
+
+import fsspec
+
 from llama_index.constants import DOC_STORE_KEY, INDEX_STORE_KEY, VECTOR_STORE_KEY
 from llama_index.storage.docstore.simple_docstore import SimpleDocumentStore
-from llama_index.storage.docstore.types import BaseDocumentStore
 from llama_index.storage.docstore.types import DEFAULT_PERSIST_FNAME as DOCSTORE_FNAME
+from llama_index.storage.docstore.types import BaseDocumentStore
+from llama_index.storage.index_store.simple_index_store import SimpleIndexStore
 from llama_index.storage.index_store.types import (
     DEFAULT_PERSIST_FNAME as INDEX_STORE_FNAME,
 )
-from llama_index.vector_stores.simple import DEFAULT_PERSIST_FNAME as VECTOR_STORE_FNAME
-
-from llama_index.storage.index_store.simple_index_store import SimpleIndexStore
 from llama_index.storage.index_store.types import BaseIndexStore
+from llama_index.vector_stores.simple import DEFAULT_PERSIST_FNAME as VECTOR_STORE_FNAME
 from llama_index.vector_stores.simple import SimpleVectorStore
 from llama_index.vector_stores.types import VectorStore
 
 DEFAULT_PERSIST_DIR = "./storage"
 
 
 @dataclass
@@ -37,55 +39,61 @@
     @classmethod
     def from_defaults(
         cls,
         docstore: Optional[BaseDocumentStore] = None,
         index_store: Optional[BaseIndexStore] = None,
         vector_store: Optional[VectorStore] = None,
         persist_dir: Optional[str] = None,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> "StorageContext":
         """Create a StorageContext from defaults.
 
         Args:
             docstore (Optional[BaseDocumentStore]): document store
             index_store (Optional[BaseIndexStore]): index store
             vector_store (Optional[VectorStore]): vector store
 
         """
         if persist_dir is None:
             docstore = docstore or SimpleDocumentStore()
             index_store = index_store or SimpleIndexStore()
             vector_store = vector_store or SimpleVectorStore()
         else:
-            docstore = docstore or SimpleDocumentStore.from_persist_dir(persist_dir)
-            index_store = index_store or SimpleIndexStore.from_persist_dir(persist_dir)
+            docstore = docstore or SimpleDocumentStore.from_persist_dir(
+                persist_dir, fs=fs
+            )
+            index_store = index_store or SimpleIndexStore.from_persist_dir(
+                persist_dir, fs=fs
+            )
             vector_store = vector_store or SimpleVectorStore.from_persist_dir(
-                persist_dir
+                persist_dir, fs=fs
             )
 
         return cls(docstore, index_store, vector_store)
 
     def persist(
         self,
         persist_dir: str = DEFAULT_PERSIST_DIR,
         docstore_fname: str = DOCSTORE_FNAME,
         index_store_fname: str = INDEX_STORE_FNAME,
         vector_store_fname: str = VECTOR_STORE_FNAME,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> None:
         """Persist the storage context.
 
         Args:
             persist_dir (str): directory to persist the storage context
 
         """
         docstore_path = str(Path(persist_dir) / docstore_fname)
         index_store_path = str(Path(persist_dir) / index_store_fname)
         vector_store_path = str(Path(persist_dir) / vector_store_fname)
-        self.docstore.persist(persist_path=docstore_path)
-        self.index_store.persist(persist_path=index_store_path)
-        self.vector_store.persist(persist_path=vector_store_path)
+        self.docstore.persist(persist_path=docstore_path, fs=fs)
+        self.index_store.persist(persist_path=index_store_path, fs=fs)
+        self.vector_store.persist(persist_path=vector_store_path, fs=fs)
 
     def to_dict(self) -> dict:
         all_simple = (
             isinstance(self.vector_store, SimpleVectorStore)
             and isinstance(self.docstore, SimpleDocumentStore)
             and isinstance(self.index_store, SimpleIndexStore)
         )
@@ -107,9 +115,11 @@
     @classmethod
     def from_dict(cls, save_dict: dict) -> "StorageContext":
         """Create a StorageContext from dict."""
         docstore = SimpleDocumentStore.from_dict(save_dict[DOC_STORE_KEY])
         vector_store = SimpleVectorStore.from_dict(save_dict[VECTOR_STORE_KEY])
         index_store = SimpleIndexStore.from_dict(save_dict[INDEX_STORE_KEY])
         return cls(
-            docstore=docstore, index_store=index_store, vector_store=vector_store
+            docstore=docstore,
+            index_store=index_store,
+            vector_store=vector_store,
         )
```

### Comparing `gpt_index-0.6.8/llama_index/token_counter/mock_chain_wrapper.py` & `gpt_index-0.6.9/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/token_counter/mock_embed_model.py` & `gpt_index-0.6.9/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/token_counter/token_counter.py` & `gpt_index-0.6.9/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/token_counter/utils.py` & `gpt_index-0.6.9/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/tools/query_engine.py` & `gpt_index-0.6.9/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/tts/bark.py` & `gpt_index-0.6.9/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/tts/base.py` & `gpt_index-0.6.9/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/tts/elevenlabs.py` & `gpt_index-0.6.9/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/utils.py` & `gpt_index-0.6.9/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/__init__.py` & `gpt_index-0.6.9/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.6.9/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/chroma.py` & `gpt_index-0.6.9/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/deeplake.py` & `gpt_index-0.6.9/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/lancedb.py` & `gpt_index-0.6.9/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/metal.py` & `gpt_index-0.6.9/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/milvus.py` & `gpt_index-0.6.9/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/myscale.py` & `gpt_index-0.6.9/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/opensearch.py` & `gpt_index-0.6.9/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/pinecone.py` & `gpt_index-0.6.9/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/qdrant.py` & `gpt_index-0.6.9/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/redis.py` & `gpt_index-0.6.9/llama_index/vector_stores/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Redis Vector store index.
 
 An index that that is built on top of an existing vector store.
 """
 import logging
+import fsspec
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.readers.redis.utils import (
     TokenEscaper,
     array_to_buffer,
     check_redis_modules_exist,
@@ -247,20 +248,27 @@
             ids.append(doc.id)
             nodes.append(node)
             scores.append(1 - float(doc.vector_score))
         _logger.info(f"Found {len(nodes)} results for query with id {ids}")
 
         return VectorStoreQueryResult(nodes=nodes, ids=ids, similarities=scores)
 
-    def persist(self, persist_path: str, in_background: bool = True) -> None:
+    def persist(
+        self,
+        persist_path: str,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
+        in_background: bool = True,
+    ) -> None:
         """Persist the vector store to disk.
 
         Args:
             persist_path (str): Path to persist the vector store to. (doesn't apply)
             in_background (bool, optional): Persist in background. Defaults to True.
+            fs (fsspec.AbstractFileSystem, optional): Filesystem to persist to.
+                (doesn't apply)
 
         Raises:
             redis.exceptions.RedisError: If there is an error
                                          persisting the index to disk.
         """
         from redis.exceptions import RedisError
```

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/registry.py` & `gpt_index-0.6.9/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/simple.py` & `gpt_index-0.6.9/llama_index/vector_stores/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Simple vector store index."""
 
 import json
 import logging
 import os
+import fsspec
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, cast
 
 from dataclasses_json import DataClassJsonMixin
 
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
@@ -57,25 +58,30 @@
     """
 
     stores_text: bool = False
 
     def __init__(
         self,
         data: Optional[SimpleVectorStoreData] = None,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._data = data or SimpleVectorStoreData()
+        self._fs = fs or fsspec.filesystem("file")
 
     @classmethod
     def from_persist_dir(
-        cls, persist_dir: str = DEFAULT_PERSIST_DIR
+        cls,
+        persist_dir: str = DEFAULT_PERSIST_DIR,
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> "SimpleVectorStore":
+        """Load from persist dir."""
         persist_path = os.path.join(persist_dir, DEFAULT_PERSIST_FNAME)
-        return cls.from_persist_path(persist_path)
+        return cls.from_persist_path(persist_path, fs=fs)
 
     @property
     def client(self) -> None:
         """Get client."""
         return None
 
     def get(self, text_id: str) -> List[float]:
@@ -139,33 +145,38 @@
             raise ValueError(f"Invalid query mode: {query.mode}")
 
         return VectorStoreQueryResult(similarities=top_similarities, ids=top_ids)
 
     def persist(
         self,
         persist_path: str = os.path.join(DEFAULT_PERSIST_DIR, DEFAULT_PERSIST_FNAME),
+        fs: Optional[fsspec.AbstractFileSystem] = None,
     ) -> None:
         """Persist the SimpleVectorStore to a directory."""
+        fs = fs or self._fs
         dirpath = os.path.dirname(persist_path)
-        if not os.path.exists(dirpath):
-            os.makedirs(dirpath)
+        if not fs.exists(dirpath):
+            fs.makedirs(dirpath)
 
-        with open(persist_path, "w+") as f:
+        with fs.open(persist_path, "w") as f:
             json.dump(self._data.to_dict(), f)
 
     @classmethod
-    def from_persist_path(cls, persist_path: str) -> "SimpleVectorStore":
+    def from_persist_path(
+        cls, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
+    ) -> "SimpleVectorStore":
         """Create a SimpleKVStore from a persist directory."""
-        if not os.path.exists(persist_path):
+        fs = fs or fsspec.filesystem("file")
+        if not fs.exists(persist_path):
             raise ValueError(
                 f"No existing {__name__} found at {persist_path}, skipping load."
             )
 
         logger.debug(f"Loading {__name__} from {persist_path}.")
-        with open(persist_path, "r+") as f:
+        with fs.open(persist_path, "rb") as f:
             data_dict = json.load(f)
             data = SimpleVectorStoreData.from_dict(data_dict)
         return cls(data)
 
     @classmethod
     def from_dict(cls, save_dict: dict) -> "SimpleVectorStore":
         data = SimpleVectorStoreData.from_dict(save_dict)
```

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/types.py` & `gpt_index-0.6.9/llama_index/vector_stores/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Vector store index types."""
-
-
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, List, Optional, Protocol, Union, runtime_checkable
 
+import fsspec
 from pydantic import BaseModel
 
 from llama_index.data_structs.node import Node
 
 DEFAULT_PERSIST_DIR = "./storage"
 DEFAULT_PERSIST_FNAME = "vector_store.json"
 
@@ -148,9 +147,11 @@
         """Delete doc."""
         ...
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query vector store."""
         ...
 
-    def persist(self, persist_path: str) -> None:
+    def persist(
+        self, persist_path: str, fs: Optional[fsspec.AbstractFileSystem] = None
+    ) -> None:
         return None
```

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/utils.py` & `gpt_index-0.6.9/llama_index/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/llama_index/vector_stores/weaviate.py` & `gpt_index-0.6.9/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/setup.py` & `gpt_index-0.6.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "dataclasses_json",
     "langchain>=0.0.154",
     "numpy",
     "tenacity>=8.2.0,<9.0.0",
     "openai>=0.26.4",
     "pandas",
     "requests<2.30.0",
+    "fsspec>=2023.5.0",
 ]
 
 # NOTE: if python version >= 3.9, install tiktoken
 # else install transformers
 if sys.version_info >= (3, 9):
     install_requires.extend(["tiktoken"])
 else:
```

### Comparing `gpt_index-0.6.8/tests/callbacks/test_llama_debug.py` & `gpt_index-0.6.9/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/conftest.py` & `gpt_index-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/embeddings/test_base.py` & `gpt_index-0.6.9/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/composability/test_utils.py` & `gpt_index-0.6.9/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/conftest.py` & `gpt_index-0.6.9/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/document_summary/test_index.py` & `gpt_index-0.6.9/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/empty/test_base.py` & `gpt_index-0.6.9/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/keyword_table/test_base.py` & `gpt_index-0.6.9/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.6.9/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.6.9/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.6.9/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.6.9/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/list/test_index.py` & `gpt_index-0.6.9/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/list/test_retrievers.py` & `gpt_index-0.6.9/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/postprocessor/test_base.py` & `gpt_index-0.6.9/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/postprocessor/test_llm_rerank.py` & `gpt_index-0.6.9/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/query/conftest.py` & `gpt_index-0.6.9/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.6.9/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/query/test_compose.py` & `gpt_index-0.6.9/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/query/test_compose_vector.py` & `gpt_index-0.6.9/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/query/test_query_bundle.py` & `gpt_index-0.6.9/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/struct_store/conftest.py` & `gpt_index-0.6.9/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/struct_store/test_base.py` & `gpt_index-0.6.9/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/struct_store/test_pandas.py` & `gpt_index-0.6.9/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.6.9/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/test_loading.py` & `gpt_index-0.6.9/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/test_loading_graph.py` & `gpt_index-0.6.9/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/test_node_utils.py` & `gpt_index-0.6.9/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/test_prompt_helper.py` & `gpt_index-0.6.9/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/tree/conftest.py` & `gpt_index-0.6.9/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.6.9/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/tree/test_index.py` & `gpt_index-0.6.9/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/tree/test_retrievers.py` & `gpt_index-0.6.9/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `gpt_index-0.6.9/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/conftest.py` & `gpt_index-0.6.9/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.6.9/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/mock_services.py` & `gpt_index-0.6.9/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.6.9/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.6.9/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.6.9/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.6.9/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/test_simple.py` & `gpt_index-0.6.9/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/indices/vector_store/utils.py` & `gpt_index-0.6.9/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.6.9/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/llm_predictor/test_base.py` & `gpt_index-0.6.9/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/logger/test_base.py` & `gpt_index-0.6.9/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/mock_utils/mock_predict.py` & `gpt_index-0.6.9/tests/mock_utils/mock_predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,28 @@
     ]
     max_outputs = prompt_args["max_outputs"]
     answers = answers[:max_outputs]
 
     return json.dumps(answers)
 
 
+def _mock_sub_questions() -> str:
+    """Mock sub questions."""
+    json_str = json.dumps(
+        [
+            {
+                "sub_question": "mock question for source_1",
+                "tool_name": "source_1",
+            }
+        ],
+        indent=4,
+    )
+    return f"```json\n{json_str}\n```"
+
+
 def _mock_answer(prompt_args: Dict) -> str:
     """Mock answer."""
     return prompt_args["query_str"] + ":" + prompt_args["context_str"]
 
 
 def _mock_refine(prompt_args: Dict) -> str:
     """Mock refine."""
@@ -161,14 +175,16 @@
         response = _mock_kg_triplet_extract(full_prompt_args)
     elif prompt.prompt_type == PromptType.SIMPLE_INPUT:
         response = _mock_input(full_prompt_args)
     elif prompt.prompt_type == PromptType.SINGLE_SELECT:
         response = _mock_single_select()
     elif prompt.prompt_type == PromptType.MULTI_SELECT:
         response = _mock_multi_select(full_prompt_args)
+    elif prompt.prompt_type == PromptType.SUB_QUESTION:
+        response = _mock_sub_questions()
     elif prompt.prompt_type == PromptType.CUSTOM:
         if isinstance(prompt, DecomposeQueryTransformPrompt):
             response = _mock_decompose_query(full_prompt_args)
         elif isinstance(prompt, ChoiceSelectPrompt):
             response = _mock_choice_select(full_prompt_args)
         else:
             raise ValueError("Invalid prompt to use with mocks.")
@@ -214,14 +230,16 @@
         response = _mock_kg_triplet_extract(full_prompt_args)
     elif prompt.prompt_type == PromptType.SIMPLE_INPUT:
         response = _mock_input(full_prompt_args)
     elif prompt.prompt_type == PromptType.SINGLE_SELECT:
         response = _mock_single_select()
     elif prompt.prompt_type == PromptType.MULTI_SELECT:
         response = _mock_multi_select(full_prompt_args)
+    elif prompt.prompt_type == PromptType.SUB_QUESTION:
+        response = _mock_sub_questions()
     elif prompt.prompt_type == PromptType.CUSTOM:
         if isinstance(prompt, DecomposeQueryTransformPrompt):
             response = _mock_decompose_query(full_prompt_args)
         elif isinstance(prompt, ChoiceSelectPrompt):
             response = _mock_choice_select(full_prompt_args)
         else:
             raise ValueError("Invalid prompt to use with mocks.")
```

### Comparing `gpt_index-0.6.8/tests/mock_utils/mock_prompts.py` & `gpt_index-0.6.9/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.6.9/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/mock_utils/mock_utils.py` & `gpt_index-0.6.9/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/optimization/test_base.py` & `gpt_index-0.6.9/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/output_parsers/test_base.py` & `gpt_index-0.6.9/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/output_parsers/test_selection.py` & `gpt_index-0.6.9/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/playground/test_base.py` & `gpt_index-0.6.9/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/prompts/test_base.py` & `gpt_index-0.6.9/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/readers/test_file.py` & `gpt_index-0.6.9/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/readers/test_json.py` & `gpt_index-0.6.9/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/readers/test_mongo.py` & `gpt_index-0.6.9/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/selectors/test_llm_selectors.py` & `gpt_index-0.6.9/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/storage/conftest.py` & `gpt_index-0.6.9/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.6.9/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.6.9/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/storage/test_storage_context.py` & `gpt_index-0.6.9/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/test_utils.py` & `gpt_index-0.6.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/token_predictor/test_base.py` & `gpt_index-0.6.9/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/vector_stores/test_qdrant.py` & `gpt_index-0.6.9/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.8/tests/vector_stores/test_weaviate.py` & `gpt_index-0.6.9/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

