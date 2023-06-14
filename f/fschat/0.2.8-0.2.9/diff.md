# Comparing `tmp/fschat-0.2.8.tar.gz` & `tmp/fschat-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.8.tar", last modified: Fri May 12 09:29:50 2023, max compression
+gzip compressed data, was "fschat-0.2.9.tar", last modified: Mon May 15 13:31:51 2023, max compression
```

## Comparing `fschat-0.2.8.tar` & `fschat-0.2.9.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15741 2023-05-12 09:29:50.769843 fschat-0.2.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15247 2023-05-12 09:23:49.000000 fschat-0.2.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.757843 fschat-0.2.8/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-12 09:29:43.000000 fschat-0.2.8/fastchat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15513 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.761843 fschat-0.2.8/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.8/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.8/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      939 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/data/inspect_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.8/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.8/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3447 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.761843 fschat-0.2.8/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.8/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/model/apply_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2471 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/model/chatglm_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/make_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15843 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/model/model_adapter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3002 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/model/model_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      996 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/rwkv_model.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4377 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/protocol/openai_api_protocol.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11747 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11883 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14791 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/gradio_block_arena_anony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-12 07:21:21.000000 fschat-0.2.8/fastchat/serve/gradio_block_arena_named.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21945 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9248 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12405 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/model_worker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/serve/monitor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5594 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/basic_stats.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5609 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/clean_battle_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/elo_analysis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7159 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/monitor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22422 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/openai_api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2442 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7107 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15741 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1984 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-05-12 09:29:43.000000 fschat-0.2.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-12 09:29:50.769843 fschat-0.2.8/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2023-05-12 08:58:36.000000 fschat-0.2.8/tests/test_openai_sdk.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15845 2023-05-15 13:31:51.013331 fschat-0.2.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15351 2023-05-12 20:44:42.000000 fschat-0.2.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.005331 fschat-0.2.9/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-15 13:30:41.000000 fschat-0.2.9/fastchat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16018 2023-05-12 21:30:09.000000 fschat-0.2.9/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.005331 fschat-0.2.9/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.9/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.9/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.9/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      939 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/data/inspect_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.9/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.9/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.9/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3447 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.005331 fschat-0.2.9/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.009331 fschat-0.2.9/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.9/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2471 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/model/chatglm_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/model/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/model/make_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16303 2023-05-14 21:47:29.000000 fschat-0.2.9/fastchat/model/model_adapter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3272 2023-05-14 21:47:29.000000 fschat-0.2.9/fastchat/model/model_registry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/model/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      996 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/model/rwkv_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.009331 fschat-0.2.9/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4377 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/protocol/openai_api_protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.9/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4047 2023-05-14 22:03:00.000000 fschat-0.2.9/fastchat/serve/api_provider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4999 2023-05-12 21:30:09.000000 fschat-0.2.9/fastchat/serve/bard_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11747 2023-05-12 08:32:11.000000 fschat-0.2.9/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11883 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14840 2023-05-14 21:47:45.000000 fschat-0.2.9/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-12 07:21:21.000000 fschat-0.2.9/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21587 2023-05-14 22:03:00.000000 fschat-0.2.9/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6470 2023-05-12 21:30:09.000000 fschat-0.2.9/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2023-05-14 22:03:00.000000 fschat-0.2.9/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9248 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12433 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/serve/model_worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/fastchat/serve/monitor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5594 2023-05-12 08:32:11.000000 fschat-0.2.9/fastchat/serve/monitor/basic_stats.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5746 2023-05-14 21:47:29.000000 fschat-0.2.9/fastchat/serve/monitor/clean_battle_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-12 08:32:11.000000 fschat-0.2.9/fastchat/serve/monitor/elo_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7159 2023-05-12 08:32:11.000000 fschat-0.2.9/fastchat/serve/monitor/monitor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22422 2023-05-12 20:44:42.000000 fschat-0.2.9/fastchat/serve/openai_api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.9/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2469 2023-05-14 22:03:00.000000 fschat-0.2.9/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.9/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7107 2023-05-12 07:11:10.000000 fschat-0.2.9/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15845 2023-05-15 13:31:50.000000 fschat-0.2.9/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2045 2023-05-15 13:31:51.000000 fschat-0.2.9/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 13:31:50.000000 fschat-0.2.9/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-15 13:31:50.000000 fschat-0.2.9/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-15 13:31:50.000000 fschat-0.2.9/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-05-15 13:30:34.000000 fschat-0.2.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 13:31:51.013331 fschat-0.2.9/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 13:31:51.013331 fschat-0.2.9/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2023-05-12 20:44:42.000000 fschat-0.2.9/tests/test_openai_sdk.py
```

### Comparing `fschat-0.2.8/LICENSE` & `fschat-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/PKG-INFO` & `fschat-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.8
+Version: 0.2.9
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -126,14 +126,16 @@
 - [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 - [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
 
+Help us [add more](https://github.com/lm-sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model).
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.8 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.9 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
@@ -69,50 +69,51 @@
 huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
 chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
 [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
 [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
 oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
 project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
 huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
-//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
-around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
-See the "No Enough Memory" section below if you do not have enough memory.
-Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
-Multiple GPUs You can use model parallelism to aggregate GPU memory from
-multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
-only and does not require GPU. It requires around 60GB of CPU memory for
-Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
-you do not have enough memory, you can enable 8-bit compression by adding `--
-load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
-to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
-offloading` to commands above to offload weights that don't fit on your GPU
-onto the CPU memory. This requires 8-bit compression to be enabled and the
-bitsandbytes package to be installed, which is only available on linux
-operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
-backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
-deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
-Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. You can
-learn more about the architecture [here](docs/server_arch.md). Here are the
-commands to follow in your terminal: #### Launch the controller ```bash python3
--m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker(s) ```bash python3 -
+//huggingface.co/THUDM/chatglm-6b) Help us [add more](https://github.com/lm-
+sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model). #### Single GPU
+The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of
+GPU memory for Vicuna-7B. See the "No Enough Memory" section below if you do
+not have enough memory. Replace `/path/to/model/weights` with the a local
+folder or a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/model/weights ``` #### Multiple GPUs You can use model parallelism to
+aggregate GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
```

### Comparing `fschat-0.2.8/README.md` & `fschat-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,16 @@
 - [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 - [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
 
+Help us [add more](https://github.com/lm-sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model).
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
```

#### html2text {}

```diff
@@ -62,50 +62,51 @@
 huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
 chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
 [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
 [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
 oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
 project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
 huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
-//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
-around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
-See the "No Enough Memory" section below if you do not have enough memory.
-Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
-Multiple GPUs You can use model parallelism to aggregate GPU memory from
-multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
-only and does not require GPU. It requires around 60GB of CPU memory for
-Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
-you do not have enough memory, you can enable 8-bit compression by adding `--
-load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
-to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
-offloading` to commands above to offload weights that don't fit on your GPU
-onto the CPU memory. This requires 8-bit compression to be enabled and the
-bitsandbytes package to be installed, which is only available on linux
-operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
-backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
-deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
-Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. You can
-learn more about the architecture [here](docs/server_arch.md). Here are the
-commands to follow in your terminal: #### Launch the controller ```bash python3
--m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker(s) ```bash python3 -
+//huggingface.co/THUDM/chatglm-6b) Help us [add more](https://github.com/lm-
+sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model). #### Single GPU
+The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of
+GPU memory for Vicuna-7B. See the "No Enough Memory" section below if you do
+not have enough memory. Replace `/path/to/model/weights` with the a local
+folder or a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/model/weights ``` #### Multiple GPUs You can use model parallelism to
+aggregate GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
```

### Comparing `fschat-0.2.8/fastchat/constants.py` & `fschat-0.2.9/fastchat/constants.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/conversation.py` & `fschat-0.2.9/fastchat/conversation.py`

 * *Files 5% similar despite different names*

```diff
@@ -427,14 +427,29 @@
         offset=0,
         sep_style=SeparatorStyle.NEW_LINE,
         sep="<|im_end|>",
         stop_token_ids=[50278, 0],
     )
 )
 
+# Bard default template
+# Reference: https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L150
+#            https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L40
+register_conv_template(
+    Conversation(
+        name="bard",
+        system="",
+        roles=("0", "1"),
+        messages=(),
+        offset=0,
+        sep_style=None,
+        sep=None,
+    )
+)
+
 if __name__ == "__main__":
     conv = get_conv_template("vicuna_v1.1")
     conv.append_message(conv.roles[0], "Hello!")
     conv.append_message(conv.roles[1], "Hi!")
     conv.append_message(conv.roles[0], "How are you?")
     conv.append_message(conv.roles[1], None)
     print(conv.get_prompt())
```

### Comparing `fschat-0.2.8/fastchat/data/clean_sharegpt.py` & `fschat-0.2.9/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/hardcoded_questions.py` & `fschat-0.2.9/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/inspect_data.py` & `fschat-0.2.9/fastchat/data/inspect_data.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/merge.py` & `fschat-0.2.9/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/optional_clean.py` & `fschat-0.2.9/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/sample.py` & `fschat-0.2.9/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/data/split_long_conversation.py` & `fschat-0.2.9/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.9/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.9/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/eval/get_model_answer.py` & `fschat-0.2.9/fastchat/eval/get_model_answer.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.9/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/apply_delta.py` & `fschat-0.2.9/fastchat/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/apply_lora.py` & `fschat-0.2.9/fastchat/model/apply_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/chatglm_model.py` & `fschat-0.2.9/fastchat/model/chatglm_model.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/compression.py` & `fschat-0.2.9/fastchat/model/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/convert_fp16.py` & `fschat-0.2.9/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/make_delta.py` & `fschat-0.2.9/fastchat/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/model_adapter.py` & `fschat-0.2.9/fastchat/model/model_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Model adapter registration."""
 
+import math
 import sys
 from typing import List, Optional
 import warnings
 if sys.version_info >= (3, 9):
     from functools import cache
 else:
     from functools import lru_cache as cache
 
+import psutil
 import torch
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForCausalLM,
     AutoModelForSeq2SeqLM,
     AutoTokenizer,
@@ -438,35 +440,49 @@
         return get_conv_template("chatgpt")
 
 
 class ClaudeAdapter(BaseAdapter):
     """The model adapter for Claude."""
 
     def match(self, model_path: str):
-        return model_path == "claude-v1"
+        return model_path in ["claude-v1", "claude-instant-v1.1"]
 
     def load_model(self, model_path: str, from_pretrained_kwargs: dict):
         raise NotImplementedError()
 
     def get_default_conv_template(self, model_path: str) -> Conversation:
         return get_conv_template("claude")
 
 
+class BardAdapter(BaseAdapter):
+    """The model adapter for Bard."""
+
+    def match(self, model_path: str):
+        return model_path == "bard"
+
+    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
+        raise NotImplementedError()
+
+    def get_default_conv_template(self, model_path: str) -> Conversation:
+        return get_conv_template("bard")
+
+
 # Note: the registration order matters.
 # The one registered earlier has a higher matching priority.
 register_model_adapter(VicunaAdapter)
 register_model_adapter(T5Adapter)
 register_model_adapter(KoalaAdapter)
 register_model_adapter(ChatGLMAdapter)
 register_model_adapter(DollyV2Adapter)
 register_model_adapter(OasstPythiaAdapter)
 register_model_adapter(StableLMAdapter)
 register_model_adapter(BaizeAdapter)
 register_model_adapter(RwkvAdapter)
 register_model_adapter(OpenBuddyAdapter)
 register_model_adapter(PhoenixAdapter)
+register_model_adapter(BardAdapter)
 register_model_adapter(ChatGPTAdapter)
 register_model_adapter(ClaudeAdapter)
 register_model_adapter(MPTAdapter)
 
 # After all adapters, try the default base adapter.
 register_model_adapter(BaseAdapter)
```

### Comparing `fschat-0.2.8/fastchat/model/model_registry.py` & `fschat-0.2.9/fastchat/model/model_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,26 @@
 register_model_info(
     ["claude-v1"],
     "Claude",
     "https://www.anthropic.com/index/introducing-claude",
     "Claude by Anthropic",
 )
 register_model_info(
+    ["claude-instant-v1.1"],
+    "Claude Instant",
+    "https://www.anthropic.com/index/introducing-claude",
+    "Claude Instant by Anthropic",
+)
+register_model_info(
+    ["bard"],
+    "Bard",
+    "https://bard.google.com/",
+    "Bard by Google",
+)
+register_model_info(
     ["vicuna-13b"],
     "Vicuna",
     "https://lmsys.org/blog/2023-03-30-vicuna/",
     "a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS",
 )
 register_model_info(
     ["koala-13b"],
```

### Comparing `fschat-0.2.8/fastchat/model/monkey_patch_non_inplace.py` & `fschat-0.2.9/fastchat/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/model/rwkv_model.py` & `fschat-0.2.9/fastchat/model/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/protocol/openai_api_protocol.py` & `fschat-0.2.9/fastchat/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.9/fastchat/serve/cacheflow_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/cli.py` & `fschat-0.2.9/fastchat/serve/cli.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/controller.py` & `fschat-0.2.9/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/gradio_block_arena_anony.py` & `fschat-0.2.9/fastchat/serve/gradio_block_arena_anony.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,16 @@
         )
 
 
 DEFAULT_WEIGHTS = {
     "gpt-4": 1.5,
     "gpt-3.5-turbo": 1.5,
     "claude-v1": 1.5,
+    "claude-instant-v1.1": 1.5,
+    "bard": 1.5,
     "vicuna-13b": 1.5,
     "koala-13b": 1.5,
     "RWKV-4-Raven-14B": 1.2,
     "oasst-pythia-12b": 1.2,
     "mpt-7b-chat": 1.2,
     "fastchat-t5-3b": 1,
     "alpaca-13b": 1,
```

### Comparing `fschat-0.2.8/fastchat/serve/gradio_block_arena_named.py` & `fschat-0.2.9/fastchat/serve/gradio_block_arena_named.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/gradio_css.py` & `fschat-0.2.9/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/gradio_patch.py` & `fschat-0.2.9/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/gradio_web_server.py` & `fschat-0.2.9/fastchat/serve/gradio_web_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 """
 
 import argparse
 from collections import defaultdict
 import datetime
 import json
 import os
+import random
 import time
 import uuid
 
 import gradio as gr
 import requests
 
 from fastchat.conversation import SeparatorStyle
 from fastchat.constants import LOGDIR, WORKER_API_TIMEOUT, ErrorCode
 from fastchat.model.model_adapter import get_conversation_template
 from fastchat.model.model_registry import model_info
+from fastchat.serve.api_provider import (
+    anthropic_api_stream_iter,
+    bard_api_stream_iter,
+    openai_api_stream_iter,
+    palm_api_stream_iter,
+    init_palm_chat,
+)
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
 from fastchat.utils import (
     build_logger,
     server_error_msg,
     violates_moderation,
     moderation_msg,
@@ -198,70 +206,14 @@
         if len(blocks) % 2 == 1:
             for i in range(1, len(blocks), 2):
                 blocks[i] = blocks[i].replace("\\_", "_")
         code = sep.join(blocks)
     return code
 
 
-def openai_api_stream_iter(model_name, messages, temperature, top_p, max_new_tokens):
-    import openai
-
-    # Make requests
-    gen_params = {
-        "model": model_name,
-        "prompt": messages,
-        "temperature": temperature,
-        "top_p": top_p,
-    }
-    logger.info(f"==== request ====\n{gen_params}")
-
-    res = openai.ChatCompletion.create(
-        model=model_name, messages=messages, temperature=temperature, stream=True
-    )
-    text = ""
-    for chunk in res:
-        text += chunk["choices"][0]["delta"].get("content", "")
-        data = {
-            "text": text,
-            "error_code": 0,
-        }
-        yield data
-
-
-def anthropic_api_stream_iter(model_name, prompt, temperature, top_p, max_new_tokens):
-    import anthropic
-
-    c = anthropic.Client(os.environ["ANTHROPIC_API_KEY"])
-
-    # Make requests
-    gen_params = {
-        "model": model_name,
-        "prompt": prompt,
-        "temperature": temperature,
-        "top_p": top_p,
-    }
-    logger.info(f"==== request ====\n{gen_params}")
-
-    res = c.completion_stream(
-        prompt=prompt,
-        stop_sequences=[anthropic.HUMAN_PROMPT],
-        max_tokens_to_sample=max_new_tokens,
-        temperature=temperature,
-        top_p=top_p,
-        model=model_name,
-        stream=True,
-    )
-    for chunk in res:
-        data = {
-            "text": chunk["completion"],
-            "error_code": 0,
-        }
-        yield data
-
-
 def model_worker_stream_iter(
     conv, model_name, worker_addr, prompt, temperature, top_p, max_new_tokens
 ):
     # Make requests
     gen_params = {
         "model": model_name,
         "prompt": prompt,
@@ -307,25 +259,40 @@
         # First round of conversation
         new_state = get_conversation_template(model_name)
         new_state.conv_id = uuid.uuid4().hex
         new_state.model_name = state.model_name or model_selector
         new_state.append_message(new_state.roles[0], state.messages[-2][1])
         new_state.append_message(new_state.roles[1], None)
         state = new_state
+        if model_name == "bard":
+            state.session_state = {
+                "conversation_id": "",
+                "response_id": "",
+                "choice_id": "",
+                "req_id": 0,
+            }
+            # According to release note, "chat-bison@001" is PaLM 2 for chat.
+            # https://cloud.google.com/vertex-ai/docs/release-notes#May_10_2023
+            state.chat = init_palm_chat("chat-bison@001")
 
     if model_name == "gpt-3.5-turbo" or model_name == "gpt-4":
         prompt = state.to_openai_api_messages()
         stream_iter = openai_api_stream_iter(
             model_name, prompt, temperature, top_p, max_new_tokens
         )
-    elif model_name == "claude-v1":
+    elif model_name in ["claude-v1", "claude-instant-v1.1"]:
         prompt = state.get_prompt()
         stream_iter = anthropic_api_stream_iter(
             model_name, prompt, temperature, top_p, max_new_tokens
         )
+    elif model_name == "bard":
+        # stream_iter = bard_api_stream_iter(state)
+        stream_iter = palm_api_stream_iter(
+            state.chat, state.messages[-2][1], temperature, top_p, max_new_tokens
+        )
     else:
         # Query worker address
         ret = requests.post(
             controller_url + "/get_worker_address", json={"model": model_name}
         )
         worker_addr = ret.json()["address"]
         logger.info(f"model_name: {model_name}, worker_addr: {worker_addr}")
@@ -654,25 +621,31 @@
         help="Add OpenAI's ChatGPT models (gpt-3.5-turbo, gpt-4)",
     )
     parser.add_argument(
         "--add-claude",
         action="store_true",
         help="Add Anthropic's Claude models (claude-v1)",
     )
-
+    parser.add_argument(
+        "--add-bard",
+        action="store_true",
+        help="Add Google's Bard model",
+    )
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     set_global_vars(args.controller_url, args.moderate)
     models = get_model_list(args.controller_url)
 
     if args.add_chatgpt:
         models = ["gpt-3.5-turbo", "gpt-4"] + models
     if args.add_claude:
-        models = ["claude-v1"] + models
+        models = ["claude-v1", "claude-instant-v1.1"] + models
+    if args.add_bard:
+        models = ["bard"] + models
 
     demo = build_demo(models)
     demo.queue(
         concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
     ).launch(
         server_name=args.host, server_port=args.port, share=args.share, max_threads=200
     )
```

### Comparing `fschat-0.2.8/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.9/fastchat/serve/gradio_web_server_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,21 @@
     elif "compare" in url_params:
         selected = 2
     elif "leaderboard" in url_params:
         selected = 3
     single_updates = load_demo_single(models, url_params)
 
     models_anony = models
+    # Only enable these models in anony battles.
     if args.add_chatgpt:
         models_anony = ["gpt-4", "gpt-3.5-turbo"] + models_anony
     if args.add_claude:
         models_anony = ["claude-v1"] + models_anony
+    if args.add_bard:
+        models_anony = ["bard"] + models_anony
 
     side_by_side_anony_updates = load_demo_side_by_side_anony(models_anony, url_params)
     side_by_side_named_updates = load_demo_side_by_side_named(models, url_params)
     return (
         (gr.Tabs.update(selected=selected),)
         + single_updates
         + side_by_side_anony_updates
@@ -173,14 +176,19 @@
         help="Add OpenAI ChatGPT models (gpt-3.5-turbo, gpt-4)",
     )
     parser.add_argument(
         "--add-claude",
         action="store_true",
         help="Add Anthropic's Claude models (claude-v1)",
     )
+    parser.add_argument(
+        "--add-bard",
+        action="store_true",
+        help="Add Google's Bard model",
+    )
     parser.add_argument("--elo-results-file", type=str)
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     set_global_vars(args.controller_url, args.moderate)
     set_global_vars_named(args.moderate)
     set_global_vars_anony(args.moderate)
```

### Comparing `fschat-0.2.8/fastchat/serve/huggingface_api.py` & `fschat-0.2.9/fastchat/serve/huggingface_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+Use FastChat with Hugging Face generation APIs.
+
 Usage:
 python3 -m fastchat.serve.huggingface_api --model lmsys/fastchat-t5-3b-v1.0
 python3 -m fastchat.serve.huggingface_api --model ~/model_weights/vicuna-7b/
 """
 import argparse
 import json
```

### Comparing `fschat-0.2.8/fastchat/serve/inference.py` & `fschat-0.2.9/fastchat/serve/inference.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/model_worker.py` & `fschat-0.2.9/fastchat/serve/model_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,15 @@
         except (ValueError, RuntimeError) as e:
             ret = {
                 "text": f"{server_error_msg}\n\n({e})",
                 "error_code": ErrorCode.INTERNAL_ERROR,
             }
         return ret
 
+    @torch.inference_mode()
     def get_embeddings(self, params):
         try:
             tokenizer = self.tokenizer
             input_ids = tokenizer.encode(params["input"], return_tensors="pt").to(
                 self.device
             )
             model_output = self.model(input_ids, output_hidden_states=True)
```

### Comparing `fschat-0.2.8/fastchat/serve/monitor/basic_stats.py` & `fschat-0.2.9/fastchat/serve/monitor/basic_stats.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/monitor/clean_battle_data.py` & `fschat-0.2.9/fastchat/serve/monitor/clean_battle_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     "open assistant",
     "laion",
     "chatglm",
     "chatgpt",
     "openai",
     "anthropic",
     "claude",
+    "bard",
+    "palm",
+    "Lamda",
+    "google",
+    "**NETWORK ERROR DUE TO HIGH TRAFFIC. PLEASE REGENERATE OR REFRESH THIS PAGE.**",
 ]
 
 
 def get_log_files(max_num_files=None):
     dates = []
     for month in [4]:
         for day in range(24, 32):
```

### Comparing `fschat-0.2.8/fastchat/serve/monitor/elo_analysis.py` & `fschat-0.2.9/fastchat/serve/monitor/elo_analysis.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/monitor/monitor.py` & `fschat-0.2.9/fastchat/serve/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/openai_api_server.py` & `fschat-0.2.9/fastchat/serve/openai_api_server.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/register_worker.py` & `fschat-0.2.9/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/serve/test_message.py` & `fschat-0.2.9/fastchat/serve/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Send a test message."""
 import argparse
 import json
 
 import requests
 
 from fastchat.model.model_adapter import get_conversation_template
```

### Comparing `fschat-0.2.8/fastchat/serve/test_throughput.py` & `fschat-0.2.9/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.9/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/train/train.py` & `fschat-0.2.9/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/train/train_flant5.py` & `fschat-0.2.9/fastchat/train/train_flant5.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/train/train_lora.py` & `fschat-0.2.9/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fastchat/utils.py` & `fschat-0.2.9/fastchat/utils.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.8/fschat.egg-info/PKG-INFO` & `fschat-0.2.9/fschat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.8
+Version: 0.2.9
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -126,14 +126,16 @@
 - [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 - [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
 
+Help us [add more](https://github.com/lm-sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model).
+
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.8 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.9 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
@@ -69,50 +69,51 @@
 huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
 chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
 [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
 [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
 oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
 project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
 huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
-//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
-around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
-See the "No Enough Memory" section below if you do not have enough memory.
-Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
-Multiple GPUs You can use model parallelism to aggregate GPU memory from
-multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
-only and does not require GPU. It requires around 60GB of CPU memory for
-Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
-Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
-to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
-load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
-model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
-run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
-you do not have enough memory, you can enable 8-bit compression by adding `--
-load-8bit` to commands above. This can reduce memory usage by around half with
-slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
-backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
-4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
-to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
-offloading` to commands above to offload weights that don't fit on your GPU
-onto the CPU memory. This requires 8-bit compression to be enabled and the
-bitsandbytes package to be installed, which is only available on linux
-operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
-backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
-deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
-Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
-screenshot_gui.png] To serve using the web UI, you need three main components:
-web servers that interface with users, model workers that host one or more
-models, and a controller to coordinate the webserver and model workers. You can
-learn more about the architecture [here](docs/server_arch.md). Here are the
-commands to follow in your terminal: #### Launch the controller ```bash python3
--m fastchat.serve.controller ``` This controller manages the distributed
-workers. #### Launch the model worker(s) ```bash python3 -
+//huggingface.co/THUDM/chatglm-6b) Help us [add more](https://github.com/lm-
+sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model). #### Single GPU
+The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of
+GPU memory for Vicuna-7B. See the "No Enough Memory" section below if you do
+not have enough memory. Replace `/path/to/model/weights` with the a local
+folder or a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /
+path/to/model/weights ``` #### Multiple GPUs You can use model parallelism to
+aggregate GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
+[assets/screenshot_gui.png] To serve using the web UI, you need three main
+components: web servers that interface with users, model workers that host one
+or more models, and a controller to coordinate the webserver and model workers.
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
```

### Comparing `fschat-0.2.8/fschat.egg-info/SOURCES.txt` & `fschat-0.2.9/fschat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 fastchat/model/make_delta.py
 fastchat/model/model_adapter.py
 fastchat/model/model_registry.py
 fastchat/model/monkey_patch_non_inplace.py
 fastchat/model/rwkv_model.py
 fastchat/protocol/openai_api_protocol.py
 fastchat/serve/__init__.py
+fastchat/serve/api_provider.py
+fastchat/serve/bard_worker.py
 fastchat/serve/cacheflow_worker.py
 fastchat/serve/cli.py
 fastchat/serve/controller.py
 fastchat/serve/gradio_block_arena_anony.py
 fastchat/serve/gradio_block_arena_named.py
 fastchat/serve/gradio_css.py
 fastchat/serve/gradio_patch.py
```

### Comparing `fschat-0.2.8/pyproject.toml` & `fschat-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.8"
+version = "0.2.9"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

### Comparing `fschat-0.2.8/tests/test_openai_sdk.py` & `fschat-0.2.9/tests/test_openai_sdk.py`

 * *Files identical despite different names*

