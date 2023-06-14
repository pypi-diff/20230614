# Comparing `tmp/xturing-0.1.4.tar.gz` & `tmp/xturing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.4.tar", last modified: Tue Jun 13 14:43:38 2023, max compression
+gzip compressed data, was "xturing-0.1.5.tar", last modified: Wed Jun 14 11:35:01 2023, max compression
```

## Comparing `xturing-0.1.4.tar` & `xturing-0.1.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.173109 xturing-0.1.4/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.4/LICENSE
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.4/MANIFEST.in
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-13 14:43:38.173109 xturing-0.1.4/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7359 2023-06-13 13:40:44.000000 xturing-0.1.4/README.md
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-06-13 13:40:45.000000 xturing-0.1.4/pyproject.toml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-06-13 14:43:38.173109 xturing-0.1.4/setup.cfg
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.149109 xturing-0.1.4/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/cli/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/api.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/chat.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/cli/ui.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing/config/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/config_data_classes.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3593 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/finetuning_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3090 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/generation_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/config/read_config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/datasets/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/instruction_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/text2image_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/datasets/text_dataset.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4033 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/bloom_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7209 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/cerebras_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/distilgpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2286 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/falcon_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/galactica_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1801 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/generic_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/gptj_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/gptj_utils/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.161109 xturing-0.1.4/src/xturing/engines/llama_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/llama_utils/llama.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/engines/lora_engine/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/lora.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/save_and_load.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/lora_engine/test.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/opt_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/engines/quant_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/custom_autotune.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/engines/quant_utils/quant.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/model_apis/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/ai21.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/cohere.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/model_apis/openai.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.165109 xturing-0.1.4/src/xturing/models/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3290 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/bloom.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8363 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/cerebras.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/distilgpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1101 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/falcon.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/galactica.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1664 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/generic.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/gpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/llama.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/opt.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/models/stable_diffusion.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/preprocessors/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/instruction_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/preprocessors/text_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/registry.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/self_instruct/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/bootstrap_instructions.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/generate_instances.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/identify_if_classification.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/self_instruct/templates/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/templates/clf_task_template.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/trainers/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/trainers/lightning_trainer.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.169109 xturing-0.1.4/src/xturing/ui/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/ui/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/ui/playground.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.173109 xturing-0.1.4/src/xturing/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/external_loggers.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/hub.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/interactive.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/loss_fns.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/notebooks.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/text_splitter.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3803 2023-06-13 13:40:45.000000 xturing-0.1.4/src/xturing/utils/utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-13 14:43:38.157109 xturing-0.1.4/src/xturing.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3335 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/entry_points.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-06-13 14:43:38.000000 xturing-0.1.4/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.5/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.5/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-14 11:35:01.557886 xturing-0.1.5/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7359 2023-06-13 13:40:44.000000 xturing-0.1.5/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-06-14 11:34:56.000000 xturing-0.1.5/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-06-14 11:35:01.557886 xturing-0.1.5/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.541886 xturing-0.1.5/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3593 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3090 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4033 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     7209 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2286 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/falcon_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1801 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/generic_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6306 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    42467 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.549886 xturing-0.1.5/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3290 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2067 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8484 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1101 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/falcon.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1664 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/generic.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2259 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.553886 xturing-0.1.5/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.557886 xturing-0.1.5/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.5/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4034 2023-06-14 11:34:56.000000 xturing-0.1.5/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-06-14 11:35:01.545886 xturing-0.1.5/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    21821 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3335 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-06-14 11:35:01.000000 xturing-0.1.5/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.4/LICENSE` & `xturing-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/PKG-INFO` & `xturing-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.4/README.md` & `xturing-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/pyproject.toml` & `xturing-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.4"
+version = "0.1.5"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
```

### Comparing `xturing-0.1.4/src/xturing/cli/__init__.py` & `xturing-0.1.5/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/cli/api.py` & `xturing-0.1.5/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/cli/chat.py` & `xturing-0.1.5/src/xturing/cli/chat.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/config/__init__.py` & `xturing-0.1.5/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/config/config_data_classes.py` & `xturing-0.1.5/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.5/src/xturing/config/finetuning_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/config/generation_config.yaml` & `xturing-0.1.5/src/xturing/config/generation_config.yaml`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/config/read_config.py` & `xturing-0.1.5/src/xturing/config/read_config.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.5/src/xturing/datasets/instruction_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/datasets/text_dataset.py` & `xturing-0.1.5/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/__init__.py` & `xturing-0.1.5/src/xturing/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/bloom_engine.py` & `xturing-0.1.5/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/causal.py` & `xturing-0.1.5/src/xturing/engines/causal.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.5/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.5/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/falcon_engine.py` & `xturing-0.1.5/src/xturing/engines/falcon_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/galactica_engine.py` & `xturing-0.1.5/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/generic_engine.py` & `xturing-0.1.5/src/xturing/engines/generic_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.5/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/gptj_engine.py` & `xturing-0.1.5/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.5/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/llama_engine.py` & `xturing-0.1.5/src/xturing/engines/llama_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.5/src/xturing/engines/llama_utils/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.5/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.5/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/opt_engine.py` & `xturing-0.1.5/src/xturing/engines/opt_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.5/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.5/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/model_apis/__init__.py` & `xturing-0.1.5/src/xturing/model_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/model_apis/ai21.py` & `xturing-0.1.5/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/model_apis/base.py` & `xturing-0.1.5/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/model_apis/cohere.py` & `xturing-0.1.5/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/model_apis/openai.py` & `xturing-0.1.5/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/__init__.py` & `xturing-0.1.5/src/xturing/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/base.py` & `xturing-0.1.5/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/bloom.py` & `xturing-0.1.5/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/causal.py` & `xturing-0.1.5/src/xturing/models/causal.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,38 @@
 from xturing.engines.base import BaseEngine
 from xturing.engines.causal import CausalLoraEngine
 from xturing.models import BaseModel
 from xturing.preprocessors.base import BasePreprocessor
 from xturing.trainers.base import BaseTrainer
 from xturing.trainers.lightning_trainer import LightningTrainer
 from xturing.utils.logging import configure_logger
+from xturing.utils.utils import _filter_args
 
 logger = configure_logger(__name__)
 
 
 class CausalModel(BaseModel):
     def __init__(
         self,
         engine: str,
         weights_path: Optional[str] = None,
         model_name: Optional[str] = None,
         target_modules: Optional[List[str]] = None,
     ):
-        self.engine = BaseEngine.create(
-            engine,
+        arguments = dict(
             weights_path=weights_path,
             model_name=model_name,
             target_modules=target_modules,
         )
 
+        self.engine = BaseEngine.create(
+            engine,
+            **_filter_args(arguments),
+        )
+
         self.model_name = engine.replace("_engine", "")
 
         # Finetuning config
         self.finetuning_args = load_config(
             model_name=self.model_name,
             config_path=Path(__file__).parent.parent
             / "config"
```

