# Comparing `tmp/gptcache-0.1.8.tar.gz` & `tmp/gptcache-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptcache-0.1.8.tar", last modified: Tue Apr 11 15:26:01 2023, max compression
+gzip compressed data, was "gptcache-0.1.9.tar", last modified: Wed Apr 12 15:07:23 2023, max compression
```

## Comparing `gptcache-0.1.8.tar` & `gptcache-0.1.9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.326631 gptcache-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-11 15:25:50.000000 gptcache-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-11 15:26:01.326631 gptcache-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-11 15:25:50.000000 gptcache-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache/
--rw-r--r--   0 runner    (1001) docker     (122)     6022 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache/adapter/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/langchain_llms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/adapter/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/embedding/
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/cohere.py
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/openai.py
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/sbert.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/embedding/string.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/eviction.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/scalar_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/scalar_data/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/manager/vector_data/
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/chroma.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/faiss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/hnswlib_store.py
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/manager/vector_data/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/processor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/post.py
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/processor/pre.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.322631 gptcache-0.1.8/gptcache/similarity_evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/np.py
--rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/similarity_evaluation/similarity_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.326631 gptcache-0.1.8/gptcache/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/dependency_control.py
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-11 15:25:50.000000 gptcache-0.1.8/gptcache/utils/lazy_import.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 15:26:01.318631 gptcache-0.1.8/gptcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16700 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 15:26:01.000000 gptcache-0.1.8/gptcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 15:26:01.326631 gptcache-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-11 15:25:50.000000 gptcache-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.063656 gptcache-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-12 15:07:10.000000 gptcache-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    16698 2023-04-12 15:07:23.063656 gptcache-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16162 2023-04-12 15:07:10.000000 gptcache-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.055656 gptcache-0.1.9/gptcache/
+-rw-r--r--   0 runner    (1001) docker     (122)     6756 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache/adapter/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4009 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/adapter/langchain_llms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/adapter/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache/embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/embedding/string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache/manager/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache/manager/scalar_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/scalar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/scalar_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/scalar_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5338 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/scalar_data/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache/manager/vector_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/hnswlib_store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5971 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/manager/vector_data/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.063656 gptcache-0.1.9/gptcache/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/processor/post.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/processor/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.063656 gptcache-0.1.9/gptcache/similarity_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/np.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4633 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/similarity_evaluation/similarity_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.063656 gptcache-0.1.9/gptcache/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2267 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/utils/dependency_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/utils/lazy_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-12 15:07:10.000000 gptcache-0.1.9/gptcache/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 15:07:23.059656 gptcache-0.1.9/gptcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16698 2023-04-12 15:07:23.000000 gptcache-0.1.9/gptcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-04-12 15:07:23.000000 gptcache-0.1.9/gptcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 15:07:23.000000 gptcache-0.1.9/gptcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-12 15:07:23.000000 gptcache-0.1.9/gptcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 15:07:23.000000 gptcache-0.1.9/gptcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 15:07:23.063656 gptcache-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-04-12 15:07:10.000000 gptcache-0.1.9/setup.py
```

### Comparing `gptcache-0.1.8/LICENSE` & `gptcache-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/PKG-INFO` & `gptcache-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.8
-Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
+Version: 0.1.9
+Summary: GPTCache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPTCache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -244,15 +244,15 @@
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
   - [x] Support langchain.
-  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMa.
+  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMA.
 - **Embedding Generator**: 
 This module is created to extract embeddings from requests for similarity search. GPTCache offers a generic interface that supports multiple embedding APIs, and presents a range of solutions to choose from. 
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
```

### Comparing `gptcache-0.1.8/README.md` & `gptcache-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
   - [x] Support langchain.
-  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMa.
+  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMA.
 - **Embedding Generator**: 
 This module is created to extract embeddings from requests for similarity search. GPTCache offers a generic interface that supports multiple embedding APIs, and presents a range of solutions to choose from. 
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
```

### Comparing `gptcache-0.1.8/gptcache/__init__.py` & `gptcache-0.1.9/gptcache/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import atexit
 import os
 import time
+from typing import List, Any, Optional, Callable
+
 import openai
 
 from gptcache.embedding.string import to_embeddings as string_embedding
 from gptcache.manager.data_manager import DataManager
 from gptcache.manager.factory import get_data_manager
 from gptcache.processor.post import first
 from gptcache.processor.pre import last_content
