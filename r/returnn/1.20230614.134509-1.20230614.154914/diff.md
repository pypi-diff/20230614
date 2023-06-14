# Comparing `tmp/returnn-1.20230614.134509.tar.gz` & `tmp/returnn-1.20230614.154914.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230614.134509.tar", last modified: Wed Jun 14 12:10:12 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230614.154914.tar", last modified: Wed Jun 14 14:10:11 2023, max compression
```

## Comparing `returnn-1.20230614.134509.tar` & `returnn-1.20230614.154914.tar`

### file list

```diff
@@ -1,448 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 12:09:51.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99665 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35124 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   552605 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 14:09:46.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-14 14:09:49.000000 returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99665 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35763 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   552605 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:10:11.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-14 14:09:44.000000 returnn-1.20230614.154914/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230614.134509/.gitignore` & `returnn-1.20230614.154914/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/.gitmodules` & `returnn-1.20230614.154914/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/CHANGELOG.md` & `returnn-1.20230614.154914/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/CODEOWNERS` & `returnn-1.20230614.154914/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/CONTRIBUTING.md` & `returnn-1.20230614.154914/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/LICENSE` & `returnn-1.20230614.154914/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/MANIFEST.in` & `returnn-1.20230614.154914/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/PKG-INFO` & `returnn-1.20230614.154914/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230614.134509
+Version: 1.20230614.154914
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230614.134509/README.rst` & `returnn-1.20230614.154914/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/__init__.py` & `returnn-1.20230614.154914/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/12AX.cluster_map` & `returnn-1.20230614.154914/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-fwd.config` & `returnn-1.20230614.154914/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-horovod-mpi.py` & `returnn-1.20230614.154914/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230614.154914/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-hyper-param-tuning.config` & `returnn-1.20230614.154914/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-iter-dataset.py` & `returnn-1.20230614.154914/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-list-devices.py` & `returnn-1.20230614.154914/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-lua-torch-layer.config` & `returnn-1.20230614.154914/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230614.154914/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-returnn-as-framework.py` & `returnn-1.20230614.154914/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-rf.config` & `returnn-1.20230614.154914/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-rhn-enwik8.config` & `returnn-1.20230614.154914/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-sprint-interface.py` & `returnn-1.20230614.154914/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-att-copy.config` & `returnn-1.20230614.154914/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-attention.config` & `returnn-1.20230614.154914/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-enc-dec.config` & `returnn-1.20230614.154914/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230614.154914/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230614.154914/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230614.154914/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230614.154914/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230614.154914/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-rec-self-att.config` & `returnn-1.20230614.154914/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230614.154914/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230614.154914/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-torch.config` & `returnn-1.20230614.154914/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230614.154914/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/demo.sh` & `returnn-1.20230614.154914/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230614.154914/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/README.txt` & `returnn-1.20230614.154914/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/config_demo` & `returnn-1.20230614.154914/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230614.154914/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/config_real` & `returnn-1.20230614.154914/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230614.154914/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/decode.py` & `returnn-1.20230614.154914/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230614.154914/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230614.154914/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230614.154914/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230614.154914/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230614.154914/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230614.154914/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230614.154914/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230614.154914/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/__init__.py` & `returnn-1.20230614.154914/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/__main__.py` & `returnn-1.20230614.154914/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/__old_mod_loader__.py` & `returnn-1.20230614.154914/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/__setup__.py` & `returnn-1.20230614.154914/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/config.py` & `returnn-1.20230614.154914/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/audio.py` & `returnn-1.20230614.154914/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/basic.py` & `returnn-1.20230614.154914/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/bundle_file.py` & `returnn-1.20230614.154914/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/cached.py` & `returnn-1.20230614.154914/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/cached2.py` & `returnn-1.20230614.154914/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/generating.py` & `returnn-1.20230614.154914/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/hdf.py` & `returnn-1.20230614.154914/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/lm.py` & `returnn-1.20230614.154914/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/map.py` & `returnn-1.20230614.154914/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/meta.py` & `returnn-1.20230614.154914/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/multi_proc.py` & `returnn-1.20230614.154914/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/normalization_data.py` & `returnn-1.20230614.154914/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/numpy_dump.py` & `returnn-1.20230614.154914/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/raw_wav.py` & `returnn-1.20230614.154914/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/sprint.py` & `returnn-1.20230614.154914/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/stereo.py` & `returnn-1.20230614.154914/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230614.154914/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/datasets/util/vocabulary.py` & `returnn-1.20230614.154914/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/engine/base.py` & `returnn-1.20230614.154914/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/engine/batch.py` & `returnn-1.20230614.154914/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230614.154914/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/edit.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/select.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/transform.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/extern/graph_editor/util.py` & `returnn-1.20230614.154914/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/forward_iface.py` & `returnn-1.20230614.154914/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/__init__.py` & `returnn-1.20230614.154914/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/_backend.py` & `returnn-1.20230614.154914/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/_numpy_backend.py` & `returnn-1.20230614.154914/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/_utils.py` & `returnn-1.20230614.154914/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/array_.py` & `returnn-1.20230614.154914/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/attention.py` & `returnn-1.20230614.154914/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/cond.py` & `returnn-1.20230614.154914/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/const.py` & `returnn-1.20230614.154914/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/container.py` & `returnn-1.20230614.154914/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/conv.py` & `returnn-1.20230614.154914/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/device.py` & `returnn-1.20230614.154914/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/dims.py` & `returnn-1.20230614.154914/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/dropout.py` & `returnn-1.20230614.154914/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/dtype.py` & `returnn-1.20230614.154914/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/encoder/base.py` & `returnn-1.20230614.154914/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/encoder/conformer.py` & `returnn-1.20230614.154914/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/init.py` & `returnn-1.20230614.154914/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/linear.py` & `returnn-1.20230614.154914/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/loop.py` & `returnn-1.20230614.154914/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/loss.py` & `returnn-1.20230614.154914/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/math_.py` & `returnn-1.20230614.154914/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/matmul.py` & `returnn-1.20230614.154914/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/module.py` & `returnn-1.20230614.154914/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/normalization.py` & `returnn-1.20230614.154914/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/parameter.py` & `returnn-1.20230614.154914/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/rand.py` & `returnn-1.20230614.154914/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/rec.py` & `returnn-1.20230614.154914/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/reduce.py` & `returnn-1.20230614.154914/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/run_ctx.py` & `returnn-1.20230614.154914/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/signal.py` & `returnn-1.20230614.154914/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/state.py` & `returnn-1.20230614.154914/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/tensor_array.py` & `returnn-1.20230614.154914/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/frontend/types.py` & `returnn-1.20230614.154914/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/import_/common.py` & `returnn-1.20230614.154914/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/import_/git.py` & `returnn-1.20230614.154914/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/import_/import_.py` & `returnn-1.20230614.154914/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/learning_rate_control.py` & `returnn-1.20230614.154914/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/log.py` & `returnn-1.20230614.154914/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/native_op.cpp` & `returnn-1.20230614.154914/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/native_op.py` & `returnn-1.20230614.154914/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/pretrain.py` & `returnn-1.20230614.154914/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/sprint/cache.py` & `returnn-1.20230614.154914/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/sprint/control.py` & `returnn-1.20230614.154914/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/sprint/error_signals.py` & `returnn-1.20230614.154914/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/sprint/extern_interface.py` & `returnn-1.20230614.154914/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/sprint/interface.py` & `returnn-1.20230614.154914/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/_dim_extra.py` & `returnn-1.20230614.154914/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/_tensor_extra.py` & `returnn-1.20230614.154914/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230614.154914/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230614.154914/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230614.154914/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/dim.py` & `returnn-1.20230614.154914/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/marked_dim.py` & `returnn-1.20230614.154914/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/tensor.py` & `returnn-1.20230614.154914/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/tensor_dict.py` & `returnn-1.20230614.154914/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tensor/utils.py` & `returnn-1.20230614.154914/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/compat.py` & `returnn-1.20230614.154914/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/data_pipeline.py` & `returnn-1.20230614.154914/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/distributed.py` & `returnn-1.20230614.154914/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/engine.py` & `returnn-1.20230614.154914/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230614.154914/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230614.154914/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/horovod.py` & `returnn-1.20230614.154914/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230614.154914/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/base.py` & `returnn-1.20230614.154914/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/basic.py` & `returnn-1.20230614.154914/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/rec.py` & `returnn-1.20230614.154914/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/segmental_model.py` & `returnn-1.20230614.154914/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/signal_processing.py` & `returnn-1.20230614.154914/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/layers/variable.py` & `returnn-1.20230614.154914/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/native_op.py` & `returnn-1.20230614.154914/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/network.py` & `returnn-1.20230614.154914/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/sprint.py` & `returnn-1.20230614.154914/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/updater.py` & `returnn-1.20230614.154914/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/util/basic.py` & `returnn-1.20230614.154914/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/util/data.py` & `returnn-1.20230614.154914/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/util/ken_lm.py` & `returnn-1.20230614.154914/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/tf/util/open_fst.py` & `returnn-1.20230614.154914/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/data/pipeline.py` & `returnn-1.20230614.154914/returnn/torch/data/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -236,7 +236,50 @@
                 current_max_sequence_lengths = sequence_lengths
             else:
                 current_batch.append(data_dict)
                 current_max_sequence_lengths = max_sequence_lengths_if_included
 
         if current_batch:
             yield current_batch
