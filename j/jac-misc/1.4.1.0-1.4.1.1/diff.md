# Comparing `tmp/jac_misc-1.4.1.0.tar.gz` & `tmp/jac_misc-1.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_misc-1.4.1.0.tar", last modified: Wed Jun  7 18:25:06 2023, max compression
+gzip compressed data, was "jac_misc-1.4.1.1.tar", last modified: Wed Jun 14 19:22:28 2023, max compression
```

## Comparing `jac_misc-1.4.1.0.tar` & `jac_misc-1.4.1.1.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.556879 jac_misc-1.4.1.0/jac_misc/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/cluster.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/cluster/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/example_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/example_module.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/example_module/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/huggingface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/openai/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/pdf_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/pdf_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/test_pdf_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/ph/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/ph_train_data.json
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/run_ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.564879 jac_misc-1.4.1.0/jac_misc/ph/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/ph/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/jac_misc/translator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/jac_misc/translator/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:06.560879 jac_misc-1.4.1.0/jac_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 18:25:06.000000 jac_misc-1.4.1.0/jac_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:06.568879 jac_misc-1.4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 18:24:45.000000 jac_misc-1.4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/cluster/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/tests/fixtures/cluster.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/cluster/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/example_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/example_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/example_module/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/example_module/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/huggingface/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/huggingface/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/huggingface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/langchain/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/langchain/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/openai/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/openai/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/pdf_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/pdf_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/test_pdf_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/ph/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/ph_train_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/run_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/ph/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/ph/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/jac_misc/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/translator/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/jac_misc/translator/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:22:28.581032 jac_misc-1.4.1.1/jac_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-14 19:22:28.000000 jac_misc-1.4.1.1/jac_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-14 19:22:28.000000 jac_misc-1.4.1.1/jac_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:22:28.000000 jac_misc-1.4.1.1/jac_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 19:22:28.000000 jac_misc-1.4.1.1/jac_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 19:22:28.000000 jac_misc-1.4.1.1/jac_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:22:28.585032 jac_misc-1.4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-14 19:22:12.000000 jac_misc-1.4.1.1/setup.py
```

### Comparing `jac_misc-1.4.1.0/README.md` & `jac_misc-1.4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/cluster/cluster.py` & `jac_misc-1.4.1.1/jac_misc/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/cluster/tests/fixtures/cluster.jac` & `jac_misc-1.4.1.1/jac_misc/cluster/tests/fixtures/cluster.jac`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/cluster/tests/test_cluster.py` & `jac_misc-1.4.1.1/jac_misc/cluster/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/huggingface/huggingface.py` & `jac_misc-1.4.1.1/jac_misc/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/huggingface/utils.py` & `jac_misc-1.4.1.1/jac_misc/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/openai/main.py` & `jac_misc-1.4.1.1/jac_misc/openai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     -------
     responses : list of str
         A list of responses generated by the GPT-3.5 model based on the provided messages.
     """
 
     response = openai.ChatCompletion.create(
         model=model,
-        prompt=messages,
+        messages=messages,
         temperature=temperature,
         top_p=top_p,
         n=n,
         stop=stop,
         presence_penalty=presence_penalty,
         frequency_penalty=frequency_penalty,
     )
```

### Comparing `jac_misc-1.4.1.0/jac_misc/pdf_ext/pdf_ext.py` & `jac_misc-1.4.1.1/jac_misc/pdf_ext/pdf_ext.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac` & `jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/fixtures/pdf_ext.jac`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/pdf_ext/tests/test_pdf_ext.py` & `jac_misc-1.4.1.1/jac_misc/pdf_ext/tests/test_pdf_ext.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/config.yaml` & `jac_misc-1.4.1.1/jac_misc/ph/config.yaml`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/custom.py` & `jac_misc-1.4.1.1/jac_misc/ph/custom.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/inference.py` & `jac_misc-1.4.1.1/jac_misc/ph/inference.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/ph.py` & `jac_misc-1.4.1.1/jac_misc/ph/ph.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/ph_train_data.json` & `jac_misc-1.4.1.1/jac_misc/ph/ph_train_data.json`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/run_ph.py` & `jac_misc-1.4.1.1/jac_misc/ph/run_ph.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/train.py` & `jac_misc-1.4.1.1/jac_misc/ph/train.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/base.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/base.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/dataloader.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/logger.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/logger.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/loss.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/loss.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/metric.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/metric.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/model.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/model.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/process.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/process.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/trainer.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/ph/utils/util.py` & `jac_misc-1.4.1.1/jac_misc/ph/utils/util.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc/translator/translator.py` & `jac_misc-1.4.1.1/jac_misc/translator/translator.py`

 * *Files identical despite different names*

### Comparing `jac_misc-1.4.1.0/jac_misc.egg-info/SOURCES.txt` & `jac_misc-1.4.1.1/jac_misc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 jac_misc/example_module/__init__.py
 jac_misc/example_module/example_module.py
 jac_misc/example_module/requirements.txt
 jac_misc/huggingface/__init__.py
 jac_misc/huggingface/huggingface.py
 jac_misc/huggingface/requirements.txt
 jac_misc/huggingface/utils.py
+jac_misc/langchain/__init__.py
+jac_misc/langchain/main.py
+jac_misc/langchain/requirements.txt
 jac_misc/openai/__init__.py
 jac_misc/openai/main.py
 jac_misc/openai/requirements.txt
 jac_misc/pdf_ext/__init__.py
 jac_misc/pdf_ext/pdf_ext.py
 jac_misc/pdf_ext/requirements.txt
 jac_misc/pdf_ext/tests/__init__.py
```

### Comparing `jac_misc-1.4.1.0/jac_misc.egg-info/requires.txt` & `jac_misc-1.4.1.1/jac_misc.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jaseci==1.4.1.0
+jaseci==1.4.1.1
 pytest<7.1,>=7.0.1
 pytest-order<1.1,>=1.0.1
 
 [all]
 PyPDF2<1.28,>=1.27.12
 transformers>=4.0.0
 torch<2.0.0,>=1.10.2
@@ -10,21 +10,31 @@
 protobuf<3.21,>=3.20.1
 hdbscan==0.8.29
 umap-learn==0.5.3
 uuid<2.0.0,>=1.30
 transformers>=4.25.1
 openai<0.28,>=0.27.4
 soundfile<0.13,>=0.12.1
+langchain
+openai
+chromadb
+tiktoken
 
 [cluster]
 hdbscan==0.8.29
 umap-learn==0.5.3
 
 [huggingface]
 
+[langchain]
+langchain
+openai
+chromadb
+tiktoken
+
 [openai]
 openai<0.28,>=0.27.4
 soundfile<0.13,>=0.12.1
 
 [pdf_ext]
 PyPDF2<1.28,>=1.27.12
```

### Comparing `jac_misc-1.4.1.0/setup.py` & `jac_misc-1.4.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from setuptools import setup, find_packages
 from os.path import join
 
-MODULES = ["pdf_ext", "translator", "cluster", "ph", "openai", "huggingface"]
+MODULES = [
+    "pdf_ext",
+    "translator",
+    "cluster",
+    "ph",
+    "openai",
+    "huggingface",
+    "langchain",
+]
 
 
 def get_ver():
     with open(join("./jac_misc", "VERSION")) as version_file:
         return version_file.read().strip()
```