@@ -46,22 +48,26 @@
 
             from gptcache import Config
 
             configs = Config(similarity_threshold=0.6)
     """
 
     def __init__(
-        self,
-        log_time_func=None,
-        similarity_threshold=0.8,
+            self,
+            log_time_func: Optional[Callable[[str, float], None]] = None,
+            similarity_threshold: float = 0.8,
+            prompts: Optional[List[str]] = None
     ):
         if similarity_threshold < 0 or similarity_threshold > 1:
-            raise CacheError("Invalid the similarity threshold param, reasonable range: 0-1")
+            raise CacheError(
+                "Invalid the similarity threshold param, reasonable range: 0-1"
+            )
         self.log_time_func = log_time_func
         self.similarity_threshold = similarity_threshold
+        self.prompts = prompts
 
 
 class Report:
     """Get GPTCache report including time and counts for different operations."""
 
     def __init__(self):
         self.embedding_all_time = 0
@@ -130,30 +136,30 @@
 
     # it should be called when start the cache system
     def __init__(self):
         self.has_init = False
         self.cache_enable_func = None
         self.pre_embedding_func = None
         self.embedding_func = None
-        self.data_manager = None
+        self.data_manager: Optional[DataManager] = None
         self.post_process_messages_func = None
         self.config = Config()
         self.report = Report()
         self.next_cache = None
 
     def init(
-        self,
-        cache_enable_func=cache_all,
-        pre_embedding_func=last_content,
-        embedding_func=string_embedding,
-        data_manager: DataManager = get_data_manager(),
-        similarity_evaluation=ExactMatchEvaluation(),
-        post_process_messages_func=first,
-        config=Config(),
-        next_cache=None,
+            self,
+            cache_enable_func=cache_all,
+            pre_embedding_func=last_content,
+            embedding_func=string_embedding,
+            data_manager: DataManager = get_data_manager(),
+            similarity_evaluation=ExactMatchEvaluation(),
+            post_process_messages_func=first,
+            config=Config(),
+            next_cache=None,
     ):
         """Pass parameters to initialize GPTCache.
 
         :param cache_enable_func: a function to enable cache, defaults to ``cache_all``
         :param pre_embedding_func: a function to preprocess embedding, defaults to ``last_content``
         :param embedding_func: a function to extract embeddings from requests for similarity search, defaults to ``string_embedding``
         :param data_manager: a ``DataManager`` module, defaults to ``get_data_manager()``
@@ -175,13 +181,26 @@
         @atexit.register
         def close():
             try:
                 self.data_manager.close()
             except Exception as e:  # pylint: disable=W0703
                 print(e)
 
+    def import_data(self, questions: List[Any], answers: List[Any]) -> None:
+        """ Import data to GPTCache
+
+        :param questions: preprocessed question Data
+        :param answers: list of answers to questions
+        :return: None
+        """
+        self.data_manager.import_data(
+            questions=questions,
+            answers=answers,
+            embedding_datas=[self.embedding_func(question) for question in questions],
+        )
+
     @staticmethod
     def set_openai_key():
         openai.api_key = os.getenv("OPENAI_API_KEY")
 
 
 cache = Cache()
```

### Comparing `gptcache-0.1.8/gptcache/adapter/adapter.py` & `gptcache-0.1.9/gptcache/adapter/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     cache_enable = chat_cache.cache_enable_func(*args, **kwargs)
     context = kwargs.pop("cache_context", {})
     embedding_data = None
     # you want to retry to send the request to chatgpt when the cache is negative
     cache_skip = kwargs.pop("cache_skip", False)
     cache_factor = kwargs.pop("cache_factor", 1.0)
     pre_embedding_data = chat_cache.pre_embedding_func(
-        kwargs, extra_param=context.get("pre_embedding_func", None)
+        kwargs,
+        extra_param=context.get("pre_embedding_func", None),
+        prompts=chat_cache.config.prompts,
     )
     if cache_enable:
         embedding_data = time_cal(
             chat_cache.embedding_func,
             func_name="embedding",
             report_func=chat_cache.report.embedding,
         )(pre_embedding_data, extra_param=context.get("embedding_func", None))
```

### Comparing `gptcache-0.1.8/gptcache/adapter/langchain_llms.py` & `gptcache-0.1.9/gptcache/adapter/langchain_llms.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/adapter/openai.py` & `gptcache-0.1.9/gptcache/adapter/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 from typing import Iterator
 
 import openai
 
 from gptcache.adapter.adapter import adapt
+from gptcache.utils.response import get_message_from_openai_answer, get_stream_message_from_openai_answer
 
 
 class ChatCompletion:
     """Openai ChatCompletion Wrapper"""
 
     @classmethod
     def create(cls, *args, **kwargs):
@@ -79,15 +80,7 @@
         {
             "gptcache": True,
             "choices": [{"delta": {}, "finish_reason": "stop", "index": 0}],
             "created": created,
             "object": "chat.completion.chunk",
         },
     ]