+
+
+class LenFilterDataPipe(torch.utils.data.IterDataPipe):
+    """
+    Removes sequences which are either too long or too short from a dataset
+    Returns dataset yielding list of data lengths within the defined range
+    """
+
+    def __init__(
+        self,
+        dataset: torch.utils.data.IterableDataset,
+        min_seq_length: Union[int, NumbersDict] = None,
+        max_seq_length: Union[int, NumbersDict] = None,
+    ):
+        """
+        :param dataset: dataset to apply the filter to
+        :param min_seq_length: minimum sequence length either in general or per data_key via dict
+        :param max_seq_length: maximum sequence length either in general or per data_key via dict
+        """
+        super().__init__()
+        self._dataset = dataset
+        self._min_seq_length = NumbersDict(0 if min_seq_length is None else min_seq_length)
+        self._max_seq_length = NumbersDict(sys.maxsize if max_seq_length is None else max_seq_length)
+
+    def __iter__(self):
+        """
+        :return: generator providing filtered data where each sequence is a dict
+          data_key -> data_array.
+        :rtype: Iterable[dict[str, numpy.ndarray]]
+        """
+        for data_dict in self._dataset:
+            # TODO: This assumes all data has time as first dimension. Currently we can't know better..
+            sequence_lengths = NumbersDict(
+                {data_key: data.shape[0] for data_key, data in data_dict.items() if data.shape}
+            )
+            if sequence_lengths.any_compare(self._min_seq_length, lambda a, b: a < b):
+                continue
+            if sequence_lengths.any_compare(self._max_seq_length, lambda a, b: a > b):
+                continue
+            yield data_dict
+
+    def __getitem__(self, index):
+        raise Exception(f"{self.__class__.__name__}.__getitem__ not supported")
```

### Comparing `returnn-1.20230614.134509/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230614.154914/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/data/tensor_utils.py` & `returnn-1.20230614.154914/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/distributed.py` & `returnn-1.20230614.154914/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/engine.py` & `returnn-1.20230614.154914/returnn/torch/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,20 @@
         self.eval_datasets = {}
         self.extern_data = None  # type: Optional[TensorDict]
         self._train_dataloader = None  # type: Optional[DataLoader2]
         self._eval_dataloaders = {}  # type: Dict[str, DataLoader2]
 
         self._start_epoch = None  # type: Optional[int]
         self._final_epoch = None  # type: Optional[int]
