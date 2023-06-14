# Comparing `tmp/so_vits_svc_fork-4.0.0.tar.gz` & `tmp/so_vits_svc_fork-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.0.0.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.0.1.tar", max compression
```

## Comparing `so_vits_svc_fork-4.0.0.tar` & `so_vits_svc_fork-4.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-05-29 12:04:20.100162 so_vits_svc_fork-4.0.0/LICENSE
--rw-r--r--   0        0        0    27605 2023-05-29 12:04:20.100162 so_vits_svc_fork-4.0.0/README.md
--rw-r--r--   0        0        0     3091 2023-05-29 12:04:21.044174 so_vits_svc_fork-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-05-29 12:04:20.996173 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24434 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    29784 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24604 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9408 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    14797 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    29411 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-05-29 12:50:56.414961 so_vits_svc_fork-4.0.1/LICENSE
+-rw-r--r--   0        0        0    27605 2023-05-29 12:50:56.414961 so_vits_svc_fork-4.0.1/README.md
+-rw-r--r--   0        0        0     3091 2023-05-29 12:50:57.246956 so_vits_svc_fork-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-29 12:50:57.198956 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24434 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24604 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9408 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2023-05-29 12:50:56.418961 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    14797 2023-05-29 12:50:56.422962 so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    29411 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.1/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.0.0/LICENSE` & `so_vits_svc_fork-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/README.md` & `so_vits_svc_fork-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/pyproject.toml` & `so_vits_svc_fork-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.0.0"
+version = "4.0.1"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import multiprocessing
+import os
 from copy import copy
 from logging import getLogger
 from pathlib import Path
 
 import PySimpleGUI as sg
 import sounddevice as sd
 import soundfile as sf
@@ -499,62 +500,95 @@
     # frames
     frames = {}
     for name, items in frame_contents.items():
         frame = sg.Frame(name, items)
         frame.expand_x = True
         frames[name] = [frame]
 
+    bottoms = [
+        [
+            sg.Checkbox(
+                key="use_gpu",
+                default=get_optimal_device() != torch.device("cpu"),
+                text="Use GPU"
+                + (
+                    " (not available; if your device has GPU, make sure you installed PyTorch with CUDA support)"
+                    if get_optimal_device() == torch.device("cpu")
+                    else ""
+                ),
+                disabled=get_optimal_device() == torch.device("cpu"),
+            )
+        ],
+        [
+            sg.Button("Infer", key="infer"),
+            sg.Button("(Re)Start Voice Changer", key="start_vc"),
+            sg.Button("Stop Voice Changer", key="stop_vc"),
+            sg.Push(),
+            # sg.Button("ONNX Export", key="onnx_export"),
+        ],
+    ]
     column1 = sg.Column(
         [
             frames["Paths"],
             frames["Common"],
         ],
         vertical_alignment="top",
     )
     column2 = sg.Column(
         [
             frames["File"],
             frames["Realtime"],
             frames["Presets"],
-            [
-                sg.Checkbox(
-                    key="use_gpu",
-                    default=get_optimal_device() != torch.device("cpu"),
-                    text="Use GPU"
-                    + (
-                        " (not available; if your device has GPU, make sure you installed PyTorch with CUDA support)"
-                        if get_optimal_device() == torch.device("cpu")
-                        else ""
-                    ),
-                    disabled=get_optimal_device() == torch.device("cpu"),
-                )
-            ],
-            [
-                sg.Button("Infer", key="infer"),
-                sg.Button("(Re)Start Voice Changer", key="start_vc"),
-                sg.Button("Stop Voice Changer", key="stop_vc"),
-                sg.Push(),
-                # sg.Button("ONNX Export", key="onnx_export"),
-            ],
         ]
+        + bottoms
     )
-
     # columns
     layout = [[column1, column2]]
-    # layout = [[sg.Column(layout, vertical_alignment="top", scrollable=True, expand_x=True, expand_y=True)]]
+    # get screen size
+    screen_width, screen_height = sg.Window.get_screen_size()
+    if screen_height < 720:
+        layout = [
+            [
+                sg.Column(
+                    layout,
+                    vertical_alignment="top",
+                    scrollable=False,
+                    expand_x=True,
+                    expand_y=True,
+                    vertical_scroll_only=True,
+                    key="main_column",
+                )
+            ]
+        ]
     window = sg.Window(
         f"{__name__.split('.')[0].replace('_', '-')} v{__version__}",
         layout,
         grab_anywhere=True,
         finalize=True,
+        scaling=1,
+        font=("Yu Gothic UI", 11) if os.name == "nt" else None,
+        # resizable=True,
+        # size=(1280, 720),
         # Below disables taskbar, which may be not useful for some users
         # use_custom_titlebar=True, no_titlebar=False
         # Keep on top
         # keep_on_top=True
     )
+
+    # event, values = window.read(timeout=0.01)
+    # window["main_column"].Scrollable = True
+
+    # make slider height smaller
+    try:
+        for v in window.element_list():
+            if isinstance(v, sg.Slider):
+                v.Widget.configure(sliderrelief="flat", width=10, sliderlength=20)
+    except Exception as e:
+        LOG.exception(e)
+
     # for n in ["input_device", "output_device"]:
     #     window[n].Widget.configure(justify="right")
     event, values = window.read(timeout=0.01)
 
     def update_speaker() -> None:
         from . import utils
```

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.0.1/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.0/PKG-INFO` & `so_vits_svc_fork-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.0.0
+Version: 4.0.1
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.0.0 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.0.1 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