-
-
-def get_message_from_openai_answer(openai_data):
-    return openai_data["choices"][0]["message"]["content"]
-
-
-def get_stream_message_from_openai_answer(openai_data):
-    return openai_data["choices"][0]["delta"].get("content", "")
```

### Comparing `gptcache-0.1.8/gptcache/embedding/__init__.py` & `gptcache-0.1.9/gptcache/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/cohere.py` & `gptcache-0.1.9/gptcache/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/fasttext.py` & `gptcache-0.1.9/gptcache/embedding/fasttext.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/huggingface.py` & `gptcache-0.1.9/gptcache/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/onnx.py` & `gptcache-0.1.9/gptcache/embedding/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/openai.py` & `gptcache-0.1.9/gptcache/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/embedding/sbert.py` & `gptcache-0.1.9/gptcache/embedding/sbert.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/manager/data_manager.py` & `gptcache-0.1.9/gptcache/manager/data_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from abc import abstractmethod, ABCMeta
 import pickle
+from typing import List, Any
+
 import cachetools
 import numpy as np
 
-from gptcache.utils.error import CacheError
-from gptcache.manager.scalar_data.base import CacheStorage
-from gptcache.manager.vector_data.base import VectorBase, ClearStrategy
+from gptcache.utils.error import CacheError, ParamError
+from gptcache.manager.scalar_data.base import CacheStorage, CacheData
+from gptcache.manager.vector_data.base import VectorBase, VectorData
 from gptcache.manager.eviction import EvictionManager
 
 
 class DataManager(metaclass=ABCMeta):
     """DataManager manage the cache data, including save and search"""
 
     @abstractmethod
     def save(self, question, answer, embedding_data, **kwargs):
         pass
 
+    @abstractmethod
+    def import_data(
+        self, questions: List[Any], answers: List[Any], embedding_datas: List[Any]
+    ):
+        pass
+
     # should return the tuple, (question, answer)
     @abstractmethod
     def get_scalar_data(self, res_data, **kwargs):
         pass
 
     @abstractmethod
     def search(self, embedding_data, **kwargs):
@@ -45,35 +53,43 @@
         try:
             with open(self.data_path, "rb") as f:
                 self.data = pickle.load(f)
         except FileNotFoundError:
             return
         except PermissionError:
             raise CacheError(  # pylint: disable=W0707
-                f"You don't have permission to access this file <${self.data_path}>."
+                f"You don't have permission to access this file <{self.data_path}>."
             )
 
     def save(self, question, answer, embedding_data, **kwargs):
         self.data[embedding_data] = (question, answer)
 
+    def import_data(
+        self, questions: List[Any], answers: List[Any], embedding_datas: List[Any]
+    ):
+        if len(questions) != len(answers) or len(questions) != len(embedding_datas):
+            raise ParamError("Make sure that all parameters have the same length")
+        for i, embedding_data in enumerate(embedding_datas):
+            self.data[embedding_data] = (questions[i], answers[i])
+
     def get_scalar_data(self, res_data, **kwargs):
         return res_data
 
     def search(self, embedding_data, **kwargs):
         try:
             return [self.data[embedding_data]]
         except KeyError:
             return []
 
     def close(self):
         try:
             with open(self.data_path, "wb") as f:
                 pickle.dump(self.data, f)
         except PermissionError:
-            print(f"You don't have permission to access this file <${self.data_path}>.")
+            print(f"You don't have permission to access this file <{self.data_path}>.")
 
 
 def normalize(vec):
     magnitude = np.linalg.norm(vec)
     normalized_v = vec / magnitude
     return normalized_v
 
@@ -103,22 +119,16 @@
         self.s = s
         self.v = v
         self.eviction = EvictionManager(self.s, self.v, eviction)
         self.cur_size = self.s.count()
 
     def _clear(self):
         self.eviction.soft_evict(self.clean_size)
-        if not self.eviction.check_evict():
-            pass
-        elif self.v.clear_strategy() == ClearStrategy.DELETE:
+        if self.eviction.check_evict():
             self.eviction.delete()
-        elif self.v.clear_strategy() == ClearStrategy.REBUILD:
-            self.eviction.rebuild()
-        else:
-            raise RuntimeError("Unknown clear strategy")
         self.cur_size = self.s.count()
 
     def save(self, question, answer, embedding_data, **kwargs):
         """Save the data and vectors to cache and vector storage.
 
         :param question: question data.
         :type question: str
@@ -135,21 +145,42 @@
 
                 data_manager = get_data_manager(CacheBase('sqlite'), VectorBase('faiss', dimension=128))
                 data_manager.save('hello', 'hi', np.random.random((128, )).astype('float32'))
         """
 
         if self.cur_size >= self.max_size:
             self._clear()