+        self._min_seq_length = config.typed_value("min_seq_length", None) or config.int(
+            "min_seq_length", None
+        )  # type: Union[int,float,Dict[str,int],NumbersDict]
+        self._max_seq_length = config.typed_value("max_seq_length", None) or config.int(
+            "max_seq_length", None
+        )  # type: Union[int,float,Dict[str,int],NumbersDict]
         self._orig_model = None  # type: Optional[Union[rf.Module, torch.nn.Module]]
         self._pt_model = None  # type: Optional[torch.nn.Module]
         self._train_step_func = None  # type: Optional[Callable]
         self._forward_step_func = self.config.typed_value("forward_step")  # type: Optional[Callable]
         self._forward_step_expected_outputs = None  # type: Optional[TensorDict]
         if self.config.typed_value("model_outputs") is not None:
             self._forward_step_expected_outputs = TensorDict()
@@ -412,15 +418,18 @@
         # Make sure that _dataset_reset does not keep a ref to `self`,
         # otherwise it would trigger to pickle `self` and all its members.
         dataset_reset = returnn_dataset_wrapper.ReturnnDatasetResetMpSharedEpochCallback(
             dataset=dataset, epoch_mp_shared=self._epoch_mp_shared
         )
 
         wrapped_dataset = returnn_dataset_wrapper.ReturnnDatasetIterDataPipe(dataset, reset_callback=dataset_reset)
