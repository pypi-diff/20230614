# Comparing `tmp/unitorch-0.0.0.2.tar.gz` & `tmp/unitorch-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitorch-0.0.0.2.tar", last modified: Wed May 31 15:58:31 2023, max compression
+gzip compressed data, was "unitorch-0.0.0.3.tar", last modified: Wed Jun 14 07:40:32 2023, max compression
```

## Comparing `unitorch-0.0.0.2.tar` & `unitorch-0.0.0.3.tar`

### file list

```diff
@@ -1,465 +1,465 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.120706 unitorch-0.0.0.2/.pytest_cache/
--rw-r--r--   0 root         (0) root         (0)      302 2023-05-31 15:58:14.000000 unitorch-0.0.0.2/.pytest_cache/README.md
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8981 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7952 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.124706 unitorch-0.0.0.2/benchmarks/
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/benchmarks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.124706 unitorch-0.0.0.2/docs/search/
--rw-r--r--   0 root         (0) root         (0)  1019191 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/docs/search/search_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.128706 unitorch-0.0.0.2/examples/
--rw-r--r--   0 root         (0) root         (0)     2311 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.128706 unitorch-0.0.0.2/examples/configs/caption/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.132706 unitorch-0.0.0.2/examples/configs/classification/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)     1700 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/clip.ini
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/image_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.132706 unitorch-0.0.0.2/examples/configs/classification/lora/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1588 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1806 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/roberta.ini
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/swin.ini
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/text_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.136707 unitorch-0.0.0.2/examples/configs/generation/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/chatglm.ini
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/llama.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/generation/lora/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1585 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/mbart.ini
--rw-r--r--   0 root         (0) root         (0)     1597 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/mt5.ini
--rw-r--r--   0 root         (0) root         (0)     1655 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/pegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/t5.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/xpegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/xprophetnet.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/pretrain/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/pretrain/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/configs/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/services/zip_image/config.ini
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/services/zip_image/config_v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/caption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/classification/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/generation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/llama.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/xpegasus.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/notebooks/
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/notebooks/README.md
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/src/unitorch/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.144707 unitorch-0.0.0.2/src/unitorch/cli/
--rw-r--r--   0 root         (0) root         (0)     6024 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/console/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/eval.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/infer.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/script.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/service.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/train.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/datasets/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12406 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/datasets/hf.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/loss/
--rw-r--r--   0 root         (0) root         (0)     4063 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.152708 unitorch-0.0.0.2/src/unitorch/cli/models/
--rw-r--r--   0 root         (0) root         (0)     2787 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/bart/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/beit/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/bert/
--rw-r--r--   0 root         (0) root         (0)     1177 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/blip/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22703 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7788 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13026 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13764 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)     9143 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/classification_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.164709 unitorch-0.0.0.2/src/unitorch/cli/models/clip/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.164709 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/
--rw-r--r--   0 root         (0) root         (0)     4492 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing_v2.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/detection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)     2807 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/processing_stable.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/label_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/llama/
--rw-r--r--   0 root         (0) root         (0)     1429 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14017 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8206 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      887 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)    15281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/modeling_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.172709 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5815 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.172709 unitorch-0.0.0.2/src/unitorch/cli/models/peft/
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30502 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_bloom.py
--rw-r--r--   0 root         (0) root         (0)    30560 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_llama.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/processing.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/random_utils.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/ranking_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/segmentation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/swin/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/t5/
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)     1310 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8538 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/vit/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)     2314 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7238 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7811 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/optim/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/scheduler/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/score/
--rw-r--r--   0 root         (0) root         (0)    13366 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/score/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/scripts/
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scripts/README.md
--rw-r--r--   0 root         (0) root         (0)      213 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/services/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/tasks/
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26530 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/deepspeed.py
--rw-r--r--   0 root         (0) root         (0)    31564 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/supervised.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/writer/
--rw-r--r--   0 root         (0) root         (0)    10545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/datasets/
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6832 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/datasets/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/loss/
--rw-r--r--   0 root         (0) root         (0)     4712 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/prophetnet.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/models/
--rw-r--r--   0 root         (0) root         (0)     7429 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/models/bart/
--rw-r--r--   0 root         (0) root         (0)      204 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13544 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/beit/
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/bert/
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8351 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/blip/
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30316 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7700 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.204712 unitorch-0.0.0.2/src/unitorch/models/bloom/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10867 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     9140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.208712 unitorch-0.0.0.2/src/unitorch/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11157 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)    55823 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11091 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/tokenization_chatglm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.208712 unitorch-0.0.0.2/src/unitorch/models/clip/
--rw-r--r--   0 root         (0) root         (0)      281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15100 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/deberta/
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/processing_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/processing_stable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/llama/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.216713 unitorch-0.0.0.2/src/unitorch/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13928 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/modeling_ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.216713 unitorch-0.0.0.2/src/unitorch/models/mt5/
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14219 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/peft/
--rw-r--r--   0 root         (0) root         (0)     5424 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9891 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9487 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_lora.py
--rw-r--r--   0 root         (0) root         (0)    10082 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9266 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_lora.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/roberta/
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/swin/
--rw-r--r--   0 root         (0) root         (0)      193 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/t5/
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13285 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2343 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/vit/
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13693 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/modules/
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/modules/replace/
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14643 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/beam_search_v2.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/datasets_v2.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/hf_hub_v2.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/timm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/ops/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16794 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/dyhead.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/optim/
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/rl/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/rl/utils/buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/scheduler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/score/
--rw-r--r--   0 root         (0) root         (0)     1803 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/bleu.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/map.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/rouge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/tasks/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.244715 unitorch-0.0.0.2/src/unitorch/utils/
--rw-r--r--   0 root         (0) root         (0)    13580 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/palette.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/torch_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.144707 unitorch-0.0.0.2/src/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8981 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12862 2023-05-31 15:58:31.000000 unitorch-0.0.0.2/src/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.244715 unitorch-0.0.0.2/wiki/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.248715 unitorch-0.0.0.2/wiki/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/benchmarks/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.248715 unitorch-0.0.0.2/wiki/cli/
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/ast.md
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/csv.md
--rw-r--r--   0 root         (0) root         (0)      414 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/datatypes.md
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/deepspeed.md
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/jsonl.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/cli/models/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bert.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      761 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/index.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      359 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)     1712 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      398 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/parquet.md
--rw-r--r--   0 root         (0) root         (0)      851 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/postprocess.md
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/preprocess.md
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/supervised.md
--rw-r--r--   0 root         (0) root         (0)     4600 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.116705 unitorch-0.0.0.2/wiki/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/caption/
--rw-r--r--   0 root         (0) root         (0)     4659 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/caption/blip.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/classification/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/clip.md
--rw-r--r--   0 root         (0) root         (0)     4130 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/roberta.md
--rw-r--r--   0 root         (0) root         (0)     4525 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/swin.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/diffusion/
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/diffusion/controlnet.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/generation/
--rw-r--r--   0 root         (0) root         (0)     4145 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/generation/bart.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/service/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/service/zip_image.md
--rw-r--r--   0 root         (0) root         (0)     1346 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/index.md
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/labs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/labs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/wiki/models/
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bert.md
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      322 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      402 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/index.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      375 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)     4524 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/overview.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/.pytest_cache/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-14 07:40:17.000000 unitorch-0.0.0.3/.pytest_cache/README.md
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8985 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7956 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/benchmarks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.055503 unitorch-0.0.0.3/docs/search/
+-rw-r--r--   0 root         (0) root         (0)  1019191 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/docs/search/search_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.059503 unitorch-0.0.0.3/examples/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.059503 unitorch-0.0.0.3/examples/configs/caption/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.063503 unitorch-0.0.0.3/examples/configs/classification/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/clip.ini
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.063503 unitorch-0.0.0.3/examples/configs/classification/lora/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/roberta.ini
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/swin.ini
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.067503 unitorch-0.0.0.3/examples/configs/generation/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/llama.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/generation/lora/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/mbart.ini
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/mt5.ini
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/t5.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/pretrain/
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/configs/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/configs/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/examples/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/caption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/classification/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.071503 unitorch-0.0.0.3/examples/hub/generation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/llama.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/notebooks/README.md
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.043503 unitorch-0.0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch/
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch/cli/
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/console/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/script.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/service.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/console/train.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/datasets/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12406 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.079503 unitorch-0.0.0.3/src/unitorch/cli/loss/
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.083503 unitorch-0.0.0.3/src/unitorch/cli/models/
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.083503 unitorch-0.0.0.3/src/unitorch/cli/models/bart/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/beit/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/bert/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.087503 unitorch-0.0.0.3/src/unitorch/cli/models/blip/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13026 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13764 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.091503 unitorch-0.0.0.3/src/unitorch/cli/models/clip/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.095503 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.095503 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/llama/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14017 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8206 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.099503 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/peft/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30502 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 root         (0) root         (0)    30560 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.103504 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/swin/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.107504 unitorch-0.0.0.3/src/unitorch/cli/models/t5/
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/vit/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.111503 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7811 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/optim/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.115504 unitorch-0.0.0.3/src/unitorch/cli/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/score/
+-rw-r--r--   0 root         (0) root         (0)    14137 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/scripts/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/services/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.119504 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/tasks/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26523 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)    31557 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/cli/writer/
+-rw-r--r--   0 root         (0) root         (0)    10545 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/datasets/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.123504 unitorch-0.0.0.3/src/unitorch/loss/
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/
+-rw-r--r--   0 root         (0) root         (0)     7429 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/bart/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13544 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.127504 unitorch-0.0.0.3/src/unitorch/models/beit/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8355 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/blip/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30316 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7700 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.131504 unitorch-0.0.0.3/src/unitorch/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     9140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.135504 unitorch-0.0.0.3/src/unitorch/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11157 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.139504 unitorch-0.0.0.3/src/unitorch/models/clip/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15100 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.139504 unitorch-0.0.0.3/src/unitorch/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/llama/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13928 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.143504 unitorch-0.0.0.3/src/unitorch/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14219 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.147504 unitorch-0.0.0.3/src/unitorch/models/peft/
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9487 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 root         (0) root         (0)    10082 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9266 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.147504 unitorch-0.0.0.3/src/unitorch/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.151504 unitorch-0.0.0.3/src/unitorch/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/prophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.151504 unitorch-0.0.0.3/src/unitorch/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/swin/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/t5/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13285 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.155504 unitorch-0.0.0.3/src/unitorch/models/vit/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13693 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.159504 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13514 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/modules/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/modules/replace/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14643 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/modules/timm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/ops/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16794 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.163504 unitorch-0.0.0.3/src/unitorch/optim/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/rl/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/score/
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/map.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/score/rouge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.167504 unitorch-0.0.0.3/src/unitorch/tasks/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.171504 unitorch-0.0.0.3/src/unitorch/utils/
+-rw-r--r--   0 root         (0) root         (0)    13580 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/palette.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.075503 unitorch-0.0.0.3/src/unitorch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8985 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12862 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-14 07:40:31.000000 unitorch-0.0.0.3/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.175505 unitorch-0.0.0.3/wiki/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.175505 unitorch-0.0.0.3/wiki/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/benchmarks/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.179504 unitorch-0.0.0.3/wiki/cli/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/ast.md
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/csv.md
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/datatypes.md
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/deepspeed.md
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/jsonl.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/cli/models/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      783 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      359 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      664 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      425 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/parquet.md
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/postprocess.md
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/preprocess.md
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/cli/supervised.md
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.051503 unitorch-0.0.0.3/wiki/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/caption/
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/caption/blip.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/classification/
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/clip.md
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/roberta.md
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/classification/swin.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.187505 unitorch-0.0.0.3/wiki/examples/diffusion/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/examples/generation/
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/generation/bart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/examples/service/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/examples/service/zip_image.md
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/index.md
+-rw-r--r--   0 root         (0) root         (0)      890 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.191505 unitorch-0.0.0.3/wiki/labs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/labs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:40:32.199505 unitorch-0.0.0.3/wiki/models/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-06-14 07:31:19.000000 unitorch-0.0.0.3/wiki/overview.md
```

### Comparing `unitorch-0.0.0.2/LICENSE` & `unitorch-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/PKG-INFO` & `unitorch-0.0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -27,15 +27,15 @@
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
 
 
 [Documentation](https://fuliucansheng.github.io/unitorch) •
-[Installation Instructions](https://fuliucansheng.github.io/unitorch/#/install) •
+[Installation Instructions](https://fuliucansheng.github.io/unitorch/installation/) •
 [Reporting Issues](https://github.com/fuliucansheng/unitorch/issues/new?assignees=&labels=&template=bug-report.yml)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unitorch)](https://pypi.org/project/unitorch/)
 [![PyPI Version](https://badge.fury.io/py/unitorch.svg)](https://badge.fury.io/py/unitorch)
 [![PyPI Downloads](https://pepy.tech/badge/unitorch)](https://pepy.tech/project/unitorch)
 [![Github Downloads](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=downloads&logo=github&logoColor=lightgrey)](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=Downloads&logo=github&logoColor=lightgrey)
```

### Comparing `unitorch-0.0.0.2/README.md` & `unitorch-0.0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
 
 
 [Documentation](https://fuliucansheng.github.io/unitorch) •
-[Installation Instructions](https://fuliucansheng.github.io/unitorch/#/install) •
+[Installation Instructions](https://fuliucansheng.github.io/unitorch/installation/) •
 [Reporting Issues](https://github.com/fuliucansheng/unitorch/issues/new?assignees=&labels=&template=bug-report.yml)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unitorch)](https://pypi.org/project/unitorch/)
 [![PyPI Version](https://badge.fury.io/py/unitorch.svg)](https://badge.fury.io/py/unitorch)
 [![PyPI Downloads](https://pepy.tech/badge/unitorch)](https://pepy.tech/project/unitorch)
 [![Github Downloads](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=downloads&logo=github&logoColor=lightgrey)](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=Downloads&logo=github&logoColor=lightgrey)
```

### Comparing `unitorch-0.0.0.2/docs/search/search_index.json` & `unitorch-0.0.0.3/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/README.md` & `unitorch-0.0.0.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/caption/blip.ini` & `unitorch-0.0.0.3/examples/configs/caption/blip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/bert.ini` & `unitorch-0.0.0.3/examples/configs/classification/bert.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/clip.ini` & `unitorch-0.0.0.3/examples/configs/classification/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/image_clip.ini` & `unitorch-0.0.0.3/examples/configs/classification/image_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/lora/bloom.ini` & `unitorch-0.0.0.3/examples/configs/classification/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/lora/bloom_ds.ini` & `unitorch-0.0.0.3/examples/configs/classification/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/lora/llama.ini` & `unitorch-0.0.0.3/examples/configs/classification/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/lora/llama_ds.ini` & `unitorch-0.0.0.3/examples/configs/classification/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/roberta.ini` & `unitorch-0.0.0.3/examples/configs/classification/roberta.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/swin.ini` & `unitorch-0.0.0.3/examples/configs/classification/swin.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/classification/text_clip.ini` & `unitorch-0.0.0.3/examples/configs/classification/text_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/bart.ini` & `unitorch-0.0.0.3/examples/configs/generation/bart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/bloom.ini` & `unitorch-0.0.0.3/examples/configs/generation/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/chatglm.ini` & `unitorch-0.0.0.3/examples/configs/generation/chatglm.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/llama.ini` & `unitorch-0.0.0.3/examples/configs/generation/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/lora/bloom.ini` & `unitorch-0.0.0.3/examples/configs/generation/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/lora/bloom_ds.ini` & `unitorch-0.0.0.3/examples/configs/generation/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/lora/llama.ini` & `unitorch-0.0.0.3/examples/configs/generation/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/lora/llama_ds.ini` & `unitorch-0.0.0.3/examples/configs/generation/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/mbart.ini` & `unitorch-0.0.0.3/examples/configs/generation/mbart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/mt5.ini` & `unitorch-0.0.0.3/examples/configs/generation/mt5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/pegasus.ini` & `unitorch-0.0.0.3/examples/configs/generation/pegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/t5.ini` & `unitorch-0.0.0.3/examples/configs/generation/t5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/xpegasus.ini` & `unitorch-0.0.0.3/examples/configs/generation/xpegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/generation/xprophetnet.ini` & `unitorch-0.0.0.3/examples/configs/generation/xprophetnet.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/examples/configs/pretrain/clip.ini` & `unitorch-0.0.0.3/examples/configs/pretrain/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/pyproject.toml` & `unitorch-0.0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/setup.py` & `unitorch-0.0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/__init__.py` & `unitorch-0.0.0.3/src/unitorch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_cache_home():
     return UNITORCH_CACHE
 
 
 ### version
-VERSION = "0.0.0.2"
+VERSION = "0.0.0.3"
 
 ### is offline mode
 UNITORCH_OFFLINE = os.environ.get("UNITORCH_OFFLINE", "0").upper()
 
 
 def is_offline_mode():
     return UNITORCH_OFFLINE in ENV_VARS_TRUE_VALUES
```

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/console/eval.py` & `unitorch-0.0.0.3/src/unitorch/cli/console/eval.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/console/infer.py` & `unitorch-0.0.0.3/src/unitorch/cli/console/infer.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/console/script.py` & `unitorch-0.0.0.3/src/unitorch/cli/console/script.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/console/service.py` & `unitorch-0.0.0.3/src/unitorch/cli/console/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/console/train.py` & `unitorch-0.0.0.3/src/unitorch/cli/console/train.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/core.py` & `unitorch-0.0.0.3/src/unitorch/cli/core.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/datasets/hf.py` & `unitorch-0.0.0.3/src/unitorch/cli/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/decorators.py` & `unitorch-0.0.0.3/src/unitorch/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/loss/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/loss/ranking.py` & `unitorch-0.0.0.3/src/unitorch/cli/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bart/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bart/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bart/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/beit/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/beit/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/beit/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bert/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bert/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bert/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/blip/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/blip/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/blip/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bloom/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bloom/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/bloom/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/classification_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/classification_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/clip/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/clip/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/clip/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/deberta/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling_v2.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing_v2.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/detection_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/detection_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/diffusion_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/diffusion_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/generation_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/image_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/label_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/label_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/llama/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/llama/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/llama/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mbart/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mbart/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mbart/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/modeling_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mt5/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mt5/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/mt5/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/peft/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_bloom.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_llama.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/peft/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/processing_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/random_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/ranking_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/ranking_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/roberta/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/roberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/roberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/segmentation_utils.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/swin/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/swin/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/swin/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/t5/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/t5/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/t5/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/vit/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/vit/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/vit/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/modeling.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/processing.py` & `unitorch-0.0.0.3/src/unitorch/cli/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/optim/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/optim/lion.py` & `unitorch-0.0.0.3/src/unitorch/cli/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/scheduler/warmup.py` & `unitorch-0.0.0.3/src/unitorch/cli/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/score/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/score/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     map50_score,
     rouge1_score,
     rouge2_score,
     rougel_score,
     roc_auc_score,
     ndcg_score,
     matthews_corrcoef,
+    pearsonr,
     auc,
     precision_recall_curve,
 )
 from unitorch.cli import add_default_section_for_init, register_score
 from unitorch.cli.models import (
     ModelOutputs,
     ModelTargets,
@@ -296,14 +297,42 @@
         if targets.dim() == 2 and targets.size(-1) == 1:
             targets = targets[:, 0]
 
         assert outputs.dim() == 1 and targets.dim() == 1
 
         return matthews_corrcoef(targets, outputs)
 
+@register_score("core/score/pearsonr_corr")
+class PearsonrCorrScore(Score):
+    def __init__(
+        self,
+    ):
+        super().__init__()
+
+    @classmethod
+    @add_default_section_for_init("core/score/pearsonr_corr")
+    def from_core_configure(cls, config, **kwargs):
+        pass
+
+    def forward(
+        self,
+        outputs: ClassificationOutputs,
+        targets: ClassificationTargets,
+    ):
+        if isinstance(outputs, ClassificationOutputs):
+            outputs = outputs.outputs
+        if isinstance(targets, ClassificationTargets):
+            targets = targets.targets
+
+        outputs = outputs.view(-1)
+        targets = targets.view(-1)
+
+        assert outputs.numel() == targets.numel()
+
+        return pearsonr(targets, outputs)
 
 @register_score("core/score/bleu")
 class BleuScore(Score):
     def __init__(
         self,
     ):
         super().__init__()
```

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/service.py` & `unitorch-0.0.0.3/src/unitorch/cli/services/zip_image/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/tasks/deepspeed.py` & `unitorch-0.0.0.3/src/unitorch/cli/tasks/deepspeed.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
                 optim=optim if save_optimizer else None,
                 scheduler=scheduler if save_scheduler else None,
                 ema_model=self.ema_ema_model if use_ema else None,
                 best_score=self.best_score,
                 info_path=info_path,
                 local_rank=self.local_rank,
                 global_epoch=e,
-                global_step=step + 1,
+                global_step=0,
             )
 
     @torch.no_grad()
     @add_default_section_for_function("core/task/deepspeed/supervised")
     def eval(
         self,
         monitor_fns: Union[str, List[str]],
```

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/tasks/supervised.py` & `unitorch-0.0.0.3/src/unitorch/cli/tasks/supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,15 +646,15 @@
                 optim=optim if save_optimizer else None,
                 scheduler=scheduler if save_scheduler else None,
                 ema_model=self.ema_ema_model if use_ema else None,
                 best_score=self.best_score,
                 info_path=info_path,
                 local_rank=self.local_rank,
                 global_epoch=e,
-                global_step=step + 1,
+                global_step=0,
             )
 
     @torch.no_grad()
     @add_default_section_for_function("core/task/supervised")
     def eval(
         self,
         monitor_fns: Union[str, List[str]],
```

### Comparing `unitorch-0.0.0.2/src/unitorch/cli/writer/__init__.py` & `unitorch-0.0.0.3/src/unitorch/cli/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/datasets/hf.py` & `unitorch-0.0.0.3/src/unitorch/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/loss/__init__.py` & `unitorch-0.0.0.3/src/unitorch/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/loss/prophetnet.py` & `unitorch-0.0.0.3/src/unitorch/loss/prophetnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/loss/ranking.py` & `unitorch-0.0.0.3/src/unitorch/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/__init__.py` & `unitorch-0.0.0.3/src/unitorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bart/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bart/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/beit/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/beit/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bert/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bert/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/bert/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,20 +157,20 @@
         )
 
         max_predictions_per_seq = pop_value(
             max_predictions_per_seq,
             self.max_predictions_per_seq,
         )
 
-        tokens = self.tokenizer.tokenize(str(text))
+        _tokens = self.tokenizer.tokenize(str(text))
         tokens_pair = self.tokenizer.tokenize(str(text_pair))
-        truncate_sequence_pair(tokens, tokens_pair, max_seq_length - 3)
+        truncate_sequence_pair(_tokens, tokens_pair, max_seq_length - 3)
         tokens = (
             [self.cls_token]
-            + tokens
+            + _tokens
             + [self.sep_token]
             + tokens_pair
             + [self.sep_token]
         )
 
         covered_indexes = get_random_mask_indexes(
             tokens,
@@ -197,15 +197,15 @@
                     tokens[index]
                     if random.random() < 0.5
                     else get_random_word(self.vocab_words)
                 )
             tokens[index] = mask_token
 
         input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        token_type_ids = [0] + [0] * len(tokens) + [0] + [1] * len(tokens_pair) + [1]
+        token_type_ids = [0] + [0] * len(_tokens) + [0] + [1] * len(tokens_pair) + [1]
         attention_mask = [1] * len(input_ids)
 
         padding = [0] * (max_seq_length - len(input_ids))
         input_ids += len(padding) * [self.pad_token_id]
         attention_mask += padding
         token_type_ids += len(padding) * [1]
```

### Comparing `unitorch-0.0.0.2/src/unitorch/models/blip/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/blip/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bloom/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/bloom/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/configuration_chatglm.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling_chatglm.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/quantization.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/chatglm/tokenization_chatglm.py` & `unitorch-0.0.0.3/src/unitorch/models/chatglm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/clip/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/clip/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/deberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/deberta/modeling_v2.py` & `unitorch-0.0.0.3/src/unitorch/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/deberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/deberta/processing_v2.py` & `unitorch-0.0.0.3/src/unitorch/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/llama/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/llama/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/mbart/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/mbart/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/modeling_ema.py` & `unitorch-0.0.0.3/src/unitorch/models/modeling_ema.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/mt5/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/mt5/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/peft/__init__.py` & `unitorch-0.0.0.3/src/unitorch/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_adalora.py` & `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_lora.py` & `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_bloom_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_adalora.py` & `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_lora.py` & `unitorch-0.0.0.3/src/unitorch/models/peft/modeling_llama_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/pegasus/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/pegasus/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/processing_utils.py` & `unitorch-0.0.0.3/src/unitorch/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/prophetnet/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/prophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/prophetnet/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/prophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/roberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/roberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/swin/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/swin/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/t5/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/t5/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/visualbert/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/visualbert/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/visualbert/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,22 +40,16 @@
             special_input_ids (Optional[Dict]): Special input IDs. Defaults to an empty dictionary.
             do_lower_case (Optional[bool]): Whether to convert text to lowercase. Defaults to True.
             do_basic_tokenize (Optional[bool]): Whether to perform basic tokenization. Defaults to True.
             do_whole_word_mask (Optional[bool]): Whether to use whole word masking. Defaults to True.
             masked_lm_prob (Optional[float]): Probability for masked LM. Defaults to 0.15.
             max_predictions_per_seq (Optional[int]): Maximum number of masked LM predictions per sequence. Defaults to 20.
         """
-        tokenizer = get_bert_tokenizer(
-            vocab_path,
-            do_lower_case=do_lower_case,
-            do_basic_tokenize=do_basic_tokenize,
-            special_input_ids=special_input_ids,
-        )
         super().__init__(
-            tokenizer=tokenizer,
+            vocab_path=vocab_path,
             max_seq_length=max_seq_length,
             do_lower_case=do_lower_case,
             do_basic_tokenize=do_basic_tokenize,
             do_whole_word_mask=do_whole_word_mask,
             masked_lm_prob=masked_lm_prob,
             max_predictions_per_seq=max_predictions_per_seq,
         )
```

### Comparing `unitorch-0.0.0.2/src/unitorch/models/vit/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/vit/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xpegasus/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xpegasus/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xprophetnet/modeling.py` & `unitorch-0.0.0.3/src/unitorch/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/models/xprophetnet/processing.py` & `unitorch-0.0.0.3/src/unitorch/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/modules/classifier.py` & `unitorch-0.0.0.3/src/unitorch/modules/classifier.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/modules/replace/beam_search_v2.py` & `unitorch-0.0.0.3/src/unitorch/modules/replace/beam_search_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/modules/replace/datasets_v2.py` & `unitorch-0.0.0.3/src/unitorch/modules/replace/datasets_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/modules/replace/hf_hub_v2.py` & `unitorch-0.0.0.3/src/unitorch/modules/replace/hf_hub_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/modules/timm.py` & `unitorch-0.0.0.3/src/unitorch/modules/timm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/ops/dyhead.py` & `unitorch-0.0.0.3/src/unitorch/ops/dyhead.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/ops/ngram_repeat_block.py` & `unitorch-0.0.0.3/src/unitorch/ops/ngram_repeat_block.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/optim/lion.py` & `unitorch-0.0.0.3/src/unitorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/scheduler/warmup.py` & `unitorch-0.0.0.3/src/unitorch/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/score/__init__.py` & `unitorch-0.0.0.3/src/unitorch/score/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 import torch
 import torch.nn as nn
+import numpy as np
 from sklearn.metrics import (
     accuracy_score,
     f1_score,
     matthews_corrcoef,
     precision_score,
     recall_score,
     roc_auc_score,
@@ -49,12 +50,15 @@
         }
     elif isinstance(inputs, frozenset):
         return frozenset(
             remove_strings_ignore_tokens(element, ignore_tokens) for element in inputs
         )
     else:
         return inputs
+    
+
+pearsonr = lambda y_true, y_pred: np.corrcoef(y_true, y_pred)[0, 1]
 
 
 from unitorch.score.bleu import bleu_score
 from unitorch.score.rouge import rouge1_score, rouge2_score, rougel_score
 from unitorch.score.map import map_score, map50_score
```

### Comparing `unitorch-0.0.0.2/src/unitorch/score/bleu.py` & `unitorch-0.0.0.3/src/unitorch/score/bleu.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/score/map.py` & `unitorch-0.0.0.3/src/unitorch/score/map.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/score/rouge.py` & `unitorch-0.0.0.3/src/unitorch/score/rouge.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/__init__.py` & `unitorch-0.0.0.3/src/unitorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/decorators.py` & `unitorch-0.0.0.3/src/unitorch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/functional.py` & `unitorch-0.0.0.3/src/unitorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/image_utils.py` & `unitorch-0.0.0.3/src/unitorch/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/import_utils.py` & `unitorch-0.0.0.3/src/unitorch/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/io.py` & `unitorch-0.0.0.3/src/unitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/palette.py` & `unitorch-0.0.0.3/src/unitorch/utils/palette.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch/utils/torch_utils.py` & `unitorch-0.0.0.3/src/unitorch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/src/unitorch.egg-info/PKG-INFO` & `unitorch-0.0.0.3/src/unitorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -27,15 +27,15 @@
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
 
 
 [Documentation](https://fuliucansheng.github.io/unitorch) •
-[Installation Instructions](https://fuliucansheng.github.io/unitorch/#/install) •
+[Installation Instructions](https://fuliucansheng.github.io/unitorch/installation/) •
 [Reporting Issues](https://github.com/fuliucansheng/unitorch/issues/new?assignees=&labels=&template=bug-report.yml)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unitorch)](https://pypi.org/project/unitorch/)
 [![PyPI Version](https://badge.fury.io/py/unitorch.svg)](https://badge.fury.io/py/unitorch)
 [![PyPI Downloads](https://pepy.tech/badge/unitorch)](https://pepy.tech/project/unitorch)
 [![Github Downloads](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=downloads&logo=github&logoColor=lightgrey)](https://img.shields.io/github/downloads/fuliucansheng/unitorch/total?color=blue&label=Downloads&logo=github&logoColor=lightgrey)
```

### Comparing `unitorch-0.0.0.2/src/unitorch.egg-info/SOURCES.txt` & `unitorch-0.0.0.3/src/unitorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/blip.md` & `unitorch-0.0.0.3/wiki/cli/models/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/bloom.md` & `unitorch-0.0.0.3/wiki/cli/models/bloom.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/chatglm.md` & `unitorch-0.0.0.3/wiki/cli/models/chatglm.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/clip.md` & `unitorch-0.0.0.3/wiki/cli/models/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/deberta.md` & `unitorch-0.0.0.3/wiki/cli/models/deberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/llama.md` & `unitorch-0.0.0.3/wiki/cli/models/llama.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/peft.md` & `unitorch-0.0.0.3/wiki/cli/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/visualbert.md` & `unitorch-0.0.0.3/wiki/cli/models/visualbert.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/models/xlm_roberta.md` & `unitorch-0.0.0.3/wiki/cli/models/xlm_roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/cli/postprocess.md` & `unitorch-0.0.0.3/wiki/cli/postprocess.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/configuration.md` & `unitorch-0.0.0.3/wiki/configuration.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/caption/blip.md` & `unitorch-0.0.0.3/wiki/examples/caption/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/classification/clip.md` & `unitorch-0.0.0.3/wiki/examples/classification/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/classification/roberta.md` & `unitorch-0.0.0.3/wiki/examples/classification/roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/classification/swin.md` & `unitorch-0.0.0.3/wiki/examples/classification/swin.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/generation/bart.md` & `unitorch-0.0.0.3/wiki/examples/generation/bart.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/examples/service/zip_image.md` & `unitorch-0.0.0.3/wiki/examples/service/zip_image.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/index.md` & `unitorch-0.0.0.3/wiki/index.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/installation.md` & `unitorch-0.0.0.3/wiki/installation.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/models/peft.md` & `unitorch-0.0.0.3/wiki/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.2/wiki/overview.md` & `unitorch-0.0.0.3/wiki/overview.md`

 * *Files identical despite different names*