### Comparing `xturing-0.1.4/src/xturing/models/cerebras.py` & `xturing-0.1.5/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/distilgpt2.py` & `xturing-0.1.5/src/xturing/models/distilgpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/falcon.py` & `xturing-0.1.5/src/xturing/models/falcon.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/galactica.py` & `xturing-0.1.5/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/generic.py` & `xturing-0.1.5/src/xturing/models/generic.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/gpt2.py` & `xturing-0.1.5/src/xturing/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/gptj.py` & `xturing-0.1.5/src/xturing/models/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/llama.py` & `xturing-0.1.5/src/xturing/models/llama.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/opt.py` & `xturing-0.1.5/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/models/stable_diffusion.py` & `xturing-0.1.5/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.5/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.5/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/registry.py` & `xturing-0.1.5/src/xturing/registry.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.5/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.5/src/xturing/self_instruct/generate_instances.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.5/src/xturing/self_instruct/identify_if_classification.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.5/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.5/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.5/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.5/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.5/src/xturing/trainers/lightning_trainer.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/ui/playground.py` & `xturing-0.1.5/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/hub.py` & `xturing-0.1.5/src/xturing/utils/hub.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/logging.py` & `xturing-0.1.5/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/loss_fns.py` & `xturing-0.1.5/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/notebooks.py` & `xturing-0.1.5/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/text_splitter.py` & `xturing-0.1.5/src/xturing/utils/text_splitter.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.4/src/xturing/utils/utils.py` & `xturing-0.1.5/src/xturing/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,7 +120,17 @@
                     txt_file.write(f"{name}\n\n{text}")
             except Exception as e:
                 print(f"Error processing file {file_path}: {e}")
 
     print(f"Finished processing directory, the text files are stored in {temp_dir}.")
 
     return temp_dir
+
+
+def _filter_args(arguments: dict):
+    to_delete = []
+    for key, value in arguments.items():
+        if value is None:
+            to_delete.append(key)
+    for key in to_delete:
+        del arguments[key]
+    return arguments
```

### Comparing `xturing-0.1.4/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.5/src/xturing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xturing-0.1.4/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.5/src/xturing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