-
+        if (self._min_seq_length is not None) or (self._max_seq_length is not None):
+            wrapped_dataset = data_pipeline.LenFilterDataPipe(
+                wrapped_dataset, min_seq_length=self._min_seq_length, max_seq_length=self._max_seq_length
+            )
         chunking = self.config.typed_value("chunking", None)
         if chunking:
             wrapped_dataset = data_pipeline.ChunkingIterDataPipe(wrapped_dataset, chunking)
 
         batch_size = self.config.typed_value("batch_size", 1)
         max_seqs = self.config.int("max_seqs", -1)
         batches_dataset = data_pipeline.BatchingIterDataPipe(wrapped_dataset, batch_size=batch_size, max_seqs=max_seqs)
```

### Comparing `returnn-1.20230614.134509/returnn/torch/frontend/_backend.py` & `returnn-1.20230614.154914/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/frontend/_rand.py` & `returnn-1.20230614.154914/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/frontend/bridge.py` & `returnn-1.20230614.154914/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/torch/updater.py` & `returnn-1.20230614.154914/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/basic.py` & `returnn-1.20230614.154914/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/better_exchook.py` & `returnn-1.20230614.154914/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/bpe.py` & `returnn-1.20230614.154914/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/debug.py` & `returnn-1.20230614.154914/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/debug_helpers.py` & `returnn-1.20230614.154914/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/fsa.py` & `returnn-1.20230614.154914/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230614.154914/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/pprint.py` & `returnn-1.20230614.154914/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/py-to-pickle.cpp` & `returnn-1.20230614.154914/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/sig_proc.py` & `returnn-1.20230614.154914/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn/util/task_system.py` & `returnn-1.20230614.154914/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/returnn.egg-info/PKG-INFO` & `returnn-1.20230614.154914/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230614.134509
+Version: 1.20230614.154914
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230614.134509/returnn.egg-info/SOURCES.txt` & `returnn-1.20230614.154914/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/setup.py` & `returnn-1.20230614.154914/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/DummySprintExec.py` & `returnn-1.20230614.154914/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230614.154914/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230614.154914/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230614.154914/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/_set_num_threads1.py` & `returnn-1.20230614.154914/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/_setup_test_env.py` & `returnn-1.20230614.154914/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/bpe-unicode-demo.codes` & `returnn-1.20230614.154914/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/bpe-unicode-demo.vocab` & `returnn-1.20230614.154914/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/lexicon_opt.isyms` & `returnn-1.20230614.154914/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/lexicon_opt.jpg` & `returnn-1.20230614.154914/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/lint_common.py` & `returnn-1.20230614.154914/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/pycharm-inspect.py` & `returnn-1.20230614.154914/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/pylint.py` & `returnn-1.20230614.154914/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/returnn-as-framework.py` & `returnn-1.20230614.154914/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/rf_utils.py` & `returnn-1.20230614.154914/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/spelling.dic` & `returnn-1.20230614.154914/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Config.py` & `returnn-1.20230614.154914/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Dataset.py` & `returnn-1.20230614.154914/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Fsa.py` & `returnn-1.20230614.154914/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_GeneratingDataset.py` & `returnn-1.20230614.154914/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_HDFDataset.py` & `returnn-1.20230614.154914/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_LearningRateControl.py` & `returnn-1.20230614.154914/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Log.py` & `returnn-1.20230614.154914/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_MultiProcDataset.py` & `returnn-1.20230614.154914/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_PTDataset.py` & `returnn-1.20230614.154914/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Pretrain.py` & `returnn-1.20230614.154914/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_ResNet.py` & `returnn-1.20230614.154914/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_SprintDataset.py` & `returnn-1.20230614.154914/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_SprintInterface.py` & `returnn-1.20230614.154914/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFEngine.py` & `returnn-1.20230614.154914/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFNativeOp.py` & `returnn-1.20230614.154914/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFNetworkLayer.py` & `returnn-1.20230614.154914/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230614.154914/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230614.154914/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFUpdater.py` & `returnn-1.20230614.154914/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TFUtil.py` & `returnn-1.20230614.154914/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TF_determinism.py` & `returnn-1.20230614.154914/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TaskSystem.py` & `returnn-1.20230614.154914/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230614.154914/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_TranslationDataset.py` & `returnn-1.20230614.154914/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_Util.py` & `returnn-1.20230614.154914/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_demos.py` & `returnn-1.20230614.154914/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_fork_exec.py` & `returnn-1.20230614.154914/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_hdf_dump.py` & `returnn-1.20230614.154914/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_array.py` & `returnn-1.20230614.154914/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_attention.py` & `returnn-1.20230614.154914/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_base.py` & `returnn-1.20230614.154914/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_cond.py` & `returnn-1.20230614.154914/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_container.py` & `returnn-1.20230614.154914/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_conv.py` & `returnn-1.20230614.154914/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_encoder_conformer.py` & `returnn-1.20230614.154914/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_loop.py` & `returnn-1.20230614.154914/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_math.py` & `returnn-1.20230614.154914/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_normalization.py` & `returnn-1.20230614.154914/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_rec.py` & `returnn-1.20230614.154914/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_reduce.py` & `returnn-1.20230614.154914/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_rf_signal.py` & `returnn-1.20230614.154914/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_tensor.py` & `returnn-1.20230614.154914/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_tools.py` & `returnn-1.20230614.154914/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_torch_frontend.py` & `returnn-1.20230614.154914/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tests/test_torch_internal_frontend.py` & `returnn-1.20230614.154914/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/analyze-dataset-batches.py` & `returnn-1.20230614.154914/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/bliss-collect-seq-lens.py` & `returnn-1.20230614.154914/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/bliss-dump-text.py` & `returnn-1.20230614.154914/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/bliss-get-segment-names.py` & `returnn-1.20230614.154914/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/bliss-to-ogg-zip.py` & `returnn-1.20230614.154914/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/bpe-create-lexicon.py` & `returnn-1.20230614.154914/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/calculate-word-error-rate.py` & `returnn-1.20230614.154914/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/cleanup-old-models.py` & `returnn-1.20230614.154914/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/collect-orth-symbols.py` & `returnn-1.20230614.154914/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/collect-words.py` & `returnn-1.20230614.154914/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/compile_native_op.py` & `returnn-1.20230614.154914/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/compile_tf_graph.py` & `returnn-1.20230614.154914/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/debug-dump-search-scores.py` & `returnn-1.20230614.154914/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/debug-plot-search-scores.py` & `returnn-1.20230614.154914/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-dataset-raw-strings.py` & `returnn-1.20230614.154914/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-dataset.py` & `returnn-1.20230614.154914/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-forward-stats.py` & `returnn-1.20230614.154914/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-forward.py` & `returnn-1.20230614.154914/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-network-json.py` & `returnn-1.20230614.154914/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/dump-pickle.py` & `returnn-1.20230614.154914/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230614.154914/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/get-attention-weights.py` & `returnn-1.20230614.154914/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/get-best-model-epoch.py` & `returnn-1.20230614.154914/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/hdf_dump.py` & `returnn-1.20230614.154914/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230614.154914/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/import-blocks-mt-model.py` & `returnn-1.20230614.154914/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/import-t2t-mt-model.py` & `returnn-1.20230614.154914/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/Makefile` & `returnn-1.20230614.154914/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/README.md` & `returnn-1.20230614.154914/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/example/README.md` & `returnn-1.20230614.154914/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230614.154914/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230614.154914/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230614.154914/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/file.h` & `returnn-1.20230614.154914/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230614.154914/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230614.154914/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/main.cc` & `returnn-1.20230614.154914/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230614.154914/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230614.154914/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230614.154914/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/tf_avg_checkpoints.py` & `returnn-1.20230614.154914/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/tf_inspect_checkpoint.py` & `returnn-1.20230614.154914/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/tf_inspect_summary_log.py` & `returnn-1.20230614.154914/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230614.134509/tools/torch_export_to_onnx.py` & `returnn-1.20230614.154914/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