-        embedding_data = normalize(embedding_data)
-        if self.v.clear_strategy() == ClearStrategy.DELETE:
-            key = self.s.insert(question, answer)
-        elif self.v.clear_strategy() == ClearStrategy.REBUILD:
-            key = self.s.insert(question, answer, embedding_data.astype("float32"))
-        self.v.add(key, embedding_data)
-        self.cur_size += 1
+
+        self.import_data([question], [answer], [embedding_data])
+
+    def import_data(
+        self, questions: List[Any], answers: List[Any], embedding_datas: List[Any]
+    ):
+        if len(questions) != len(answers) or len(questions) != len(embedding_datas):
+            raise ParamError("Make sure that all parameters have the same length")
+        cache_datas = []
+        embedding_datas = [
+            normalize(embedding_data) for embedding_data in embedding_datas
+        ]
+        for i, embedding_data in enumerate(embedding_datas):
+            cache_datas.append(
+                CacheData(
+                    question=questions[i],
+                    answer=answers[i],
+                    embedding_data=embedding_data.astype("float32"),
+                )
+            )
+        ids = self.s.batch_insert(cache_datas)
+        self.v.mul_add(
+            [
+                VectorData(id=ids[i], data=embedding_data)
+                for i, embedding_data in enumerate(embedding_datas)
+            ]
+        )
+        self.cur_size += len(questions)
 
     def get_scalar_data(self, res_data, **kwargs):
         return self.s.get_data_by_id(res_data[1])
 
     def search(self, embedding_data, **kwargs):
         embedding_data = normalize(embedding_data)
         return self.v.search(embedding_data)
```

### Comparing `gptcache-0.1.8/gptcache/manager/eviction.py` & `gptcache-0.1.9/gptcache/manager/eviction.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/manager/factory.py` & `gptcache-0.1.9/gptcache/manager/factory.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/manager/scalar_data/__init__.py` & `gptcache-0.1.9/gptcache/manager/scalar_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/manager/scalar_data/manager.py` & `gptcache-0.1.9/gptcache/manager/scalar_data/manager.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/manager/scalar_data/sqlalchemy.py` & `gptcache-0.1.9/gptcache/manager/scalar_data/sqlalchemy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import numpy as np
+from typing import List
+
 from datetime import datetime
 
 from gptcache.utils import import_sqlalchemy
-from gptcache.manager.scalar_data.base import CacheStorage
+from gptcache.manager.scalar_data.base import CacheStorage, CacheData
 
 import_sqlalchemy()
 
 from sqlalchemy import func, create_engine, Column, Sequence  # pylint: disable=C0413
 from sqlalchemy.types import (  # pylint: disable=C0413
     String,
     DateTime,
@@ -25,16 +26,16 @@
         cache_table
         """
 
         __tablename__ = table_name
         __table_args__ = {"extend_existing": True}
 
         id = Column(Integer, primary_key=True, autoincrement=True)
-        data = Column(String(1000), nullable=False)
-        reply = Column(String(1000), nullable=False)
+        question = Column(String(1000), nullable=False)
+        answer = Column(String(1000), nullable=False)
         create_on = Column(DateTime, default=datetime.now)
         last_access = Column(DateTime, default=datetime.now)
         embedding_data = Column(LargeBinary, nullable=True)
         state = Column(Integer, default=0)
         type = Column(Integer, default=0)
 
     class CacheTableSequence(Base):
@@ -44,16 +45,16 @@
 
         __tablename__ = table_name
         __table_args__ = {"extend_existing": True}
 
         id = Column(
             Integer, Sequence("id_seq", start=1), primary_key=True, autoincrement=True
         )
-        data = Column(String(1000), nullable=False)
-        reply = Column(String(1000), nullable=False)
+        question = Column(String(1000), nullable=False)
+        answer = Column(String(1000), nullable=False)
         create_on = Column(DateTime, default=datetime.now)
         last_access = Column(DateTime, default=datetime.now)
         embedding_data = Column(LargeBinary, nullable=True)
         state = Column(Integer, default=0)
         type = Column(Integer, default=0)
 
     if db_type == "oracle":
@@ -64,42 +65,48 @@
 
 class SQLDataBase(CacheStorage):
     """
     Using sqlalchemy to manage SQLite, PostgreSQL, MySQL, MariaDB, SQL Server and Oracle.
     """
 
     def __init__(
-            self,
-            db_type: str = "sqlite",
-            url: str = "sqlite:///./sqlite.db",
-            table_name: str = "gptcache",
+        self,
+        db_type: str = "sqlite",
+        url: str = "sqlite:///./sqlite.db",
+        table_name: str = "gptcache",
     ):
         self._url = url
         self._model = get_model(table_name, db_type)
         self._engine = create_engine(self._url)
         Session = sessionmaker(bind=self._engine)  # pylint: disable=invalid-name
         self._session = Session()
         self.create()
 
     def create(self):
         self._model.__table__.create(bind=self._engine, checkfirst=True)
 
-    def insert(self, data, reply, embedding_data: np.ndarray = None):
-        if embedding_data is None:
-            model_obj = self._model(data=data, reply=reply)
-        else:
-            embedding_data = embedding_data.tobytes()
-            model_obj = self._model(data=data, reply=reply, embedding_data=embedding_data)
-        self._session.add(model_obj)
+    def batch_insert(self, datas: List[CacheData]):
+        model_objs = []
+        for data in datas:
+            model_obj = self._model(
+                question=data.question,
+                answer=data.answer,
+                embedding_data=data.embedding_data.tobytes()
+                if data.embedding_data is not None
+                else None,
+            )
+            model_objs.append(model_obj)
+
+        self._session.add_all(model_objs)
         self._session.commit()
-        return model_obj.id
+        return [model_obj.id for model_obj in model_objs]
 
     def get_data_by_id(self, key):
         res = (
-            self._session.query(self._model.data, self._model.reply)
+            self._session.query(self._model.question, self._model.answer)
             .filter(self._model.id == key)
             .filter(self._model.state == 0)
             .first()
         )
         return res
 
     def get_ids_by_state(self, state):
```

### Comparing `gptcache-0.1.8/gptcache/manager/vector_data/__init__.py` & `gptcache-0.1.9/gptcache/manager/vector_data/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     :param secure: whether it is https with Zilliz Cloud, defaults to False.
     :type secures: bool.
     :param index_params: the index parameters for Milvus, defaults to the HNSW index: {'metric_type': 'L2', 'index_type': 'HNSW', 'params': {'M':
                          8, 'efConstruction': 64}}.
     :type index_params: dict
     :param collection_name: the name of the collection for Milvus vector database, defaults to 'gptcache'.
     :type collection_name: str.
+    :param local_mode: if true, will start a local mivlus server.
+    :type local_mode: bool.
+    :param local_data: required when local_mode is True.
+    :type local_data: str.
 
     :param index_path: the path to hnswlib index, defaults to 'hnswlib_index.bin'.
     :type index_path: str.
     :param max_elements: max_elements of hnswlib, defaults 100000.
     :type max_elements: int.
     """
     return vector_manager.VectorBase.get(name, **kwargs)
```

### Comparing `gptcache-0.1.8/gptcache/manager/vector_data/base.py` & `gptcache-0.1.9/gptcache/manager/scalar_data/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,62 @@
-from abc import ABC, abstractmethod
-from enum import Enum
+from abc import ABCMeta, abstractmethod
+from dataclasses import dataclass
+from typing import Optional, Any, List
 
+import numpy as np
 
-class ClearStrategy(Enum):
-    REBUILD = 0
-    DELETE = 1
 
+@dataclass
+class CacheData:
+    question: Any
+    answer: Any
+    embedding_data: Optional[np.ndarray] = None
 
-class VectorBase(ABC):
-    """VectorBase: base vector store interface"""
+
+class CacheStorage(metaclass=ABCMeta):
+    """
+    BaseStorage for scalar data.
+    """
+
+    @abstractmethod
+    def create(self):
+        pass
+
+    @abstractmethod
+    def batch_insert(self, datas: List[CacheData]):
+        pass
+
+    @abstractmethod
+    def get_data_by_id(self, key):
+        pass
 
     @abstractmethod
-    def add(self, key: str, data: "ndarray"):
+    def get_embedding_data(self, offset, size):
         pass
 
     @abstractmethod
-    def search(self, data: "ndarray"):
+    def remove_by_state(self):
         pass
 
     @abstractmethod
-    def clear_strategy(self):
+    def update_access_time(self, key):
         pass
 
-    def rebuild(self) -> bool:
-        raise NotImplementedError
+    @abstractmethod
+    def update_state(self, keys):
+        pass
+
+    @abstractmethod
+    def count(self):
+        pass
 
-    def delete(self, ids) -> bool:
-        raise NotImplementedError
+    @abstractmethod
+    def get_old_access(self, count):
+        pass
+
+    @abstractmethod
+    def get_old_create(self, count):
+        pass
 
     @abstractmethod
     def close(self):
         pass
```

### Comparing `gptcache-0.1.8/gptcache/manager/vector_data/hnswlib_store.py` & `gptcache-0.1.9/gptcache/manager/vector_data/hnswlib_store.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 import os
+from typing import List
+
 import numpy as np
 
-from gptcache.manager.vector_data.base import VectorBase, ClearStrategy
+from gptcache.manager.vector_data.base import VectorBase, VectorData
 from gptcache.utils import import_hnswlib
 
 import_hnswlib()
 
 import hnswlib  # pylint: disable=C0413
 
 
 class Hnswlib(VectorBase):
     """vector store: hnswlib"""
 
-    def __init__(self, index_file_path: int, top_k: str, dimension: int, max_elements: int):
+    def __init__(self, index_file_path: str, dimension: int, top_k: int, max_elements: int):
         self._index_file_path = index_file_path
         self._dimension = dimension
         self._max_elements = max_elements
         self._index =  hnswlib.Index(space="l2", dim=self._dimension)
         self._top_k = top_k
         if os.path.isfile(self._index_file_path):
             self._index.load_index(self._index_file_path, max_elements=max_elements)
         else:
             self._index.init_index(max_elements=max_elements, ef_construction=100, M=16)
             self._index.set_ef(self._top_k * 2)
 
-    def add(self, key: int, data: "ndarray"):
+    def add(self, key: int, data: np.ndarray):
         np_data = np.array(data).astype("float32").reshape(1, -1)
-        self._index.add_items(np_data, np.asarray([key]))
+        self._index.add_items(np_data, np.array([key]))
 
-    def _mult_add(self, data, keys):
-        np_data = np.array(data).astype("float32")
-        self._index.add_items(np_data, np.asarray(keys))
+    def mul_add(self, datas: List[VectorData]):
+        data_array, id_array = map(list, zip(*((data.data, data.id) for data in datas)))
+        np_data = np.array(data_array).astype("float32")
+        ids = np.array(id_array)
+        self._index.add_items(np_data, ids)
 
-    def search(self, data: "ndarray"):
+    def search(self, data: np.ndarray):
         np_data = np.array(data).astype("float32").reshape(1, -1)
         ids, dist = self._index.knn_query(data=np_data, k=self._top_k)
         return list(zip(dist[0], ids[0]))
 
-    def clear_strategy(self):
-        return ClearStrategy.REBUILD
-
-    def rebuild(self, all_data, keys):
+    def rebuild(self, ids):
+        all_data = self._index.get_items(ids)
         new_index = hnswlib.Index(space="l2", dim=self._dimension)
         new_index.init_index(max_elements=self._max_elements, ef_construction=100, M=16)
         new_index.set_ef(self._top_k * 2)
         self._index = new_index
-        self._mult_add(all_data, keys)
+        datas = []
+        for key, data in zip(ids, all_data):
+            datas.append(VectorData(id=key, data=data))
+        self.mul_add(datas)
+
+    def delete(self, ids):
+        for i in ids:
+            self._index.mark_deleted(i)
 
     def close(self):
         self._index.save_index(self._index_file_path)
```

### Comparing `gptcache-0.1.8/gptcache/manager/vector_data/manager.py` & `gptcache-0.1.9/gptcache/manager/vector_data/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,25 +49,29 @@
             port = kwargs.get("port", MILVUS_PORT)
             user = kwargs.get("user", MILVUS_USER)
             password = kwargs.get("password", MILVUS_PSW)
             secure = kwargs.get("secure", MILVUS_SECURE)
             collection_name = kwargs.get("collection_name", COLLECTION_NAME)
             index_params = kwargs.get("index_params", MILVUS_INDEX_PARAMS)
             search_params = kwargs.get("search_params", None)
+            local_mode = kwargs.get("local_mode", False)
+            local_data = kwargs.get("local_data", "./milvus_data")
             vector_base = Milvus(
                 host=host,
                 port=port,
                 user=user,
                 password=password,
                 secure=secure,
                 collection_name=collection_name,
                 dimension=dimension,
                 top_k=top_k,
                 index_params=index_params,
                 search_params=search_params,
+                local_mode=local_mode,
+                local_data=local_data
             )
         elif name == "faiss":
             from gptcache.manager.vector_data.faiss import Faiss
 
             dimension = kwargs.get("dimension", DIMENSION)
             index_path = kwargs.pop("index_path", FAISS_INDEX_PATH)
             VectorBase.check_dimension(dimension)
```

### Comparing `gptcache-0.1.8/gptcache/manager/vector_data/milvus.py` & `gptcache-0.1.9/gptcache/manager/vector_data/milvus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import List
 from uuid import uuid4
 import numpy as np
 
 from gptcache.utils import import_pymilvus
-from gptcache.manager.vector_data.base import VectorBase, ClearStrategy
+from gptcache.manager.vector_data.base import VectorBase, VectorData
+
 
 import_pymilvus()
 
 from pymilvus import (  # pylint: disable=C0413
     connections,
     utility,
     FieldSchema,
@@ -41,15 +43,44 @@
         password: str = "",
         secure: bool = False,
         collection_name: str = "gptcache",
         dimension: int = 0,
         top_k: int = 1,
         index_params: dict = None,
         search_params: dict = None,
+        local_mode: bool = False,
+        local_data: str = "./milvus_data"
     ):
+        if dimension <= 0:
+            raise ValueError(
+                f"invalid `dim` param: {dimension} in the Milvus vector store."
+            )
+        self._local_mode = local_mode
+        self._local_data = local_data
+        self.dimension = dimension
+        self.top_k = top_k
+        self.index_params = index_params
+        if self._local_mode:
+            self._create_local(port, local_data)
+        self._connect(host, port, user, password, secure)
+        self._create_collection(collection_name)
+        self.search_params = (
+            search_params or self.SEARCH_PARAM[self.index_params["index_type"]]
+        )
+
+    def _create_local(self, port, local_data):
+        from gptcache.utils import import_milvus_lite  # pylint: disable=import-outside-toplevel
+        import_milvus_lite()
+        from milvus import MilvusServer  # pylint: disable=import-outside-toplevel
+        self._server = MilvusServer()
+        self._server.set_base_dir(local_data)
+        self._server.listen_port = int(port)
+        self._server.start()
+
+    def _connect(self, host, port, user, password, secure):
         try:
             i = [
                 connections.get_connection_addr(x[0])
                 for x in connections.list_connections()
             ].index({"host": host, "port": port})
             self.alias = connections.list_connections()[i][0]
         except ValueError:
@@ -58,26 +89,16 @@
             connections.connect(
                 alias=self.alias,
                 host=host,
                 port=port,
                 user=user,  # type: ignore
                 password=password,  # type: ignore
                 secure=secure,
+                timeout=10
             )
-        if dimension <= 0:
-            raise ValueError(
-                f"invalid `dim` param: {dimension} in the Milvus vector store."
-            )
-        self.dimension = dimension
-        self.top_k = top_k
-        self.index_params = index_params
-        self._create_collection(collection_name)
-        self.search_params = (
-            search_params or self.SEARCH_PARAM[self.index_params["index_type"]]
-        )
 
     def _create_collection(self, collection_name):
         if not utility.has_collection(collection_name, using=self.alias):
             schema = [
                 FieldSchema(
                     name="id",
                     dtype=DataType.INT64,
@@ -113,29 +134,33 @@
                 self.col.create_index("embedding", index_params=i_p)
                 self.index_params = i_p
         else:
             self.index_params = self.col.indexes[0].to_dict()["index_param"]
 
         self.col.load()
 
-    def add(self, key: str, data: np.ndarray):
-        entities = [[key], data.reshape(1, self.dimension)]
+    def mul_add(self, datas: List[VectorData]):
+        data_array, id_array = map(list, zip(*((data.data, data.id) for data in datas)))
+        np_data = np.array(data_array).astype("float32")
+        entities = [id_array, np_data]
         self.col.insert(entities)
 
     def search(self, data: np.ndarray):
         search_result = self.col.search(
             data=data.reshape(1, -1).tolist(),
             anns_field="embedding",
             param=self.search_params,
             limit=self.top_k,
         )
-        return zip(search_result[0].distances, search_result[0].ids)
-
-    def clear_strategy(self):
-        return ClearStrategy.DELETE
+        return list(zip(search_result[0].distances, search_result[0].ids))
 
     def delete(self, ids):
         del_ids = ",".join([str(x) for x in ids])
         self.col.delete(f"id in [{del_ids}]")
 
+    def rebuild(self, ids=None):  # pylint: disable=unused-argument
+        self.col.compact()
+
     def close(self):
         self.col.flush(_async=True)
+        if self._local_mode:
+            self._server.stop()
```

### Comparing `gptcache-0.1.8/gptcache/similarity_evaluation/__init__.py` & `gptcache-0.1.9/gptcache/similarity_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/similarity_evaluation/distance.py` & `gptcache-0.1.9/gptcache/similarity_evaluation/distance.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/similarity_evaluation/exact_match.py` & `gptcache-0.1.9/gptcache/similarity_evaluation/exact_match.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/similarity_evaluation/np.py` & `gptcache-0.1.9/gptcache/similarity_evaluation/np.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/similarity_evaluation/onnx.py` & `gptcache-0.1.9/gptcache/similarity_evaluation/onnx.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/utils/__init__.py` & `gptcache-0.1.9/gptcache/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = [
     "import_pymilvus",
+    "import_milvus_lite",
     "import_huggingface_hub",
     "import_faiss",
     "import_hnswlib",
     "import_chromadb",
     "import_sqlalchemy",
     "import_sql_client",
     "import_huggingface",
@@ -30,14 +31,18 @@
     return is_avail
 
 
 def import_pymilvus():
     _check_library("pymilvus")
 
 
+def import_milvus_lite():
+    _check_library("milvus")
+
+
 def import_sbert():
     _check_library("sentence-transformers")
 
 
 def import_cohere():
     _check_library("cohere")
```

### Comparing `gptcache-0.1.8/gptcache/utils/dependency_control.py` & `gptcache-0.1.9/gptcache/utils/dependency_control.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache/utils/error.py` & `gptcache-0.1.9/gptcache/utils/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class CacheError(Exception):
     """GPTCache base error"""
 
 
 class NotInitError(CacheError):
     """Raise when the cache has been used before it's inited"""
     def __init__(self):
-        super().__init__("the cache should be inited before using")
+        super().__init__("The cache should be inited before using")
 
 
 class NotFoundStoreError(CacheError):
     """Raise when getting an unsupported store."""
     def __init__(self, store_type, current_type_name):
         super().__init__(f"Unsupported ${store_type}: {current_type_name}")
 
@@ -18,7 +18,12 @@
     """Raise when receiving an invalid param."""
 
 
 class PipInstallError(CacheError):
     """Raise when failed to install package."""
     def __init__(self, package):
         super().__init__(f"Ran into error installing {package}.")
+
+
+class NotFoundStrategyError(CacheError):
+    def __init__(self, strategy):
+        super().__init__(f"Unsupported vector store strategy, {strategy}.")
```

### Comparing `gptcache-0.1.8/gptcache/utils/lazy_import.py` & `gptcache-0.1.9/gptcache/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `gptcache-0.1.8/gptcache.egg-info/PKG-INFO` & `gptcache-0.1.9/gptcache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptcache
-Version: 0.1.8
-Summary: GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
+Version: 0.1.9
+Summary: GPTCache, a powerful caching library that can be used to speed up and lower the cost of chat applications that rely on the LLM service. GPTCache works as a memcache for AIGC applications, similar to how Redis works for traditional applications.
 Home-page: https://github.com/zilliztech/GPTCache
 Author: SimFG
 Author-email: bang.fu@zilliz.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -244,15 +244,15 @@
 
 ![GPTCache Struct](docs/GPTCacheStructure.png)
 
 - **LLM Adapter**: 
 The LLM Adapter is designed to integrate different LLM models by unifying their APIs and request protocols. GPTCache offers a standardized interface for this purpose, with current support for ChatGPT integration.
   - [x] Support OpenAI ChatGPT API.
   - [x] Support langchain.
-  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMa.
+  - [ ] Support other LLMs, such as Hugging Face Hub, Bard, Anthropic, and self-hosted models like LLaMA.
 - **Embedding Generator**: 
 This module is created to extract embeddings from requests for similarity search. GPTCache offers a generic interface that supports multiple embedding APIs, and presents a range of solutions to choose from. 
   - [x] Disable embedding. This will turn GPTCache into a keyword-matching cache.
   - [x] Support OpenAI embedding API.
   - [x] Support [ONNX](https://onnx.ai/) with the GPTCache/paraphrase-albert-onnx model.
   - [x] Support [Hugging Face](https://huggingface.co/) embedding API.
   - [x] Support [Cohere](https://docs.cohere.ai/reference/embed) embedding API.
```

### Comparing `gptcache-0.1.8/gptcache.egg-info/SOURCES.txt` & `gptcache-0.1.9/gptcache.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 gptcache/similarity_evaluation/exact_match.py
 gptcache/similarity_evaluation/np.py
 gptcache/similarity_evaluation/onnx.py
 gptcache/similarity_evaluation/similarity_evaluation.py
 gptcache/utils/__init__.py
 gptcache/utils/dependency_control.py
 gptcache/utils/error.py
-gptcache/utils/lazy_import.py
+gptcache/utils/lazy_import.py
+gptcache/utils/response.py
```

### Comparing `gptcache-0.1.8/setup.py` & `gptcache-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,19 @@
             if require.strip() and not require.startswith('#')
         ]
 
 
 setuptools.setup(
     name="gptcache",
     packages=find_packages(),
-    version="0.1.8",
+    version="0.1.9",
     author="SimFG",
     author_email="bang.fu@zilliz.com",
-    description="GPT Cache, a powerful caching library that can be used to speed up and lower the cost of chat "
-                "applications that rely on the LLM service. GPT Cache works as a memcache for AIGC applications, "
+    description="GPTCache, a powerful caching library that can be used to speed up and lower the cost of chat "
+                "applications that rely on the LLM service. GPTCache works as a memcache for AIGC applications, "
                 "similar to how Redis works for traditional applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=parse_requirements('requirements.txt'),
     url="https://github.com/zilliztech/GPTCache",
     license='https://opensource.org/license/mit/',
     python_requires='>=3.8.1',
```

